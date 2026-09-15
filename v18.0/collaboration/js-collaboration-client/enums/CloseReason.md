# Enumeration: CloseReason

连接关闭的原因。

## Table of contents

### Enumeration members

- [CLIENT\_DISCONNECT](CloseReason.md#client_disconnect)
- [PING\_TIMEOUT](CloseReason.md#ping_timeout)
- [SERVER\_DISCONNECT](CloseReason.md#server_disconnect)
- [TRANSPORT\_CLOSE](CloseReason.md#transport_close)
- [TRANSPORT\_ERROR](CloseReason.md#transport_error)

## Enumeration members

### <a id="client_disconnect" name="client_disconnect"></a> CLIENT\_DISCONNECT

• **CLIENT\_DISCONNECT**

客户端已手动断开连接。

___

### <a id="ping_timeout" name="ping_timeout"></a> PING\_TIMEOUT

• **PING\_TIMEOUT**

客户端在 pingTimeout 延迟时间内未发送 PONG 数据包。

___

### <a id="server_disconnect" name="server_disconnect"></a> SERVER\_DISCONNECT

• **SERVER\_DISCONNECT**

服务器已手动断开连接。

___

### <a id="transport_close" name="transport_close"></a> TRANSPORT\_CLOSE

• **TRANSPORT\_CLOSE**

传输连接已关闭。

___

### <a id="transport_error" name="transport_error"></a> TRANSPORT\_ERROR

• **TRANSPORT\_ERROR**

传输连接遇到了错误。
