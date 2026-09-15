# Interface: IEvents

## Table of contents

### Methods

- [close](IEvents.md#close)
- [connectionStateChanged](IEvents.md#connectionstatechanged)
- [error](IEvents.md#error)
- [message](IEvents.md#message)
- [open](IEvents.md#open)
- [reconnect](IEvents.md#reconnect)
- [reconnectAttempts](IEvents.md#reconnectattempts)
- [reconnectFailed](IEvents.md#reconnectfailed)

## Methods

### <a id="close" name="close"></a> close

▸ **close**(`reason`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `reason` | [`CloseReason`](../enums/CloseReason.md) |

#### Returns

`void`

___

### <a id="connectionstatechanged" name="connectionstatechanged"></a> connectionStateChanged

▸ **connectionStateChanged**(): `void`

#### Returns

`void`

___

### <a id="error" name="error"></a> error

▸ **error**(`e`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `unknown` |

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

### <a id="open" name="open"></a> open

▸ **open**(): `void`

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

▸ **reconnectFailed**(`err?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `err?` | `Error` |

#### Returns

`void`
