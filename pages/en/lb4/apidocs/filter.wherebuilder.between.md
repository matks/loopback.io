---
lang: en
title: 'API docs: filter.wherebuilder.between'
keywords: LoopBack 4.0, LoopBack 4, Node.js, TypeScript, OpenAPI
sidebar: lb4_sidebar
editurl: https://github.com/loopbackio/loopback-next/tree/master/packages/filter
permalink: /doc/en/lb4/apidocs.filter.wherebuilder.between.html
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@loopback/filter](./filter.md) &gt; [WhereBuilder](./filter.wherebuilder.md) &gt; [between](./filter.wherebuilder.between.md)

## WhereBuilder.between() method

Add a `between` condition

<b>Signature:</b>

```typescript
between<K extends KeyOf<MT>>(key: K, val1: MT[K], val2: MT[K]): this;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  key | K | Property name |
|  val1 | MT\[K\] | Property value lower bound |
|  val2 | MT\[K\] | Property value upper bound |

<b>Returns:</b>

this


