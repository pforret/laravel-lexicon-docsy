---
layout: post
title: Arrow Function
subtitle:
description: fn($post) => $post->id
image: /assets/img/unsplash/arrow_function.jpg
category: php
tags:
  - anonymous
  - function
  - closure
  - arrow
  - callback
author: pforret
---
## Definition

> Arrow functions were introduced in PHP 7.4 as a more concise syntax for [anonymous functions](/anonymous-function) &bull; [php.net](https://www.php.net/manual/en/functions.arrow.php)

## Usage

> Besides the obvious advantage of being shorter and more readable than classic anonymous functions, arrow functions can access variables from the parent scope through a technique called "_implicit by-value scope binding_" &bull; [codepunker.com](https://www.codepunker.com/blog/basic-usage-of-closures-in-php)

## Examples
    $posts = [/* … */];
    
    // classic closure 
    $ids = array_map(function ($post) {
            return $post->id;
        }, $posts);
    
    // short closure/arrow function
    $ids = array_map(fn($post) => $post->id, $posts);

## References
* [PHP Docs: Arrow functions](https://www.php.net/manual/en/functions.arrow.php)
* [Arrow functions in PHP 7.4](https://stitcher.io/blog/short-closures-in-php)
* [Basic Usage Of Closures In PHP](https://www.codepunker.com/blog/basic-usage-of-closures-in-php)
