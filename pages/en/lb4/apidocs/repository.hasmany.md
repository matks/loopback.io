---
lang: en
title: 'API docs: repository.hasmany'
keywords: LoopBack 4.0, LoopBack 4, Node.js, TypeScript, OpenAPI
sidebar: lb4_sidebar
editurl: https://github.com/loopbackio/loopback-next/tree/master/packages/repository
permalink: /doc/en/lb4/apidocs.repository.hasmany.html
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@loopback/repository](./repository.md) &gt; [hasMany](./repository.hasmany.md)

## hasMany() function

Decorator for hasMany Calls property.array decorator underneath the hood and infers foreign key name from target model name unless explicitly specified

<b>Signature:</b>

```typescript
export declare function hasMany<T extends Entity>(targetResolver: EntityResolver<T>, definition?: Partial<HasManyDefinition>): (decoratedTarget: object, key: string) => void;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  targetResolver | [EntityResolver](./repository.entityresolver.md)<!-- -->&lt;T&gt; | Target model for hasMany relation |
|  definition | Partial&lt;[HasManyDefinition](./repository.hasmanydefinition.md)<!-- -->&gt; | <i>(Optional)</i> Optional metadata for setting up hasMany relation |

<b>Returns:</b>

(decoratedTarget: object, key: string) =&gt; void

A property decorator


