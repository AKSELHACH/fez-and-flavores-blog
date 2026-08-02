---
layout: default
title: "Recipes"
permalink: /recipes/
description: "Discover Moroccan recipes, French pastry techniques, baking instructions, and culinary inspiration from Fez & Flavores."
---

# Recipes

Welcome to the **Fez & Flavores recipe collection**.

Here you will discover authentic Moroccan recipes, French pastry techniques, helpful baking tips, and step-by-step instructions designed for home cooks and pastry enthusiasts.

{% assign recipe_posts = site.categories.recipes %}

{% if recipe_posts %}

<div class="category-list">

{% for post in recipe_posts %}

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
    View complete recipe →
  </a>

</article>

{% endfor %}

</div>

{% else %}

<div class="coming-soon">

## Recipes Are Coming Soon

Our first recipes are currently being prepared.

Return soon for Moroccan breads, traditional pastries, French desserts, cakes, creams, mousses, and professional pastry techniques.

</div>

{% endif %}

---

## What You Will Find in Our Recipes

Each complete recipe may include:

- Preparation and cooking time
- Number of servings
- Ingredients and exact measurements
- Step-by-step instructions
- Professional pastry tips
- Storage and serving recommendations
- Ingredient substitutions when possible
- Original Fez & Flavores photographs

> Some signature Fez & Flavores products and proprietary recipes may not include every professional production detail.
