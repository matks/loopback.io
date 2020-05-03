---
lang: en
title: 'API docs: authorization.authorizationoptions'
keywords: LoopBack 4.0, LoopBack 4
sidebar: lb4_sidebar
editurl: https://github.com/strongloop/loopback-next/tree/master/packages/authorization
permalink: /doc/en/lb4/apidocs.authorization.authorizationoptions.html
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@loopback/authorization](./authorization.md) &gt; [AuthorizationOptions](./authorization.authorizationoptions.md)

## AuthorizationOptions interface

<b>Signature:</b>

```typescript
export interface AuthorizationOptions 
```

## Properties

|  Property | Type | Description |
|  --- | --- | --- |
|  [defaultDecision](./authorization.authorizationoptions.defaultdecision.md) | <code>AuthorizationDecision.DENY &#124; AuthorizationDecision.ALLOW</code> | Default decision if all authorizers vote for ABSTAIN If not set, default to <code>AuthorizationDecision.DENY</code> |
|  [defaultMetadata](./authorization.authorizationoptions.defaultmetadata.md) | <code>AuthorizationMetadata</code> | Default authorization metadata if a method is not decorated with <code>@authorize</code>. If not set, no authorization will be enforced for those methods that are not associated with authorization metadata. |
|  [precedence](./authorization.authorizationoptions.precedence.md) | <code>AuthorizationDecision.DENY &#124; AuthorizationDecision.ALLOW</code> | Controls if Allow/Deny vote takes precedence and override other votes. If not set, default to <code>AuthorizationDecision.DENY</code>.<!-- -->Once a vote matches the <code>precedence</code>, it becomes the final decision. The rest of votes will be skipped. |

