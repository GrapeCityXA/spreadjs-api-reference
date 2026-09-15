# js-collaboration-ot

## Table of contents

### Enumerations

- [MessageActions](enums/MessageActions.md)

### Classes

- [Db](classes/Db.md)
- [DocumentServices](classes/DocumentServices.md)
- [MemoryDb](classes/MemoryDb.md)
- [ReadSnapshotsRequest](classes/ReadSnapshotsRequest.md)
- [SubmitRequest](classes/SubmitRequest.md)
- [TypesManager](classes/TypesManager.md)

### Interfaces

- [ICommitSnapshot](interfaces/ICommitSnapshot.md)
- [IContext](interfaces/IContext.md)
- [ICreateComponent](interfaces/ICreateComponent.md)
- [ICustomOptions](interfaces/ICustomOptions.md)
- [IDatabaseAdapter](interfaces/IDatabaseAdapter.md)
- [IDocConfig](interfaces/IDocConfig.md)
- [IDocHookContext](interfaces/IDocHookContext.md)
- [IDocMiddlewareContext](interfaces/IDocMiddlewareContext.md)
- [IDocMiddlewareContextBase](interfaces/IDocMiddlewareContextBase.md)
- [IDocReadOpMiddlewareContext](interfaces/IDocReadOpMiddlewareContext.md)
- [IDocReadSnapshotsMiddlewareContext](interfaces/IDocReadSnapshotsMiddlewareContext.md)
- [IDocReceiveMiddlewareContext](interfaces/IDocReceiveMiddlewareContext.md)
- [IDocReplyMiddlewareContext](interfaces/IDocReplyMiddlewareContext.md)
- [IDocSubmitMiddlewareContext](interfaces/IDocSubmitMiddlewareContext.md)
- [IDocument](interfaces/IDocument.md)
- [IErrorData](interfaces/IErrorData.md)
- [IMilestoneDatabaseAdapter](interfaces/IMilestoneDatabaseAdapter.md)
- [IOp](interfaces/IOp.md)
- [IReadOpRequest](interfaces/IReadOpRequest.md)
- [IReplyMessage](interfaces/IReplyMessage.md)
- [IRequestMessage](interfaces/IRequestMessage.md)
- [IRequestMessageExtra](interfaces/IRequestMessageExtra.md)
- [IRestoreComponent](interfaces/IRestoreComponent.md)
- [ISnapshot](interfaces/ISnapshot.md)
- [ISnapshotFragmentsChanges](interfaces/ISnapshotFragmentsChanges.md)
- [ISnapshotFragmentsRequest](interfaces/ISnapshotFragmentsRequest.md)
- [ISnapshotMeta](interfaces/ISnapshotMeta.md)
- [OT\_Type](interfaces/OT_Type.md)

### Type aliases

- [ISnapshotFragments](Overview.md#isnapshotfragments)
- [SnapshotTypes](Overview.md#snapshottypes)

### Functions

- [documentFeature](Overview.md#documentfeature)

## Type aliases

### <a id="isnapshotfragments" name="isnapshotfragments"></a> ISnapshotFragments

Ƭ **ISnapshotFragments**<`S`\>: `Object`

#### Type parameters

| Name | Type |
| :------ | :------ |
| `S` | `unknown` |

#### Index signature

▪ [key: `string`]: `S`

___

### <a id="snapshottypes" name="snapshottypes"></a> SnapshotTypes

Ƭ **SnapshotTypes**: ``"current"`` \| ``"byVersion"``

## Functions

### <a id="documentfeature" name="documentfeature"></a> documentFeature

▸ **documentFeature**<`S`, `T`\>(`service?`): `IFeature`

创建一个用于操作转换（OT）文档的功能。

**`example`**
```javascript
const server = new Server({ httpServer });
server.useFeature(documentFeature());
```

#### Type parameters

| Name | Type |
| :------ | :------ |
| `S` | `unknown` |
| `T` | `unknown` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `service?` | [`DocumentServices`](classes/DocumentServices.md)<`S`, `T`\> |

#### Returns

`IFeature`

OT 文档功能。
