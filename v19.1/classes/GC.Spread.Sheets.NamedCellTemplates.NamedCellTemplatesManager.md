# Class: NamedCellTemplatesManager

[Sheets](../modules/GC.Spread.Sheets.md).[NamedCellTemplates](../modules/GC.Spread.Sheets.NamedCellTemplates.md).NamedCellTemplatesManager

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.NamedCellTemplates.NamedCellTemplatesManager.md#constructor)

### Methods

- [add](GC.Spread.Sheets.NamedCellTemplates.NamedCellTemplatesManager.md#add)
- [all](GC.Spread.Sheets.NamedCellTemplates.NamedCellTemplatesManager.md#all)
- [clear](GC.Spread.Sheets.NamedCellTemplates.NamedCellTemplatesManager.md#clear)
- [createFromCell](GC.Spread.Sheets.NamedCellTemplates.NamedCellTemplatesManager.md#createfromcell)
- [get](GC.Spread.Sheets.NamedCellTemplates.NamedCellTemplatesManager.md#get)
- [has](GC.Spread.Sheets.NamedCellTemplates.NamedCellTemplatesManager.md#has)
- [remove](GC.Spread.Sheets.NamedCellTemplates.NamedCellTemplatesManager.md#remove)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new NamedCellTemplatesManager**()

表示命名单元格模板管理器。
用于存储和检索可应用于单元格的配置模板。

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`name`, `template`): `void`

添加新的命名单元格模板。如果名称已存在，则会覆盖旧模板。

**`example`**
```javascript
var template = {
    style: { backColor: 'red', foreColor: 'white' },
    dataValidations: [{ type: 1, comparisonOperator: 6, condition: { expected: [1, 100] } }]
};
workbook.namedCellTemplates.add('myTemplate', template);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 此模板的唯一名称。 |
| `template` | [`INamedCellTemplate`](../interfaces/GC.Spread.Sheets.NamedCellTemplates.INamedCellTemplate.md) | 模板定义。 |

#### Returns

`void`

___

### <a id="all" name="all"></a> all

▸ **all**(): [`INamedCellTemplate`](../interfaces/GC.Spread.Sheets.NamedCellTemplates.INamedCellTemplate.md)[]

获取所有模板。

**`example`**
```javascript
var templates = workbook.namedCellTemplates.all();
templates.forEach(function(template) {
    console.log(template.name);
});
```

#### Returns

[`INamedCellTemplate`](../interfaces/GC.Spread.Sheets.NamedCellTemplates.INamedCellTemplate.md)[]

所有模板（副本）的数组。

___

### <a id="clear" name="clear"></a> clear

▸ **clear**(): `void`

清除所有模板。

**`example`**
```javascript
workbook.namedCellTemplates.clear();
```

#### Returns

`void`

___

### <a id="createfromcell" name="createfromcell"></a> createFromCell

▸ **createFromCell**(`name`, `sheet`, `row`, `col`, `templateOptions?`): `void`

根据现有单元格配置创建模板。

**`example`**
```javascript
var sheet = spread.getActiveSheet();
// 从单元格 A1 创建一个包含所有属性的模板
workbook.namedCellTemplates.createFromCell('cellTemplate', sheet, 0, 0);
// 从单元格 B2 创建一个仅包含样式的模板
workbook.namedCellTemplates.createFromCell('styleOnly', sheet, 1, 1, { style: true, conditionalFormat: false, dataValidation: false, cellState: false });
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 此模板的唯一名称。 |
| `sheet` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 包含该单元格的工作表。 |
| `row` | `number` | 单元格的行索引。 |
| `col` | `number` | 单元格的列索引。 |
| `templateOptions?` | [`ICellTemplateOptions`](../interfaces/GC.Spread.Sheets.NamedCellTemplates.ICellTemplateOptions.md) | - |

#### Returns

`void`

___

### <a id="get" name="get"></a> get

▸ **get**(`name`): ``null`` \| [`INamedCellTemplate`](../interfaces/GC.Spread.Sheets.NamedCellTemplates.INamedCellTemplate.md)

根据名称获取模板，返回模板的副本。

**`example`**
```javascript
var template = workbook.namedCellTemplates.get('myTemplate');
if (template) {
    console.log(template.style);
}
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要获取的模板名称。 |

#### Returns

``null`` \| [`INamedCellTemplate`](../interfaces/GC.Spread.Sheets.NamedCellTemplates.INamedCellTemplate.md)

模板对象；如果未找到则返回 null。

___

### <a id="has" name="has"></a> has

▸ **has**(`name`): `boolean`

检查是否存在指定名称的模板。

**`example`**
```javascript
if (workbook.namedCellTemplates.has('myTemplate')) {
    console.log('Template exists');
}
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要检查的模板名称。 |

#### Returns

`boolean`

如果模板存在则返回 true，否则返回 false。

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`name`): ``null`` \| [`INamedCellTemplate`](../interfaces/GC.Spread.Sheets.NamedCellTemplates.INamedCellTemplate.md)

根据名称移除模板。

**`example`**
```javascript
var removedTemplate = workbook.namedCellTemplates.remove('myTemplate');
if (removedTemplate) {
    console.log('Template removed:', removedTemplate.name);
}
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要移除的模板名称。 |

#### Returns

``null`` \| [`INamedCellTemplate`](../interfaces/GC.Spread.Sheets.NamedCellTemplates.INamedCellTemplate.md)

被移除的模板；如果未找到则返回 null。
