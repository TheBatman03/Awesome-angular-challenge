---
title: 🔴 Typed ContextOutlet
description: Challenge 4 is about strongly typing ngContextOutlet directives
author: thomas-laforge
contributors:
  - tomalaforge
  - tomer953
  - svenson95
  - jdegand
challengeNumber: 4
command: angular-context-outlet-type
blogLink: https://medium.com/@thomas.laforge/ngtemplateoutlet-type-checking-5d2dcb07a2c6
sidebar:
  order: 201
---

## Information

You can improve template type checking for custom directives by adding template guard properties to your directive definition. Angular offer the static function [`ngTemplateContextGuard`](https://angular.io/guide/structural-directives#typing-the-directives-context) to strongly type structural directives.

However the context of **NgTemplateOutlet** type is **Object**. But with the help of the above guard, we can improve that behavior.

If you’re not very familiar with `ngTemplateOutlet`, check out this article.

- [NgTemplateOutlet Type Checking](https://medium.com/@thomas.laforge/ngtemplateoutlet-type-checking-5d2dcb07a2c6)

## Statement

In this exercise we want to learn how to strongly type our `ng-template` in our `AppComponent`.

This exercise has two levels of complexity.

### Level 1: Known Interface

Currently we have the following piece of code.

![Unkown Person](../../../../assets/4/unknown-person.png 'Unkown Person')

As we can see `name` is of type `any`. We want to infer the correct type using a custom directive `PersonDirective`.

### Level 2: Generic Interface

Currently we have the following piece of code.

![Unkown Student](../../../../assets/4/unknown-student.png 'Unkown Student')

As we can see `student` is of type `any`. We want to infer the correct type using a custom directive `ListDirective`.

But in this part, we want to pass a list of **any object** to `ListComponent`. And we still want the correct type to be inferred.
