# Interface: IDocSubmitMiddlewareContext<S, T\>

当发起提交操作时的上下文。

## Type parameters

| Name |
| :------ |
| `S` |
| `T` |

## Hierarchy

- [`IDocMiddlewareContextBase`](IDocMiddlewareContextBase.md)

  ↳ **`IDocSubmitMiddlewareContext`**

## Table of contents

### Properties

- [connection](IDocSubmitMiddlewareContext.md#connection)
- [request](IDocSubmitMiddlewareContext.md#request)

## Properties

### <a id="connection" name="connection"></a> connection

• `Optional` **connection**: `Connection`

#### Inherited from

[IDocMiddlewareContextBase](IDocMiddlewareContextBase.md).[connection](IDocMiddlewareContextBase.md#connection)

___

### <a id="request" name="request"></a> request

• **request**: [`SubmitRequest`](../classes/SubmitRequest.md)<`S`, `T`\>
