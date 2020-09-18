---
date: 2020-01-06 12:26:40
layout: post
title: Facade
subtitle: 
description: design pattern that provides a simplified (but limited) interface to a complex system of classes, library or framework
image: /assets/img/unsplash/facade.jpg
category: php
tags:
  - class
author: pforret
---

## Definition

> Facade is a structural design pattern that provides a simplified (but limited) interface to a complex system of classes, library or framework. &bull; [refactoring.guru](https://refactoring.guru/design-patterns/facade)


## Usage

A facade is a class that provides a simple interface to a complex subsystem which contains lots of moving parts. A facade might provide limited functionality in comparison to working with the subsystem directly. However, it includes only those features that clients really care about.

Having a facade is handy when you need to integrate your app with a sophisticated library that has dozens of features, but you just need a tiny bit of its functionality.

For instance, an app that uploads short funny videos with cats to social media could potentially use a professional video conversion library. However, all that it really needs is a class with the single method encode(filename, format). After creating such a class and connecting it with the video conversion library, you’ll have your first facade.

## Examples




## References

* [Laravel Docs: Facades](https://laravel.com/docs/8.x/facades)
* [Refactoring Guru: Facade](https://refactoring.guru/design-patterns/facade/)
* [Design Patterns: Facade](https://designpatternsphp.readthedocs.io/en/latest/Structural/Facade/README.html)