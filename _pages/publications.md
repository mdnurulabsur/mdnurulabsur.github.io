---
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

{% for post in site.publications reversed %}
  <p>
    <strong>{{ post.title }}</strong><br>
    {{ post.venue }}<br>
    {% if post.paperurl %}<a href="{{ post.paperurl }}" target="_blank" rel="noopener noreferrer">DOI</a>{% endif %}
  </p>
{% endfor %}
