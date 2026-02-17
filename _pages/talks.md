---
layout: archive
title: "Talks and presentations"
permalink: /talks/
author_profile: true
---

{% if site.talkmap_link == true %}

<p style="text-decoration:underline;"><a href="/talkmap.html">See a map of all the places I've given a talk!</a></p>

{% endif %}

{% include base_path %}

{% for post in site.talks reversed %}

**{{ post.title }}**
: {{ post.venue }}
: {{ post.date | default: "1900-01-01" | date: "%B %Y" }} ({{ post.location }})

{{ post.excerpt }}
---
{% endfor %}

# Scientific gatherings I attended

{% for post in site.conferences reversed %}
 **{{ post.title }}**
: {{ post.date | default: "1900-01-01" | date: "%B %Y" }}, {% if post.type != 'conference' %} {{ post.type }}, {% endif %}{{ post.venue }} ({{ post.country }})

---
{% endfor %}