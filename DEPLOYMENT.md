# Deployment and migration notes

## Publishing

The site is built and deployed by [.github/workflows/jekyll.yml](.github/workflows/jekyll.yml) on
every push to `main`, and can also be run manually from the Actions tab.

One-time setup after importing this repository to GitHub:

1. Push to `NEWSLabNTU/DanielShih` with `main` as the default branch (the workflow triggers on
   `main`; change the `branches:` list if you use a different name).
2. **Settings → Pages → Build and deployment → Source: GitHub Actions.** This is required — the
   default "Deploy from a branch" mode would run GitHub's own Jekyll 3.9 build, which cannot load
   `_plugins/BetterTube.rb` or jekyll-scholar.
3. Confirm `url` and `baseurl` in `_config.yml` match the published address
   (`https://newslabntu.github.io` + `/DanielShih`).

The workflow passes `--baseurl "${{ steps.pages.outputs.base_path }}"`, so the deployed baseurl
always follows the repository name even if `_config.yml` drifts.

## Fallback: publishing from a branch

[bin/deploy](bin/deploy) builds locally and force-pushes `_site/` to a `gh-pages` branch. It is a
fallback for when Actions is unavailable; it requires Pages to be switched back to
"Deploy from a branch". Run it from a clean working tree:

```bash
./bin/deploy                 # source branch: main, deploy branch: gh-pages
```

## What changed from DanielFolio (Jekyll 3.9 → 4.3)

| Area | Jekyll 3.9 site | This site |
| --- | --- | --- |
| Gems | `github-pages` gem (pins Jekyll 3.9.5, forbids custom plugins) | `jekyll ~> 4.3.4` with plugins pinned directly |
| Ruby | 2.7.2 | 3.4 |
| Scholar | jekyll-scholar 5.16 | jekyll-scholar 7.3 (5.x calls `File.exists?` and `Proc.new` without a block, both removed in modern Ruby) |
| Highlighter | `highlighter: pygments` | `highlighter: rouge` — Jekyll 4 removed the pygments option |
| Markdown | kramdown, with GFM applied implicitly by GitHub Pages | `kramdown: input: GFM` declared explicitly, plus the `kramdown-parser-gfm` gem (kramdown 2 unbundled it) |
| Sass | libsass via jekyll-sass-converter 1.5 | Dart Sass via jekyll-sass-converter 3.1 |
| Collection defaults | `collections.news.defaults.layout` — not a real Jekyll key, silently ignored | top-level `defaults:` mapping `type: news` to `layout: post` |
| Bibliography path | `source: /_bibliography/` | `source: ./_bibliography` (jekyll-scholar 7 resolves a leading `/` against the filesystem root) |
| Deploy | `github-pages` build on push | `bundle exec jekyll build` in Actions, uploaded as a Pages artifact |

Content changes made during the migration:

- **`{% link %}` now includes the baseurl.** In Jekyll 3 it did not, so the theme wrote
  `{{ site.baseurl }}{% link ... %}`. Under Jekyll 4 that produced `/DanielShih/DanielShih/...`.
  The redundant prefix was removed from 14 links in `_pages/teaching.md` and the three
  `UNIQ_NTU*` posts.
- **Hardcoded `https://newslabntu.github.io/DanielFolio/...` links** in 22 posts and news items were
  replaced with `{{ site.baseurl }}/...` so they follow `_config.yml` instead of pointing at the old site.
- **Sass division**: `$a / $b` is deprecated in Dart Sass. `_sass/_media-queries.scss` and
  `_sass/_header.scss` now use `math.div()`. The compiled values are unchanged.

## Known issues carried over from the old site

- **Duplicate blog URL.** `_posts/2023-03-02-Messages-To-New-Students.markdown` and
  `_posts/2023-11-22-Messages-To-New-Students.markdown` both resolve to
  `/blog/2023/Messages-To-New-Students/`; the November post wins and the March post is unreachable.
  Jekyll 4 reports this as a `Conflict` warning at build time (3.9 did so silently). Fix by
  changing one post's `title:` or giving it an explicit `permalink:`.
- **Build warnings `Empty slug generated for '-'/'--'`.** These come from `pages = {--}` and
  `issn = {-}` placeholder fields in `_bibliography/papers.bib`, which also render as
  "2026, p. –" on the publications page. Filling in or removing those fields clears both.
- **Google Analytics.** `_config.yml` still carries the placeholder `UA-XXXXXXXXX`, and
  `_includes/hemline.html` loads the retired `analytics.js`. Universal Analytics stopped
  processing data in 2023; the snippet needs replacing with GA4 (`gtag.js`) or removing.
- **Sass `@import`.** The theme's partials still use `@import`, which Dart Sass has deprecated
  (removal in Dart Sass 3.0). The warnings are silenced via `sass.silence_deprecations` in
  `_config.yml`; migrating `_sass/` to `@use`/`@forward` is the eventual fix.

The old repository's `ConfigEnviron.txt` described a local build VM and included its login
credentials in plaintext; those were deliberately not carried over. If that VM is still in use,
keep its credentials outside the repository.
