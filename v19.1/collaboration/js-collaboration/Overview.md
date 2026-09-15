# js-collaboration

## Table of contents

### Classes

- [Connection](classes/Connection.md)
- [Server](classes/Server.md)

### Interfaces

- [IConnectContext](interfaces/IConnectContext.md)
- [IConnectMiddlewareContext](interfaces/IConnectMiddlewareContext.md)
- [ICreateRoomContext](interfaces/ICreateRoomContext.md)
- [IDeactivateServerLicenseResult](interfaces/IDeactivateServerLicenseResult.md)
- [IDestroyRoomContext](interfaces/IDestroyRoomContext.md)
- [IDisconnectContext](interfaces/IDisconnectContext.md)
- [IEnterRoomContext](interfaces/IEnterRoomContext.md)
- [IFeature](interfaces/IFeature.md)
- [IHook](interfaces/IHook.md)
- [IHookContext](interfaces/IHookContext.md)
- [IHooks](interfaces/IHooks.md)
- [ILeaveRoomContext](interfaces/ILeaveRoomContext.md)
- [IMessageContext](interfaces/IMessageContext.md)
- [IMessageMiddlewareContext](interfaces/IMessageMiddlewareContext.md)
- [IMiddleware](interfaces/IMiddleware.md)
- [IMiddlewareContext](interfaces/IMiddlewareContext.md)
- [IMiddlewares](interfaces/IMiddlewares.md)
- [INext](interfaces/INext.md)
- [IServerConfig](interfaces/IServerConfig.md)

### Type aliases

- [MessageData](Overview.md#messagedata)
- [MessageType](Overview.md#messagetype)

### Functions

- [deactivateServerLicense](Overview.md#deactivateserverlicense)
- [getMachineIdForServerLicense](Overview.md#getmachineidforserverlicense)

## Type aliases

### <a id="messagedata" name="messagedata"></a> MessageData

Ƭ **MessageData**: `unknown`

___

### <a id="messagetype" name="messagetype"></a> MessageType

Ƭ **MessageType**: `string` \| ``null``

## Functions

### <a id="deactivateserverlicense" name="deactivateserverlicense"></a> deactivateServerLicense

▸ **deactivateServerLicense**(): [`IDeactivateServerLicenseResult`](interfaces/IDeactivateServerLicenseResult.md)[]

停用当前机器上注册的许可证密钥。
该函数会停用许可证，并返回当前机器上所有停用记录的数组。
数组按时间顺序排列，最近的停用记录位于索引 [0]。

#### Returns

[`IDeactivateServerLicenseResult`](interfaces/IDeactivateServerLicenseResult.md)[]

___

### <a id="getmachineidforserverlicense" name="getmachineidforserverlicense"></a> getMachineIdForServerLicense

▸ **getMachineIdForServerLicense**(): `string`

获取当前机器的唯一授权 ID。

#### Returns

`string`

当前机器的 ID 字符串。
