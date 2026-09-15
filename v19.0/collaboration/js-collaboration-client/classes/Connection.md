# Class: Connection

表示客户端协作连接。

## Table of contents

### Constructors

- [constructor](Connection.md#constructor)

### Accessors

- [connected](Connection.md#connected)
- [id](Connection.md#id)
- [roomId](Connection.md#roomid)

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

### <a id="connected" name="connected"></a> connected

• `get` **connected**(): `boolean`

指示连接是否处于活动状态并能够发送消息。

#### Returns

`boolean`

如果连接处于活动状态，则为 true，否则为 false.

___

### <a id="id" name="id"></a> id

• `get` **id**(): `string`

获取连接的唯一标识符。

#### Returns

`string`

连接的 ID。

___

### <a id="roomid" name="roomid"></a> roomId

• `get` **roomId**(): `string`

获取连接的房间标识符。

#### Returns

`string`

与连接关联的房间 ID。

## Methods

### <a id="close" name="close"></a> close

▸ **close**(): `void`

关闭与服务器的连接。

#### Returns

`void`

___

### <a id="destroy" name="destroy"></a> destroy

▸ **destroy**(): `void`

销毁可观察对象并清理资源。

#### Returns

`void`

___

### <a id="off" name="off"></a> off

▸ **off**<`NAME`\>(`name`, `f`): `void`

移除特定事件的监听器。

#### Type parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `NAME` | extends keyof [`IConnectionEvents`](../interfaces/IConnectionEvents.md) | 事件名称的类型，扩展 IConnectionEvents 的键。 |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `NAME` | 要移除监听器的事件的名称。 |
| `f` | [`IConnectionEvents`](../interfaces/IConnectionEvents.md)[`NAME`] | 要移除的事件处理程序函数。 |

#### Returns

`void`

___

### <a id="on" name="on"></a> on

▸ **on**<`NAME`\>(`name`, `f`): [`IConnectionEvents`](../interfaces/IConnectionEvents.md)[`NAME`]

注册特定事件的监听器。

#### Type parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `NAME` | extends keyof [`IConnectionEvents`](../interfaces/IConnectionEvents.md) | 事件名称的类型，扩展 IConnectionEvents 的键。 |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `NAME` | 要监听的事件的名称。 |
| `f` | [`IConnectionEvents`](../interfaces/IConnectionEvents.md)[`NAME`] | 事件处理程序函数。 |

#### Returns

[`IConnectionEvents`](../interfaces/IConnectionEvents.md)[`NAME`]

___

### <a id="once" name="once"></a> once

▸ **once**<`NAME`\>(`name`, `f`): `void`

注册特定事件的一次性监听器。

#### Type parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `NAME` | extends keyof [`IConnectionEvents`](../interfaces/IConnectionEvents.md) | 事件名称的类型，扩展 IConnectionEvents 的键。 |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `NAME` | 要监听的事件的名称。 |
| `f` | [`IConnectionEvents`](../interfaces/IConnectionEvents.md)[`NAME`] | 事件处理程序函数。 |

#### Returns

`void`

___

### <a id="send" name="send"></a> send

▸ **send**(`data`, `type?`): `void`

向服务器发送消息。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `unknown` | 要发送的数据。 |
| `type?` | [`MessageType`](../README.md#messagetype) | - |

#### Returns

`void`
