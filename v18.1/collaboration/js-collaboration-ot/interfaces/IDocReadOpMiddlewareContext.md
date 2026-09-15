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
- [id](IDocReadOpMiddlewareContext.md#id)
- [op](IDocReadOpMiddlewareContext.md#op)

## Properties

### <a id="connection" name="connection"></a> connection

• `Optional` **connection**: `Connection`

#### Inherited from

[IDocMiddlewareContextBase](IDocMiddlewareContextBase.md).[connection](IDocMiddlewareContextBase.md#connection)

___

### <a id="id" name="id"></a> id

• **id**: `string`

___

### <a id="op" name="op"></a> op

• **op**: [`IOp`](IOp.md)<`T`\>
