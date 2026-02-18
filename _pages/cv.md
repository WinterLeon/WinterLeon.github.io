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
: Thesis: *Traces and extensions of non abelian gauge covariant Sobolev spaces*, supervised by J. Van Schaftingen.
: Fall 2022: Abroad studies at **Tohoku University** (Japan), completing the COLABS program under supervision of Fu. Nakano. 

*June 2021*
: **Bachelor in mathematics**, Université catholique de Louvain.
: Thesis: *La fonction Gamma d'Euler et la fonction zêta de Riemann : Construction et propriété*, supervised by T. Cleays.

---

Publications & Preprints
---
{% for post in site.publications reversed %}
*{{ post.year }}*
: **{{ post.title }}**, {% if post.category == 'manuscripts' %} *{{ post.venue }}*, {% elsif post.category == 'submitted' %} {{ post.category }}, {% endif %}{{ post.authors }}, {{ post.year }}
: {% if post.doi and post.arxivurl %}
<span style="font-size: 0.8em;"><a href=" https://doi.org/{{ post.doi }} ">doi:{{ post.doi }}</a> - <a href=" https://arxiv.org/abs/{{ post.arxivurl }} ">arXiv:{{ post.arxivurl }}</a></span>
{% elsif post.arxivurl %}
<span style="font-size: 0.8em;"><a href=" https://arxiv.org/abs/{{ post.arxivurl }} ">arXiv:{{ post.arxivurl }}</a></span>
{% else %}
<span style="font-size: 0.8em;">Unavailable</span>
{% endif %}
{% endfor %}

---

Talks
---
*See also [Talks]({% link _pages/talks.md %}).*

{% for post in site.talks reversed %}

*{{ post.date | default: "1900-01-01" | date: "%B %Y" }} ({{ post.location }})*
: **{{ post.title }}**
: {{ post.venue }}
{% endfor %}
---

Teaching experience
---
*See also [Teaching]({% link _pages/teaching.md %}).*

{% for post in site.teaching reversed %}
*{{ post.period }}*
: **{{ post.title }}**
: {% if post.type == "Bachelor's thesis" %}
  Bachelor's thesis supervision.
  {% else %}
  Exercise sessions for {{ post.students }} students at {{ post.venue }}, in {{ post.language }}.
  {% endif %}
{% endfor %}
---

