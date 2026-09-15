# Interface: IMilestoneDataBaseAdapter<S\>

里程碑数据库适配器接口。

## Type parameters

| Name |
| :------ |
| `S` |

## Table of contents

### Properties

- [interval](IMilestoneDataBaseAdapter.md#interval)

### Methods

- [getMilestoneSnapshot](IMilestoneDataBaseAdapter.md#getmilestonesnapshot)
- [saveMilestoneSnapshot](IMilestoneDataBaseAdapter.md#savemilestonesnapshot)

## Properties

### <a id="interval" name="interval"></a> interval

• **interval**: `number`

保存里程碑快照的时间间隔。
默认值为 1000。

## Methods

### <a id="getmilestonesnapshot" name="getmilestonesnapshot"></a> getMilestoneSnapshot

▸ **getMilestoneSnapshot**(`id`, `version`): `Promise`<`undefined` \| [`ISnapshot`](ISnapshot.md)<`S`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `version` | `number` |

#### Returns

`Promise`<`undefined` \| [`ISnapshot`](ISnapshot.md)<`S`\>\>

___

### <a id="savemilestonesnapshot" name="savemilestonesnapshot"></a> saveMilestoneSnapshot

▸ **saveMilestoneSnapshot**(`snapshot`): `Promise`<`boolean`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `snapshot` | [`ISnapshot`](ISnapshot.md)<`S`\> |

#### Returns

`Promise`<`boolean`\>
