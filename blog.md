---
layout: default
title: Blog
permalink: /blog/
---

# Blog Posts

## Categories

<div class="category-nav">
  <a href="#deep-learning">Deep Learning</a> |
  <a href="#agentic-ai">Agentic AI</a> |
  <a href="#full-stack">Full Stack</a>
</div>

<h2 id="deep-learning">Deep Learning</h2>
{% assign deep_learning_posts = site.posts | where: "category", "deep-learning" %}
{% for post in deep_learning_posts %}
## [{{ post.title }}]({{ post.url | relative_url }})
*{{ post.date | date: "%B %d, %Y" }}*

{{ post.excerpt }}

[Read more]({{ post.url | relative_url }})

---
{% endfor %}

<h2 id="agentic-ai">Agentic AI</h2>
{% assign agentic_ai_posts = site.posts | where: "category", "agentic-ai" %}
{% for post in agentic_ai_posts %}
## [{{ post.title }}]({{ post.url | relative_url }})
*{{ post.date | date: "%B %d, %Y" }}*

{{ post.excerpt }}

[Read more]({{ post.url | relative_url }})

---
{% endfor %}

<h2 id="full-stack">Full Stack</h2>
{% assign full_stack_posts = site.posts | where: "category", "full-stack" %}
{% for post in full_stack_posts %}
## [{{ post.title }}]({{ post.url | relative_url }})
*{{ post.date | date: "%B %d, %Y" }}*

{{ post.excerpt }}

[Read more]({{ post.url | relative_url }})

---
{% endfor %}

{% if site.posts.size == 0 %}
No blog posts yet! Check back soon.
{% endif %}