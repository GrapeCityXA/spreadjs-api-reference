# Interface: IDocReadOpMiddlewareContext<T\>

当从数据库加载操作时的上下文。

## Type parameters

| Name |
| :------ |
| `T` |

## Hierarchy

- [`IDocMiddlewareContextBase`](IDocMiddlewareContextBase.md)

  ↳ **`IDocReadOpMiddlewareContext`**

## Table of contents

### Properties

- [connection](IDocReadOpMiddlewareContext.md#connection)
- [request](IDocReadOpMiddlewareContext.md#request)

## Properties

### <a id="connection" name="connection"></a> connection

• `Optional` **connection**: `Connection`

#### Inherited from

[IDocMiddlewareContextBase](IDocMiddlewareContextBase.md).[connection](IDocMiddlewareContextBase.md#connection)

___

### <a id="request" name="request"></a> request

• **request**: [`IReadOpRequest`](IReadOpRequest.md)<`T`\>
