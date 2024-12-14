---
layout: page
title: Home
id: home
permalink: /
---

# Welcome to Navdeesh's Digital Garden! 🌱

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  Start your journey by exploring <span style="font-weight: bold">[[Daily Notes]]</span> or dive into <span style="font-weight: bold">[[Goals and Projects]]</span>.
</p>

This space is a growing collection of ideas, thoughts, and knowledge curated to organize my life and studies. Feel free to explore, learn, and get inspired! 🌟

### Quick Links

- **School Work**: Navigate through [[Subjects]] to find class-specific notes and exam prep materials.
- **Personal Growth**: Check out my [[Habits]] and [[Goals]] for self-improvement.
- **Career & Projects**: Explore my [[Data Science]] projects and resources.
- **YouTube Ideas**: Peek into my [[YouTube Videos]] for creative content.

### Recently Updated Notes

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

### What is this?

This digital garden is my personal space for growth and exploration. It's built using [this template](https://github.com/maximevaillancourt/digital-garden-jekyll-template) and nurtured with daily updates.

You can start your own digital garden too! Follow this [guide](https://maximevaillancourt.com/blog/setting-up-your-own-digital-garden-with-jekyll).

<style>
  .wrapper {
    max-width: 46em;
  }
</style>