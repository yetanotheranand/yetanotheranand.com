---
layout: page
title: About
permalink: /about/
weight: 3
---

Hi I am **{{ site.author.name }}** :wave:,<br>
I’m a full-stack developer and currently pursuing my Masters in Software Engineering from [Arizona State University](https://www.asu.edu){:target="_blank"}. I have completed my undergraduate studies in Computer Science from [Institute of Engineering and Technology](https://www.ietlucknow.ac.in){:target="_blank"}, and have 8 years of professional experience in the software industry in the design, development and maintenance of mobile and web-based applications in an agile manner.

{% include about/coursework.html %}

<div class="row">
  <h2 class="mb-3">Skills</h2>
</div>
<div class="row">
{% include about/skills.html title="Programming/Scripting Languages" source=site.data.programming-skills %}
{% include about/skills.html title="Tools, Frameworks & Libraries" source=site.data.other-programming-skills %}
</div>

<div class="row">
{% include about/skills.html title="Databases" source=site.data.database-skills %}
{% include about/skills.html title="Others" source=site.data.other-skills %}
</div>

{% include about/education-timeline.html %}
{% include about/professional-experience-timeline.html %}
