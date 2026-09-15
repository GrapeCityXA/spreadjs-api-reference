# js-collaboration-ot

## Table of contents

### Enumerations

- [MessageActions](enums/MessageActions.md)
- [SubmitSnapshotTrigger](enums/SubmitSnapshotTrigger.md)

### Classes

- [Db](classes/Db.md)
- [DocumentServices](classes/DocumentServices.md)
- [MemoryDb](classes/MemoryDb.md)
- [ReadSnapshotsRequest](classes/ReadSnapshotsRequest.md)
- [SubmitRequest](classes/SubmitRequest.md)
- [SubmitSnapshotRequest](classes/SubmitSnapshotRequest.md)
- [TypesManager](classes/TypesManager.md)

### Interfaces

- [IAfterCommitCallback](interfaces/IAfterCommitCallback.md)
- [ICommitSnapshot](interfaces/ICommitSnapshot.md)
- [IContext](interfaces/IContext.md)
- [ICreateComponent](interfaces/ICreateComponent.md)
- [ICustomOptions](interfaces/ICustomOptions.md)
- [IDataBaseAdapter](interfaces/IDataBaseAdapter.md)
- [IDocConfig](interfaces/IDocConfig.md)
- [IDocHookContext](interfaces/IDocHookContext.md)
- [IDocMiddlewareContext](interfaces/IDocMiddlewareContext.md)
- [IDocMiddlewareContextBase](interfaces/IDocMiddlewareContextBase.md)
- [IDocReadOpMiddlewareContext](interfaces/IDocReadOpMiddlewareContext.md)
- [IDocReadSnapshotsMiddlewareContext](interfaces/IDocReadSnapshotsMiddlewareContext.md)
- [IDocReceiveMiddlewareContext](interfaces/IDocReceiveMiddlewareContext.md)
- [IDocReplyMiddlewareContext](interfaces/IDocReplyMiddlewareContext.md)
- [IDocSubmitMiddlewareContext](interfaces/IDocSubmitMiddlewareContext.md)
- [IDocSubmitSnapshotMiddlewareContext](interfaces/IDocSubmitSnapshotMiddlewareContext.md)
- [IDocument](interfaces/IDocument.md)
- [IErrorData](interfaces/IErrorData.md)
- [IMilestoneDataBaseAdapter](interfaces/IMilestoneDataBaseAdapter.md)
- [IOp](interfaces/IOp.md)
- [IReplyMessage](interfaces/IReplyMessage.md)
- [IRequestMessage](interfaces/IRequestMessage.md)
- [IRequestMessageExtra](interfaces/IRequestMessageExtra.md)
- [ISnapshot](interfaces/ISnapshot.md)
- [ISnapshotFragmentsChanges](interfaces/ISnapshotFragmentsChanges.md)
- [ISnapshotFragmentsRequest](interfaces/ISnapshotFragmentsRequest.md)
- [ISnapshotMeta](interfaces/ISnapshotMeta.md)
- [ISubmitSnapshotContext](interfaces/ISubmitSnapshotContext.md)
- [OT\_Type](interfaces/OT_Type.md)

### Type aliases

- [ISnapshotFragments](README.md#isnapshotfragments)
- [SnapshotTypes](README.md#snapshottypes)

### Functions

- [documentFeature](README.md#documentfeature)

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

OT 文档的功能。

**`example`**
const server = new Server({ httpServer });
server.useFeature(documentFeature());

#### Type parameters

| Name | Type |
| :------ | :------ |
| `S` | `unknown` |
| `T` | `unknown` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `service?` | [`DocumentServices`](classes/DocumentServices.md)<`S`, `T`\> | 文档服务要使用的服务 |

#### Returns

`IFeature`

OT 文档功能。
