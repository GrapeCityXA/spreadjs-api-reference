# spread-sheets-collaboration-client

## Table of contents

### Enumerations

- [BrowsingMode](enums/BrowsingMode.md)

### Interfaces

- [IBindPresenceOptions](interfaces/IBindPresenceOptions.md)
- [IChangeSet](interfaces/IChangeSet.md)
- [IOpComponent](interfaces/IOpComponent.md)
- [IPermission](interfaces/IPermission.md)
- [IPresence](interfaces/IPresence.md)
- [ISelections](interfaces/ISelections.md)
- [IUser](interfaces/IUser.md)
- [IWorksheet](interfaces/IWorksheet.md)

### Variables

- [type](README.md#type)

### Functions

- [bind](README.md#bind)
- [bindPresence](README.md#bindpresence)

## Variables

### <a id="type" name="type"></a> type

• **type**: `OT_Type`

电子表格的操作转换（OT）类型。

## Functions

### <a id="bind" name="bind"></a> bind

▸ **bind**(`workbook`, `doc`): `void`

将工作簿与文档进行绑定。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workbook` | `any` | `GC.Spread.Sheets.Workbook` 的实例。 |
| `doc` | `SharedDoc`<`any`, [`IChangeSet`](interfaces/IChangeSet.md)\> | `SharedDoc` 的实例。 |

#### Returns

`void`

___

### <a id="bindpresence" name="bindpresence"></a> bindPresence

▸ **bindPresence**(`workbook`, `presence`, `user`, `options?`): `void`

将工作簿与在线状态进行绑定。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workbook` | `any` | `GC.Spread.Sheets.Workbook` 的实例。 |
| `presence` | `Presence`<[`IPresence`](interfaces/IPresence.md)\> | `Presence` 的实例。 |
| `user` | [`IUser`](interfaces/IUser.md) | 用户信息。 |
| `options?` | [`IBindPresenceOptions`](interfaces/IBindPresenceOptions.md) | - |

#### Returns

`void`
