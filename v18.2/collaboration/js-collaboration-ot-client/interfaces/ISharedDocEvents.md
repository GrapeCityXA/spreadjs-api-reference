# Interface: ISharedDocEvents<S, T\>

由 SharedDoc 发出的事件。

## Type parameters

| Name | Description |
| :------ | :------ |
| `S` | 快照数据的类型。 |
| `T` | 操作数据的类型。 |

## Table of contents

### Methods

- [beforeOp](ISharedDocEvents.md#beforeop)
- [create](ISharedDocEvents.md#create)
- [del](ISharedDocEvents.md#del)
- [error](ISharedDocEvents.md#error)
- [hardRollback](ISharedDocEvents.md#hardrollback)
- [load](ISharedDocEvents.md#load)
- [op](ISharedDocEvents.md#op)

## Methods

### <a id="beforeop" name="beforeop"></a> beforeOp

▸ **beforeOp**(`op`, `source?`): `void`

在应用操作之前触发。

#### Parameters

| Name | Type |
| :------ | :------ |
| `op` | `T` |
| `source?` | `unknown` |

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

当发生错误时触发。

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

在客户端获取或订阅快照后触发。

#### Returns

`void`

___

### <a id="op" name="op"></a> op

▸ **op**(`op`, `source?`): `void`

在应用操作之后触发。

#### Parameters

| Name | Type |
| :------ | :------ |
| `op` | `T` |
| `source?` | `unknown` |

#### Returns

`void`
