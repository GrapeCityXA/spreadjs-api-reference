# Class: Table

[GC](../modules/GC.md).[Data](../modules/GC.Data.md).Table

## Table of contents

### Constructors

- [constructor](GC.Data.Table.md#constructor)

### Properties

- [columns](GC.Data.Table.md#columns)
- [name](GC.Data.Table.md#name)
- [options](GC.Data.Table.md#options)
- [views](GC.Data.Table.md#views)

### Methods

- [addView](GC.Data.Table.md#addview)
- [clearIndexes](GC.Data.Table.md#clearindexes)
- [createIndexes](GC.Data.Table.md#createindexes)
- [dropIndexes](GC.Data.Table.md#dropindexes)
- [fetch](GC.Data.Table.md#fetch)
- [getIndexes](GC.Data.Table.md#getindexes)
- [removeView](GC.Data.Table.md#removeview)
- [search](GC.Data.Table.md#search)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Table**(`name`, `dataSourceOption`)

表示表。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 表名称。 |
| `dataSourceOption` | [`IDataSourceOption`](../modules/GC.Data.md#idatasourceoption) | 表的数据源。 |

## Properties

### <a id="columns" name="columns"></a> columns

• **columns**: [`IColumnCollection`](../modules/GC.Data.md#icolumncollection)

表示表的默认列，仅在获取表后可用。键是列名，值是列信息。

___

### <a id="name" name="name"></a> name

• **name**: `string`

表示表的名称。

___

### <a id="options" name="options"></a> options

• **options**: [`IDataSourceOption`](../modules/GC.Data.md#idatasourceoption)

表示表的数据源选项。

___

### <a id="views" name="views"></a> views

• **views**: [`IViews`](../interfaces/GC.Data.IViews.md)

表示表的视图集合。键是视图名，值是GC.Data.View实例。

## Methods

### <a id="addview" name="addview"></a> addView

▸ **addView**(`name`, `columnInfos?`, `includeDefaultColumns?`, `options?`): [`View`](GC.Data.View.md)

添加一个视图，其宿主表是当前表。

**`property`** {string} name - 列的唯一名称。

**`property`** {string} [value] - 列的值，可以是数据库中表的字段名，或使用字段名的公式。

**`property`** {string | string[]} [caption] - 列的标题。

**`property`** {number | string} [width] - 列的宽度，支持以像素为单位的数字，或星号大小。

**`property`** {GC.Data.StyleOptions} [style] - 列样式选项。

**`property`** {(GC.Data.CellValueRuleOptions | GC.Data.SpecificTextRuleOptions | GC.Data.FormulaRuleOptions | GC.Data.DateOccurringRuleOptions | GC.Data.Top10RuleOptions | GC.Data.UniqueRuleOptions | GC.Data.DuplicateRuleOptions | GC.Data.AverageRuleOptions | GC.Data.TwoScaleRuleOptions | GC.Data.ThreeScaleRuleOptions | GC.Data.DataBarRuleOptions | GC.Data.IconSetRuleOptions)[]} [conditionalFormats] - 条件规则数组。

**`property`** {GC.Data.NumberValidatorOptions | GC.Data.DateValidatorOptions | GC.Data.TimeValidatorOptions | GC.Data.TextLengthValidatorOptions | GC.Data.FormulaValidatorOptions | GC.Data.FormulaListValidatorOptions | GC.Data.ListValidatorOptions} [validators] - 默认数据验证器。

**`property`** {boolean} [isPrimaryKey] - 将列标记为主键列。

**`property`** {boolean} [readonly] - 标记列是只读的。

**`property`** {boolean} [required] - 标记插入新行时列是必需的。

**`property`** {Object} [defaultValue] - 插入新行时提供默认值，可以是常量或公式。

**`property`** {GC.Data.HeaderStyleOptions} [style] - 列标题样式选项。

**`example`**
```javascript
// 通过字符串数组列添加视图
productTable.addView("productView", [
    "id", "name", "reorderLevel", "unitPrice", "unitsInStock", "unitsOnOrder"
]);

// 通过自定义列添加视图
productTable.addView("productView", [{
    value: "id",
    caption: "ID",
    isPrimaryKey: true
}, {
    value: "name",
    caption: "NAME",
    required: true
}, {
    value: "quantityPerUnit",
    caption: "QUANTITY PER UNIT"
}, {
    value: "unitPrice",
    caption: "UNIT PRICE"
}, {
    value: "unitsInStock",
    caption: "UNITS IN STOCK",
    readonly: true
}, {
    value: "unitsOnOrder",
    caption: "UNITS ON ORDER"
}, {
    value: "reorderLevel",
    caption: "REORDER LEVEL"
}, {
    value: "discontinued",
    caption: "DISCONTINUED",
    defaultValue: false
});

// 添加带有关系列的视图
var supplierRelationship = dataManager.addRelationship(productTable, "supplierId", "supplier", supplierTable, "id", "products");
productTable.addView("productWithSupplierView", [{
    value: "id",
    caption: "ID"
}, {
    value: "name",
    caption: "NAME"
}, {
    value: "supplier.companyName", // 关系
    caption: "SUPPLIER NAME"
}, {
    value: "supplier.contactName", // 关系
    caption: "SUPPLIER CONTACT NAME"
}, {
    value: "supplier.contactTitle", // 关系
    caption: "SUPPLIER CONTACT TITLE"
});

// 添加带有计算字段列的视图
var supplierRelationship = dataManager.addRelationship(productTable, "supplierId", "supplier", supplierTable, "id", "products");
productTable.addView("productWithSupplierView", [{
    value: "id",
    caption: "ID"
}, {
    value: "name",
    caption: "NAME"
}, {
    caption: "TOTAL PRICE",
    value: "=(unitsInStock + unitsOnOrder) * unitPrice"
}, {
    caption: "SUPPLIER'S INFO",
    value: "=CONCAT(supplierTable.companyName, ', ', supplierTable.contactName)"
});

```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 视图名。 |
| `columnInfos?` | `string`[] \| [`IColumn`](../modules/GC.Data.md#icolumn)[] | 列信息，每列包含以下属性。 |
| `includeDefaultColumns?` | `boolean` | 当列信息为空时是否包含当前表的默认列。其默认值为true. |
| `options?` | [`ViewOptions`](../modules/GC.Data.md#viewoptions) | 视图选项。 |

#### Returns

[`View`](GC.Data.View.md)

返回该视图。

___

### <a id="clearindexes" name="clearindexes"></a> clearIndexes

▸ **clearIndexes**(): `void`

清除所有索引字段。

**`example`**
```javascript
// 清除所有索引字段。
table.clearIndexes();
```

#### Returns

`void`

___

### <a id="createindexes" name="createindexes"></a> createIndexes

▸ **createIndexes**(`fields`): `void`

为字段创建索引。

**`example`**
```javascript
// 创建索引。
table.createIndexes(["name", "country", "project"]);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fields` | `string`[] | 索引字段。 |

#### Returns

`void`

___

### <a id="dropindexes" name="dropindexes"></a> dropIndexes

▸ **dropIndexes**(`fields`): `void`

删除索引字段。

**`example`**
```javascript
// 删除索引字段。
table.dropIndexes(["name", "country", "project"]);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fields` | `string`[] | 已索引的字段。 |

#### Returns

`void`

___

### <a id="fetch" name="fetch"></a> fetch

▸ **fetch**(`reload?`): `Promise`<`any`\>

根据数据源选项从本地数据源或远程数据源请求表数据。

**`example`**
```javascript
// 使用获取的数据构建集算表
productTable.fetch().then(function(data) {
    var productView = productTable.addView("productView");
    var tableSheet = spread.addSheetTab(0, "productTableSheet", GC.Spread.Sheets.SheetType.tableSheet);
    tableSheet.setDataView(productView);
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `reload?` | `boolean` | 是否强制从服务器端重新加载数据。 |

#### Returns

`Promise`<`any`\>

解析的Promise thenable。您可以在Promise.then()中获取数据。

___

### <a id="getindexes" name="getindexes"></a> getIndexes

▸ **getIndexes**(): `string`[]

获取所有索引字段。

**`example`**
```javascript
// 存在索引字段。
table.getIndexes(); // 返回 ["name", "country", "project"]
// 没有索引字段。
table.getIndexes(); // 返回 []
```

#### Returns

`string`[]

索引字段。

___

### <a id="removeview" name="removeview"></a> removeView

▸ **removeView**(`name`): `void`

移除一个视图。

**`example`**
```javascript
// 按名称移除视图
dataManager.removeView("productView");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要移除的视图名称。 |

#### Returns

`void`

___

### <a id="search" name="search"></a> search

▸ **search**(`value`, `field`): `any`[]

使用搜索值搜索记录，返回所有精确匹配的记录。

**`example`**
```javascript
// 搜索值并成功
table.search("SpreadJS", "group"); // 返回 [ {id: 1, project: "DataManager", group: "SpreadJS"}, {id: 3, project: "TableSheet", group: "SpreadJS"} ]
// 搜索值但失败
table.search("WPS", "project"); // 返回 []
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 搜索值。始终将非字符串转换为字符串类型。 |
| `field` | `string` | 目标字段。 |

#### Returns

`any`[]

所有匹配的记录。
