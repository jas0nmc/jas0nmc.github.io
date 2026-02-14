---
title: "8th Grade English"
permalink: /8th/english/
layout: single
---

<div class="page-with-sidebar" style="display:flex; flex-wrap:nowrap;">

<!-- Left sidebar -->
<div class="page-sidebar" style="width:220px; margin-right:20px; border-right:1px solid #ddd; padding-right:15px;">
  <h3 style="margin-top:0;">Grades</h3>
  <ul style="list-style:none; padding-left:0; margin:0;">
    <li><strong>8th Grade</strong>
      <ul style="margin:6px 0 12px 12px;">
        <li><a href="/8th/english/">English</a></li>
        <li><a href="/8th/math/">Math</a></li>
        <li><a href="/8th/science/">Science</a></li>
      </ul>
    </li>
    <li><strong>9th Grade</strong>
      <ul style="margin:6px 0 12px 12px;">
        <li><a href="/9th/english/">English</a></li>
      </ul>
    </li>
    <li><strong>10th Grade</strong>
      <ul style="margin:6px 0 12px 12px;">
        <li><a href="/10th/english/">English</a></li>
      </ul>
    </li>
  </ul>
</div>

<!-- Main content -->
<div style="flex:1; padding-left:10px;">

## Assignments

{% assign english_posts = site.posts | where: "grade", 8 | where: "subject", "english" | sort: "assignment_number" %}

{% for post in english_posts %}
- **Assignment {{ post.assignment_number }}:** [{{ post.title }}]({{ post.url }})
{% endfor %}

</div>
</div>
