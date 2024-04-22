---
title: 🟠 Hold to save button
description: You're tasked with implementing Lucie's button design, requiring holding it for a set time to save, taking over from Sacha; functionalities include configuring duration, countdown initiation on "mousedown", progress bar reset on "mouseleave" or "mouseup", reflecting remaining time, and simulating save request on hold completion, using RxJS operators and ensuring declarative code.
author: timothy-alcaide
contributors:
  - alcaidio
challengeNumber: 49
command: rxjs-hold-to-save-btn
sidebar:
  order: 19
  badge: New
---

## Context

As a member of the development team, you have to respond to a specific request from the UX designer, 👩🏻‍🎨 Lucie, who has designed a button that must be held down for X amount of time to save a save request.

Sacha 👶🏼 the trainee has already integrated the design but doesn't know how to perform the "holdable" functionality.

So you're going to take over from him.

## Functional expectation

> "As a user, I would like to save something by holding down the button for a certain amount of time."

Here the prototype made by Lucie :

![prototype gif](../../../../../../docs/src/assets/rxjs/49/prototype.gif)

## Acceptance Criteria

1. We should be able to configure a maintenance duration in milliseconds.
2. Pressing and holding the button triggers the countdown on "mousedown" event.
3. On "mouseleave" or "mouseup" events, the progress bar is reset to 0.
4. The progress bar representing the remaining relative time should reflect the remaining time.
5. Simulates a backup request when the hold time is over (console log or alert).
6. You must maximize the use of RxJS operators and be as declarative as possible.

<details>
    <summary>Tips 🤫 (if you really need it and after careful consideration)</summary>
    <ul>
      <li>Create the `HolddableDirective`</li>
      <li>Use `TemplateRef` and `fromEvent` from rxjs to catch events OR `@HostListener`</li>
      <li>Perhaps the following rxjs operators can help you: interval, takeUntil, switchmap, takeWhile/retry...</li>
    </ul>
</details>
