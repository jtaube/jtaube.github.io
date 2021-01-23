---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

## Current projects:
<!-- add photos!!!! -->
For my undergraduate honors thesis I am constructing a COVID-19 disease transmission model. We use networks to account for heterogeneous contact patterns and evolutionary game theory to represent rational decision making about masking, social distancing, and quarantine behaviors. This work is inspired by and will expand on that of <a href="https://doi.org/10.1016/j.mbs.2012.04.003">Poletti and colleagues</a> by eliminating the assumption of homogeneous mixing and incorporating individual variation in willingness to mask and social distance, for example. I'm advised on this project by Professors <a href="http://www.bowdoin.edu/~mirfan/">Mohammad Irfan</a> and <a href="https://www.bowdoin.edu/profiles/faculty/mlzeeman/">Mary Lou Zeeman</a>. 


## Publications:

{% if author.googlescholar %}
  %You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}
{% include base_path %}
{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}


