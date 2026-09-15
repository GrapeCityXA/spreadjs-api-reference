# Class: TypesManager

管理协作中的操作转换（OT）类型，通过 URI 注册和检索。

## Table of contents

### Constructors

- [constructor](TypesManager.md#constructor)

### Methods

- [getType](TypesManager.md#gettype)
- [register](TypesManager.md#register)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new TypesManager**()

## Methods

### <a id="gettype" name="gettype"></a> getType

▸ `Static` **getType**<`S`, `T`\>(`typeUri`): [`OT_Type`](../interfaces/OT_Type.md)<`S`, `T`\>

通过其 URI 检索 OT 类型。

#### Type parameters

| Name | Description |
| :------ | :------ |
| `S` | 快照数据的类型。 |
| `T` | 操作数据的类型。 |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `typeUri` | `string` | 要检索的类型的 URI。 |

#### Returns

[`OT_Type`](../interfaces/OT_Type.md)<`S`, `T`\>

与指定 URI 关联的 OT 类型。

___

### <a id="register" name="register"></a> register

▸ `Static` **register**<`S`, `T`\>(`type`): `void`

注册一个自定义的 OT 类型。

#### Type parameters

| Name | Description |
| :------ | :------ |
| `S` | 快照数据的类型。 |
| `T` | 操作数据的类型。 |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | [`OT_Type`](../interfaces/OT_Type.md)<`S`, `T`\> | 要注册的用户定义的 OT 类型。 |

#### Returns

`void`
