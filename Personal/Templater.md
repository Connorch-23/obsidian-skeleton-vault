---
title: "Introduction - Templater"
source: "https://silentvoid13.github.io/Templater/introduction.html"
author:
published:
created: 2025-04-30
description:
tags:
  - "clippings"
---
[Templater](https://github.com/SilentVoid13/Templater) is a template language that lets you insert **variables** and **functions** results into your notes. It will also let you execute JavaScript code manipulating those variables and functions.

With [Templater](https://github.com/SilentVoid13/Templater), you will be able to create powerful templates to automate manual tasks.

The following template file, that is using [Templater](https://github.com/SilentVoid13/Templater) syntax:

```javascript
---
creation date: 2025-04-30 12:12
modification date: Wednesday 30th April 2025 12:12:33
---

<< [[2025-04-29]] | [[2025-05-01]] >>

# Introduction - Templater

> [!quote] Minds are like parachutes. They only function when open.
> — Thomas Dewar
```

Will produce the following result when inserted:

```javascript
---
creation date: 2021-01-07 17:20
modification date: Thursday 7th January 2021 17:20:43
---

<< [[2021-04-08]] | [[2021-04-10]] >>

# Test Test

> Do the best you can until you know better. Then when you know better, do better.
> &mdash; <cite>Maya Angelou</cite>
```