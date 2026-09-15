# Class: Presence<P\>

**`example`**
```
const uiComponent = new xxx.uiComponent();
const conn = new Client('ws://localhost:8080/').connect('room1');
const presence = new Presence(conn);
presence.subscribe(() => {
    uiComponent.showPresences(presence.others);
    uiComponent.on('selectionChanges', () => {
        uiComponent.submitLocal({ userId: xxx, selection: xxx });
    });
    presence.on('add', () => {
        uiComponent.showPresences(presence.others);
    });
    presence.on('update', () => {
        uiComponent.showPresences(presence.others);
    });
    presence.on('remove', () => {
        uiComponent.showPresences(presence.others);
    });
    presence.submitLocal({ userId: xxx, selection: xxx });
});
```

## Type parameters

| Name |
| :------ |
| `P` |

## Table of contents

### Constructors

- [constructor](Presence.md#constructor)

### Properties

- [conn](Presence.md#conn)
- [local](Presence.md#local)
- [others](Presence.md#others)

### Accessors

- [id](Presence.md#id)

### Methods

- [destroy](Presence.md#destroy)
- [off](Presence.md#off)
- [on](Presence.md#on)
- [once](Presence.md#once)
- [removeLocal](Presence.md#removelocal)
- [submitLocal](Presence.md#submitlocal)
- [subscribe](Presence.md#subscribe)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Presence**<`P`\>(`conn`)

#### Type parameters

| Name |
| :------ |
| `P` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `conn` | `Connection` |

## Properties

### <a id="conn" name="conn"></a> conn

• **conn**: `Connection`

___

### <a id="local" name="local"></a> local

• `Optional` **local**: `P`

本地在线状态对象。

___

### <a id="others" name="others"></a> others

• **others**: [`IPresences`](../interfaces/IPresences.md)<`P`\>

其他在线状态对象。

## Accessors

### <a id="id" name="id"></a> id

• `get` **id**(): `string`

#### Returns

`string`

## Methods

### <a id="destroy" name="destroy"></a> destroy

▸ **destroy**(): `void`

销毁可观察对象。

#### Returns

`void`

___

### <a id="off" name="off"></a> off

▸ **off**<`NAME_2`\>(`name`, `f`): `void`

移除某个事件的监听器。

#### Type parameters

| Name | Type |
| :------ | :------ |
| `NAME_2` | extends ``"add"`` \| ``"update"`` \| ``"remove"`` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `NAME_2` | 事件名称。 |
| `f` | [`IEvents`](../interfaces/IEvents.md)<`P`\>[`NAME_2`] | 事件处理程序。 |

#### Returns

`void`

___

### <a id="on" name="on"></a> on

▸ **on**<`NAME`\>(`name`, `f`): [`IEvents`](../interfaces/IEvents.md)<`P`\>[`NAME`]

注册某个事件的监听器。

#### Type parameters

| Name | Type |
| :------ | :------ |
| `NAME` | extends ``"add"`` \| ``"update"`` \| ``"remove"`` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `NAME` | 事件名称。 |
| `f` | [`IEvents`](../interfaces/IEvents.md)<`P`\>[`NAME`] | 事件处理程序。 |

#### Returns

[`IEvents`](../interfaces/IEvents.md)<`P`\>[`NAME`]

___

### <a id="once" name="once"></a> once

▸ **once**<`NAME_1`\>(`name`, `f`): `void`

注册一个只调用一次的事件监听器。

#### Type parameters

| Name | Type |
| :------ | :------ |
| `NAME_1` | extends ``"add"`` \| ``"update"`` \| ``"remove"`` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `NAME_1` | 事件名称。 |
| `f` | [`IEvents`](../interfaces/IEvents.md)<`P`\>[`NAME_1`] | 事件处理程序。 |

#### Returns

`void`

___

### <a id="removelocal" name="removelocal"></a> removeLocal

▸ **removeLocal**(): `void`

从服务器移除本地在线状态对象，服务器会将此消息广播给其他客户端。

#### Returns

`void`

___

### <a id="submitlocal" name="submitlocal"></a> submitLocal

▸ **submitLocal**(`p`): `void`

将本地在线状态对象提交到服务器，服务器会将该在线状态对象广播给其他客户端。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `p` | `P` | The local presence object. |

#### Returns

`void`

___

### <a id="subscribe" name="subscribe"></a> subscribe

▸ **subscribe**(`callback`): `void`

订阅在线状态。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback` | () => `void` | 订阅成功后，可通过 “presence.others” 获取其他在线状态。 |

#### Returns

`void`
