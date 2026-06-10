---
layout: archive
title: "Other"
permalink: /Other/
author_profile: true
redirect_from:
  - /Other
---

{% assign other_items = site.other | sort: "date" | reverse %}

{% for post in other_items %}
  {% include archive-single.html %}
{% endfor %}