---
layout: default
title: NNlk05's Venting Hole
---

# NNlk05's Venting Hole

## Otherwise known as my personal blog

I am NNlk05 (any pronouns, they/them preferred), a programer, geek, and Minecraft world generation nerd.
{:.float-left}

![](https://nnlk05.github.io/pfp.png)

### Recent Posts

<ul style="list-style: none; padding: 0; display: inline-block; text-align: left;">
  {% for post in site.posts %}
    <li style="margin-bottom: 0.5rem; display: flex; align-items: center; justify-content: center;">
      <span style="color: #94cdff; margin-right: 10px; font-family: monospace;">{{ post.date | date: "%Y-%m-%d" }}</span>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

### Browse by Topic

<div class="icons" style="display: flex; flex-wrap: wrap; justify-content: center; gap: 8px; margin-bottom: 2rem;">
  {% assign sorted_tags = site.tags | sort %}
  {% for tag in sorted_tags %}
    <a href="{{ '/topics.html' | relative_url }}#{{ tag[0] | slugify }}" class="margin-fix" style="padding: 4px 10px; border-radius: 4px; display: inline-block; font-family: monospace;">
      🏷️ {{ tag[0] }} ({{ tag[1].size }})
    </a>
  {% endfor %}
</div>
