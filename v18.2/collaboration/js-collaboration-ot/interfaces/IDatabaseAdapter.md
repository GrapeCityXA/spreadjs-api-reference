# Interface: IDatabaseAdapter<S, T\>

定义操作转换中的数据库适配器接口。

## Type parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `S` | `unknown` | 快照数据的类型。 |
| `T` | `unknown` | 操作数据的类型。 |

## Implemented by

- [`Db`](../classes/Db.md)

## Table of contents

### Methods

- [close](IDatabaseAdapter.md#close)
- [commitOp](IDatabaseAdapter.md#commitop)
- [commitSnapshot](IDatabaseAdapter.md#commitsnapshot)
- [getCommittedOpVersion](IDatabaseAdapter.md#getcommittedopversion)
- [getDocument](IDatabaseAdapter.md#getdocument)
- [getFragment](IDatabaseAdapter.md#getfragment)
- [getFragments](IDatabaseAdapter.md#getfragments)
- [getOps](IDatabaseAdapter.md#getops)
- [getSnapshot](IDatabaseAdapter.md#getsnapshot)

## Methods

### <a id="close" name="close"></a> close

▸ **close**(): `Promise`<`void`\>

关闭数据库连接。

#### Returns

`Promise`<`void`\>

一个 Promise，当数据库被关闭时， Promise 被解决。

___

### <a id="commitop" name="commitop"></a> commitOp

▸ **commitOp**(`id`, `op`, `document`, `options?`): `Promise`<`boolean`\>

将一个操作提交到数据库。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | 文档的 ID。 |
| `op` | [`IOp`](IOp.md)<`T`\> | 要提交的操作。 |
| `document` | [`IDocument`](IDocument.md) | 文档元数据。 |
| `options?` | `unknown` | - |

#### Returns

`Promise`<`boolean`\>

一个 Promise，当操作被提交时， Promise 被解决。

___

### <a id="commitsnapshot" name="commitsnapshot"></a> commitSnapshot

▸ **commitSnapshot**(`id`, `snapshot`, `options?`): `Promise`<`boolean`\>

将一个快照提交到数据库。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | 文档的 ID。 |
| `snapshot` | [`ICommitSnapshot`](ICommitSnapshot.md)<`S`\> | 要提交的快照。 |
| `options?` | `unknown` | - |

#### Returns

`Promise`<`boolean`\>

一个 Promise，当快照被提交时， Promise 被解决。

___

### <a id="getcommittedopversion" name="getcommittedopversion"></a> getCommittedOpVersion

▸ **getCommittedOpVersion**(`id`, `to`, `op`): `Promise`<`undefined` \| `number`\>

检索已提交操作的版本，如果存在。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | 文档的 ID。 |
| `to` | `number` | 要检查的结束版本。 |
| `op` | [`IOp`](IOp.md)<`unknown`\> | 要验证的操作。 |

#### Returns

`Promise`<`undefined` \| `number`\>

一个 Promise，当操作被提交时， Promise 被解决。

___

### <a id="getdocument" name="getdocument"></a> getDocument

▸ **getDocument**(`id`, `options?`): `Promise`<`undefined` \| ``null`` \| [`IDocument`](IDocument.md)\>

通过 ID 检索文档信息。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | 文档的 ID。 |
| `options?` | `unknown` | - |

#### Returns

`Promise`<`undefined` \| ``null`` \| [`IDocument`](IDocument.md)\>

一个 Promise，在文档信息被检索后，文档信息被检索。

___

### <a id="getfragment" name="getfragment"></a> getFragment

▸ **getFragment**(`id`, `fragmentId`, `options?`): `Promise`<`undefined` \| ``null`` \| `S`\>

通过 ID 检索文档的特定片段。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | 文档的 ID。 |
| `fragmentId` | `string` | 片段的 ID。 |
| `options?` | `unknown` | - |

#### Returns

`Promise`<`undefined` \| ``null`` \| `S`\>

一个 Promise，在片段数据被检索后，片段数据被检索。

___

### <a id="getfragments" name="getfragments"></a> getFragments

▸ **getFragments**(`id`, `fragmentIds?`, `options?`): `Promise`<{ `[id: string]`: `S`;  }\>

通过 ID 检索文档的多个片段。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | 文档的 ID。 |
| `fragmentIds?` | `string`[] | - |
| `options?` | `unknown` | - |

#### Returns

`Promise`<{ `[id: string]`: `S`;  }\>

>} 一个 Promise，在片段数据被检索后，片段数据被检索。

___

### <a id="getops" name="getops"></a> getOps

▸ **getOps**(`id`, `from`, `to?`, `options?`): `Promise`<[`IOp`](IOp.md)<`T`\>[]\>

检索两个版本之间的操作（包括 'from'，不包括 'to'）。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | 文档的 ID。 |
| `from` | `number` | 起始版本。 |
| `to?` | `number` | - |
| `options?` | `unknown` | - |

#### Returns

`Promise`<[`IOp`](IOp.md)<`T`\>[]\>

一个 Promise，在操作数组被检索后，操作数组被检索。

___

### <a id="getsnapshot" name="getsnapshot"></a> getSnapshot

▸ **getSnapshot**(`id`, `options?`): `Promise`<`undefined` \| ``null`` \| [`ISnapshot`](ISnapshot.md)<`S`\>\>

通过 ID 检索文档的快照。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | 文档的 ID。 |
| `options?` | `unknown` | - |

#### Returns

`Promise`<`undefined` \| ``null`` \| [`ISnapshot`](ISnapshot.md)<`S`\>\>

一个 Promise，在快照被检索后，快照被检索。
