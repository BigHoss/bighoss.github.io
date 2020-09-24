---
layout: post
title: ConcurrencyException when db Trigger
tags: ef core, entity framework, csharp
published: true
---

We have a database that sums related datasets to another table.
As Ef tries to insert datasets there was a Exception that there was change in 1 row expected but was 0.

In the trigger there was ```SET NOCOUNT ON``` and because of that the error occured
