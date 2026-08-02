---
layout: default
title: "Moroccan Food Stories"
permalink: /moroccan-food-stories/
description: "Explore the traditions, history, culture, and stories behind Moroccan cuisine and the culinary heritage of Fez."
---

# Moroccan Food Stories

Moroccan cuisine is more than a collection of recipes. It is a living expression of family, hospitality, history, celebration, and regional identity.

Through **Moroccan Food Stories**, Fez & Flavores explores the traditions behind the dishes, ingredients, techniques, and ceremonies that have shaped Morocco’s culinary heritage.

{% assign story_posts = site.categories.moroccan-stories %}

{% if story_posts %}

<div class="category-list">

{% for post in story_posts %}

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
    Read the complete story →
  </a>

</article>

{% endfor %}

</div>

{% else %}

<div class="coming-soon" markdown="1">

## Stories Are Coming Soon

We are preparing stories about the culinary heritage of Fez, Moroccan hospitality, traditional celebrations, regional ingredients, and the meaning behind Morocco’s most treasured dishes.

</div>

{% endif %}

---

## Stories We Will Explore

Future articles will include:

- The culinary heritage of the city of Fez
- The tradition of Moroccan mint tea
- The history and symbolism of pastilla
- Moroccan hospitality and the family table
- Traditional Ramadan and Eid foods
- Moroccan wedding pastries and celebrations
- The cultural story behind chebakia and sellou
- Regional flavours and spices of Morocco
- How recipes are passed between generations
- The relationship between food, memory, and identity

> Every dish carries a story, and every flavour connects us to a place, a family, and a tradition.
