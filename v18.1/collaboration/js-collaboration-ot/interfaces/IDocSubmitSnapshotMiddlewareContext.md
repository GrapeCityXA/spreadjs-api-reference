# Interface: IDocSubmitSnapshotMiddlewareContext<S, T\>

当发起提交快照时的上下文。

## Type parameters

| Name |
| :------ |
| `S` |
| `T` |

## Hierarchy

- [`IDocMiddlewareContextBase`](IDocMiddlewareContextBase.md)

  ↳ **`IDocSubmitSnapshotMiddlewareContext`**

## Table of contents

### Properties

- [connection](IDocSubmitSnapshotMiddlewareContext.md#connection)
- [request](IDocSubmitSnapshotMiddlewareContext.md#request)

## Properties

### <a id="connection" name="connection"></a> connection

• `Optional` **connection**: `Connection`

#### Inherited from

[IDocMiddlewareContextBase](IDocMiddlewareContextBase.md).[connection](IDocMiddlewareContextBase.md#connection)

___

### <a id="request" name="request"></a> request

• **request**: [`SubmitSnapshotRequest`](../classes/SubmitSnapshotRequest.md)<`S`, `T`\>
