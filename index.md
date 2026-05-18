---
layout: default
title: NNlk05's Venting Hole
---

# NNlk05's Venting Hole

## Otherwise known as my personal blog

<p class="float-left">
I am NNlk05 (any pronouns, they/them preferred), a programer, geek, and Minecraft world generation nerd.
</p>
![](){:.pfp .float-right style="background-image: url('https://nnlk05.github.io/pfp.png');"}

### Recent Posts

<ul>
  {% for post in site.posts %}
    <li>
      <span style="color: #94cdff; margin-right: 10px;">{{ post.date | date: "%Y-%m-%d" }}</span>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
