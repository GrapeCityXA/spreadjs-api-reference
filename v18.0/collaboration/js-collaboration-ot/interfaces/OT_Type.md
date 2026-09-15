# Interface: OT\_Type<S, T\>

OT（操作转换）类型的接口，用户可自定义协作的 OT 行为。

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

文档的类型 URI。

## Methods

### <a id="apply" name="apply"></a> apply

▸ `Optional` **apply**(`snapshot`, `op`): `S`

将操作应用于快照数据。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `snapshot` | `S` | 快照数据 |
| `op` | `T` | 操作数据 |

#### Returns

`S`

快照数据

___

### <a id="applyfragments" name="applyfragments"></a> applyFragments

▸ `Optional` **applyFragments**(`request`, `op`): `S`

将操作应用于快照片段。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `request` | [`ISnapshotFragmentsRequest`](ISnapshotFragmentsRequest.md)<`unknown`\> | 快照片段请求 |
| `op` | `T` | 操作数据 |

#### Returns

`S`

快照数据

___

### <a id="composefragments" name="composefragments"></a> composeFragments

▸ `Optional` **composeFragments**(`fragments`): `S`

从快照片段创建快照数据。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fragments` | [`ISnapshotFragments`](../README.md#isnapshotfragments)<`unknown`\> | 快照片段 |

#### Returns

`S`

快照数据

___

### <a id="create" name="create"></a> create

▸ `Optional` **create**(`data`): `S`

从操作数据创建一个快照数据。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `S` | 快照数据 |

#### Returns

`S`

快照数据

___

### <a id="createfragments" name="createfragments"></a> createFragments

▸ `Optional` **createFragments**(`data`): [`ISnapshotFragments`](../README.md#isnapshotfragments)<`unknown`\>

从操作数据创建快照片段。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `S` | 快照数据 |

#### Returns

[`ISnapshotFragments`](../README.md#isnapshotfragments)<`unknown`\>

快照片段

___

### <a id="transform" name="transform"></a> transform

▸ **transform**(`op1`, `op2`, `side`): `T`

转换操作 op1 以处理冲突。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `op1` | `T` | 要转换的操作。 |
| `op2` | `T` | 被转换操作的基础（op1 基于 op2 进行转换）。 |
| `side` | ``"left"`` \| ``"right"`` | 表示哪个参数对应的操作后到达服务器。 |

#### Returns

`T`

转换后的 op1。
