---
title: "Publications"
permalink: /publications/
author_profile: true
---

## PhD and Core Research

{% for post in site.publications reversed %}
{% if post.pub_group == "phd" %}
**{{ post.title }}**  
{{ post.venue }}  
{% if post.paperurl %}[DOI]({{ post.paperurl }}){% endif %}
{% if post.pdfurl %} | [PDF]({{ post.pdfurl }}){% endif %}

{% endif %}
{% endfor %}

---

## Collaboration Papers

{% for post in site.publications reversed %}
{% if post.pub_group == "collab" %}
**{{ post.title }}**  
{{ post.venue }}  
{% if post.paperurl %}[DOI]({{ post.paperurl }}){% endif %}
{% if post.pdfurl %} | [PDF]({{ post.pdfurl }}){% endif %}

{% endif %}
{% endfor %}
