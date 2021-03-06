---
title: 'Patterns'
layout: pattern
date: 2014-10-31 18:25
updated: 2016-08-15 01:08
unique_id: patterns
permalink: /patterns/
description: 'A collection of patterns for this website.'
image:
  - src: 2016-03-16-flag.svg
    png_src: 2016-03-16-flag.png
    alt: ''
---

This is a collection of all of the patterns on [olivermak.es]({{ site.url }}), organized by [color](/patterns/color/), [text](/patterns/text/), modular [components](/patterns/component/), and other [interface](/patterns/interface/) elements. These patterns serve as living documentation for this site’s present design. They also prescribe use and specification for every element on the site. The source for these patterns is [on GitHub]({{ site.source_url.repo }}).
{:.content--pattern}

<div class="pattern-index">
{% assign items = site.patterns-categories | sort: 'priority', 'last' %}
{% for item in items %}
{% include block/item--pattern.html %}
{% endfor %}
</div>
