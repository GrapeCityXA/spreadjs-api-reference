# Interface: IDocReadSnapshotsMiddlewareContext<S\>

当从数据库加载一个或多个快照用于 fetch 或 subscribe 操作时的上下文。

## Type parameters

| Name |
| :------ |
| `S` |

## Hierarchy

- [`IDocMiddlewareContextBase`](IDocMiddlewareContextBase.md)

  ↳ **`IDocReadSnapshotsMiddlewareContext`**

## Table of contents

### Properties

- [connection](IDocReadSnapshotsMiddlewareContext.md#connection)
- [request](IDocReadSnapshotsMiddlewareContext.md#request)

## Properties

### <a id="connection" name="connection"></a> connection

• `Optional` **connection**: `Connection`

#### Inherited from

[IDocMiddlewareContextBase](IDocMiddlewareContextBase.md).[connection](IDocMiddlewareContextBase.md#connection)

___

### <a id="request" name="request"></a> request

• **request**: [`ReadSnapshotsRequest`](../classes/ReadSnapshotsRequest.md)<`S`\>
