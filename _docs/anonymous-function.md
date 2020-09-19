---
layout: post
title: Anonymous function
subtitle: 
description: function($object){ ... }
image: /assets/img/unsplash/anonymous_function.jpg
category: php
tags:
  - function
  - callback
  - anonymous
  - closure
author: pforret
---
## Definition

> Anonymous functions, also known as [closures](/closure), allow the creation of functions which have no specified name. They are most useful as the value of callback parameters (...) &bull; [php.net](https://www.php.net/manual/en/functions.anonymous.php)

## Usage

Typical use is for a lambda or a closure, or anywhere a callback function is required as a parameter of a function.

## Examples

    // anonymous function
	function () {  
		return "Hello world";  
	}  

    // anonymous function with parameter
	function ($name) {  
		return "Hello $name";  
	}  

    // anonymous function with scope inheritance
	function ($name) use ($language) {  
		return $language === 'fr' ? "Bonjour $name" : Hello $name";  
	}  



## References
* <https://www.php.net/manual/en/functions.anonymous.php>
* <https://www.elated.com/php-anonymous-functions/>
