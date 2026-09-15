# Class: Connection

客户端的协作连接。

## Table of contents

### Constructors

- [constructor](Connection.md#constructor)

### Accessors

- [canSend](Connection.md#cansend)
- [id](Connection.md#id)

### Methods

- [close](Connection.md#close)
- [destroy](Connection.md#destroy)
- [off](Connection.md#off)
- [on](Connection.md#on)
- [once](Connection.md#once)
- [send](Connection.md#send)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Connection**()

## Accessors

### <a id="cansend" name="cansend"></a> canSend

• `get` **canSend**(): `boolean`

获取该连接是否可以发送消息。

#### Returns

`boolean`

返回该连接是否可以发送消息。

___

### <a id="id" name="id"></a> id

• `get` **id**(): `string`

获取连接 ID。

#### Returns

`string`

返回连接 ID。

## Methods

### <a id="close" name="close"></a> close

▸ **close**(): `void`

关闭连接。

#### Returns

`void`

___

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
| `NAME_2` | extends ``"open"`` \| ``"message"`` \| ``"close"`` \| ``"error"`` \| ``"reconnect"`` \| ``"reconnectFailed"`` \| ``"reconnectAttempts"`` \| ``"connectionStateChanged"`` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `NAME_2` | 事件名称。 |
| `f` | [`IEvents`](../interfaces/IEvents.md)[`NAME_2`] | 事件处理程序。 |

#### Returns

`void`

___

### <a id="on" name="on"></a> on

▸ **on**<`NAME`\>(`name`, `f`): [`IEvents`](../interfaces/IEvents.md)[`NAME`]

为某个事件注册一个监听器。

#### Type parameters

| Name | Type |
| :------ | :------ |
| `NAME` | extends ``"open"`` \| ``"message"`` \| ``"close"`` \| ``"error"`` \| ``"reconnect"`` \| ``"reconnectFailed"`` \| ``"reconnectAttempts"`` \| ``"connectionStateChanged"`` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `NAME` | 事件名称。 |
| `f` | [`IEvents`](../interfaces/IEvents.md)[`NAME`] | 事件处理程序。 |

#### Returns

[`IEvents`](../interfaces/IEvents.md)[`NAME`]

___

### <a id="once" name="once"></a> once

▸ **once**<`NAME_1`\>(`name`, `f`): `void`

为某个事件注册一个只调用一次的监听器。

#### Type parameters

| Name | Type |
| :------ | :------ |
| `NAME_1` | extends ``"open"`` \| ``"message"`` \| ``"close"`` \| ``"error"`` \| ``"reconnect"`` \| ``"reconnectFailed"`` \| ``"reconnectAttempts"`` \| ``"connectionStateChanged"`` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `NAME_1` | 事件名称。 |
| `f` | [`IEvents`](../interfaces/IEvents.md)[`NAME_1`] | 事件处理程序。 |

#### Returns

`void`

___

### <a id="send" name="send"></a> send

▸ **send**(`data`, `type?`): `void`

向服务器发送一条消息。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `unknown` | 要发送的数据。 |
| `type?` | [`MessageType`](../README.md#messagetype) | - |

#### Returns

`void`
