# spread-sheets-collaboration-client

## Table of contents

### Enumerations

- [BrowsingMode](enums/BrowsingMode.md)
- [OpType](enums/OpType.md)
- [PermissionTypes](enums/PermissionTypes.md)

### Interfaces

- [IBindPresenceOptions](interfaces/IBindPresenceOptions.md)
- [IChangeSet](interfaces/IChangeSet.md)
- [IOpComponent](interfaces/IOpComponent.md)
- [IPermission](interfaces/IPermission.md)
- [IPresence](interfaces/IPresence.md)
- [IRange](interfaces/IRange.md)
- [ISelections](interfaces/ISelections.md)
- [IUser](interfaces/IUser.md)
- [IUserWithPermission](interfaces/IUserWithPermission.md)

### Type aliases

- [IImageSource](Overview.md#iimagesource)

### Variables

- [type](Overview.md#type)

### Functions

- [bind](Overview.md#bind)
- [bindPresence](Overview.md#bindpresence)

## Type aliases

### <a id="iimagesource" name="iimagesource"></a> IImageSource

Ƭ **IImageSource**: { `kind`: ``"url"`` ; `src`: `string`  } \| { `dataUrl`: `string` ; `kind`: ``"data"``  } \| { `blobUrl`: `string` ; `kind`: ``"blobUrl"``  } \| { `blob`: `Blob` ; `kind`: ``"blob"``  } \| { `file`: `File` ; `kind`: ``"file"``  }

{
kind: 'url';
src: string;
} | {
kind: 'data';
dataUrl: string;
} | {
kind: 'blobUrl';
blobUrl: string;
} | {
kind: 'blob';
blob: Blob;
} | {
kind: 'file';
file: File;
}

## Variables

### <a id="type" name="type"></a> type

• **type**: `OT_Type`<`unknown`, [`IChangeSet`](interfaces/IChangeSet.md)\>

定义电子表格的 OT 类型。

## Functions

### <a id="bind" name="bind"></a> bind

▸ **bind**(`workbook`, `doc`): `Promise`<`void`\>

将工作簿绑定到共享文档。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workbook` | `any` | 工作簿实例。 |
| `doc` | `SharedDoc`<`any`, [`IChangeSet`](interfaces/IChangeSet.md)\> | SharedDoc 实例。 |

#### Returns

`Promise`<`void`\>

一个 Promise，当绑定完成时解析。

___

### <a id="bindpresence" name="bindpresence"></a> bindPresence

▸ **bindPresence**(`workbook`, `presence`, `user`, `options?`): `Promise`<`void`\>

将工作簿绑定到 presence 实例。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workbook` | `any` | 工作簿实例。 |
| `presence` | `Presence`<[`IPresence`](interfaces/IPresence.md)\> | presence 实例。 |
| `user` | [`IUserWithPermission`](interfaces/IUserWithPermission.md) | 用户信息。 |
| `options?` | [`IBindPresenceOptions`](interfaces/IBindPresenceOptions.md) | - |

#### Returns

`Promise`<`void`\>

一个 Promise，当绑定完成时解析。
