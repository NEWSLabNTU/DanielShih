---
layout: page
title: researches
permalink: /projects/
description: A growing collection of my research projects.
---

<div class="img_row">
    <img class="col three" src="{{ site.baseurl
    }}/assets/img/LabStudent2018.jpg" alt="" title="2018 Welcome and
	Farewell Party"/>
</div>
<div class="col three caption">
2018 Welcome and Farewell Party
</div>

My researches aim on software design and theory for embedded real-time
systems in general. Here is a video version of my researches for
[2021-2022](https://youtu.be/mf09bHq3uKg) and related to IoT in 2020:
[Research on IoT](https://youtu.be/H7j_MtQ9zoY).

Ongoing Research for 2022-2023:[PDF]({% link /assets/files/OnGoingResearch.pdf %})
{% include youtube.html id='GzkLTNMnmyk' %}


{% for project in site.projects %}

{% if project.redirect %}
<div class="project">
    <div class="thumbnail">
        <a href="{{ project.redirect }}" target="_blank">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img | prepend: site.baseurl | prepend: site.url }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>
{% else %}

<div class="project ">
    <div class="thumbnail">
        <a href="{{ project.url | prepend: site.baseurl | prepend: site.url }}">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img | prepend: site.baseurl | prepend: site.url }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>

{% endif %}
{% endfor %}

