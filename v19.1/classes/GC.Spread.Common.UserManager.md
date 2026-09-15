# Class: UserManager

[Spread](../modules/GC.Spread.md).[Common](../modules/GC.Spread.Common.md).UserManager

## Table of contents

### Constructors

- [constructor](GC.Spread.Common.UserManager.md#constructor)

### Methods

- [bind](GC.Spread.Common.UserManager.md#bind)
- [configure](GC.Spread.Common.UserManager.md#configure)
- [current](GC.Spread.Common.UserManager.md#current)
- [get](GC.Spread.Common.UserManager.md#get)
- [unbind](GC.Spread.Common.UserManager.md#unbind)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new UserManager**()

表示一个用户管理器。

## Methods

### <a id="bind" name="bind"></a> bind

▸ `Static` **bind**(`event`, `handler`): `void`

绑定事件处理程序。

**`static`**

**`example`**
```javascript
GC.Spread.Common.UserManager.bind(GC.Spread.Common.Events.CurrentUserChanged, (event, args) => {
    console.log(event);
    console.log(args.oldCurrentUser);
    console.log(args.newCurrentUser);
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `event` | [`Events`](GC.Spread.Common.Events.md) | 事件类型。 |
| `handler` | `Function` | 事件处理程序。 |

#### Returns

`void`

___

### <a id="configure" name="configure"></a> configure

▸ `Static` **configure**(`options`): `void`

配置用户管理器选项。

**`static`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`IUserManagerOptions`](../interfaces/GC.Spread.Common.IUserManagerOptions.md) | 用户管理器选项。 |

#### Returns

`void`

___

### <a id="current" name="current"></a> current

▸ `Static` **current**(`userId?`): `undefined` \| `string`

获取或设置当前用户。

**`static`**

**`example`**
```javascript
// 从登录页面导航，并获取登录用户ID
spread.users.current('715CFB19-2BB9-4B94-BE0C-08D0F9A019D4'); // { id: "715CFB19-2BB9-4B94-BE0C-08D0F9A019D4", name: "John Doe" }
console.log(spread.users.getSync(spread.users.current()).name); // "John Doe"
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `userId?` | `string` | 当前用户 ID。 |

#### Returns

`undefined` \| `string`

当前用户 ID。

___

### <a id="get" name="get"></a> get

▸ `Static` **get**(`userId`): `Promise`<`undefined` \| [`IUser`](../interfaces/GC.Spread.Common.IUser.md)\>

通过用户ID获取用户。

**`static`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `userId` | `string` | 用户ID。 |

#### Returns

`Promise`<`undefined` \| [`IUser`](../interfaces/GC.Spread.Common.IUser.md)\>

用户。

___

### <a id="unbind" name="unbind"></a> unbind

▸ `Static` **unbind**(`event`, `handler`): `void`

取消绑定事件处理程序。

**`static`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `event` | [`Events`](GC.Spread.Common.Events.md) | 事件类型。 |
| `handler` | `Function` | 事件处理程序。 |

#### Returns

`void`
