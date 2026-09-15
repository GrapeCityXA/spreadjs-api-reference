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
- [compose](OT_Type.md#compose)
- [create](OT_Type.md#create)
- [createDeserialized](OT_Type.md#createdeserialized)
- [deserialize](OT_Type.md#deserialize)
- [normalize](OT_Type.md#normalize)
- [transform](OT_Type.md#transform)
- [transformX](OT_Type.md#transformx)

## Properties

### <a id="uri" name="uri"></a> uri

• **uri**: `string`

操作转换类型的类型统一资源标识符（URI）。

## Methods

### <a id="apply" name="apply"></a> apply

▸ `Optional` **apply**(`snapshot`, `op`): `S`

将操作应用到快照上。

#### Parameters

| Name | Type |
| :------ | :------ |
| `snapshot` | `S` |
| `op` | `T` |

#### Returns

`S`

应用操作后的快照。

___

### <a id="compose" name="compose"></a> compose

▸ `Optional` **compose**(`op1`, `op2`): `T`

将两个操作合并为一个。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `op1` | `T` | 要与 op2 合并的操作。 |
| `op2` | `T` | 要与 op1 合并的操作。 |

#### Returns

`T`

合并后的操作。

___

### <a id="create" name="create"></a> create

▸ `Optional` **create**(`data`): `S`

从操作数据创建快照数据。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `S` | 快照的数据。 |

#### Returns

`S`

快照数据。

___

### <a id="createdeserialized" name="createdeserialized"></a> createDeserialized

▸ `Optional` **createDeserialized**(`data`): `undefined` \| `S`

从操作数据创建客户端文档数据。

#### Parameters

| Name | Type |
| :------ | :------ |
| `data` | `S` |

#### Returns

`undefined` \| `S`

反序列化后的快照数据。

___

### <a id="deserialize" name="deserialize"></a> deserialize

▸ `Optional` **deserialize**(`snapshot`): `S`

从快照数据创建客户端文档数据。

#### Parameters

| Name | Type |
| :------ | :------ |
| `snapshot` | `S` |

#### Returns

`S`

反序列化后的快照数据。

___

### <a id="normalize" name="normalize"></a> normalize

▸ `Optional` **normalize**(`op`): `T`

规范化操作。

#### Parameters

| Name | Type |
| :------ | :------ |
| `op` | `T` |

#### Returns

`T`

规范化后的操作。

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

___

### <a id="transformx" name="transformx"></a> transformX

▸ `Optional` **transformX**(`op1`, `op2`): `T`[]

转换后的 op1 和 op2。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `op1` | `T` | 基于 op2 要转换的操作。 |
| `op2` | `T` | 基于 op1 要转换的操作。 |

#### Returns

`T`[]

转换后的 op1 和 op2。
