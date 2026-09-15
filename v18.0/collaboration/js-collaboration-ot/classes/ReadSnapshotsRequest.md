# Class: ReadSnapshotsRequest<S\>

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

___

### <a id="snapshots" name="snapshots"></a> snapshots

• **snapshots**: [`ISnapshot`](../interfaces/ISnapshot.md)<`S`\>[]

## Methods

### <a id="rejectsnapshotreadsilent" name="rejectsnapshotreadsilent"></a> rejectSnapshotReadSilent

▸ **rejectSnapshotReadSilent**(`snapshot`, `errorMessage`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `snapshot` | [`ISnapshot`](../interfaces/ISnapshot.md)<`S`\> |
| `errorMessage` | `string` |

#### Returns

`void`
