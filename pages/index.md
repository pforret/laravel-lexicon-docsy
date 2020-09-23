---
layout: page
title: Laravel Lexicon
permalink: /
---

# Laravel Lexicon (BETA)
![Laravel Lexicon Logo](assets/img/logo/android-chrome-512x512.png)

This site explains most of the technical programming terms and concepts you will need as a PHP/Laravel developer.

<div class="section-index">
    <hr class="panel-line">
    {% for post in site.docs  %}        
    <i class="fas fa-question-circle"></i> <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
    {% endfor %}
</div>
