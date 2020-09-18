---
layout: post
title: Ternary Operator
subtitle:
description: "$condition ? $if_true : $if_false"
image: /assets/img/unsplash/ternary_operator.jpg
category: php
tags:
  - ifthen
  - ternary
  - operator
  - conditional
author: pforret
---
## Definition

> The expression `(expr1) ? (expr2) : (expr3)` evaluates to expr2 if expr1 does not evaluate to FALSE, and expr3 if expr1 evaluates to FALSE.
> Since PHP 5.3, it is possible to leave out the middle part of the ternary operator. 
> Expression `expr1 ?: expr3` (_short-hand ternary_) returns expr1 if expr1 evaluates to TRUE, and  expr3 otherwise. &bull; [php.net](https://www.php.net/manual/en/language.operators.comparison.php)

#### Aliases 

* _(expr1) ? (expr2) : (expr3)_ : [conditional operator, inline if (iif), or ternary if](https://en.wikipedia.org/wiki/%3F:)
* _expr1 ?: expr3_ : [Elvis operator](https://en.wikipedia.org/wiki/Elvis_operator)

### Usage

It is a shorter form of if-then-else, easily written in one line.
 
## Examples

    $result = $is_singular ? 'word' : 'words';      // normal ternary operator
    
    $title = $specified_title ?: $default_title ;   // shorthand ternary operator
        // which is equivalent to 
    $title = $specified_title != false ? $specified_title : $default_title    

## References

* [PHP Docs: Comparison Operators](https://www.php.net/manual/en/language.operators.comparison.php)
* [Shorthand comparisons in PHP](https://stitcher.io/blog/shorthand-comparisons-in-php)