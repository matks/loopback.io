---
lang: en
title: 'API docs: repository.buildmodeldefinition'
keywords: LoopBack 4.0, LoopBack 4, Node.js, TypeScript, OpenAPI
sidebar: lb4_sidebar
editurl: https://github.com/loopbackio/loopback-next/tree/master/packages/repository
permalink: /doc/en/lb4/apidocs.repository.buildmodeldefinition.html
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@loopback/repository](./repository.md) &gt; [buildModelDefinition](./repository.buildmodeldefinition.md)

## buildModelDefinition() function

Build model definition from decorations

<b>Signature:</b>

```typescript
export declare function buildModelDefinition(target: Function & {
    definition?: ModelDefinition | undefined;
}, def?: ModelDefinitionSyntax): ModelDefinition;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  target | Function &amp; { definition?: [ModelDefinition](./repository.modeldefinition.md) \| undefined; } | Target model class |
|  def | [ModelDefinitionSyntax](./repository.modeldefinitionsyntax.md) | <i>(Optional)</i> Model definition spec |

<b>Returns:</b>

[ModelDefinition](./repository.modeldefinition.md)


