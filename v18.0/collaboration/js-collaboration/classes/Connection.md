# Class: Connection

服务器的协作连接。

## Table of contents

### Constructors

- [constructor](Connection.md#constructor)

### Properties

- [tags](Connection.md#tags)

### Accessors

- [auth](Connection.md#auth)
- [id](Connection.md#id)
- [query](Connection.md#query)
- [roomId](Connection.md#roomid)

### Methods

- [broadcast](Connection.md#broadcast)
- [close](Connection.md#close)
- [send](Connection.md#send)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Connection**()

## Properties

### <a id="tags" name="tags"></a> tags

• **tags**: `Map`<`string`, `unknown`\>

为每个连接保存自定义数据。

## Accessors

### <a id="auth" name="auth"></a> auth

• `get` **auth**(): `Object`

获取连接的认证数据。

#### Returns

`Object`

返回连接的认证数据。

___

### <a id="id" name="id"></a> id

• `get` **id**(): `string`

获取连接的 ID。

#### Returns

`string`

返回连接的 ID。

___

### <a id="query" name="query"></a> query

• `get` **query**(): `Record`<`string`, `unknown`\>

获取连接的查询参数。

#### Returns

`Record`<`string`, `unknown`\>

返回连接的查询参数。

___

### <a id="roomid" name="roomid"></a> roomId

• `get` **roomId**(): `string`

连接所在的房间 ID。

#### Returns

`string`

返回连接所在的房间 ID。

## Methods

### <a id="broadcast" name="broadcast"></a> broadcast

▸ **broadcast**(`data`, `type`, `includeSelf?`): `void`

向房间内的所有连接广播消息

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `string` \| `Uint8Array` | 要发送的消息数据 |
| `type` | [`MessageType`](../README.md#messagetype) | 消息类型 |
| `includeSelf?` | `boolean` | 是否发送给自己 |

#### Returns

`void`

___

### <a id="close" name="close"></a> close

▸ **close**(): `void`

关闭连接

#### Returns

`void`

___

### <a id="send" name="send"></a> send

▸ **send**(`data`, `type?`): `void`

向客户端发送消息

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `unknown` | 要发送的消息数据 |
| `type?` | [`MessageType`](../README.md#messagetype) | 消息类型 |

#### Returns

`void`
