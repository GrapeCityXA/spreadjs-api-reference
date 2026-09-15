# Class: DocumentServices<S, T\>

提供协作操作转换的文档服务。

## Type parameters

| Name | Description |
| :------ | :------ |
| `S` | 快照数据的类型。 |
| `T` | 操作数据的类型。 |

## Table of contents

### Constructors

- [constructor](DocumentServices.md#constructor)

### Properties

- [db](DocumentServices.md#db)
- [maxSubmitRetries](DocumentServices.md#maxsubmitretries)
- [milestoneDb](DocumentServices.md#milestonedb)
- [submitSnapshotBatchSize](DocumentServices.md#submitsnapshotbatchsize)

### Methods

- [fetch](DocumentServices.md#fetch)
- [fetchHistorySnapshot](DocumentServices.md#fetchhistorysnapshot)
- [getOps](DocumentServices.md#getops)
- [on](DocumentServices.md#on)
- [submit](DocumentServices.md#submit)
- [use](DocumentServices.md#use)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new DocumentServices**<`S`, `T`\>(`config?`)

#### Type parameters

| Name |
| :------ |
| `S` |
| `T` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `config?` | [`IDocConfig`](../interfaces/IDocConfig.md)<`S`, `T`\> |

## Properties

### <a id="db" name="db"></a> db

• **db**: [`IDatabaseAdapter`](../interfaces/IDatabaseAdapter.md)<`S`, `T`\>

用于存储文档数据的数据库适配器。

**`template`** 快照数据的类型。

**`template`** 操作数据的类型。

___

### <a id="maxsubmitretries" name="maxsubmitretries"></a> maxSubmitRetries

• `Optional` **maxSubmitRetries**: `number`

提交操作的最大重试次数。

**`default`** undefined - 没有重试限制。

___

### <a id="milestonedb" name="milestonedb"></a> milestoneDb

• **milestoneDb**: [`IMilestoneDatabaseAdapter`](../interfaces/IMilestoneDatabaseAdapter.md)<`S`\>

用于快照里程碑的里程碑数据库适配器。

**`template`** 快照数据的类型。

___

### <a id="submitsnapshotbatchsize" name="submitsnapshotbatchsize"></a> submitSnapshotBatchSize

• **submitSnapshotBatchSize**: `number`

提交快照的批量大小。

**`default`** 100

## Methods

### <a id="fetch" name="fetch"></a> fetch

▸ **fetch**(`id`, `context?`): `Promise`<[`ISnapshot`](../interfaces/ISnapshot.md)<`S`\>\>

检索文档的最新快照。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | 文档的 ID。 |
| `context?` | [`IContext`](../interfaces/IContext.md) | - |

#### Returns

`Promise`<[`ISnapshot`](../interfaces/ISnapshot.md)<`S`\>\>

一个 Promise，在文档快照被检索后，文档快照被检索。

___

### <a id="fetchhistorysnapshot" name="fetchhistorysnapshot"></a> fetchHistorySnapshot

▸ **fetchHistorySnapshot**(`id`, `version?`, `context?`): `Promise`<[`ISnapshot`](../interfaces/ISnapshot.md)<`S`\>\>

通过版本检索文档的历史快照。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | 文档的 ID。 |
| `version?` | `number` | - |
| `context?` | [`IContext`](../interfaces/IContext.md) | - |

#### Returns

`Promise`<[`ISnapshot`](../interfaces/ISnapshot.md)<`S`\>\>

一个 Promise，在历史快照被检索后，历史快照被检索。

___

### <a id="getops" name="getops"></a> getOps

▸ **getOps**(`id`, `from`, `to?`, `context?`): `Promise`<[`IOp`](../interfaces/IOp.md)<`T`\>[]\>

检索两个版本之间的操作（包括 'from'，不包括 'to'）。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | 文档的 ID。 |
| `from` | `number` | 起始版本。 |
| `to?` | `number` | - |
| `context?` | [`IContext`](../interfaces/IContext.md) | - |

#### Returns

`Promise`<[`IOp`](../interfaces/IOp.md)<`T`\>[]\>

一个 Promise，在操作数组被检索后，操作数组被检索。

___

### <a id="on" name="on"></a> on

▸ **on**<`K`\>(`hookName`, `hook`): `void`

注册一个钩子用于特定事件。

#### Type parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `K` | extends keyof [`IDocHookContext`](../interfaces/IDocHookContext.md) | 钩子名称的类型，扩展 keyof IDocHookContext。 |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hookName` | `K` | 要注册的钩子名称。 |
| `hook` | `IHook`<[`IDocHookContext`](../interfaces/IDocHookContext.md)[`K`]\> | 要注册的钩子。 |

#### Returns

`void`

___

### <a id="submit" name="submit"></a> submit

▸ **submit**(`id`, `op`, `context?`): `Promise`<[`IOp`](../interfaces/IOp.md)<`T`\>[]\>

提交一个操作到文档（必须包含 {op:}、{create:} 或 {del:} 字段）。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | 文档的 ID。 |
| `op` | [`IOp`](../interfaces/IOp.md)<`T`\> | 要提交的操作。 |
| `context?` | [`IContext`](../interfaces/IContext.md) | - |

#### Returns

`Promise`<[`IOp`](../interfaces/IOp.md)<`T`\>[]\>

一个 Promise，在操作数组被检索后，操作数组被检索。

___

### <a id="use" name="use"></a> use

▸ **use**<`K`\>(`action`, `middleware`): `void`

注册一个中间件用于特定操作。

#### Type parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `K` | extends keyof [`IDocMiddlewareContext`](../interfaces/IDocMiddlewareContext.md)<`S`, `T`\> | 操作名称的类型，扩展 keyof IDocMiddlewareContext<S, T>。 |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `action` | `K` | 要与中间件关联的操作名称。 |
| `middleware` | `IMiddleware`<[`IDocMiddlewareContext`](../interfaces/IDocMiddlewareContext.md)<`S`, `T`\>[`K`]\> | 要注册的中间件。 |

#### Returns

`void`
