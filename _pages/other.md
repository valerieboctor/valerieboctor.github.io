<!-- ---
title: "Recipes + Blog"
permalink: /recipes-blog/
layout: archive
author_profile: true
entries_layout: grid
---

{% assign recipes = site.documents | where_exp: "doc", "doc.collection == 'recipes'" %}
{% assign blog = site.documents | where_exp: "doc", "doc.collection == 'blog'" %}

{% assign all_entries = recipes | concat: blog | sort: "date" | reverse %}

{% for post in all_entries %}
  {% include archive-single.html %}
{% endfor %} -->

---
layout: archive
title: "Other"
permalink: /Other/
author_profile: true
redirect_from:
  - /Other
---

