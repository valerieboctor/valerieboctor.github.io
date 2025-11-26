---
title: "Recipes + Blog"
permalink: /recipes-blog/
layout: archive
author_profile: true
entries_layout: grid   # or 'list' if you prefer
---

{% assign recipes = site.recipes | default: site.collections.recipes.docs %}
{% assign blog    = site.blog    | default: site.collections.blog.docs %}

{% assign all_entries = recipes | concat: blog | sort: "date" | reverse %}

{% for post in all_entries %}
  {% include archive-single.html %}
{% endfor %}