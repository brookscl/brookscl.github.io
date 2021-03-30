---
title: Yearly Archive
layout: archive
author_profile: true
permalink: /yearly-archive/
entries_layout: grid
---


{% assign entries_layout = page.entries_layout | default: 'grid' %}
<div class="entries-{{ entries_layout }}">
{% assign current_year = "now" | date: "%Y" %}
{% for year in (2003..current_year) %}
    <div class="grid__item">
      <a href="/year/{{ year }}">{{ year }}</a>
    </div>
    {% endfor %}
</div>
