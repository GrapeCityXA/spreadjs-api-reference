# Interface: IServerConfig

## Table of contents

### Properties

- [allowRequest](IServerConfig.md#allowrequest)
- [cors](IServerConfig.md#cors)
- [httpServer](IServerConfig.md#httpserver)
- [maxDecompressedMessageSize](IServerConfig.md#maxdecompressedmessagesize)
- [maxHttpBufferSize](IServerConfig.md#maxhttpbuffersize)
- [path](IServerConfig.md#path)
- [port](IServerConfig.md#port)
- [socketIoAdapter](IServerConfig.md#socketioadapter)

## Properties

### <a id="allowrequest" name="allowrequest"></a> allowRequest

• `Optional` **allowRequest**: `any`

直接透传给 Socket.IO 的 `allowRequest` 选项。
可使用此项控制是否接受握手或升级请求。

**`see`** https://socket.io/docs/v4/server-options/#allowrequest

___

### <a id="cors" name="cors"></a> cors

• `Optional` **cors**: `any`

直接透传给 Socket.IO 的 `cors` 选项。
可使用此项配置 Socket.IO HTTP 请求的 CORS 行为。

**`see`** https://socket.io/docs/v4/handling-cors/

___

### <a id="httpserver" name="httpserver"></a> httpServer

• `Optional` **httpServer**: `Server` \| `Server` \| `Http2SecureServer` \| `Http2Server`

___

### <a id="maxdecompressedmessagesize" name="maxdecompressedmessagesize"></a> maxDecompressedMessageSize

• `Optional` **maxDecompressedMessageSize**: `number`

压缩消息解压后的最大允许字节数。
超过此限制时会报告消息错误，但不会导致服务器进程崩溃。
默认值为当前 Node.js 的最大字符串长度；如果运行时未暴露该限制，则默认为 512 MiB。

___

### <a id="maxhttpbuffersize" name="maxhttpbuffersize"></a> maxHttpBufferSize

• `Optional` **maxHttpBufferSize**: `number`

传入消息的最大字节数。
当负载超过该值时，Socket.IO 会关闭连接。
默认值为 512 MiB.

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
