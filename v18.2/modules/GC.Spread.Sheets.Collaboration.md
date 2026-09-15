# Namespace: Collaboration

[Spread](GC.Spread.md).[Sheets](GC.Spread.Sheets.md).Collaboration

## Table of contents

### Enumerations

- [BrowsingMode](../enums/GC.Spread.Sheets.Collaboration.BrowsingMode.md)
- [OpType](../enums/GC.Spread.Sheets.Collaboration.OpType.md)
- [PermissionTypes](../enums/GC.Spread.Sheets.Collaboration.PermissionTypes.md)

### Classes

- [Collaboration](../classes/GC.Spread.Sheets.Collaboration.Collaboration.md)

### Interfaces

- [IChangeSet](../interfaces/GC.Spread.Sheets.Collaboration.IChangeSet.md)
- [IOT\_Type](../interfaces/GC.Spread.Sheets.Collaboration.IOT_Type.md)
- [IOpComponent](../interfaces/GC.Spread.Sheets.Collaboration.IOpComponent.md)

### Type aliases

- [IChangeSetHandler](GC.Spread.Sheets.Collaboration.md#ichangesethandler)
- [IPermission](GC.Spread.Sheets.Collaboration.md#ipermission)
- [IPresence](GC.Spread.Sheets.Collaboration.md#ipresence)
- [ISelections](GC.Spread.Sheets.Collaboration.md#iselections)
- [IStatus](GC.Spread.Sheets.Collaboration.md#istatus)
- [IUser](GC.Spread.Sheets.Collaboration.md#iuser)

## Type aliases

### <a id="ichangesethandler" name="ichangesethandler"></a> IChangeSetHandler

Ƭ **IChangeSetHandler**: (`changeSet`: [`IChangeSet`](../interfaces/GC.Spread.Sheets.Collaboration.IChangeSet.md)) => `void`

#### Type declaration

▸ (`changeSet`): `void`

此回调用于处理更改集。

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `changeSet` | [`IChangeSet`](../interfaces/GC.Spread.Sheets.Collaboration.IChangeSet.md) | 要处理的更改集。 |

##### Returns

`void`

___

### <a id="ipermission" name="ipermission"></a> IPermission

Ƭ **IPermission**: `Object`

**`property`** {GC.Spread.Sheets.Collaboration.BrowsingMode} [mode]

**`property`** {GC.Spread.Sheets.Collaboration.PermissionTypes} [viewModePermissions]

#### Type declaration

| Name | Type |
| :------ | :------ |
| `mode?` | [`BrowsingMode`](../enums/GC.Spread.Sheets.Collaboration.BrowsingMode.md) |
| `viewModePermissions?` | [`PermissionTypes`](../enums/GC.Spread.Sheets.Collaboration.PermissionTypes.md) |

___

### <a id="ipresence" name="ipresence"></a> IPresence

Ƭ **IPresence**: `Object`

**`property`** {GC.Spread.Sheets.Collaboration.IUser} [user]

**`property`** {GC.Spread.Sheets.Collaboration.IStatus} [status]

#### Type declaration

| Name | Type |
| :------ | :------ |
| `status?` | [`IStatus`](GC.Spread.Sheets.Collaboration.md#istatus) |
| `user?` | [`IUser`](GC.Spread.Sheets.Collaboration.md#iuser) |

___

### <a id="iselections" name="iselections"></a> ISelections

Ƭ **ISelections**: `Object`

**`property`** {GC.Spread.Sheets.IRange[]} [selections]

**`property`** {string} [sheetId]

#### Type declaration

| Name | Type |
| :------ | :------ |
| `selections?` | [`IRange`](../interfaces/GC.Spread.Sheets.IRange.md)[] |
| `sheetId?` | `string` |

___

### <a id="istatus" name="istatus"></a> IStatus

Ƭ **IStatus**: `Object`

**`property`** {GC.Spread.Sheets.Collaboration.ISelections} [selections]

#### Type declaration

| Name | Type |
| :------ | :------ |
| `selections?` | [`ISelections`](GC.Spread.Sheets.Collaboration.md#iselections) |

___

### <a id="iuser" name="iuser"></a> IUser

Ƭ **IUser**: `Object`

**`property`** {string} [id]

**`property`** {string} [name]

**`property`** {string} [color]

**`property`** {GC.Spread.Sheets.Collaboration.IPermission} [permission]

#### Type declaration

| Name | Type |
| :------ | :------ |
| `color?` | `string` |
| `id?` | `string` |
| `name` | `string` |
| `permission?` | [`IPermission`](GC.Spread.Sheets.Collaboration.md#ipermission) |
