# Interface: IDocReceiveMiddlewareContext<T\>

当文档收到来自客户端的消息时的上下文。

## Type parameters

| Name |
| :------ |
| `T` |

## Hierarchy

- [`IDocMiddlewareContextBase`](IDocMiddlewareContextBase.md)

  ↳ **`IDocReceiveMiddlewareContext`**

## Table of contents

### Properties

- [connection](IDocReceiveMiddlewareContext.md#connection)
- [request](IDocReceiveMiddlewareContext.md#request)

## Properties

### <a id="connection" name="connection"></a> connection

• `Optional` **connection**: `Connection`

#### Inherited from

[IDocMiddlewareContextBase](IDocMiddlewareContextBase.md).[connection](IDocMiddlewareContextBase.md#connection)

___

### <a id="request" name="request"></a> request

• **request**: [`IRequestMessage`](IRequestMessage.md)<`T`\>
