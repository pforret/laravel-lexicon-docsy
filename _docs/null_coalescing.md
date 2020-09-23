---
layout: post
title: Null Coalescing operator
subtitle:
description: "$array['value'] ?? $default_value"
image: /assets/img/unsplash/null_coalescing_operator.jpg
category: php
tags:
  - binary
  - operator
  - ifthen
  - conditional
author: pforret
---
## Definition

    $value ?? $default_value;

## Usage

short for `isset($value) ? $value : $default_value;`

## Examples
 
    $width = $parameters['width'] ?? $default_width;
    // which is equivalent to ternary operator
    $width = isset($params['width']) ? $params['width'] : $default_width;

    // chaining is possible
    $width = $params['width'] ?? $params['resize_to'] ?? $default_width;
    
    // null coalescing assignment operator (since PHP 7.4)
    $person['language'] ??= 'en';
    // which is equivalent to
    $person['language'] = $person['language'] ?? 'en';

## References
 
* [Wikipedia: Null coalescing operator](https://en.wikipedia.org/wiki/Null_coalescing_operator)
* [Shorthand comparisons in PHP](https://stitcher.io/blog/shorthand-comparisons-in-php)