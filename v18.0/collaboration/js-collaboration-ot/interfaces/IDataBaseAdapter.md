# Interface: IDataBaseAdapter<S, T\>

数据库适配器接口。

## Type parameters

| Name | Type |
| :------ | :------ |
| `S` | `unknown` |
| `T` | `unknown` |

## Implemented by

- [`Db`](../classes/Db.md)

## Table of contents

### Methods

- [close](IDataBaseAdapter.md#close)
- [commitOp](IDataBaseAdapter.md#commitop)
- [commitSnapshot](IDataBaseAdapter.md#commitsnapshot)
- [getCommittedOpVersion](IDataBaseAdapter.md#getcommittedopversion)
- [getDocument](IDataBaseAdapter.md#getdocument)
- [getFragment](IDataBaseAdapter.md#getfragment)
- [getFragments](IDataBaseAdapter.md#getfragments)
- [getOps](IDataBaseAdapter.md#getops)
- [getSnapshot](IDataBaseAdapter.md#getsnapshot)

## Methods

### <a id="close" name="close"></a> close

▸ **close**(): `Promise`<`void`\>

关闭数据库。

#### Returns

`Promise`<`void`\>

___

### <a id="commitop" name="commitop"></a> commitOp

▸ **commitOp**(`id`, `op`, `document`, `options?`): `Promise`<`boolean`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `op` | [`IOp`](IOp.md)<`T`\> |
| `document` | [`IDocument`](IDocument.md) |
| `options?` | `unknown` |

#### Returns

`Promise`<`boolean`\>

___

### <a id="commitsnapshot" name="commitsnapshot"></a> commitSnapshot

▸ **commitSnapshot**(`id`, `snapshot`, `options?`): `Promise`<`boolean`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `snapshot` | [`ICommitSnapshot`](ICommitSnapshot.md)<`S`\> |
| `options?` | `unknown` |

#### Returns

`Promise`<`boolean`\>

___

### <a id="getcommittedopversion" name="getcommittedopversion"></a> getCommittedOpVersion

▸ **getCommittedOpVersion**(`id`, `to`, `op`): `Promise`<`undefined` \| `number`\>

获取已提交的操作版本，如果操作已提交，则返回已提交的版本，否则返回 undefined。

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `to` | `number` |
| `op` | [`IOp`](IOp.md)<`unknown`\> |

#### Returns

`Promise`<`undefined` \| `number`\>

___

### <a id="getdocument" name="getdocument"></a> getDocument

▸ **getDocument**(`id`, `options?`): `Promise`<`undefined` \| ``null`` \| [`IDocument`](IDocument.md)\>

通过 ID 获取文档信息。

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `options?` | `unknown` |

#### Returns

`Promise`<`undefined` \| ``null`` \| [`IDocument`](IDocument.md)\>

___

### <a id="getfragment" name="getfragment"></a> getFragment

▸ **getFragment**(`id`, `fragmentId`, `options?`): `Promise`<`undefined` \| ``null`` \| `S`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `fragmentId` | `string` |
| `options?` | `unknown` |

#### Returns

`Promise`<`undefined` \| ``null`` \| `S`\>

___

### <a id="getfragments" name="getfragments"></a> getFragments

▸ **getFragments**(`id`, `fragmentIds?`, `options?`): `Promise`<{ `[id: string]`: `S`;  }\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `fragmentIds?` | `string`[] |
| `options?` | `unknown` |

#### Returns

`Promise`<{ `[id: string]`: `S`;  }\>

___

### <a id="getops" name="getops"></a> getOps

▸ **getOps**(`id`, `from`, `to?`, `options?`): `Promise`<[`IOp`](IOp.md)<`T`\>[]\>

获取两个版本之间的操作，包含起始版本，不包含结束版本。

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `from` | `number` |
| `to?` | `number` |
| `options?` | `unknown` |

#### Returns

`Promise`<[`IOp`](IOp.md)<`T`\>[]\>

___

### <a id="getsnapshot" name="getsnapshot"></a> getSnapshot

▸ **getSnapshot**(`id`, `options?`): `Promise`<`undefined` \| ``null`` \| [`ISnapshot`](ISnapshot.md)<`S`\>\>

通过 ID 获取快照。

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `options?` | `unknown` |

#### Returns

`Promise`<`undefined` \| ``null`` \| [`ISnapshot`](ISnapshot.md)<`S`\>\>
