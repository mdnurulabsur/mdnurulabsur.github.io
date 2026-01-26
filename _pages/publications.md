---
title: "Publications"
permalink: /publications/
author_profile: true
---

## PhD and Core Research

{% assign phd_posts = site.publications | where: "pub_group", "phd" | sort: "date" | reverse %}

{% assign current_year = "" %}
{% for post in phd_posts %}
  {% assign y = post.date | date: "%Y" %}
  {% if y != current_year %}
### {{ y }}
  {% assign current_year = y %}
  {% endif %}

**{{ post.title }}**  
{{ post.venue }}  
{% if post.paperurl %}<a href="{{ post.paperurl }}" target="_blank" rel="noopener noreferrer">DOI</a>{% endif %}{% if post.pdfurl %} | <a href="{{ post.pdfurl }}" target="_blank" rel="noopener noreferrer">PDF</a>{% endif %}

{% endfor %}

---

## Collaboration Papers

{% assign collab_posts = site.publications | where: "pub_group", "collab" | sort: "date" | reverse %}

{% assign current_year = "" %}
{% for post in collab_posts %}
  {% assign y = post.date | date: "%Y" %}
  {% if y != current_year %}
### {{ y }}
  {% assign current_year = y %}
  {% endif %}

**{{ post.title }}**  
{{ post.venue }}  
{% if post.paperurl %}<a href="{{ post.paperurl }}" target="_blank" rel="noopener noreferrer">DOI</a>{% endif %}{% if post.pdfurl %} | <a href="{{ post.pdfurl }}" target="_blank" rel="noopener noreferrer">PDF</a>{% endif %}

{% endfor %}
