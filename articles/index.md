---
layout: default
title: Articles
---

# Articles

<ul>
{% assign sorted = site.articles | sort: 'date' | reverse %}
{% for a in sorted %}
  <li>
    <a href="{{ a.url | relative_url }}">{{ a.title }}</a><br>
    <small>{{ a.authors }}</small>
  </li>
{% endfor %}
</ul>