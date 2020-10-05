---
layout: page
title: Laravel Lexicon
permalink: /
---

# Laravel Lexicon (BETA)
![Laravel Lexicon Logo](assets/img/lexicon.jpg)

Dictionary of PHP / Laravel technical terms and concepts

<div class="section-index">
    <hr class="panel-line">
    {% for post in site.docs  %}        
    <i class="fas fa-question-circle"></i> <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
    {% endfor %}
</div>
