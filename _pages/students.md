---
layout: archive
title: "PhD students"
permalink: /students/
author_profile: true
---

Supervising young researchers is one of the most rewarding parts of my work. Two of my students have received the Sacks Prize of the Association for Symbolic Logic for the best doctoral dissertation in mathematical logic: **Matteo Viale** (2005) and **Obrad Kasum** (2025).

Current students
------
{% for s in site.data.students.current %}
* **{{ s.name }}** ({{ s.university }}, since {{ s.since }}): *{{ s.topic }}*{% if s.note %}. {{ s.note }}{% endif %}.
{%- endfor %}

Former students
------
{% for s in site.data.students.former %}
* **{{ s.name }}**{% if s.year %}, {{ s.year }}{% endif %}, {{ s.university }}{% if s.cosupervisors %}, co-supervised with {{ s.cosupervisors }}{% endif %}{% if s.title %}.<br>{% if s.thesis_url %}[*{{ s.title }}*]({{ s.thesis_url }}){% else %}*{{ s.title }}*{% endif %}{% elsif s.thesis_url %}. [Thesis]({{ s.thesis_url }}){% endif %}{% if s.award %}<br>🏆 **{{ s.award }}**{% endif %}
{%- endfor %}

See also my page on the [Mathematics Genealogy Project](https://www.mathgenealogy.org/id.php?id=10233).
