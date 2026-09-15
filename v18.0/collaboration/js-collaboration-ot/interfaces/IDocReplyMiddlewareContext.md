# Interface: IDocReplyMiddlewareContext<S, T\>

## Type parameters

| Name |
| :------ |
| `S` |
| `T` |

## Hierarchy

- [`IDocMiddlewareContextBase`](IDocMiddlewareContextBase.md)

  ↳ **`IDocReplyMiddlewareContext`**

## Table of contents

### Properties

- [connection](IDocReplyMiddlewareContext.md#connection)
- [reply](IDocReplyMiddlewareContext.md#reply)
- [request](IDocReplyMiddlewareContext.md#request)

## Properties

### <a id="connection" name="connection"></a> connection

• `Optional` **connection**: `Connection`

#### Inherited from

[IDocMiddlewareContextBase](IDocMiddlewareContextBase.md).[connection](IDocMiddlewareContextBase.md#connection)

___

### <a id="reply" name="reply"></a> reply

• **reply**: [`IReplyMessage`](IReplyMessage.md)<`S`, `T`\>

___

### <a id="request" name="request"></a> request

• **request**: [`IRequestMessage`](IRequestMessage.md)<`T`\>
