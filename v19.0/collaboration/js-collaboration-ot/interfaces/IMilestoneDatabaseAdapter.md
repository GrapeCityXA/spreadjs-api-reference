# Interface: IMilestoneDatabaseAdapter<S\>

定义里程碑数据库适配器接口。

## Type parameters

| Name |
| :------ |
| `S` |

## Table of contents

### Properties

- [interval](IMilestoneDatabaseAdapter.md#interval)

### Methods

- [getMilestoneSnapshot](IMilestoneDatabaseAdapter.md#getmilestonesnapshot)
- [saveMilestoneSnapshot](IMilestoneDatabaseAdapter.md#savemilestonesnapshot)

## Properties

### <a id="interval" name="interval"></a> interval

• **interval**: `number`

保存里程碑快照的间隔; -1 表示禁用里程碑快照保存。

## Methods

### <a id="getmilestonesnapshot" name="getmilestonesnapshot"></a> getMilestoneSnapshot

▸ **getMilestoneSnapshot**(`id`, `version`): `Promise`<``null`` \| [`ISnapshot`](ISnapshot.md)<`S`\>\>

通过文档 ID 和版本检索一个里程碑快照。

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `version` | `number` |

#### Returns

`Promise`<``null`` \| [`ISnapshot`](ISnapshot.md)<`S`\>\>

___

### <a id="savemilestonesnapshot" name="savemilestonesnapshot"></a> saveMilestoneSnapshot

▸ **saveMilestoneSnapshot**(`snapshot`): `Promise`<`boolean`\>

保存一个里程碑快照。

#### Parameters

| Name | Type |
| :------ | :------ |
| `snapshot` | [`ISnapshot`](ISnapshot.md)<`S`\> |

#### Returns

`Promise`<`boolean`\>
