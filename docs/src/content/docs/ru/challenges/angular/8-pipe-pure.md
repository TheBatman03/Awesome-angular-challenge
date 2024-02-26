---
title: 🟢Чистый пайп
description: Испытание 8 про создание чистого пайпа
author: thomas-laforge
challengeNumber: 8
command: angular-pipe-easy
blogLink: https://medium.com/ngconf/deep-dive-into-angular-pipes-c040588cd15d
sidebar:
  order: 3
---

## Информация

This is the first of three `@Pipe()` challenges, the goal of this series is to master **pipes** in Angular.
Это первое испытание про `@Pipe()` из трех, цель этой серии испытаний - освоить работу с **pipes** в Angular.

Пайпы - удобный способ трансформации данных в вашем шаблоне. Разница между вызовом функции и пайпом заключается в том, что результат, возвращаемый чистыми пайпами, кэшируется. Таким образом, они не будут пересчитываться при каждом цикле обнаружения изменений, если их входные значения не изменились.

Pipes разработаны так, чтобы быть эффективными и оптимизированными для производительности. Они используют механизмы обнаружения изменений, чтобы пересчитывать значение только в случае изменения входных данных, минимизируя ненужные вычисления и улучшая производительность рендеринга.

По умолчанию пайпы чистые, но вы должны знать, что установка `pure` в false может привести к неэффективности, поскольку это увеличивает количество перерисовок.

:::note[Примечание]
**Чистые** пайп вызывается только когда изменяется входное значение.\
**Нечистый** пайп вызывается на каждый цикл обнаружения изменений.
:::

Существуют несколько полезных предопределенных пайпов, таких как DatePipe, UpperCasePipe и CurrencyPipe. Чтобы узнать больше о пайпах в Angular, ознакомьтесь с документацией API [здесь](https://angular.io/guide/pipes).

## Пояснение

В этом упражнении необходимо превратить вызов функции в шаблоне в использование пайпа.

## Ограничение

- Пайп должен быть типизирован.