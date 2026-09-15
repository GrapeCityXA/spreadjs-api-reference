# Class: Client

协作客户端，提供双向通信功能。

## Table of contents

### Constructors

- [constructor](Client.md#constructor)

### Properties

- [url](Client.md#url)

### Methods

- [connect](Client.md#connect)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Client**(`url?`)

创建一个新的协作客户端。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `url?` | `string` | 服务器地址。 |

## Properties

### <a id="url" name="url"></a> url

• **url**: `string`

## Methods

### <a id="connect" name="connect"></a> connect

▸ **connect**(`roomId`, `options?`): [`Connection`](Connection.md)

连接到一个房间。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `roomId` | `string` | 房间 ID。 |
| `options?` | [`IConnectOptions`](../interfaces/IConnectOptions.md) | 连接选项。 |

#### Returns

[`Connection`](Connection.md)
