---
permalink: /
title: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Since October 2023, I have been a Ph.D. student in **Geometric Analysis** under the supervision of Prof. [Jean Van Schaftingen](https://perso.uclouvain.be/jean.vanschaftingen/index.php?lang=en) at the [Institut de Recherche en Mathématique et Physique (IRMP)](https://www.uclouvain.be/en/research-institutes/irmp) of the [Université catholique de Louvain (UCLouvain)](https://www.uclouvain.be/en), Belgium.

Since October 2025, I have held an Aspirant (Research Fellow) position with the [Fonds de la Recherche Scientifique - FNRS](https://www.frs-fnrs.be/en/). Prior to that, my work was funded by the Fonds Spécial de Recherche (FSR) of the UCLouvain.

My research lies in geometric analysis, with a particular emphasis on **Sobolev-type spaces in geometric settings**. This includes **gauge-covariant Sobolev spaces** arising in gauge theories and **Sobolev spaces of mappings between manifolds**, where nonlinear constraints appear in the codomain. Current work focuses on [Sobolev mappings between manifolds](https://en.wikipedia.org/wiki/Sobolev_mapping), with special attention to trace theory. More broadly, my interests span topics in geometric analysis, and I also enjoy learning about analytic number theory.

------
# Have we met?
You might have met me at one of the following gatherings:

{% for post in site.conferences reversed %}
- **{{ post.title }}**, {{ post.date | default: "1900-01-01" | date: "%B %Y" }}<br>
{% if post.type != 'conference' %} {{ post.type }}, {% endif %}{{ post.venue }} ({{ post.country }})<br>
{%- endfor -%}

  
