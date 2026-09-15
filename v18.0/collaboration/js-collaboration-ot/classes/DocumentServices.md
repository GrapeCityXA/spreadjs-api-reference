# Class: DocumentServices<S, T\>

The document services for collaboration.

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

• **db**: [`IDataBaseAdapter`](../interfaces/IDataBaseAdapter.md)<`S`, `T`\>

数据库适配器。

**`template`** 快照数据的类型。

**`template`** 操作数据的类型。

___

### <a id="maxsubmitretries" name="maxsubmitretries"></a> maxSubmitRetries

• `Optional` **maxSubmitRetries**: `number`

提交操作时的最大重试次数。

**`default`** undefined - 无限制

___

### <a id="milestonedb" name="milestonedb"></a> milestoneDb

• **milestoneDb**: [`IMilestoneDataBaseAdapter`](../interfaces/IMilestoneDataBaseAdapter.md)<`S`\>

里程碑数据库适配器。

**`template`** 快照数据的类型。

___

### <a id="submitsnapshotbatchsize" name="submitsnapshotbatchsize"></a> submitSnapshotBatchSize

• **submitSnapshotBatchSize**: `number`

提交快照时的批量大小。

**`default`** 100

## Methods

### <a id="fetch" name="fetch"></a> fetch

▸ **fetch**(`id`, `context?`): `Promise`<[`ISnapshot`](../interfaces/ISnapshot.md)<`S`\>\>

获取最新的快照

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | document id |
| `context?` | [`IContext`](../interfaces/IContext.md) | - |

#### Returns

`Promise`<[`ISnapshot`](../interfaces/ISnapshot.md)<`S`\>\>

___

### <a id="fetchhistorysnapshot" name="fetchhistorysnapshot"></a> fetchHistorySnapshot

▸ **fetchHistorySnapshot**(`id`, `version?`, `context?`): `Promise`<[`ISnapshot`](../interfaces/ISnapshot.md)<`S`\>\>

按版本获取历史快照

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | document id |
| `version?` | `number` | - |
| `context?` | [`IContext`](../interfaces/IContext.md) | - |

#### Returns

`Promise`<[`ISnapshot`](../interfaces/ISnapshot.md)<`S`\>\>

___

### <a id="getops" name="getops"></a> getOps

▸ **getOps**(`id`, `from`, `to?`, `context?`): `Promise`<[`IOp`](../interfaces/IOp.md)<`T`\>[]\>

获取两个版本之间的操作，包含起始版本，但不包含结束版本

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | document id |
| `from` | `number` | from version |
| `to?` | `number` | to version |
| `context?` | [`IContext`](../interfaces/IContext.md) | - |

#### Returns

`Promise`<[`IOp`](../interfaces/IOp.md)<`T`\>[]\>

___

### <a id="on" name="on"></a> on

▸ **on**<`K`\>(`hookName`, `hook`): `void`

向文档服务注册钩子

#### Type parameters

| Name | Type |
| :------ | :------ |
| `K` | extends keyof [`IDocHookContext`](../interfaces/IDocHookContext.md) |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hookName` | `K` | 钩子名称 |
| `hook` | `IHook`<[`IDocHookContext`](../interfaces/IDocHookContext.md)[`K`]\> | the 要注册的钩子 |

#### Returns

`void`

___

### <a id="submit" name="submit"></a> submit

▸ **submit**(`id`, `op`, `context?`, `afterCommitCallback?`): `Promise`<[`IOp`](../interfaces/IOp.md)<`T`\>[]\>

提交操作。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | 文档 ID |
| `op` | [`IOp`](../interfaces/IOp.md)<`T`\> | 操作 |
| `context?` | [`IContext`](../interfaces/IContext.md) | 上下文 |
| `afterCommitCallback?` | [`IAfterCommitCallback`](../interfaces/IAfterCommitCallback.md)<`S`, `T`\> | 向数据库提交操作后的回调 |

#### Returns

`Promise`<[`IOp`](../interfaces/IOp.md)<`T`\>[]\>

___

### <a id="use" name="use"></a> use

▸ **use**<`K`\>(`action`, `middleware`): `void`

向文档服务注册中间件

#### Type parameters

| Name | Type |
| :------ | :------ |
| `K` | extends keyof [`IDocMiddlewareContext`](../interfaces/IDocMiddlewareContext.md)<`S`, `T`\> |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `action` | `K` | 动作名称 |
| `middleware` | `IMiddleware`<[`IDocMiddlewareContext`](../interfaces/IDocMiddlewareContext.md)<`S`, `T`\>[`K`]\> | 要注册的中间件 |

#### Returns

`void`
