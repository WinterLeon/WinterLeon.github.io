---
layout: archive
title: "Teaching"
permalink: /teaching/
author_profile: true
entries_layout: grid
---

{% include base_path %}

{% for post in site.teaching reversed %}

**{{ post.title }}**
: *{{ post.period }}*
: Exercise sessions for {{ post.students }} students at {{ post.venue }}, in {{ post.language }}.

{{ post.excerpt }}
---
{% endfor %}