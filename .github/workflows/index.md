---
layout: default
title: Home
---

# 🌿 Welcome to Fez & Flavores

**Where flavor meets tradition**

Welcome to our blog! We share authentic recipes, food stories, and cultural insights from Fez and beyond.

---

## 📝 Latest Posts

{% for post in site.posts %}
  <div class="post-preview">
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
    <p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
  </div>
{% endfor %}

---

## 📸 Follow Us

Stay updated on Instagram: [@Fez_Flavores](https://instagram.com/Fez_Flavores)
