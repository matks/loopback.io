---
lang: en
title: 'API docs: context.context.get_1'
keywords: LoopBack 4.0, LoopBack 4, Node.js, TypeScript, OpenAPI
sidebar: lb4_sidebar
editurl: https://github.com/loopbackio/loopback-next/tree/master/packages/context
permalink: /doc/en/lb4/apidocs.context.context.get_1.html
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@loopback/context](./context.md) &gt; [Context](./context.context.md) &gt; [get](./context.context.get_1.md)

## Context.get() method

Get the value bound to the given key, optionally return a (deep) property of the bound value.

<b>Signature:</b>

```typescript
get<ValueType>(keyWithPath: BindingAddress<ValueType>, options: ResolutionOptions): Promise<ValueType | undefined>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  keyWithPath | [BindingAddress](./context.bindingaddress.md)<!-- -->&lt;ValueType&gt; | The binding key, optionally suffixed with a path to the (deeply) nested property to retrieve. |
|  options | [ResolutionOptions](./context.resolutionoptions.md) | Options for resolution. |

<b>Returns:</b>

Promise&lt;ValueType \| undefined&gt;

A promise of the bound value, or a promise of undefined when the optional binding is not found.

## Example


```ts
// get "rest" property from the value bound to "config"
// use `undefined` when no config is provided
const config = await ctx.get<RestComponentConfig>('config#rest', {
  optional: true
});
```


