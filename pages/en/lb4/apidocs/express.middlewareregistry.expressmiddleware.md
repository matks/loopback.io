---
lang: en
title: 'API docs: express.middlewareregistry.expressmiddleware'
keywords: LoopBack 4.0, LoopBack 4
sidebar: lb4_sidebar
editurl: https://github.com/strongloop/loopback-next/tree/master/packages/express
permalink: /doc/en/lb4/apidocs.express.middlewareregistry.expressmiddleware.html
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@loopback/express](./express.md) &gt; [MiddlewareRegistry](./express.middlewareregistry.md) &gt; [expressMiddleware](./express.middlewareregistry.expressmiddleware.md)

## MiddlewareRegistry.expressMiddleware() method

Bind an Express middleware to this server context

<b>Signature:</b>

```typescript
expressMiddleware(key: BindingAddress, middleware: ExpressRequestHandler | ExpressRequestHandler[], options?: MiddlewareBindingOptions): Binding<Middleware>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  key | [BindingAddress](./context.bindingaddress.md) | Middleware binding key |
|  middleware | [ExpressRequestHandler](./express.expressrequesthandler.md) \| [ExpressRequestHandler](./express.expressrequesthandler.md)<!-- -->\[\] | Express middleware handler function(s) |
|  options | [MiddlewareBindingOptions](./express.middlewarebindingoptions.md) |  |

<b>Returns:</b>

[Binding](./context.binding.md)<!-- -->&lt;[Middleware](./express.middleware.md)<!-- -->&gt;

## Example


```ts
import myExpressMiddlewareFactory from 'my-express-middleware';
const myExpressMiddlewareConfig= {};
const myExpressMiddleware = myExpressMiddlewareFactory(myExpressMiddlewareConfig);
server.expressMiddleware('middleware.express.my', myExpressMiddleware);
// Or
server.expressMiddleware('middleware.express.my', [myExpressMiddleware]);

```

