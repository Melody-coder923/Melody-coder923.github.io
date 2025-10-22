---
layout: default
title: About Me
permalink: /
---

# About Me

<div class="profile-photo">
    <img src="/assets/images/profile.jpg" alt="Melody Zhao in a green beret against a scenic mountain landscape">
</div>

<div class="social-links">
    <a href="https://github.com/Melody-coder923" target="_blank">
        <i class="fab fa-github"></i>
        <span>GitHub</span>
    </a>
    <a href="https://www.linkedin.com/in/yan-zhao-092348239/" target="_blank">
        <i class="fab fa-linkedin"></i>
        <span>LinkedIn</span>
    </a>
</div>

I'm Melody Zhao, an AI Software Engineer and graduate student in Computer Software Engineering. With a passion for artificial intelligence and software development, I'm always eager to learn and tackle new challenges.

## Recent Blog Posts

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}