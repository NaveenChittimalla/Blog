---
title: Second Post
date: 2024-05-12
---

**My Second Post"
This is my second post.

**All Posts**
<ul>
  {% for post in site.data.settings %}
    <li>
      <a href="https://naveenchittimalla.github.io/skills-github-pages{{ post.location }}">
        {{ post.name }}
      </a>
    </li>
  {% endfor %}
</ul>
