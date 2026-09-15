# Interface: OT\_Type<S, T\>

定义用于自定义协作中操作转换（OT）行为的接口。

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

### <a id="compose" name="compose"></a> compose

▸ `Optional` **compose**(`op1`, `op2`): `T`

将两个操作组合成一个操作。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `op1` | `T` | 要组合的第一个操作。 |
| `op2` | `T` | 与 op1 组合的第二个操作。 |

#### Returns

`T`

组合的操作。

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

### <a id="createdeserialized" name="createdeserialized"></a> createDeserialized

▸ `Optional` **createDeserialized**(`data`): `undefined` \| `S`

从快照数据创建反序列化的客户端文档数据。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `S` | 要反序列化的快照数据。 |

#### Returns

`undefined` \| `S`

反序列化的快照数据，或 undefined 如果不适用于。

___

### <a id="deserialize" name="deserialize"></a> deserialize

▸ `Optional` **deserialize**(`snapshot`): `S`

为客户端使用反序列化快照数据。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `snapshot` | `S` | 要反序列化的快照数据。 |

#### Returns

`S`

反序列化的快照数据。

___

### <a id="normalize" name="normalize"></a> normalize

▸ `Optional` **normalize**(`op`): `T`

规范化一个操作。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `op` | `T` | 要规范化的操作。 |

#### Returns

`T`

规范化的操作。

___

### <a id="transform" name="transform"></a> transform

▸ **transform**(`op1`, `op2`, `side`): `T`

将一个操作转换为解决与其他操作的冲突。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `op1` | `T` | 要转换的操作。 |
| `op2` | `T` | 作为转换基础的操作。 |
| `side` | ``"left"`` \| ``"right"`` | 指示哪个操作在服务器上稍后到达。 |

#### Returns

`T`

转换后的操作。

___

### <a id="transformx" name="transformx"></a> transformX

▸ `Optional` **transformX**(`op1`, `op2`): `T`[]

将两个操作相互转换。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `op1` | `T` | 要基于 op2 转换的操作。 |
| `op2` | `T` | 要基于 op1 转换的操作。 |

#### Returns

`T`[]

包含转换后的 op1 和 op2 的数组。
