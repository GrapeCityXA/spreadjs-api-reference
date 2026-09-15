# Class: SharedDoc<S, T\>

表示用于请求快照和操作的共享文档。

## Type parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `S` | `unknown` | 快照数据的类型。 |
| `T` | `unknown` | 操作数据的类型。 |

## Table of contents

### Constructors

- [constructor](SharedDoc.md#constructor)

### Accessors

- [connection](SharedDoc.md#connection)
- [data](SharedDoc.md#data)
- [id](SharedDoc.md#id)
- [type](SharedDoc.md#type)
- [version](SharedDoc.md#version)

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
- [restore](SharedDoc.md#restore)
- [submitOp](SharedDoc.md#submitop)
- [subscribe](SharedDoc.md#subscribe)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new SharedDoc**<`S`, `T`\>(`conn`)

创建一个新的共享文档实例。

#### Type parameters

| Name | Type |
| :------ | :------ |
| `S` | `unknown` |
| `T` | `unknown` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `conn` | `Connection` |

## Accessors

### <a id="connection" name="connection"></a> connection

• `get` **connection**(): `Connection`

检索与共享文档关联的连接。

#### Returns

`Connection`

连接实例。

___

### <a id="data" name="data"></a> data

• `get` **data**(): `undefined` \| `S`

检索当前快照的数据。

#### Returns

`undefined` \| `S`

___

### <a id="id" name="id"></a> id

• `get` **id**(): `string`

检索共享文档的 ID。

#### Returns

`string`

文档 ID。

___

### <a id="type" name="type"></a> type

• `get` **type**(): `undefined` \| [`OT_Type`](../interfaces/OT_Type.md)<`S`, `T`\>

检索快照的 OT 类型。

#### Returns

`undefined` \| [`OT_Type`](../interfaces/OT_Type.md)<`S`, `T`\>

___

### <a id="version" name="version"></a> version

• `get` **version**(): `undefined` \| `number`

检索当前快照的版本。

#### Returns

`undefined` \| `number`

## Methods

### <a id="create" name="create"></a> create

▸ **create**(`data`, `type`, `options`): `Promise`<`void`\>

创建一个新文档。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `S` | 用于初始化快照的数据。 |
| `type` | `string` | OT 类型的 URI。 |
| `options` | [`IOptions`](../interfaces/IOptions.md) | 操作的选项。 |

#### Returns

`Promise`<`void`\>

一个 Promise，在文档被创建后，文档被创建。

___

### <a id="del" name="del"></a> del

▸ **del**(`options`): `Promise`<`void`\>

删除文档。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`IOptions`](../interfaces/IOptions.md) | 操作的选项。 |

#### Returns

`Promise`<`void`\>

一个 Promise，在文档被删除后，文档被删除。

___

### <a id="destroy" name="destroy"></a> destroy

▸ **destroy**(): `void`

销毁可观察对象并清理资源。

#### Returns

`void`

___

### <a id="fetch" name="fetch"></a> fetch

▸ **fetch**(): `Promise`<`void`\>

检索快照数据。

#### Returns

`Promise`<`void`\>

一个 Promise，在快照被获取后，获取的快照数据为 'doc.data'。

___

### <a id="fetchhistorysnapshot" name="fetchhistorysnapshot"></a> fetchHistorySnapshot

▸ **fetchHistorySnapshot**(`options`): `Promise`<[`ISnapshot`](../interfaces/ISnapshot.md)<`S`\>\>

检索历史快照数据。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [`IHistorySnapshotRequestOptions`](../interfaces/IHistorySnapshotRequestOptions.md) | 历史快照请求的选项。 |

#### Returns

`Promise`<[`ISnapshot`](../interfaces/ISnapshot.md)<`S`\>\>

一个 Promise，在历史快照被检索后，历史快照被检索。

___

### <a id="hardrollback" name="hardrollback"></a> hardRollback

▸ **hardRollback**(): `Promise`<`void`\>

硬回滚快照数据到最新版本。

#### Returns

`Promise`<`void`\>

一个 Promise，在回滚完成后，回滚完成。

___

### <a id="off" name="off"></a> off

▸ **off**<`NAME`\>(`name`, `f`): `void`

移除特定事件的监听器。

#### Type parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `NAME` | extends keyof [`ISharedDocEvents`](../interfaces/ISharedDocEvents.md)<`S`, `T`\> | 事件名称的类型，扩展 ISharedDocEvents<S, T> 的键。 |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `NAME` | 事件的名称。 |
| `f` | [`ISharedDocEvents`](../interfaces/ISharedDocEvents.md)<`S`, `T`\>[`NAME`] | 要移除的事件处理程序函数。 |

#### Returns

`void`

___

### <a id="on" name="on"></a> on

▸ **on**<`NAME`\>(`name`, `f`): [`ISharedDocEvents`](../interfaces/ISharedDocEvents.md)<`S`, `T`\>[`NAME`]

注册特定事件的监听器。

#### Type parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `NAME` | extends keyof [`ISharedDocEvents`](../interfaces/ISharedDocEvents.md)<`S`, `T`\> | 事件名称的类型，扩展 ISharedDocEvents<S, T> 的键。 |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `NAME` | 事件的名称。 |
| `f` | [`ISharedDocEvents`](../interfaces/ISharedDocEvents.md)<`S`, `T`\>[`NAME`] | 事件处理程序函数。 |

#### Returns

[`ISharedDocEvents`](../interfaces/ISharedDocEvents.md)<`S`, `T`\>[`NAME`]

注册的事件处理程序。

___

### <a id="once" name="once"></a> once

▸ **once**<`NAME`\>(`name`, `f`): `void`

注册一次性监听器。

#### Type parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `NAME` | extends keyof [`ISharedDocEvents`](../interfaces/ISharedDocEvents.md)<`S`, `T`\> | 事件名称的类型，扩展 ISharedDocEvents<S, T> 的键。 |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `NAME` | 事件的名称。 |
| `f` | [`ISharedDocEvents`](../interfaces/ISharedDocEvents.md)<`S`, `T`\>[`NAME`] | 一次调用的事件处理程序函数。 |

#### Returns

`void`

___

### <a id="restore" name="restore"></a> restore

▸ **restore**(`targetVersion`, `options?`): `Promise`<`void`\>

将文档恢复到指定版本。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `targetVersion` | `number` | 要恢复到的目标版本号。 |
| `options?` | [`IOptions`](../interfaces/IOptions.md) | 操作的选项。 |

#### Returns

`Promise`<`void`\>

文档恢复完成后解决的 Promise。

___

### <a id="submitop" name="submitop"></a> submitOp

▸ **submitOp**(`component`, `options?`): `Promise`<`void`\>

提交一个操作到文档。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `component` | `T` | 操作组件。 |
| `options?` | [`IOptions`](../interfaces/IOptions.md) | - |

#### Returns

`Promise`<`void`\>

一个 Promise，在操作被提交后，操作被提交。

___

### <a id="subscribe" name="subscribe"></a> subscribe

▸ **subscribe**(): `Promise`<`void`\>

订阅快照数据。

#### Returns

`Promise`<`void`\>

一个 Promise，在快照被订阅后，订阅的快照数据为 'doc.data'。
