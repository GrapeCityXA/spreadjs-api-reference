# Class: Connection

表示服务器上的协作连接。

## Table of contents

### Constructors

- [constructor](Connection.md#constructor)

### Accessors

- [auth](Connection.md#auth)
- [id](Connection.md#id)
- [query](Connection.md#query)
- [roomId](Connection.md#roomid)
- [tags](Connection.md#tags)

### Methods

- [broadcast](Connection.md#broadcast)
- [close](Connection.md#close)
- [send](Connection.md#send)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Connection**()

## Accessors

### <a id="auth" name="auth"></a> auth

• `get` **auth**(): `Object`

检索连接的身份验证数据。

#### Returns

`Object`

与连接关联的身份验证数据。

___

### <a id="id" name="id"></a> id

• `get` **id**(): `string`

检索连接的唯一标识符。

#### Returns

`string`

连接的 ID。

___

### <a id="query" name="query"></a> query

• `get` **query**(): `Record`<`string`, `unknown`\>

检索连接的查询参数。

#### Returns

`Record`<`string`, `unknown`\>

连接的查询参数。

___

### <a id="roomid" name="roomid"></a> roomId

• `get` **roomId**(): `string`

检索连接的房间标识符。

#### Returns

`string`

与连接关联的房间 ID。

___

### <a id="tags" name="tags"></a> tags

• `get` **tags**(): `Map`<`string`, `unknown`\>

检索为连接保存的自定义数据。

#### Returns

`Map`<`string`, `unknown`\>

连接的自定义标签映射。

## Methods

### <a id="broadcast" name="broadcast"></a> broadcast

▸ **broadcast**(`data`, `type?`, `includeSelf?`): `void`

向房间中的所有连接广播消息。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `unknown` | 要广播的消息数据。 |
| `type?` | [`MessageType`](../README.md#messagetype) | - |
| `includeSelf?` | `boolean` | - |

#### Returns

`void`

___

### <a id="close" name="close"></a> close

▸ **close**(): `void`

关闭连接。

#### Returns

`void`

___

### <a id="send" name="send"></a> send

▸ **send**(`data`, `type?`): `void`

向客户端发送消息。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `unknown` | 要发送的消息数据。 |
| `type?` | [`MessageType`](../README.md#messagetype) | - |

#### Returns

`void`
