---
title: "8th Grade English"
permalink: /8th/english/
layout: single
---

<div class="page-with-sidebar" style="display:flex; flex-wrap:nowrap;">

  {% include sidebar-grades.html %}

  <div style="flex:1; padding-left:10px;">

    <!-- Hero / Page Intro -->
    <div style="background-color:#f0f8ff; padding:28px; border-radius:8px; margin-bottom:18px; text-align:center;">
      <h1 style="color:#0d6efd; margin-bottom:10px;">8th Grade English - My Portfolio</h1>
      <p style="color:#333; font-size:1.05em; max-width:720px; margin:0 auto;">
        Browse all 8th Grade English assignments here. Assignments are numbered for easy reference.
      </p>
    </div>

    <!-- Assignments List -->
    <h2>Assignments</h2>
    {% assign english_posts = site.posts | where: "grade", 8 | where: "subject", "english" | sort: "assignment_number" %}
    <ul>
    {% for post in english_posts %}
      <li><strong>Assignment {{ post.assignment_number }}:</strong> <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
    </ul>

  </div>
</div>
