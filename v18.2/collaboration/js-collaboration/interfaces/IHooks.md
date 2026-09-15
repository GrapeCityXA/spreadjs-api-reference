# Interface: IHooks

## Table of contents

### Properties

- [connect](IHooks.md#connect)
- [createRoom](IHooks.md#createroom)
- [destroyRoom](IHooks.md#destroyroom)
- [disconnect](IHooks.md#disconnect)
- [enterRoom](IHooks.md#enterroom)
- [leaveRoom](IHooks.md#leaveroom)
- [message](IHooks.md#message)

## Properties

### <a id="connect" name="connect"></a> connect

• `Optional` **connect**: [`IHook`](IHook.md)<[`IConnectContext`](IConnectContext.md)\>

___

### <a id="createroom" name="createroom"></a> createRoom

• `Optional` **createRoom**: [`IHook`](IHook.md)<[`ICreateRoomContext`](ICreateRoomContext.md)\>

___

### <a id="destroyroom" name="destroyroom"></a> destroyRoom

• `Optional` **destroyRoom**: [`IHook`](IHook.md)<[`IDestroyRoomContext`](IDestroyRoomContext.md)\>

___

### <a id="disconnect" name="disconnect"></a> disconnect

• `Optional` **disconnect**: [`IHook`](IHook.md)<[`IDisconnectContext`](IDisconnectContext.md)\>

___

### <a id="enterroom" name="enterroom"></a> enterRoom

• `Optional` **enterRoom**: [`IHook`](IHook.md)<[`IEnterRoomContext`](IEnterRoomContext.md)\>

___

### <a id="leaveroom" name="leaveroom"></a> leaveRoom

• `Optional` **leaveRoom**: [`IHook`](IHook.md)<[`ILeaveRoomContext`](ILeaveRoomContext.md)\>

___

### <a id="message" name="message"></a> message

• `Optional` **message**: [`IHook`](IHook.md)<[`IMessageContext`](IMessageContext.md)\>
