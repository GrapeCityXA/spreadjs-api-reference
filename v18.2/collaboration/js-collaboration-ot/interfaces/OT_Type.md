# Interface: OT\_Type<S, T\>

定义协作中操作转换（OT）行为的接口。

## Type parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `S` | `unknown` | 快照数据的类型。 |
| `T` | `unknown` | 操作数据的类型。 |

## Table of contents

### Properties

- [uri](OT_Type.md#uri)

### Methods

- [apply](OT_Type.md#apply)
- [applyFragments](OT_Type.md#applyfragments)
- [composeFragments](OT_Type.md#composefragments)
- [create](OT_Type.md#create)
- [createFragments](OT_Type.md#createfragments)
- [transform](OT_Type.md#transform)

## Properties

### <a id="uri" name="uri"></a> uri

• **uri**: `string`

标识文档类型的 URI。

## Methods

### <a id="apply" name="apply"></a> apply

▸ `Optional` **apply**(`snapshot`, `op`): `S`

将一个操作应用到快照数据。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `snapshot` | `S` | 当前快照数据。 |
| `op` | `T` | 要应用的操作。 |

#### Returns

`S`

更新的快照数据。

___

### <a id="applyfragments" name="applyfragments"></a> applyFragments

▸ `Optional` **applyFragments**(`request`, `op`): `Promise`<`void`\>

异步地将一个操作应用到快照片段。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `request` | [`ISnapshotFragmentsRequest`](ISnapshotFragmentsRequest.md)<`unknown`\> | 包含快照片段的请求。 |
| `op` | `T` | 要应用的操作。 |

#### Returns

`Promise`<`void`\>

一个 Promise，当操作被应用时， Promise 被解决。

___

### <a id="composefragments" name="composefragments"></a> composeFragments

▸ `Optional` **composeFragments**(`fragments`): `S`

从快照片段组合快照数据。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fragments` | [`ISnapshotFragments`](../README.md#isnapshotfragments)<`unknown`\> | 快照片段。 |

#### Returns

`S`

组合的快照数据。

___

### <a id="create" name="create"></a> create

▸ `Optional` **create**(`data`): `S`

从提供的快照数据创建初始快照数据。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `S` | 初始快照数据。 |

#### Returns

`S`

创建的快照数据。

___

### <a id="createfragments" name="createfragments"></a> createFragments

▸ `Optional` **createFragments**(`data`): [`ISnapshotFragments`](../README.md#isnapshotfragments)<`unknown`\>

从快照数据生成快照片段。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `S` | 快照数据。 |

#### Returns

[`ISnapshotFragments`](../README.md#isnapshotfragments)<`unknown`\>

生成的快照片段。

___

### <a id="transform" name="transform"></a> transform

▸ **transform**(`op1`, `op2`, `side`): `T`

将一个操作转换为与另一个操作解决冲突。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `op1` | `T` | 要转换的操作。 |
| `op2` | `T` | 作为转换基础的操作。 |
| `side` | ``"left"`` \| ``"right"`` | 指示哪个操作在服务器上到达较晚。 |

#### Returns

`T`

转换后的操作。
