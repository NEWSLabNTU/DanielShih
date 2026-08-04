# Daniel's Scholar Page

[![theme](https://img.shields.io/badge/theme-al--folio-brightgreen.svg)](https://github.com/alshedivat/al-folio)
[![license](https://img.shields.io/github/license/mashape/apistatus.svg?maxAge=2592000)](LICENSE)

The personal/academic site of Dr. Chi-Sheng Shih, built with **Jekyll 4.3** and the
[al-folio](https://github.com/alshedivat/al-folio) theme (originally based on the
[\*folio theme](https://github.com/bogoli/-folio) by [Lia Bogoev](http://liabogoev.com)).

This repository supersedes `NEWSLabNTU/DanielFolio`, which was built with Jekyll 3.9 via the
`github-pages` gem. See [DEPLOYMENT.md](DEPLOYMENT.md) for what changed and how the site is published.

## Requirements

- Ruby 3.4 (see [.ruby-version](.ruby-version)); Ruby 3.1+ also works
- Bundler

## Local development

```bash
bundle install
bundle exec jekyll serve      # http://127.0.0.1:4000/DanielShih/
bundle exec jekyll build      # writes _site/
```

The site uses two things GitHub's built-in Pages builder does not allow — the custom Liquid tag in
[_plugins/BetterTube.rb](_plugins/BetterTube.rb) and the [jekyll-scholar](https://github.com/inukshuk/jekyll-scholar)
plugin — so it is built by GitHub Actions and published as a Pages artifact rather than built by
GitHub Pages itself.

## Layout

| Path | Contents |
| --- | --- |
| `_pages/` | about (site index), publications, researches, teaching, services, awards |
| `_posts/` | blog posts, published under `/blog/:year/:title/` |
| `_news/` | short news items shown on the front page (`news_limit: 6` in `_config.yml`) |
| `_projects/` | research project cards shown on the researches page |
| `_projectsArchives/` | retired project cards (not a configured collection; not built) |
| `_bibliography/papers.bib` | publication list rendered by jekyll-scholar with `myieee.csl` |
| `_layouts/`, `_includes/`, `_sass/` | theme |
| `assets/` | images, PDFs, fonts, JS, `css/main.scss` |

## Adding content

- **News item**: add `_news/announcement_<yyyymmdd>.md` with `title`, `date`, and `inline: true`
  for items that render in full on the front page. The `layout: post` default comes from
  `defaults:` in `_config.yml`.
- **Blog post**: add `_posts/YYYY-MM-DD-Title.markdown` with `layout: post`, `title`, `date`,
  `description`. The URL is `/blog/:year/:title/`, so two posts with the same title in the same
  year collide — vary the title.
- **Publication**: add the BibTeX entry to `_bibliography/papers.bib` and, if the year is new,
  add it to the `years:` list in [_pages/publications.md](_pages/publications.md).
- **Internal links**: use `{{ site.baseurl }}/path/` (or `{% link /assets/files/file.pdf %}`,
  which already includes the baseurl in Jekyll 4). Never hardcode `/DanielShih/`.

## License

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
