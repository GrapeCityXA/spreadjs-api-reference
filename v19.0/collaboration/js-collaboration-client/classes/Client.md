# Class: Client

表示一个用于双向通信的服务器协作客户端。

## Table of contents

### Constructors

- [constructor](Client.md#constructor)

### Accessors

- [url](Client.md#url)

### Methods

- [connect](Client.md#connect)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Client**(`url?`, `options?`)

创建一个新的协作客户端实例。

#### Parameters

| Name | Type |
| :------ | :------ |
| `url?` | `string` |
| `options?` | [`IClientOptions`](../interfaces/IClientOptions.md) |

## Accessors

### <a id="url" name="url"></a> url

• `get` **url**(): `string`

获取客户端的服务器 URL。

#### Returns

`string`

## Methods

### <a id="connect" name="connect"></a> connect

▸ **connect**(`roomId`, `options?`): [`Connection`](Connection.md)

连接到指定的房间。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `roomId` | `string` | 要连接的房间的 ID。 |
| `options?` | [`IConnectOptions`](../interfaces/IConnectOptions.md) | - |

#### Returns

[`Connection`](Connection.md)

- 一个新的连接实例。
