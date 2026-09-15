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

表

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 表名 |
| `dataSourceOption` | [`IDataSourceOption`](../modules/GC.Data.md#idatasourceoption) | 表的数据源选项 |

## Properties

### <a id="columns" name="columns"></a> columns

• **columns**: [`IColumnCollection`](../modules/GC.Data.md#icolumncollection)

表的默认列，只有在表获取数据后后才可用，键为列名，值为列信息。

___

### <a id="name" name="name"></a> name

• **name**: `string`

表的名称

___

### <a id="options" name="options"></a> options

• **options**: [`IDataSourceOption`](../modules/GC.Data.md#idatasourceoption)

表的数据源选项

___

### <a id="views" name="views"></a> views

• **views**: [`IViews`](../interfaces/GC.Data.IViews.md)

表的视图集合，键为视图的名称，值为GC.Data.View类的实例。

## Methods

### <a id="addview" name="addview"></a> addView

▸ **addView**(`name`, `columnInfos?`, `includeDefaultColumns?`, `options?`): [`View`](GC.Data.View.md)

添加一个视图, 以当前的表做为主表。

**`property`** {string} name - 列的唯一名称

**`property`** {string} [value] - 列的值可以是数据库中表的字段名称，也可以是使用了字段名称的公式。

**`property`** {string | string[]} [caption] - 列标题

**`property`** {number | string} [width] - 列的宽度，支持以像素为单位的数值，或星号尺寸。

**`property`** {GC.Data.StyleOptions} [style] - 列样式选项

**`property`** {(GC.Data.CellValueRuleOptions | GC.Data.SpecificTextRuleOptions | GC.Data.FormulaRuleOptions | GC.Data.DateOccurringRuleOptions | GC.Data.Top10RuleOptions | GC.Data.UniqueRuleOptions | GC.Data.DuplicateRuleOptions | GC.Data.AverageRuleOptions | GC.Data.TwoScaleRuleOptions | GC.Data.ThreeScaleRuleOptions | GC.Data.DataBarRuleOptions | GC.Data.IconSetRuleOptions)[]} [conditionalFormats] - 条件格式数组

**`property`** {GC.Data.NumberValidatorOptions | GC.Data.DateValidatorOptions | GC.Data.TimeValidatorOptions | GC.Data.TextLengthValidatorOptions | GC.Data.FormulaValidatorOptions | GC.Data.FormulaListValidatorOptions | GC.Data.ListValidatorOptions} [validators] - 默认数据验证器

**`property`** {boolean} [isPrimaryKey] - 将该列标记为主键列

**`property`** {boolean} [readonly] - 将列标记为只读

**`property`** {boolean} [required] - 在插入新行时，将此列标记为必填项。

**`property`** {Object} [defaultValue] - 在插入新行时，提供默认值，可以是常量或公式。

**`property`** {GC.Data.HeaderStyleOptions} [style] - 列标题样式选项

**`代码示例`**
``` javascript
// 按字符串数组列添加视图
productTable.addView("productView", [
    "id", "name", "reorderLevel", "unitPrice", "unitsInStock", "unitsOnOrder"
]);

// 按自定义列添加视图
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

// 添加具有关系列的视图
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

// 添加具有计算字段列的视图
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
| `name` | `string` | 视图名称 |
| `columnInfos?` | `string`[] \| [`IColumn`](../modules/GC.Data.md#icolumn)[] | - |
| `includeDefaultColumns?` | `boolean` | 当列信息为空时，是否包含当前表的默认列。其默认值为 true。 |
| `options?` | [`ViewOptions`](../modules/GC.Data.md#viewoptions) | - |

#### Returns

[`View`](GC.Data.View.md)

返回视图

___

### <a id="clearindexes" name="clearindexes"></a> clearIndexes

▸ **clearIndexes**(): `void`

清除所有索引字段

**`代码示例`**
``` javascript
// 清除所有索引字段
table.clearIndexes();
```

#### Returns

`void`

___

### <a id="createindexes" name="createindexes"></a> createIndexes

▸ **createIndexes**(`fields`): `void`

为字段创建索引

**`代码示例`**
``` javascript
// 创建索引
table.createIndexes(["name", "country", "project"]);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fields` | `string`[] | 索引字段 |

#### Returns

`void`

___

### <a id="dropindexes" name="dropindexes"></a> dropIndexes

▸ **dropIndexes**(`fields`): `void`

删除索引字段

**`代码示例`**
``` javascript
// 删除索引字段
table.dropIndexes(["name", "country", "project"]);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fields` | `string`[] | 索引字段 |

#### Returns

`void`

___

### <a id="fetch" name="fetch"></a> fetch

▸ **fetch**(`reload?`): `Promise`<`any`\>

通过数据源选项，从本地数据源或远程数据源请求表数据。

**`代码示例`**
``` javascript
// 使用请求的数据构建集算表
productTable.fetch().then(function(data) {
    var productView = productTable.addView("productView");
    var tableSheet = spread.addSheetTab(0, "productTableSheet", GC.Spread.Sheets.SheetType.tableSheet);
    tableSheet.setDataView(productView);
});
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `reload?` | `boolean` |

#### Returns

`Promise`<`any`\>

返回解析中的 Promise 对象。您可以通过 Promise.then() 获取数据。

___

### <a id="getindexes" name="getindexes"></a> getIndexes

▸ **getIndexes**(): `string`[]

获取所有索引字段

**`代码示例`**
``` javascript
// 存在索引字段
table.getIndexes(); // 返回 ["name", "country", "project"]
// 不存在索引字段
table.getIndexes(); // 返回 []
```

#### Returns

`string`[]

索引字段

___

### <a id="removeview" name="removeview"></a> removeView

▸ **removeView**(`name`): `void`

删除视图

**`代码示例`**
``` javascript
// 按名称删除视图
dataManager.removeView("productView");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要删除的视图的名称 |

#### Returns

`void`

___

### <a id="search" name="search"></a> search

▸ **search**(`value`, `field`): `any`[]

使用搜索值查找记录，返回所有完全匹配的记录。

**`代码示例`**
``` javascript
// 成功查找到数据
table.search("SpreadJS", "group"); // 返回 [ {id: 1, project: "DataManager", group: "SpreadJS"}, {id: 3, project: "TableSheet", group: "SpreadJS"} ]
// 未成功查找到数据
table.search("WPS", "project"); // 返回 []
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 搜索值。始终将非字符串转换为字符串类型。 |
| `field` | `string` | 目标字段 |

#### Returns

`any`[]

所有匹配的记录
