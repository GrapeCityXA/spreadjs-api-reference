# Class: Presence<P\>

管理实时协作中的 presence 信息。

**`example`**
const uiComponent = new xxx.uiComponent();
const connection = new Client('ws://localhost:8080/').connect('room1');
const presence = new Presence(connection);
presence.subscribe().then(() => {
    uiComponent.showPresences(presence.otherStates);
    presence.submitLocalState({ userId: xxx, selection: xxx });
    uiComponent.on('selectionChanges', () => {
        presence.submitLocalStateField('selection', xxx);
    });
    presence.on('add', () => {
        uiComponent.showPresences(presence.otherStates);
    });
    presence.on('update', () => {
        uiComponent.showPresences(presence.otherStates);
    });
    presence.on('remove', () => {
        uiComponent.showPresences(presence.otherStates);
    });
});

## Type parameters

| Name | Description |
| :------ | :------ |
| `P` | presence 数据类型。 |

## Table of contents

### Constructors

- [constructor](Presence.md#constructor)

### Accessors

- [connection](Presence.md#connection)
- [id](Presence.md#id)
- [localState](Presence.md#localstate)
- [otherStates](Presence.md#otherstates)

### Methods

- [destroy](Presence.md#destroy)
- [off](Presence.md#off)
- [on](Presence.md#on)
- [once](Presence.md#once)
- [removeLocalState](Presence.md#removelocalstate)
- [submitLocalState](Presence.md#submitlocalstate)
- [submitLocalStateField](Presence.md#submitlocalstatefield)
- [subscribe](Presence.md#subscribe)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Presence**<`P`\>(`connection`)

#### Type parameters

| Name |
| :------ |
| `P` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `connection` | `Connection` |

## Accessors

### <a id="connection" name="connection"></a> connection

• `get` **connection**(): `Connection`

检索关联的连接对象。

#### Returns

`Connection`

连接实例。

___

### <a id="id" name="id"></a> id

• `get` **id**(): `string`

检索 presence 实例的唯一标识符。

#### Returns

`string`

presence  ID。

___

### <a id="localstate" name="localstate"></a> localState

• `get` **localState**(): `undefined` \| `P`

检索本地 presence 状态。

#### Returns

`undefined` \| `P`

本地 presence 数据，或未设置时为 undefined。

___

### <a id="otherstates" name="otherstates"></a> otherStates

• `get` **otherStates**(): [`IPresences`](../interfaces/IPresences.md)<`P`\>

检索其他客户端的 presence 状态。

#### Returns

[`IPresences`](../interfaces/IPresences.md)<`P`\>

其他客户端的 presence 数据集合。

## Methods

### <a id="destroy" name="destroy"></a> destroy

▸ **destroy**(): `void`

销毁 presence 实例并清理资源。

#### Returns

`void`

___

### <a id="off" name="off"></a> off

▸ **off**<`NAME`\>(`name`, `f`): `void`

移除特定事件的监听器。

#### Type parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `NAME` | extends keyof [`IPresenceEvents`](../interfaces/IPresenceEvents.md)<`P`\> | 事件名称类型，扩展 keyof IPresenceEvents<P>。 |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `NAME` | 事件名称。 |
| `f` | [`IPresenceEvents`](../interfaces/IPresenceEvents.md)<`P`\>[`NAME`] | 事件处理函数。 |

#### Returns

`void`

___

### <a id="on" name="on"></a> on

▸ **on**<`NAME`\>(`name`, `f`): [`IPresenceEvents`](../interfaces/IPresenceEvents.md)<`P`\>[`NAME`]

注册特定事件的监听器。

#### Type parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `NAME` | extends keyof [`IPresenceEvents`](../interfaces/IPresenceEvents.md)<`P`\> | 事件名称类型，扩展 keyof IPresenceEvents<P>。 |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `NAME` | 事件名称。 |
| `f` | [`IPresenceEvents`](../interfaces/IPresenceEvents.md)<`P`\>[`NAME`] | 事件处理函数。 |

#### Returns

[`IPresenceEvents`](../interfaces/IPresenceEvents.md)<`P`\>[`NAME`]

注册的事件处理函数。

___

### <a id="once" name="once"></a> once

▸ **once**<`NAME`\>(`name`, `f`): `void`

注册一次性监听器。

#### Type parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `NAME` | extends keyof [`IPresenceEvents`](../interfaces/IPresenceEvents.md)<`P`\> | 事件名称类型，扩展 keyof IPresenceEvents<P>。 |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `NAME` | 事件名称。 |
| `f` | [`IPresenceEvents`](../interfaces/IPresenceEvents.md)<`P`\>[`NAME`] | 事件处理函数。 |

#### Returns

`void`

___

### <a id="removelocalstate" name="removelocalstate"></a> removeLocalState

▸ **removeLocalState**(): `void`

从服务器移除本地 presence 状态，通知其他客户端。

#### Returns

`void`

___

### <a id="submitlocalstate" name="submitlocalstate"></a> submitLocalState

▸ **submitLocalState**(`p`): `void`

提交本地 presence 状态到服务器，广播给其他客户端。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `p` | `P` | 要提交的本地 presence 数据。 |

#### Returns

`void`

___

### <a id="submitlocalstatefield" name="submitlocalstatefield"></a> submitLocalStateField

▸ **submitLocalStateField**(`name`, `value`): `void`

提交本地 presence 状态的特定字段到服务器，广播给其他客户端。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要更新的字段名称。 |
| `value` | `unknown` | 字段的新值。 |

#### Returns

`void`

___

### <a id="subscribe" name="subscribe"></a> subscribe

▸ **subscribe**(): `Promise`<`void`\>

订阅其他客户端的 presence 更新。

#### Returns

`Promise`<`void`\>

订阅完成时返回的 Promise。
