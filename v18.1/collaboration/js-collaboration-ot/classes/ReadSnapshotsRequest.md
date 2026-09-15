# Class: ReadSnapshotsRequest<S\>

当从数据库加载一个或多个快照用于 fetch 或 subscribe 操作时的上下文。

**`param`** 要读取的快照。

**`param`** 要读取的快照类型。

## Type parameters

| Name |
| :------ |
| `S` |

## Table of contents

### Constructors

- [constructor](ReadSnapshotsRequest.md#constructor)

### Properties

- [snapshotType](ReadSnapshotsRequest.md#snapshottype)
- [snapshots](ReadSnapshotsRequest.md#snapshots)

### Methods

- [rejectSnapshotReadSilent](ReadSnapshotsRequest.md#rejectsnapshotreadsilent)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new ReadSnapshotsRequest**<`S`\>()

#### Type parameters

| Name |
| :------ |
| `S` |

## Properties

### <a id="snapshottype" name="snapshottype"></a> snapshotType

• **snapshotType**: [`SnapshotTypes`](../README.md#snapshottypes)

要读取的快照类型。

___

### <a id="snapshots" name="snapshots"></a> snapshots

• **snapshots**: [`ISnapshot`](../interfaces/ISnapshot.md)<`S`\>[]

要读取的快照。

## Methods

### <a id="rejectsnapshotreadsilent" name="rejectsnapshotreadsilent"></a> rejectSnapshotReadSilent

▸ **rejectSnapshotReadSilent**(`snapshot`, `errorMessage`): `void`

拒绝读取一个特定的快照，防止其数据被发送到客户端。
设置一个特殊的错误代码，避免将错误传递给用户代码，同时仍然执行取消订阅等操作。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `snapshot` | [`ISnapshot`](../interfaces/ISnapshot.md)<`S`\> | 要拒绝的快照。 |
| `errorMessage` | `string` | 拒绝的原因。 |

#### Returns

`void`
