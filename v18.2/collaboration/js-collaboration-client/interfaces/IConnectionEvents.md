# Interface: IConnectionEvents

## Table of contents

### Methods

- [connect](IConnectionEvents.md#connect)
- [disconnect](IConnectionEvents.md#disconnect)
- [error](IConnectionEvents.md#error)
- [message](IConnectionEvents.md#message)
- [reconnect](IConnectionEvents.md#reconnect)
- [reconnectAttempts](IConnectionEvents.md#reconnectattempts)
- [reconnectFailed](IConnectionEvents.md#reconnectfailed)

## Methods

### <a id="connect" name="connect"></a> connect

▸ **connect**(): `void`

#### Returns

`void`

___

### <a id="disconnect" name="disconnect"></a> disconnect

▸ **disconnect**(`reason`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `reason` | [`DisconnectReason`](../enums/DisconnectReason.md) |

#### Returns

`void`

___

### <a id="error" name="error"></a> error

▸ **error**(`e`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `Error` |

#### Returns

`void`

___

### <a id="message" name="message"></a> message

▸ **message**(`data`, `type`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `data` | `unknown` |
| `type` | [`MessageType`](../README.md#messagetype) |

#### Returns

`void`

___

### <a id="reconnect" name="reconnect"></a> reconnect

▸ **reconnect**(`attempts`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `attempts` | `number` |

#### Returns

`void`

___

### <a id="reconnectattempts" name="reconnectattempts"></a> reconnectAttempts

▸ **reconnectAttempts**(`attempts`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `attempts` | `number` |

#### Returns

`void`

___

### <a id="reconnectfailed" name="reconnectfailed"></a> reconnectFailed

▸ **reconnectFailed**(): `void`

#### Returns

`void`
