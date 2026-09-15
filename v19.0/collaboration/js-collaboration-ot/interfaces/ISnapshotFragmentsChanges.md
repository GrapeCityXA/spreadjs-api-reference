# Interface: ISnapshotFragmentsChanges<S\>

## Type parameters

| Name | Type |
| :------ | :------ |
| `S` | `unknown` |

## Table of contents

### Properties

- [createFragments](ISnapshotFragmentsChanges.md#createfragments)
- [deleteFragments](ISnapshotFragmentsChanges.md#deletefragments)
- [deleteSnapshot](ISnapshotFragmentsChanges.md#deletesnapshot)
- [setSnapshotFragments](ISnapshotFragmentsChanges.md#setsnapshotfragments)
- [updateFragments](ISnapshotFragmentsChanges.md#updatefragments)

## Properties

### <a id="createfragments" name="createfragments"></a> createFragments

• `Optional` **createFragments**: `Object`

#### Index signature

▪ [key: `string`]: `S`

___

### <a id="deletefragments" name="deletefragments"></a> deleteFragments

• `Optional` **deleteFragments**: `string`[]

___

### <a id="deletesnapshot" name="deletesnapshot"></a> deleteSnapshot

• `Optional` **deleteSnapshot**: `boolean`

完全删除所有快照片段。

___

### <a id="setsnapshotfragments" name="setsnapshotfragments"></a> setSnapshotFragments

• `Optional` **setSnapshotFragments**: `Object`

完全替换所有快照片段。

#### Index signature

▪ [key: `string`]: `S`

___

### <a id="updatefragments" name="updatefragments"></a> updateFragments

• `Optional` **updateFragments**: `Object`

#### Index signature

▪ [key: `string`]: `S`
