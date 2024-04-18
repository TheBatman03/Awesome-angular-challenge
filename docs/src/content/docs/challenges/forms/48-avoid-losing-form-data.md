---
title: 🟠 Avoid losing form data
description: Challenge 48 is about Bob 🧙‍♂️ the product owner, he wants to develop a new feature in response to customer complaints about losing form input information.
author: timothy-alcaide
contributors:
  - alcaidio
  - svenson95
challengeNumber: 48
command: avoid-losing-form-data
sidebar:
  order: 121
  badge: New
---

## Context

As a member of the development team, you need to address a specific request from the product owner, 🧙‍♂️ Bob. He wants to develop a new feature in response to customer complaints about losing form input information.

## User Story

Here's the feature expressed as a user story with a functional expectation:

> As a user, I would like to have an alert dialog box that appears when
> I attempt to navigate away from the page, after I have started
> entering information into the form.

## Acceptance Criteria

1. If one of the form fields is not empty and the user tries to navigate to a different route or page, or wants to reload the page, show an alert dialog to _avoid losing form data_.

2. The content of `dialog.component.ts` must be used for your alert.
3. The appearance and behavior of the alert dialog must comply with W3C conventions, see [alert dialog pattern](https://www.w3.org/WAI/ARIA/apg/patterns/alertdialog/).
4. Maximize the use of the new concepts and syntax in the latest version of Angular.

<details>
    <summary>Tips 🤫 if you really need it and after careful consideration ...</summary>
    * Use the [Material CDK](https://material.angular.io/cdk/) Dialog or Overlay - dont forget to add `@import '@angular/cdk/overlay-prebuilt.css'` in `styles.scss`.
    * Use the [CanDeactivate](https://angular.io/api/router/CanDeactivate) guard in the new functional approach.
</details>
