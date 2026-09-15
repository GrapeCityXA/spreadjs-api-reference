# Enumeration: DisconnectReason

定义可能的断开连接原因。

## Table of contents

### Enumeration members

- [CLIENT\_DISCONNECT](DisconnectReason.md#client_disconnect)
- [PING\_TIMEOUT](DisconnectReason.md#ping_timeout)
- [SERVER\_DISCONNECT](DisconnectReason.md#server_disconnect)
- [TRANSPORT\_CLOSE](DisconnectReason.md#transport_close)
- [TRANSPORT\_ERROR](DisconnectReason.md#transport_error)

## Enumeration members

### <a id="client_disconnect" name="client_disconnect"></a> CLIENT\_DISCONNECT

• **CLIENT\_DISCONNECT**

表示客户端有意断开连接。

___

### <a id="ping_timeout" name="ping_timeout"></a> PING\_TIMEOUT

• **PING\_TIMEOUT**

表示客户端在 ping 超时期间没有响应 PONG 包。

___

### <a id="server_disconnect" name="server_disconnect"></a> SERVER\_DISCONNECT

• **SERVER\_DISCONNECT**

表示服务器有意断开连接。

___

### <a id="transport_close" name="transport_close"></a> TRANSPORT\_CLOSE

• **TRANSPORT\_CLOSE**

表示传输连接已关闭。

___

### <a id="transport_error" name="transport_error"></a> TRANSPORT\_ERROR

• **TRANSPORT\_ERROR**

表示传输连接中发生错误。
