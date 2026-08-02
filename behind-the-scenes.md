---
layout: default
title: "Behind the Scenes"
permalink: /behind-the-scenes/
description: "Go behind the scenes at Fez & Flavores and discover how our Moroccan specialties and French pastries are prepared."
---

# Behind the Scenes

Step inside the world of **Fez & Flavores** and discover the care, technique, and creativity behind every product.

From selecting ingredients and developing flavours to baking, decorating, and preparing an order for delivery, this section shares the work that happens before a finished creation reaches the customer.

{% assign behind_posts = site.categories.behind-scenes %}

{% if behind_posts %}

<div class="category-list">

{% for post in behind_posts %}

<article class="category-card">

  <h2>
    <a href="{{ post.url | relative_url }}">
      {{ post.title }}
    </a>
  </h2>

  <p class="post-meta">
    Published {{ post.date | date: "%B %d, %Y" }}
  </p>

  {% if post.description %}
    <p>{{ post.description }}</p>
  {% else %}
    <p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
  {% endif %}

  <a class="read-more" href="{{ post.url | relative_url }}">
    Go behind the scenes →
  </a>

</article>

{% endfor %}

</div>

{% else %}

<div class="coming-soon">

## Behind-the-Scenes Stories Are Coming Soon

We will be sharing preparation methods, kitchen moments, ingredient selections, decorating processes, packaging, and the development of new Fez & Flavores creations.

</div>

{% endif %}

---

## What Happens Behind Every Creation?

Every Fez & Flavores product involves several important stages:

1. Selecting quality ingredients
2. Planning the flavour and texture combination
3. Preparing each component
4. Baking, cooking, chilling, or setting
5. Assembling the finished product
6. Decorating with care and precision
7. Checking quality and presentation
8. Packaging the order safely
9. Preparing it for pickup or delivery

We believe that sharing this process helps customers understand the time, craftsmanship, and attention behind every handcrafted product.

> The finished dessert is only the final chapter—the real story begins with an idea, quality ingredients, and careful preparation.
