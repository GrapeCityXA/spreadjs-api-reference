# Class: CustomDocPropsManager

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).CustomDocPropsManager

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.CustomDocPropsManager.md#constructor)

### Methods

- [add](GC.Spread.Sheets.CustomDocPropsManager.md#add)
- [all](GC.Spread.Sheets.CustomDocPropsManager.md#all)
- [clear](GC.Spread.Sheets.CustomDocPropsManager.md#clear)
- [get](GC.Spread.Sheets.CustomDocPropsManager.md#get)
- [remove](GC.Spread.Sheets.CustomDocPropsManager.md#remove)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new CustomDocPropsManager**(`workbook`)

代表自定义文档属性管理器。它可以管理所有文档的自定义属性。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workbook` | [`Workbook`](GC.Spread.Sheets.Workbook.md) | 工作簿 |

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`propName`, `value`, `isLinkTarget?`): `void`

设置自定义文档属性。

**`example`**
```
spread.docProps.customDocPropsManager.add('prop1', '1');
spread.docProps.customDocPropsManager.add('prop2', 'CellAlias', true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `propName` | `string` | 属性名称 |
| `value` | [`CustomDocumentPropertyValueType`](../modules/GC.Spread.Sheets.md#customdocumentpropertyvaluetype) | 适当的值 |
| `isLinkTarget?` | `boolean` | 是内容链接吗？ |

#### Returns

`void`

___

### <a id="all" name="all"></a> all

▸ **all**(`props?`): `undefined` \| [`ICustomDocumentProperty`](../interfaces/GC.Spread.Sheets.ICustomDocumentProperty.md)[]

获取或设置自定义文档属性。

**`example`**
```
spread.docProps.customDocPropsManager.all([{ name: 'prop1', value: '1' }]);
spread.docProps.customDocPropsManager.all();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `props?` | [`ICustomDocumentProperty`](../interfaces/GC.Spread.Sheets.ICustomDocumentProperty.md)[] | 自定义文档属性 |

#### Returns

`undefined` \| [`ICustomDocumentProperty`](../interfaces/GC.Spread.Sheets.ICustomDocumentProperty.md)[]

自定义文档属性。

___

### <a id="clear" name="clear"></a> clear

▸ **clear**(): `void`

清除自定义文档属性。

**`example`**
```
spread.docProps.customDocPropsManager.clear();
```

#### Returns

`void`

___

### <a id="get" name="get"></a> get

▸ **get**(`propName`): `undefined` \| [`ICustomDocumentProperty`](../interfaces/GC.Spread.Sheets.ICustomDocumentProperty.md)

通过属性名称获取自定义文档属性。

**`example`**
```
spread.docProps.customDocPropsManager.all([{ name: 'prop1', value: '1' }]);
spread.docProps.customDocPropsManager.get('prop1');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `propName` | `string` | 属性名称 |

#### Returns

`undefined` \| [`ICustomDocumentProperty`](../interfaces/GC.Spread.Sheets.ICustomDocumentProperty.md)

自定义文档属性。

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`propName`): `void`

按属性名称删除自定义文档属性。

**`example`**
```
spread.docProps.customDocPropsManager.remove('prop1');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `propName` | `string` | 属性名称 |

#### Returns

`void`
