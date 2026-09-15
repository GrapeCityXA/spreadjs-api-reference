# Class: NameInfo

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).NameInfo

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.NameInfo.md#constructor)

### Methods

- [getColumn](GC.Spread.Sheets.NameInfo.md#getcolumn)
- [getComment](GC.Spread.Sheets.NameInfo.md#getcomment)
- [getExpression](GC.Spread.Sheets.NameInfo.md#getexpression)
- [getName](GC.Spread.Sheets.NameInfo.md#getname)
- [getRow](GC.Spread.Sheets.NameInfo.md#getrow)
- [isReadOnly](GC.Spread.Sheets.NameInfo.md#isreadonly)
- [set](GC.Spread.Sheets.NameInfo.md#set)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new NameInfo**(`name`, `expr`, `row`, `column`, `comment?`, `isReadOnly?`)

表示一个可用于公式的自定义命名表达式。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 自定义表达式名称。 |
| `expr` | [`Expression`](GC.Spread.CalcEngine.Expression.md) | 自定义命名表达式。 |
| `row` | `number` | 表达式的基础行。 |
| `column` | `number` | 表达式的基础列。 |
| `comment?` | `string` | - |
| `isReadOnly?` | `boolean` | - |

## Methods

### <a id="getcolumn" name="getcolumn"></a> getColumn

▸ **getColumn**(): `number`

获取自定义命名表达式的基础列。

#### Returns

`number`

基础列。

___

### <a id="getcomment" name="getcomment"></a> getComment

▸ **getComment**(): `string`

获取当前NameInfo对象的注释。

#### Returns

`string`

当前NameInfo对象的名称。

___

### <a id="getexpression" name="getexpression"></a> getExpression

▸ **getExpression**(): [`Expression`](GC.Spread.CalcEngine.Expression.md)

获取表达式。

#### Returns

[`Expression`](GC.Spread.CalcEngine.Expression.md)

表达式。

___

### <a id="getname" name="getname"></a> getName

▸ **getName**(): `string`

获取当前NameInfo对象的名称。

#### Returns

`string`

当前NameInfo对象的名称。

___

### <a id="getrow" name="getrow"></a> getRow

▸ **getRow**(): `number`

获取自定义命名表达式的基础行。

#### Returns

`number`

基础行。

___

### <a id="isreadonly" name="isreadonly"></a> isReadOnly

▸ **isReadOnly**(`value?`): `boolean`

获取/设置自定义命名表达式的只读状态。

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`boolean`

只读状态。

___

### <a id="set" name="set"></a> set

▸ **set**(`name?`, `formula?`, `baseRow?`, `baseCol?`, `comment?`): `void`

重命名自定义名称的名称、公式和注释。

#### Parameters

| Name | Type |
| :------ | :------ |
| `name?` | `string` |
| `formula?` | `string` |
| `baseRow?` | `number` |
| `baseCol?` | `number` |
| `comment?` | `string` |

#### Returns

`void`
