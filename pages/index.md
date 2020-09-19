---
layout: page
title: Laravel Lexicon
permalink: /
---

# Laravel Lexicon
![Laravel Lexicon Logo](assets/img/logo/android-chrome-512x512.png)

This site explains most of the technical programming terms and concepts you will need as a PHP/Laravel developer.

<div class="section-index">
    <hr class="panel-line">
    {% for post in site.docs  %}        
    &bull; <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
    {% endfor %}
</div>
