---
layout: default
title: Home
---

# Articles

<ul>
{% assign sorted = site.articles | sort: 'date' | reverse %}
{% for a in sorted %}
  <li>
    <a href="{{ a.url | relative_url }}">{{ a.title }}</a>
    {% if a.authors %}<br><small>{{ a.authors }}</small>{% endif %}
    {% if a.venue %}<br><small><em>{{ a.venue }}</em> ({{ a.year }})</small>{% endif %}
  </li>
{% endfor %}
</ul>

---

# Datasets

- **DRAD dataset** → [datasets/visionrisk](./datasets/visionrisk/)