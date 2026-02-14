---
title: "8th Grade English"
permalink: /8th/english/
layout: single
---

<div style="display: flex;">

<!-- Left sidebar -->
<div style="width: 200px; margin-right: 20px;">
  <h3>Grades</h3>
  <ul>
    <li><strong>8th Grade</strong>
      <ul>
        <li><a href="/8th/english/">English</a></li>
        <li><a href="/8th/math/">Math</a></li>
        <li><a href="/8th/science/">Science</a></li>
      </ul>
    </li>
    <li><strong>9th Grade</strong>
      <ul>
        <li><a href="/9th/english/">English</a></li>
      </ul>
    </li>
    <li><strong>10th Grade</strong>
      <ul>
        <li><a href="/10th/english/">English</a></li>
      </ul>
    </li>
  </ul>
</div>

<!-- Main content -->
<div style="flex: 1;">

## Assignments

{% assign english_posts = site.posts | where: "grade", 8 | where: "subject", "english" | sort: "assignment_number" %}

{% for post in english_posts %}
- **Assignment {{ post.assignment_number }}:**  
  [{{ post.title }}]({{ post.url }})
{% endfor %}

</div>
</div>
