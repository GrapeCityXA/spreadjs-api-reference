# Class: Collaboration

[Sheets](../modules/GC.Spread.Sheets.md).[Collaboration](../modules/GC.Spread.Sheets.Collaboration.md).Collaboration

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Collaboration.Collaboration.md#constructor)

### Methods

- [applyChangeSet](GC.Spread.Sheets.Collaboration.Collaboration.md#applychangeset)
- [fromSnapshot](GC.Spread.Sheets.Collaboration.Collaboration.md#fromsnapshot)
- [getPresences](GC.Spread.Sheets.Collaboration.Collaboration.md#getpresences)
- [getUser](GC.Spread.Sheets.Collaboration.Collaboration.md#getuser)
- [onChangeSet](GC.Spread.Sheets.Collaboration.Collaboration.md#onchangeset)
- [registerCollaborationType](GC.Spread.Sheets.Collaboration.Collaboration.md#registercollaborationtype)
- [setPresences](GC.Spread.Sheets.Collaboration.Collaboration.md#setpresences)
- [setUser](GC.Spread.Sheets.Collaboration.Collaboration.md#setuser)
- [toSnapshot](GC.Spread.Sheets.Collaboration.Collaboration.md#tosnapshot)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Collaboration**(`workbook`)

表示一个可以管理协作状态的协作管理器。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workbook` | [`Workbook`](GC.Spread.Sheets.Workbook.md) | 工作簿。 |

## Methods

### <a id="applychangeset" name="applychangeset"></a> applyChangeSet

▸ **applyChangeSet**(`changeSet`): `void`

仅在协作场景下使用，用于应用文档操作。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `changeSet` | [`IChangeSet`](../interfaces/GC.Spread.Sheets.Collaboration.IChangeSet.md) | 变更集 |

#### Returns

`void`

___

### <a id="fromsnapshot" name="fromsnapshot"></a> fromSnapshot

▸ **fromSnapshot**(`snapshot`): `void`

仅在协作场景下使用，用于将快照恢复到工作簿状态。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `snapshot` | `Object` | 快照对象 |

#### Returns

`void`

___

### <a id="getpresences" name="getpresences"></a> getPresences

▸ **getPresences**(): [`IPresence`](../modules/GC.Spread.Sheets.Collaboration.md#ipresence)[]

获取工作簿的在线状态信息

**`example`**
```
```typescript
// 此示例获取在线状态信息。
const presences = spread.collaboration.getPresences();
```

#### Returns

[`IPresence`](../modules/GC.Spread.Sheets.Collaboration.md#ipresence)[]

presences - 在线状态信息。

___

### <a id="getuser" name="getuser"></a> getUser

▸ **getUser**(): [`IUser`](../modules/GC.Spread.Sheets.Collaboration.md#iuser)

获取工作簿的用户信息

**`example`**
```
```typescript
// 此示例获取当前用户。
const user = spread.collaboration.getUser();
```

#### Returns

[`IUser`](../modules/GC.Spread.Sheets.Collaboration.md#iuser)

___

### <a id="onchangeset" name="onchangeset"></a> onChangeSet

▸ **onChangeSet**(`onOpHandler`): `void`

仅在协作场景下使用，用于监听变更集。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `onOpHandler` | [`IChangeSetHandler`](../modules/GC.Spread.Sheets.Collaboration.md#ichangesethandler) | 监听变更集的回调函数 |

#### Returns

`void`

___

### <a id="registercollaborationtype" name="registercollaborationtype"></a> registerCollaborationType

▸ **registerCollaborationType**(`type`): `void`

仅在协作场景下使用，用于注册协作类型。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | [`IOT_Type`](../interfaces/GC.Spread.Sheets.Collaboration.IOT_Type.md) | 协作类型 |

#### Returns

`void`

___

### <a id="setpresences" name="setpresences"></a> setPresences

▸ **setPresences**(`presences`): `void`

设置在线状态信息。

**`example`**
```
//此示例更新当前在线状态。
let presences = [{
    user: {
        id: '1',
        name: 'User1',
        color: '#FF0000',
        permission: {
            mode: GC.Spread.Sheets.Collaboration.BrowsingMode.edit,
        }
    },
    status: {
        selections: {
             selections: [new GC.Spread.Sheets.Range(0, 0, 1, 1)],
             sheetId: 'sheet1'
        }
    }
}, {
    user: {
        id: '2',
        name: 'User2',
        permission: {
            mode: GC.Spread.Sheets.Collaboration.BrowsingMode.edit,
        }
    },
    status: {
        selections: {
             selections: [new GC.Spread.Sheets.Range(2, 2, 3, 5)],
             sheetId: 'sheet1'
        }
    }
}]
spread.collaboration.setPresences(presences);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `presences` | [`IPresence`](../modules/GC.Spread.Sheets.Collaboration.md#ipresence)[] | 在线状态信息。 |

#### Returns

`void`

___

### <a id="setuser" name="setuser"></a> setUser

▸ **setUser**(`user`): `void`

设置当前用户。

**`example`**
```
//此示例设置当前用户。
let user = {
    id: '1',
    name: 'User1',
    color: '#FF0000',
    permission: {
        mode: GC.Spread.Sheets.Collaboration.BrowsingMode.edit,
    }
}
spread.collaboration.setUser(user);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `user` | [`IUser`](../modules/GC.Spread.Sheets.Collaboration.md#iuser) | 当前用户。 |

#### Returns

`void`

___

### <a id="tosnapshot" name="tosnapshot"></a> toSnapshot

▸ **toSnapshot**(): `Object`

仅在协作场景下使用，用于将工作簿状态保存为快照。

#### Returns

`Object`

snapshot - 快照对象
