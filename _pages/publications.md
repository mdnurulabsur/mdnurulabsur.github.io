---
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

## PhD and Core Research

{% for post in site.publications reversed %}
  {% if post.pub_group == "phd" %}
    <p>
      <strong>{{ post.title }}</strong><br>
      {{ post.venue }}<br>
      {% if post.paperurl %}<a href="{{ post.paperurl }}" target="_blank" rel="noopener noreferrer">DOI</a>{% endif %}
      {% if post.pdfurl %} | <a href="{{ post.pdfurl }}" target="_blank" rel="noopener noreferrer">PDF</a>{% endif %}
    </p>
  {% endif %}
{% endfor %}

## Collaboration Papers

{% for post in site.publications reversed %}
  {% if post.pub_group == "collab" %}
    <p>
      <strong>{{ post.title }}</strong><br>
      {{ post.venue }}<br>
      {% if post.paperurl %}<a href="{{ post.paperurl }}" target="_blank" rel="noopener noreferrer">DOI</a>{% endif %}
      {% if post.pdfurl %} | <a href="{{ post.pdfurl }}" target="_blank" rel="noopener noreferrer">PDF</a>{% endif %}
    </p>
  {% endif %}
{% endfor %}
