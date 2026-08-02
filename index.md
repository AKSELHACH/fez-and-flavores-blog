---
layout: default
title: Home
---

<div class="home-magazine-cover">
  <a
    href="{{ '/products/' | relative_url }}"
    aria-label="Explore the Fez and Flavores products and menu">

    <img
      src="{{ '/images/fez-flavores-magazine-cover-sweets.png' | relative_url }}"
      alt="Fez and Flavores magazine cover featuring Moroccan pastries and petite fours"
      width="1122"
      height="1402"
      loading="eager">

  </a>
</div>

# 🌿 Welcome to Fez & Flavores

**Where flavor meets tradition**

Welcome to our blog! We share authentic recipes, food stories, and cultural insights from Fez and beyond.

---

## 📝 Latest Posts

{% for post in site.posts %}
  <div class="post-preview">
    <h2>
      <a href="{{ post.url | relative_url }}">
        {{ post.title }}
      </a>
    </h2>

    <p class="post-meta">
      {{ post.date | date: "%B %d, %Y" }}
    </p>

    <p>
      {{ post.excerpt | strip_html | truncatewords: 30 }}
    </p>
  </div>
{% endfor %}

---

## 📸 Follow Us

Stay updated on Instagram:
[@Fez_Flavores](https://instagram.com/Fez_Flavores)
