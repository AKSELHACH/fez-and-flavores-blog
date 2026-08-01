---
layout: default
title: Fez & Flavores
---

# 🌿 Welcome to Fez & Flavores

**Where flavor meets tradition**

Welcome to our blog! We share authentic recipes, food stories, and cultural insights from Fez and beyond.

---

## 📝 Latest Posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <small>{{ post.date | date: "%B %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>

---

## 📸 Follow Us

Stay updated on Instagram: [@Fez_Flavores](https://instagram.com/Fez_Flavores)
