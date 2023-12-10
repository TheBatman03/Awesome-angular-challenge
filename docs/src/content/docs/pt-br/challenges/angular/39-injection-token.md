---
title: 🟠 InjectionToken
description: Desafio 39 é sobre aprender o poder da injenção de dependências
author: thomas-laforge
challengeNumber: 39
command: angular-injection-token
sidebar:
  order: 118
  badge: New
---

## Informação

In this small application, we start with a `VideoComponent` containing a **1-second** timer. The development team decided to use a global constant to store the timer value: `DEFAULT_TIMER`. However, a few weeks later, the product team wants to add a new screen for phone calls called `PhoneComponent`, and we want to reuse the `TimerComponent`. However, the product team wants a timer of **2 seconds**. How can we achieve this?

## Statement

Currently, the timer is still 1 second for the `PhoneComponent`. The goal of this challenge is to change the timer value to 2 seconds for the `PhoneComponent`.

## Constraints

The use of `@Input` is forbidden. This example is basic, and using `@Input` could be a good option, but in more complex applications, the component we need to update can be deeply nested, making the use of `@Input` a really bad design.

## Hint

<details>
  <summary>Dica 1</summary>

Looking at this [blog post](https://itnext.io/stop-being-scared-of-injectiontokens-ab22f72f0fe9) can be of great help.

</details>
