---
layout: post
title: Closure
subtitle: 
description: function($object) use ($parameter) {...}
image: /assets/img/unsplash/closure.jpg
category: php
tags:
  - function
  - anonymous
  - callback
author: pforret
---


## Definition

A closure is an [anonymous function](/anonymous-function) that can access variables imported from the outside scope without using any global variables. Theoretically, a closure is a function with some arguments closed (e.g. fixed) by the environment when it is defined. Closures can work around variable scope restrictions in a clean way.

## Usage


## Examples

    $callback =
        function ($quantity, $product) use ($tax, &$total)
        {
            $pricePerItem = constant(__CLASS__ . "::PRICE_" . strtoupper($product));
            $total += ($pricePerItem * $quantity) * ($tax + 1.0);
        };
        array_walk($this->products, $callback);

or

    function handle(Closure $closure) {
        $closure();
    }
    handle(function(){
        echo 'Hello!';
    });


## References

* [What are PHP Lambdas and Closures?](https://culttt.com/2013/03/25/what-are-php-lambdas-and-closures/)
* [PHP Docs: Anonymous functions](https://www.php.net/manual/en/functions.anonymous.php)
* [What is Closure in Laravel](https://stackoverflow.com/questions/47348081/what-is-closure-in-laravel)