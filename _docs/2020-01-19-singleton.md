---
layout: post
title: Singleton
subtitle: 
description: ensures that a class has only one instance, while providing a global access point to this instance.
image: /assets/img/unsplash/singleton.jpg
category: php
tags:
  - class
author: pforret
---

## Definition

> A Singleton is a creational design pattern that lets you ensure that a class has only one instance, while providing a global access point to this instance. &bull; [refactoring.guru](https://refactoring.guru/design-patterns/singleton)

All implementations of the Singleton have these two steps in common:

* Make the default constructor private, to prevent other objects from using the new operator with the Singleton class.
* Create a static creation method that acts as a constructor. Under the hood, this method calls the private constructor to create an object and saves it in a static field. All following calls to this method return the cached object.



## Usage



## Examples

	$this->app->singleton('HelpSpot\API', function ($app) {
	    return new \HelpSpot\API($app->make('HttpClient'));
	});


## References

* [Refactoring Guru: Singleton](https://refactoring.guru/design-patterns/singleton)
* [phpenthusiast: Singleton Design Pattern](https://phpenthusiast.com/blog/the-singleton-design-pattern-in-php)
* [Design Patterns: Singleton](https://designpatternsphp.readthedocs.io/en/latest/Creational/Singleton/README.html)
