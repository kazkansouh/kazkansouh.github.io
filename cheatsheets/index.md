---
layout: page
title: Cheatsheets
subtitle: For the lazy
hero_height: is-small
---

The following cheat sheets are saved on the site:
{% assign cheatsheets = site.pages | where: "layout" , "cheatsheet" | sort: "title" %}
{% for cheatsheet in cheatsheets %}
* [{{ cheatsheet.title }}]({{ cheatsheet.url }})
{% endfor %}

