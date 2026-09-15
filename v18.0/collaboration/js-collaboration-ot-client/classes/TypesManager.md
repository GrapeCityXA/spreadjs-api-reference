# Class: TypesManager

用于协作的类型管理器，提供注册操作转换（OT）类型并通过类型 URI 获取类型的方法。
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

通过类型 URI 获取操作转换（OT）类型。

#### Type parameters

| Name |
| :------ |
| `S` |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `typeUri` | `string` | 类型 URI。 |

#### Returns

[`OT_Type`](../interfaces/OT_Type.md)<`S`, `T`\>

指定类型 URI 的类型对象。

___

### <a id="register" name="register"></a> register

▸ `Static` **register**<`S`, `T`\>(`type`): `void`

注册操作转换（OT）类型。

#### Type parameters

| Name |
| :------ |
| `S` |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | [`OT_Type`](../interfaces/OT_Type.md)<`S`, `T`\> | 用户自定义的类型对象。 |

#### Returns

`void`
