# Class: SharedDoc<S, T\>

用于请求快照和操作的共享文档对象。

## Type parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `S` | `unknown` | 快照数据的类型。 |
| `T` | `unknown` | 操作数据的类型。 |

## Table of contents

### Constructors

- [constructor](SharedDoc.md#constructor)

### Properties

- [data](SharedDoc.md#data)
- [type](SharedDoc.md#type)
- [version](SharedDoc.md#version)

### Accessors

- [connection](SharedDoc.md#connection)
- [id](SharedDoc.md#id)

### Methods

- [create](SharedDoc.md#create)
- [del](SharedDoc.md#del)
- [destroy](SharedDoc.md#destroy)
- [fetch](SharedDoc.md#fetch)
- [fetchHistorySnapshot](SharedDoc.md#fetchhistorysnapshot)
- [hardRollback](SharedDoc.md#hardrollback)
- [off](SharedDoc.md#off)
- [on](SharedDoc.md#on)
- [once](SharedDoc.md#once)
- [submitOp](SharedDoc.md#submitop)
- [subscribe](SharedDoc.md#subscribe)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new SharedDoc**<`S`, `T`\>(`conn`)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `S` | `unknown` |
| `T` | `unknown` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `conn` | `Connection` |

## Properties

### <a id="data" name="data"></a> data

• `Optional` **data**: `S`

快照数据。

___

### <a id="type" name="type"></a> type

• `Optional` **type**: [`OT_Type`](../interfaces/OT_Type.md)<`S`, `T`\>

快照的操作转换（OT）类型。

___

### <a id="version" name="version"></a> version

• `Optional` **version**: `number`

快照的版本。

## Accessors

### <a id="connection" name="connection"></a> connection

• `get` **connection**(): `Connection`

共享文档的连接。

**`readonly`**

#### Returns

`Connection`

共享文档的连接。

___

### <a id="id" name="id"></a> id

• `get` **id**(): `string`

共享文档的 ID。

**`readonly`**

#### Returns

`string`

共享文档的 ID。

## Methods

### <a id="create" name="create"></a> create

▸ **create**(`data`, `type`, `options`, `callback?`): `void`

创建文档。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `S` | 操作数据。 |
| `type` | `string` | 操作转换（OT）类型。 |
| `options` | [`IOptions`](../interfaces/IOptions.md) | 操作的选项。 |
| `callback?` | [`ICallBack`](../interfaces/ICallBack.md)<`void`\> | 文档创建后将调用的回调函数。 |

#### Returns

`void`

___

### <a id="del" name="del"></a> del

▸ **del**(`options`, `callback`): `void`

Delete the document.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`IOptions`](../interfaces/IOptions.md) | 操作的选项。 |
| `callback` | [`ICallBack`](../interfaces/ICallBack.md)<`void`\> | 文档删除后将调用的回调函数。 |

#### Returns

`void`

___

### <a id="destroy" name="destroy"></a> destroy

▸ **destroy**(): `void`

销毁可观察对象。

#### Returns

`void`

___

### <a id="fetch" name="fetch"></a> fetch

▸ **fetch**(`callback?`): `void`

获取快照数据。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback?` | [`ICallBack`](../interfaces/ICallBack.md)<`void`\> | 获取快照后将调用的回调函数，获取到的快照数据为 `doc.data`。 |

#### Returns

`void`

___

### <a id="fetchhistorysnapshot" name="fetchhistorysnapshot"></a> fetchHistorySnapshot

▸ **fetchHistorySnapshot**(`options`, `callback`): `void`

获取历史快照数据。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`IHistorySnapshotRequestOptions`](../interfaces/IHistorySnapshotRequestOptions.md) | 历史快照的选项。 |
| `callback` | [`ICallBack`](../interfaces/ICallBack.md)<[`ISnapshot`](../interfaces/ISnapshot.md)<`S`\>\> | 获取历史快照后将调用的回调函数。 |

#### Returns

`void`

___

### <a id="hardrollback" name="hardrollback"></a> hardRollback

▸ **hardRollback**(): `void`

将快照数据硬回滚到最新版本。

#### Returns

`void`

___

### <a id="off" name="off"></a> off

▸ **off**<`NAME_2`\>(`name`, `f`): `void`

移除某个事件的监听器。

#### Type parameters

| Name | Type |
| :------ | :------ |
| `NAME_2` | extends ``"error"`` \| ``"load"`` \| ``"create"`` \| ``"del"`` \| ``"hardRollback"`` \| ``"beforeOp"`` \| ``"op"`` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `NAME_2` | 事件名称。 |
| `f` | [`IEvents`](../interfaces/IEvents.md)<`S`, `T`\>[`NAME_2`] | 事件处理程序。 |

#### Returns

`void`

___

### <a id="on" name="on"></a> on

▸ **on**<`NAME`\>(`name`, `f`): [`IEvents`](../interfaces/IEvents.md)<`S`, `T`\>[`NAME`]

注册某个事件的监听器。

#### Type parameters

| Name | Type |
| :------ | :------ |
| `NAME` | extends ``"error"`` \| ``"load"`` \| ``"create"`` \| ``"del"`` \| ``"hardRollback"`` \| ``"beforeOp"`` \| ``"op"`` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `NAME` | 事件名称。 |
| `f` | [`IEvents`](../interfaces/IEvents.md)<`S`, `T`\>[`NAME`] | 事件处理程序。 |

#### Returns

[`IEvents`](../interfaces/IEvents.md)<`S`, `T`\>[`NAME`]

___

### <a id="once" name="once"></a> once

▸ **once**<`NAME_1`\>(`name`, `f`): `void`

注册一个只调用一次的事件监听器。

#### Type parameters

| Name | Type |
| :------ | :------ |
| `NAME_1` | extends ``"error"`` \| ``"load"`` \| ``"create"`` \| ``"del"`` \| ``"hardRollback"`` \| ``"beforeOp"`` \| ``"op"`` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `NAME_1` | 事件名称。 |
| `f` | [`IEvents`](../interfaces/IEvents.md)<`S`, `T`\>[`NAME_1`] | 事件处理程序。 |

#### Returns

`void`

___

### <a id="submitop" name="submitop"></a> submitOp

▸ **submitOp**(`component`, `options?`, `callback?`): `void`

向文档提交一个操作。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `component` | `T` | 操作数据。 |
| `options?` | [`IOptions`](../interfaces/IOptions.md) | 操作的选项。 |
| `callback?` | [`ICallBack`](../interfaces/ICallBack.md)<`void`\> | 操作提交后将调用的回调函数。 |

#### Returns

`void`

___

### <a id="subscribe" name="subscribe"></a> subscribe

▸ **subscribe**(`callback?`): `void`

Subscribe the 快照数据.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callback?` | [`ICallBack`](../interfaces/ICallBack.md)<`void`\> | 订阅快照后将调用的回调函数，订阅到的快照数据为 `doc.data`。 |

#### Returns

`void`
