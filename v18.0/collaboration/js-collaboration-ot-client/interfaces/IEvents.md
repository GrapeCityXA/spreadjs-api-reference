# Interface: IEvents<S, T\>

共享文档的事件。

## Type parameters

| Name |
| :------ |
| `S` |
| `T` |

## Table of contents

### Methods

- [beforeOp](IEvents.md#beforeop)
- [create](IEvents.md#create)
- [del](IEvents.md#del)
- [error](IEvents.md#error)
- [hardRollback](IEvents.md#hardrollback)
- [load](IEvents.md#load)
- [op](IEvents.md#op)

## Methods

### <a id="beforeop" name="beforeop"></a> beforeOp

▸ **beforeOp**(`op`, `source?`, `src?`): `void`

在应用操作之前触发。

#### Parameters

| Name | Type |
| :------ | :------ |
| `op` | `T` |
| `source?` | `unknown` |
| `src?` | `string` |

#### Returns

`void`

___

### <a id="create" name="create"></a> create

▸ **create**(`source?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `source?` | `unknown` |

#### Returns

`void`

___

### <a id="del" name="del"></a> del

▸ **del**(`data`, `source?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `data` | `S` |
| `source?` | `unknown` |

#### Returns

`void`

___

### <a id="error" name="error"></a> error

▸ **error**(`err`): `void`

发生错误时触发。

#### Parameters

| Name | Type |
| :------ | :------ |
| `err` | [`OTError`](../classes/OTError.md) |

#### Returns

`void`

___

### <a id="hardrollback" name="hardrollback"></a> hardRollback

▸ **hardRollback**(): `void`

#### Returns

`void`

___

### <a id="load" name="load"></a> load

▸ **load**(): `void`

客户端获取或订阅快照之后触发。

#### Returns

`void`

___

### <a id="op" name="op"></a> op

▸ **op**(`op`, `source?`, `src?`): `void`

应用操作之后触发。

#### Parameters

| Name | Type |
| :------ | :------ |
| `op` | `T` |
| `source?` | `unknown` |
| `src?` | `string` |

#### Returns

`void`
