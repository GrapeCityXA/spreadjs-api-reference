# Interface: ICommitSnapshot<S\>

## Type parameters

| Name | Type |
| :------ | :------ |
| `S` | `unknown` |

## Hierarchy

- [`ISnapshot`](ISnapshot.md)<`S`\>

  ↳ **`ICommitSnapshot`**

## Table of contents

### Properties

- [data](ICommitSnapshot.md#data)
- [fragments](ICommitSnapshot.md#fragments)
- [fragmentsChanges](ICommitSnapshot.md#fragmentschanges)
- [fromVersion](ICommitSnapshot.md#fromversion)
- [id](ICommitSnapshot.md#id)
- [m](ICommitSnapshot.md#m)
- [type](ICommitSnapshot.md#type)
- [v](ICommitSnapshot.md#v)

## Properties

### <a id="data" name="data"></a> data

• `Optional` **data**: `S`

#### Inherited from

[ISnapshot](ISnapshot.md).[data](ISnapshot.md#data)

___

### <a id="fragments" name="fragments"></a> fragments

• `Optional` **fragments**: [`ISnapshotFragments`](../README.md#isnapshotfragments)<`unknown`\>

#### Inherited from

[ISnapshot](ISnapshot.md).[fragments](ISnapshot.md#fragments)

___

### <a id="fragmentschanges" name="fragmentschanges"></a> fragmentsChanges

• **fragmentsChanges**: [`ISnapshotFragmentsChanges`](ISnapshotFragmentsChanges.md)<`unknown`\>

___

### <a id="fromversion" name="fromversion"></a> fromVersion

• **fromVersion**: `number`

___

### <a id="id" name="id"></a> id

• **id**: `string`

#### Inherited from

[ISnapshot](ISnapshot.md).[id](ISnapshot.md#id)

___

### <a id="m" name="m"></a> m

• `Optional` **m**: [`ISnapshotMeta`](ISnapshotMeta.md)

#### Inherited from

[ISnapshot](ISnapshot.md).[m](ISnapshot.md#m)

___

### <a id="type" name="type"></a> type

• `Optional` **type**: `string`

#### Inherited from

[ISnapshot](ISnapshot.md).[type](ISnapshot.md#type)

___

### <a id="v" name="v"></a> v

• **v**: `number`

#### Inherited from

[ISnapshot](ISnapshot.md).[v](ISnapshot.md#v)
