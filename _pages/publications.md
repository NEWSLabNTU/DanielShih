---
layout: page
title: publications
permalink: /publications/
description: Publications by categories in reversed chronological order. 
years: [2026,2025,2024,2023,2022,2021,2020,2019,2018,2017,2016,2015,2014,2013,2012,2011,2010,2009,2008,2007,2006,2005,2004,2003,2002,2001,1998,1997]
---
{% for y in page.years %}
<h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
