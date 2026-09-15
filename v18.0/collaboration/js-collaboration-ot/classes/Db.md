# Class: Db<S, T\>

## Type parameters

| Name |
| :------ |
| `S` |
| `T` |

## Hierarchy

- **`Db`**

  ↳ [`MemoryDb`](MemoryDb.md)

## Implements

- [`IDataBaseAdapter`](../interfaces/IDataBaseAdapter.md)<`S`, `T`\>

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

关闭数据库。

#### Returns

`Promise`<`void`\>

#### Implementation of

[IDataBaseAdapter](../interfaces/IDataBaseAdapter.md).[close](../interfaces/IDataBaseAdapter.md#close)

___

### <a id="commitop" name="commitop"></a> commitOp

▸ `Abstract` **commitOp**(`id`, `op`, `document`, `options?`): `Promise`<`boolean`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `op` | [`IOp`](../interfaces/IOp.md)<`T`\> |
| `document` | [`IDocument`](../interfaces/IDocument.md) |
| `options?` | `unknown` |

#### Returns

`Promise`<`boolean`\>

#### Implementation of

[IDataBaseAdapter](../interfaces/IDataBaseAdapter.md).[commitOp](../interfaces/IDataBaseAdapter.md#commitop)

___

### <a id="commitsnapshot" name="commitsnapshot"></a> commitSnapshot

▸ `Abstract` **commitSnapshot**(`id`, `snapshot`, `options?`): `Promise`<`boolean`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `snapshot` | [`ICommitSnapshot`](../interfaces/ICommitSnapshot.md)<`S`\> |
| `options?` | `unknown` |

#### Returns

`Promise`<`boolean`\>

#### Implementation of

[IDataBaseAdapter](../interfaces/IDataBaseAdapter.md).[commitSnapshot](../interfaces/IDataBaseAdapter.md#commitsnapshot)

___

### <a id="getcommittedopversion" name="getcommittedopversion"></a> getCommittedOpVersion

▸ **getCommittedOpVersion**(`id`, `to`, `op`): `Promise`<`undefined` \| `number`\>

获取已提交的操作版本，如果操作已提交，则返回已提交的版本，否则返回 undefined。

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `to` | `number` |
| `op` | [`IOp`](../interfaces/IOp.md)<`object`\> |

#### Returns

`Promise`<`undefined` \| `number`\>

#### Implementation of

[IDataBaseAdapter](../interfaces/IDataBaseAdapter.md).[getCommittedOpVersion](../interfaces/IDataBaseAdapter.md#getcommittedopversion)

___

### <a id="getdocument" name="getdocument"></a> getDocument

▸ `Abstract` **getDocument**(`id`, `options?`): `Promise`<`undefined` \| ``null`` \| [`IDocument`](../interfaces/IDocument.md)\>

通过 ID 获取文档信息。

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `options?` | `unknown` |

#### Returns

`Promise`<`undefined` \| ``null`` \| [`IDocument`](../interfaces/IDocument.md)\>

#### Implementation of

[IDataBaseAdapter](../interfaces/IDataBaseAdapter.md).[getDocument](../interfaces/IDataBaseAdapter.md#getdocument)

___

### <a id="getfragment" name="getfragment"></a> getFragment

▸ `Abstract` **getFragment**(`id`, `fragmentId`, `options?`): `Promise`<`undefined` \| ``null`` \| `S`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `fragmentId` | `string` |
| `options?` | `unknown` |

#### Returns

`Promise`<`undefined` \| ``null`` \| `S`\>

#### Implementation of

[IDataBaseAdapter](../interfaces/IDataBaseAdapter.md).[getFragment](../interfaces/IDataBaseAdapter.md#getfragment)

___

### <a id="getfragments" name="getfragments"></a> getFragments

▸ `Abstract` **getFragments**(`id`, `fragmentIds?`, `options?`): `Promise`<{ `[id: string]`: `S`;  }\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `fragmentIds?` | `string`[] |
| `options?` | `unknown` |

#### Returns

`Promise`<{ `[id: string]`: `S`;  }\>

#### Implementation of

[IDataBaseAdapter](../interfaces/IDataBaseAdapter.md).[getFragments](../interfaces/IDataBaseAdapter.md#getfragments)

___

### <a id="getops" name="getops"></a> getOps

▸ `Abstract` **getOps**(`id`, `from`, `to?`, `options?`): `Promise`<[`IOp`](../interfaces/IOp.md)<`T`\>[]\>

获取两个版本之间的操作，包括起始版本，不包括结束版本。

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `from` | `number` |
| `to?` | `number` |
| `options?` | `unknown` |

#### Returns

`Promise`<[`IOp`](../interfaces/IOp.md)<`T`\>[]\>

#### Implementation of

[IDataBaseAdapter](../interfaces/IDataBaseAdapter.md).[getOps](../interfaces/IDataBaseAdapter.md#getops)

___

### <a id="getsnapshot" name="getsnapshot"></a> getSnapshot

▸ `Abstract` **getSnapshot**(`id`, `options?`): `Promise`<`undefined` \| ``null`` \| [`ISnapshot`](../interfaces/ISnapshot.md)<`S`\>\>

通过 ID 获取快照。

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `options?` | `unknown` |

#### Returns

`Promise`<`undefined` \| ``null`` \| [`ISnapshot`](../interfaces/ISnapshot.md)<`S`\>\>

#### Implementation of

[IDataBaseAdapter](../interfaces/IDataBaseAdapter.md).[getSnapshot](../interfaces/IDataBaseAdapter.md#getsnapshot)
