# Class: PostgresDb<S, T\>

## Type parameters

| Name | Type |
| :------ | :------ |
| `S` | `unknown` |
| `T` | `unknown` |

## Hierarchy

- `Db`<`S`, `T`\>

  ↳ **`PostgresDb`**

## Table of contents

### Constructors

- [constructor](PostgresDb.md#constructor)

### Methods

- [close](PostgresDb.md#close)
- [commitOp](PostgresDb.md#commitop)
- [commitSnapshot](PostgresDb.md#commitsnapshot)
- [getCommittedOpVersion](PostgresDb.md#getcommittedopversion)
- [getDocument](PostgresDb.md#getdocument)
- [getFragment](PostgresDb.md#getfragment)
- [getOps](PostgresDb.md#getops)
- [getSnapshot](PostgresDb.md#getsnapshot)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new PostgresDb**<`S`, `T`\>(`pool`)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `S` | `unknown` |
| `T` | `unknown` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `pool` | `Pool` |

#### Overrides

Db&lt;S, T\&gt;.constructor

## Methods

### <a id="close" name="close"></a> close

▸ **close**(): `Promise`<`void`\>

#### Returns

`Promise`<`void`\>

#### Overrides

Db.close

___

### <a id="commitop" name="commitop"></a> commitOp

▸ **commitOp**(`id`, `op`, `document`): `Promise`<`boolean`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `op` | `IOp`<`T`\> |
| `document` | `IDocument` |

#### Returns

`Promise`<`boolean`\>

#### Overrides

Db.commitOp

___

### <a id="commitsnapshot" name="commitsnapshot"></a> commitSnapshot

▸ **commitSnapshot**(`roomId`, `snapshot`): `Promise`<`boolean`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `roomId` | `string` |
| `snapshot` | `ICommitSnapshot`<`S`\> |

#### Returns

`Promise`<`boolean`\>

#### Overrides

Db.commitSnapshot

___

### <a id="getcommittedopversion" name="getcommittedopversion"></a> getCommittedOpVersion

▸ **getCommittedOpVersion**(`id`, `to`, `op`): `Promise`<``null`` \| `number`\>

Retrieves the committed version of an operation if it exists.

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `to` | `number` |
| `op` | `IOp`<`object`\> |

#### Returns

`Promise`<``null`` \| `number`\>

#### Inherited from

Db.getCommittedOpVersion

___

### <a id="getdocument" name="getdocument"></a> getDocument

▸ **getDocument**(`roomId`): `Promise`<``null`` \| `IDocument`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `roomId` | `string` |

#### Returns

`Promise`<``null`` \| `IDocument`\>

#### Overrides

Db.getDocument

___

### <a id="getfragment" name="getfragment"></a> getFragment

▸ **getFragment**(`roomId`, `fragmentId`): `Promise`<``null`` \| { `data`: ``null`` \| `S` ; `version`: `number`  }\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `roomId` | `string` |
| `fragmentId` | `string` |

#### Returns

`Promise`<``null`` \| { `data`: ``null`` \| `S` ; `version`: `number`  }\>

#### Overrides

Db.getFragment

___

### <a id="getops" name="getops"></a> getOps

▸ **getOps**(`roomId`, `fromVersion`, `toVersion?`): `Promise`<`IOp`<`T`\>[]\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `roomId` | `string` |
| `fromVersion` | `number` |
| `toVersion?` | `number` |

#### Returns

`Promise`<`IOp`<`T`\>[]\>

#### Overrides

Db.getOps

___

### <a id="getsnapshot" name="getsnapshot"></a> getSnapshot

▸ **getSnapshot**(`roomId`): `Promise`<``null`` \| `ISnapshot`<`S`\>\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `roomId` | `string` |

#### Returns

`Promise`<``null`` \| `ISnapshot`<`S`\>\>

#### Overrides

Db.getSnapshot
