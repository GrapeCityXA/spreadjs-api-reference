# Interface: IServerConfig

## Table of contents

### Properties

- [httpServer](IServerConfig.md#httpserver)
- [path](IServerConfig.md#path)
- [port](IServerConfig.md#port)
- [socketIoAdapter](IServerConfig.md#socketioadapter)

## Properties

### <a id="httpserver" name="httpserver"></a> httpServer

• `Optional` **httpServer**: `Server` \| `Server` \| `Http2SecureServer` \| `Http2Server`

___

### <a id="path" name="path"></a> path

• `Optional` **path**: `string`

服务器的请求路径。默认为 '/collaboration/'。

___

### <a id="port" name="port"></a> port

• `Optional` **port**: `number`

___

### <a id="socketioadapter" name="socketioadapter"></a> socketIoAdapter

• `Optional` **socketIoAdapter**: `any`

自定义 Socket.IO 适配器，用于多节点/分布式部署。
允许与各种消息代理（Redis、MongoDB、PostgreSQL 等）集成，
以实现跨多个服务器实例的消息广播。

**`see`** https://socket.io/docs/v4/adapter/
