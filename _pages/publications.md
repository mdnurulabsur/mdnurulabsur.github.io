---
layout: single
title: "Publications"
permalink: /publications/
author_profile: true
---

Below is a selection of my publications. I am gradually moving all entries from my CV here.

{% include base_path %}

{% for pub in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
