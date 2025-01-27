---
lang: en
title: 'API docs: context.comparebindingsbytag'
keywords: LoopBack 4.0, LoopBack 4, Node.js, TypeScript, OpenAPI
sidebar: lb4_sidebar
editurl: https://github.com/loopbackio/loopback-next/tree/master/packages/context
permalink: /doc/en/lb4/apidocs.context.comparebindingsbytag.html
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@loopback/context](./context.md) &gt; [compareBindingsByTag](./context.comparebindingsbytag.md)

## compareBindingsByTag() function

Creates a binding compare function to sort bindings by tagged phase name.

<b>Signature:</b>

```typescript
export declare function compareBindingsByTag(phaseTagName?: string, orderOfPhases?: (string | symbol)[]): BindingComparator;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  phaseTagName | string | <i>(Optional)</i> Name of the binding tag for phase |
|  orderOfPhases | (string \| symbol)\[\] | <i>(Optional)</i> An array of phase names as the predefined order |

<b>Returns:</b>

[BindingComparator](./context.bindingcomparator.md)

## Remarks

Two bindings are compared as follows:

1. Get values for the given tag as `phase` for bindings, if the tag is not present, default `phase` to `''`<!-- -->. 2. If both bindings have `phase` value in `orderOfPhases`<!-- -->, honor the order specified by `orderOfPhases`<!-- -->. 3. If a binding's `phase` does not exist in `orderOfPhases`<!-- -->, it comes before the one with `phase` exists in `orderOfPhases`<!-- -->. 4. If both bindings have `phase` value outside of `orderOfPhases`<!-- -->, they are ordered by phase names alphabetically and symbol values come before string values.


