# Class: MemoryDb<S, T\>

## Type parameters

| Name | Type |
| :------ | :------ |
| `S` | `unknown` |
| `T` | `unknown` |

## Hierarchy

- [`Db`](Db.md)<`S`, `T`\>

  ↳ **`MemoryDb`**

## Table of contents

### Constructors

- [constructor](MemoryDb.md#constructor)

### Methods

- [close](MemoryDb.md#close)
- [commitOp](MemoryDb.md#commitop)
- [commitSnapshot](MemoryDb.md#commitsnapshot)
- [getCommittedOpVersion](MemoryDb.md#getcommittedopversion)
- [getDocument](MemoryDb.md#getdocument)
- [getFragment](MemoryDb.md#getfragment)
- [getOps](MemoryDb.md#getops)
- [getSnapshot](MemoryDb.md#getsnapshot)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new MemoryDb**<`S`, `T`\>()

#### Type parameters

| Name | Type |
| :------ | :------ |
| `S` | `unknown` |
| `T` | `unknown` |

#### Inherited from

[Db](Db.md).[constructor](Db.md#constructor)

## Methods

### <a id="close" name="close"></a> close

▸ **close**(): `Promise`<`void`\>

关闭数据库连接。

#### Returns

`Promise`<`void`\>

#### Overrides

[Db](Db.md).[close](Db.md#close)

___

### <a id="commitop" name="commitop"></a> commitOp

▸ **commitOp**(`id`, `op`, `document`): `Promise`<`boolean`\>

将一个操作提交到数据库。

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `op` | [`IOp`](../interfaces/IOp.md)<`T`\> |
| `document` | [`IDocument`](../interfaces/IDocument.md) |

#### Returns

`Promise`<`boolean`\>

#### Overrides

[Db](Db.md).[commitOp](Db.md#commitop)

___

### <a id="commitsnapshot" name="commitsnapshot"></a> commitSnapshot

▸ **commitSnapshot**(`roomId`, `snapshot`): `Promise`<`boolean`\>

将一个快照提交到数据库。

#### Parameters

| Name | Type |
| :------ | :------ |
| `roomId` | `string` |
| `snapshot` | [`ICommitSnapshot`](../interfaces/ICommitSnapshot.md)<`S`\> |

#### Returns

`Promise`<`boolean`\>

#### Overrides

[Db](Db.md).[commitSnapshot](Db.md#commitsnapshot)

___

### <a id="getcommittedopversion" name="getcommittedopversion"></a> getCommittedOpVersion

▸ **getCommittedOpVersion**(`id`, `to`, `op`): `Promise`<``null`` \| `number`\>

检索已提交操作的版本（如果存在）。

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `to` | `number` |
| `op` | [`IOp`](../interfaces/IOp.md)<`object`\> |

#### Returns

`Promise`<``null`` \| `number`\>

#### Inherited from

[Db](Db.md).[getCommittedOpVersion](Db.md#getcommittedopversion)

___

### <a id="getdocument" name="getdocument"></a> getDocument

▸ **getDocument**(`roomId`): `Promise`<``null`` \| [`IDocument`](../interfaces/IDocument.md)\>

通过 ID 检索文档信息。

#### Parameters

| Name | Type |
| :------ | :------ |
| `roomId` | `string` |

#### Returns

`Promise`<``null`` \| [`IDocument`](../interfaces/IDocument.md)\>

#### Overrides

[Db](Db.md).[getDocument](Db.md#getdocument)

___

### <a id="getfragment" name="getfragment"></a> getFragment

▸ **getFragment**(`roomId`, `fragmentId`): `Promise`<``null`` \| { `data`: ``null`` \| `S` ; `version`: `number`  }\>

通过 ID 检索文档的特定片段。

#### Parameters

| Name | Type |
| :------ | :------ |
| `roomId` | `string` |
| `fragmentId` | `string` |

#### Returns

`Promise`<``null`` \| { `data`: ``null`` \| `S` ; `version`: `number`  }\>

#### Overrides

[Db](Db.md).[getFragment](Db.md#getfragment)

___

### <a id="getops" name="getops"></a> getOps

▸ **getOps**(`roomId`, `fromVersion`, `toVersion?`): `Promise`<[`IOp`](../interfaces/IOp.md)<`T`\>[]\>

检索两个版本之间的操作（包括 'from'，不包括 'to'）。

#### Parameters

| Name | Type |
| :------ | :------ |
| `roomId` | `string` |
| `fromVersion` | `number` |
| `toVersion?` | `number` |

#### Returns

`Promise`<[`IOp`](../interfaces/IOp.md)<`T`\>[]\>

#### Overrides

[Db](Db.md).[getOps](Db.md#getops)

___

### <a id="getsnapshot" name="getsnapshot"></a> getSnapshot

▸ **getSnapshot**(`roomId`): `Promise`<``null`` \| [`ISnapshot`](../interfaces/ISnapshot.md)<`S`\>\>

通过 ID 检索文档的快照。

#### Parameters

| Name | Type |
| :------ | :------ |
| `roomId` | `string` |

#### Returns

`Promise`<``null`` \| [`ISnapshot`](../interfaces/ISnapshot.md)<`S`\>\>

#### Overrides

[Db](Db.md).[getSnapshot](Db.md#getsnapshot)
