# Class: Db<S, T\>

抽象基类实现数据库适配器接口。

## Type parameters

| Name | Description |
| :------ | :------ |
| `S` | 快照数据的类型。 |
| `T` | 操作数据的类型。 |

## Hierarchy

- **`Db`**

  ↳ [`MemoryDb`](MemoryDb.md)

## Implements

- [`IDatabaseAdapter`](../interfaces/IDatabaseAdapter.md)<`S`, `T`\>

## Table of contents

### Constructors

- [constructor](Db.md#constructor)

### Methods

- [close](Db.md#close)
- [commitOp](Db.md#commitop)
- [commitSnapshot](Db.md#commitsnapshot)
- [getCommittedOpVersion](Db.md#getcommittedopversion)
- [getDocument](Db.md#getdocument)
- [getFragment](Db.md#getfragment)
- [getFragments](Db.md#getfragments)
- [getOps](Db.md#getops)
- [getSnapshot](Db.md#getsnapshot)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Db**<`S`, `T`\>()

#### Type parameters

| Name |
| :------ |
| `S` |
| `T` |

## Methods

### <a id="close" name="close"></a> close

▸ `Abstract` **close**(): `Promise`<`void`\>

关闭数据库连接。

#### Returns

`Promise`<`void`\>

一个 Promise，当数据库被关闭时， Promise 被解决。

#### Implementation of

[IDatabaseAdapter](../interfaces/IDatabaseAdapter.md).[close](../interfaces/IDatabaseAdapter.md#close)

___

### <a id="commitop" name="commitop"></a> commitOp

▸ `Abstract` **commitOp**(`id`, `op`, `document`, `options?`): `Promise`<`boolean`\>

将一个操作提交到数据库。

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `op` | [`IOp`](../interfaces/IOp.md)<`T`\> |
| `document` | [`IDocument`](../interfaces/IDocument.md) |
| `options?` | `unknown` |

#### Returns

`Promise`<`boolean`\>

一个 Promise，当操作被提交时， Promise 被解决。

#### Implementation of

[IDatabaseAdapter](../interfaces/IDatabaseAdapter.md).[commitOp](../interfaces/IDatabaseAdapter.md#commitop)

___

### <a id="commitsnapshot" name="commitsnapshot"></a> commitSnapshot

▸ `Abstract` **commitSnapshot**(`id`, `snapshot`, `options?`): `Promise`<`boolean`\>

将一个快照提交到数据库。

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `snapshot` | [`ICommitSnapshot`](../interfaces/ICommitSnapshot.md)<`S`\> |
| `options?` | `unknown` |

#### Returns

`Promise`<`boolean`\>

一个 Promise，当快照被提交时， Promise 被解决。

#### Implementation of

[IDatabaseAdapter](../interfaces/IDatabaseAdapter.md).[commitSnapshot](../interfaces/IDatabaseAdapter.md#commitsnapshot)

___

### <a id="getcommittedopversion" name="getcommittedopversion"></a> getCommittedOpVersion

▸ **getCommittedOpVersion**(`id`, `to`, `op`): `Promise`<`undefined` \| `number`\>

检索已提交操作的版本，如果存在。

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `to` | `number` |
| `op` | [`IOp`](../interfaces/IOp.md)<`object`\> |

#### Returns

`Promise`<`undefined` \| `number`\>

#### Implementation of

[IDatabaseAdapter](../interfaces/IDatabaseAdapter.md).[getCommittedOpVersion](../interfaces/IDatabaseAdapter.md#getcommittedopversion)

___

### <a id="getdocument" name="getdocument"></a> getDocument

▸ `Abstract` **getDocument**(`id`, `options?`): `Promise`<`undefined` \| ``null`` \| [`IDocument`](../interfaces/IDocument.md)\>

通过 ID 检索文档信息。

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `options?` | `unknown` |

#### Returns

`Promise`<`undefined` \| ``null`` \| [`IDocument`](../interfaces/IDocument.md)\>

一个 Promise，在文档信息被检索后，文档信息被检索。

#### Implementation of

[IDatabaseAdapter](../interfaces/IDatabaseAdapter.md).[getDocument](../interfaces/IDatabaseAdapter.md#getdocument)

___

### <a id="getfragment" name="getfragment"></a> getFragment

▸ `Abstract` **getFragment**(`id`, `fragmentId`, `options?`): `Promise`<`undefined` \| ``null`` \| `S`\>

通过 ID 检索文档的特定片段。

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `fragmentId` | `string` |
| `options?` | `unknown` |

#### Returns

`Promise`<`undefined` \| ``null`` \| `S`\>

一个 Promise，在片段数据被检索后，片段数据被检索。

#### Implementation of

[IDatabaseAdapter](../interfaces/IDatabaseAdapter.md).[getFragment](../interfaces/IDatabaseAdapter.md#getfragment)

___

### <a id="getfragments" name="getfragments"></a> getFragments

▸ `Abstract` **getFragments**(`id`, `fragmentIds?`, `options?`): `Promise`<{ `[id: string]`: `S`;  }\>

通过 ID 检索文档的多个片段。

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `fragmentIds?` | `string`[] |
| `options?` | `unknown` |

#### Returns

`Promise`<{ `[id: string]`: `S`;  }\>

>} 一个 Promise，在片段数据被检索后，片段数据被检索。

#### Implementation of

[IDatabaseAdapter](../interfaces/IDatabaseAdapter.md).[getFragments](../interfaces/IDatabaseAdapter.md#getfragments)

___

### <a id="getops" name="getops"></a> getOps

▸ `Abstract` **getOps**(`id`, `from`, `to?`, `options?`): `Promise`<[`IOp`](../interfaces/IOp.md)<`T`\>[]\>

检索两个版本之间的操作（包括 'from'，不包括 'to'）。

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `from` | `number` |
| `to?` | `number` |
| `options?` | `unknown` |

#### Returns

`Promise`<[`IOp`](../interfaces/IOp.md)<`T`\>[]\>

一个 Promise，在操作数组被检索后，操作数组被检索。

#### Implementation of

[IDatabaseAdapter](../interfaces/IDatabaseAdapter.md).[getOps](../interfaces/IDatabaseAdapter.md#getops)

___

### <a id="getsnapshot" name="getsnapshot"></a> getSnapshot

▸ `Abstract` **getSnapshot**(`id`, `options?`): `Promise`<`undefined` \| ``null`` \| [`ISnapshot`](../interfaces/ISnapshot.md)<`S`\>\>

通过 ID 检索文档的快照。

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `options?` | `unknown` |

#### Returns

`Promise`<`undefined` \| ``null`` \| [`ISnapshot`](../interfaces/ISnapshot.md)<`S`\>\>

一个 Promise，在快照被检索后，快照被检索。

#### Implementation of

[IDatabaseAdapter](../interfaces/IDatabaseAdapter.md).[getSnapshot](../interfaces/IDatabaseAdapter.md#getsnapshot)
