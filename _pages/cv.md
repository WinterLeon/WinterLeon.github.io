---
layout: archive
title: "Curriculum Vitæ"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
---
*Sept. 2023*
: **Master in mathematics (research focus)**, Université catholique de Louvain.

*June 2021*
: **Bachelor in mathematics**, Université catholique de Louvain.

Teaching experience
---
*For information on the classes, see [Teaching]({% link _pages/teaching.md %}).*

{% for post in site.teaching reversed %}
*{{ post.period }}*
: **{{ post.title }}**
: Exercise sessions for {{ post.students }} students at {{ post.venue }}, in {{ post.language }}.
{% endfor %}
---

Publications & Preprints
---
{% for post in site.publications reversed %}
*{{ post.year }}*
: **{{ post.title }}**, {{ post.authors }}, {{ post.year}}{% if post.doi and post.arxivurl %}
: <span style="font-size: 0.8em;"><a href=" https://doi.org/{{ post.doi }} ">doi:{{ post.doi }}</a> - <a href=" https://arxiv.org/abs/{{ post.arxivurl }} ">arXiv:{{ post.arxivurl }}</a></span>
{% elsif post.arxivurl %}
: <span style="font-size: 0.8em;"><a href=" https://arxiv.org/abs/{{ post.arxivurl }} ">arXiv:{{ post.arxivurl }}</a></span>
{% endif %}
{% endfor %}
  
Talks
---
Under construction, sorry.
  