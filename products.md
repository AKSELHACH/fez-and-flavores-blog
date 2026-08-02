---
layout: default
title: "Products & Menu"
permalink: /products/
description: "Explore the Fez & Flavores menu of Moroccan specialties, French pastries, breads, cakes, and handcrafted desserts."
---

# Products & Menu

Welcome to the **Fez & Flavores** menu, where Moroccan tradition meets refined French pastry craftsmanship.

Explore our freshly prepared breads, savoury specialties, cakes, pastries, and handcrafted desserts. Product availability and prices may vary according to size, ingredients, season, and customization.

{% assign product_posts = site.categories.products | sort: "menu_order" %}

{% if product_posts %}

<div class="category-list">

{% for post in product_posts %}

<article class="category-card">

  <h2>
    <a href="{{ post.url | relative_url }}">
      {{ post.title }}
    </a>
  </h2>

  <p class="post-meta">
    Updated {{ post.date | date: "%B %d, %Y" }}
  </p>

  {% if post.description %}
    <p>{{ post.description }}</p>
  {% else %}
    <p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
  {% endif %}

  <a class="read-more" href="{{ post.url | relative_url }}">
    View products and prices →
  </a>

</article>

{% endfor %}

</div>

{% else %}

<p>Our complete menu is being prepared. Please return soon to discover our latest products.</p>

{% endif %}

---

## Customized Orders

Looking for a customized birthday cake, celebration cake, dessert table, or Moroccan catering selection?

Prices for customized products depend on the size, flavour, ingredients, decoration, and design complexity.

<a
  class="order-button"
  href="https://instagram.com/Fez_Flavores"
  target="_blank"
  rel="noopener noreferrer">
  Request a Quote on Instagram
</a>

> **Pricing notice:** Prices may change based on ingredients, size, customization, and availability. Please contact Fez & Flavores to confirm current pricing before ordering.
