---
layout: archive
title: "Teaching"
permalink: /teaching/
author_profile: true
entries_layout: grid
---
{% include base_path %}

During the final year of my bachelor’s degree (2020), I was appointed as a tutor for exercise sessions in **undergraduate courses**, a role I continued throughout my master’s studies. At the beginning of my Ph.D. (2023), I began teaching exercise sessions in **master’s-level courses**.

In the academic year 2025–-2026, I **supervised a Bachelor’s thesis** at UCLouvain.

I have taught in both **French** and **English**.

# List of past teaching duties
{% for post in site.teaching reversed %}

**{{ post.title }}**
: *{{ post.period }}*
: {% if post.type == "Bachelor's thesis" %}
  Bachelor's thesis supervision.
  {% else %}
  Exercise sessions for {{ post.students }} students at {{ post.venue }}, in {{ post.language }}.
  {% endif %}

---
{% endfor %}