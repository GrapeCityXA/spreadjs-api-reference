# Interface: ICustomDocPropsManager

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).ICustomDocPropsManager

## Table of contents

### Methods

- [add](GC.Spread.Sheets.ICustomDocPropsManager.md#add)
- [all](GC.Spread.Sheets.ICustomDocPropsManager.md#all)
- [clear](GC.Spread.Sheets.ICustomDocPropsManager.md#clear)
- [get](GC.Spread.Sheets.ICustomDocPropsManager.md#get)
- [remove](GC.Spread.Sheets.ICustomDocPropsManager.md#remove)

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`propName`, `value`, `isLinkTarget?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `propName` | `string` |
| `value` | [`CustomDocumentPropertyValueType`](../modules/GC.Spread.Sheets.md#customdocumentpropertyvaluetype) |
| `isLinkTarget?` | `boolean` |

#### Returns

`void`

___

### <a id="all" name="all"></a> all

▸ **all**(`props?`): [`ICustomDocumentProperty`](GC.Spread.Sheets.ICustomDocumentProperty.md)[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `props?` | [`ICustomDocumentProperty`](GC.Spread.Sheets.ICustomDocumentProperty.md)[] |

#### Returns

[`ICustomDocumentProperty`](GC.Spread.Sheets.ICustomDocumentProperty.md)[]

___

### <a id="clear" name="clear"></a> clear

▸ **clear**(): `void`

#### Returns

`void`

___

### <a id="get" name="get"></a> get

▸ **get**(`propName`): [`ICustomDocumentProperty`](GC.Spread.Sheets.ICustomDocumentProperty.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `propName` | `string` |

#### Returns

[`ICustomDocumentProperty`](GC.Spread.Sheets.ICustomDocumentProperty.md)

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`propName`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `propName` | `string` |

#### Returns

`void`
