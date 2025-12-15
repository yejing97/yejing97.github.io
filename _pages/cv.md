---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* Ph.D in [Your Field], [Your University], 20XX
* M.S. in [Your Field], [Your University], 20XX
* B.S. in [Your Field], [Your University], 20XX

Work experience
======
* 20XX - Present: [Your Current Position]
  * [Your Current Institution]
  * Duties include: [Key responsibilities]
  * [Additional details]

* 20XX - 20XX: [Previous Position]
  * [Previous Institution]
  * Duties included: [Key responsibilities]
  * Supervisor: [Supervisor name]

* 20XX - 20XX: [Earlier Position]
  * [Institution]
  * Duties included: [Key responsibilities]
  * Supervisor: [Supervisor name]
  
Skills
======
* Technical Skills
  * Skill 1
  * Skill 2
  * Skill 3
* Research Skills
  * Research methodology
  * Statistical analysis
  * [Other relevant skills]
* Professional Skills
  * Written communication
  * Presentation
  * Project management

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Service and leadership
======
* [Professional association/committee name] - [role], [years]
* [University committee name] - [role], [years]
* [Other service activities]
