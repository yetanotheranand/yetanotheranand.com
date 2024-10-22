---
layout: page
title: About
permalink: /about/
weight: 3
---

Hi I am **{{ site.author.name }}** :wave:,<br>
I'm a software engineer with a passion for developing systems that can have a positive impact in the real world. I have been predominantly working in the digital experience domain, focusing on efficiency and reliability, ensuring the systems I design can handle growth without compromise. I recently graduated with Masters in Software Engineering from [Arizona State University](https://www.asu.edu){:target="_blank"}. I have completed my undergraduate studies in Computer Science and Engineering from [Institute of Engineering and Technology](https://www.ietlucknow.ac.in){:target="_blank"}.

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
