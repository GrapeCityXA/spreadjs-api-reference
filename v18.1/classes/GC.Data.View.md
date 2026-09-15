# Class: View

[GC](../modules/GC.md).[Data](../modules/GC.Data.md).View

## Table of contents

### Constructors

- [constructor](GC.Data.View.md#constructor)

### Properties

- [autoFilter](GC.Data.View.md#autofilter)
- [autoSort](GC.Data.View.md#autosort)

### Methods

- [addColumn](GC.Data.View.md#addcolumn)
- [addStyleRule](GC.Data.View.md#addstylerule)
- [clearStyleRules](GC.Data.View.md#clearstylerules)
- [fetch](GC.Data.View.md#fetch)
- [getColumn](GC.Data.View.md#getcolumn)
- [getStyleRule](GC.Data.View.md#getstylerule)
- [length](GC.Data.View.md#length)
- [removeColumn](GC.Data.View.md#removecolumn)
- [removeStyleRule](GC.Data.View.md#removestylerule)
- [visibleLength](GC.Data.View.md#visiblelength)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new View**(`name`, `columnInfos?`, `includeDefaultColumns?`, `options?`)

表示视图。

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

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 视图名称。 |
| `columnInfos?` | `string`[] \| [`IColumn`](../modules/GC.Data.md#icolumn)[] | - |
| `includeDefaultColumns?` | `boolean` | - |
| `options?` | [`ViewOptions`](../modules/GC.Data.md#viewoptions) | - |

## Properties

### <a id="autofilter" name="autofilter"></a> autoFilter

• **autoFilter**: `boolean`

数据更改后是否再次过滤。其默认值为true。

___

### <a id="autosort" name="autosort"></a> autoSort

• **autoSort**: `boolean`

数据更改后是否再次排序。其默认值为true。

## Methods

### <a id="addcolumn" name="addcolumn"></a> addColumn

▸ **addColumn**(`column`): `void`

向当前视图添加一列。

**`example`**
```
// 向视图添加列
var productTable = dataManager.addTable("products", {
     remote: {
        read: {
            url: "https://demodata.mescius.io/northwind/api/v1/products"
        }
    }
});
var productView = productTable.addView("productView", [ "id", "name" ]);
productTable.fetch().then(function() {
    productView.addColumn("reorderLevel");
    productView.addColumn({ value: "unitPrice", caption: "UNIT PRICE" });
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `column` | `string` \| [`IColumn`](../modules/GC.Data.md#icolumn) | 列字符串或对象。当参数是字符串时，列名和值都是该字符串。 |

#### Returns

`void`

___

### <a id="addstylerule" name="addstylerule"></a> addStyleRule

▸ **addStyleRule**(`name`, `style?`, `rule?`): `void`

向视图添加一个样式规则。

**`example`**
```
// 添加一个样式规则
view.addStyleRule("dirtyRowStyle", { backColor: "yellow" }, {
   direction: GC.Data.StateRuleDirection.row,
   state: GC.Data.RowColumnStates.dirty
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 样式规则名称。 |
| `style?` | [`StyleOptions`](../modules/GC.Data.md#styleoptions) | - |
| `rule?` | [`FormulaRule`](../modules/GC.Data.md#formularule) \| [`StateRule`](../modules/GC.Data.md#staterule) | - |

#### Returns

`void`

___

### <a id="clearstylerules" name="clearstylerules"></a> clearStyleRules

▸ **clearStyleRules**(): `void`

从视图中清除所有样式规则。

**`example`**
```
// 移除一个样式规则
view.clearStyleRules();
```

#### Returns

`void`

___

### <a id="fetch" name="fetch"></a> fetch

▸ **fetch**(`reload?`): `Promise`<`any`\>

从其宿主表和相关表请求视图数据。

**`example`**
```
// 使用自定义视图设置集算表
var tablesheet = spread.addSheetTab(0, "TableSheet1", GC.Spread.Sheets.SheetType.tableSheet);
var dataManager = new GC.Data.DataManager();
var productTable = dataManager.addTable("productTable", {
    remote: {
        read: {
            url: "https://demodata.mescius.io/northwind/api/v1/products"
        }
    }
});
var productView = productTable.addView("productView", [
    "id", "name", "reorderLevel", "unitPrice", "unitsInStock", "unitsOnOrder"
]);
productView.fetch().then(function () {
    // 使用视图设置数据源
    tablesheet.setDataView(productView);
});
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `reload?` | `boolean` |

#### Returns

`Promise`<`any`\>

解析的Promise thenable。您可以在Promise.then()中获取数据。

___

### <a id="getcolumn" name="getcolumn"></a> getColumn

▸ **getColumn**(`index?`): [`IColumn`](../modules/GC.Data.md#icolumn) \| [`IColumn`](../modules/GC.Data.md#icolumn)[]

获取当前视图的一列。

**`example`**
```
// 获取所有列
var allColumns = productWithSupplierView.getColumn();
// 获取第二列
var column1 = productWithSupplierView.getColumn(1);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `index?` | `number` |

#### Returns

[`IColumn`](../modules/GC.Data.md#icolumn) \| [`IColumn`](../modules/GC.Data.md#icolumn)[]

按指定索引返回一列，或在省略参数时返回所有列。

___

### <a id="getstylerule" name="getstylerule"></a> getStyleRule

▸ **getStyleRule**(`name?`): `undefined` \| [`StyleRule`](../modules/GC.Data.md#stylerule) \| [`StyleRules`](../modules/GC.Data.md#stylerules)

获取一个样式规则或所有样式规则。

**`example`**
```
// 获取一个样式规则
view.getStyleRule("dirtyRowStyle");
// 获取所有样式规则
view.getStyleRule();
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `name?` | `string` |

#### Returns

`undefined` \| [`StyleRule`](../modules/GC.Data.md#stylerule) \| [`StyleRules`](../modules/GC.Data.md#stylerules)

返回一个样式规则或所有样式规则。

___

### <a id="length" name="length"></a> length

▸ **length**(): `number`

获取视图宿主表数据源的长度。

**`example`**
```
// 获取数据后，可以获取视图数据源的长度。
let dataSourceLength = productView.length();
```

#### Returns

`number`

宿主表数据源的长度。

___

### <a id="removecolumn" name="removecolumn"></a> removeColumn

▸ **removeColumn**(`column`): `void`

从当前视图中移除一列。

**`example`**
```
// 移除一列
productWithSupplierView.removeColumn("discontinued");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `column` | `string` | 列值。 |

#### Returns

`void`

___

### <a id="removestylerule" name="removestylerule"></a> removeStyleRule

▸ **removeStyleRule**(`name`): `void`

按名称从视图中移除一个样式规则。

**`example`**
```
// 移除一个样式规则
view.removeStyleRule("dirtyRowStyle");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 样式规则名称。 |

#### Returns

`void`

___

### <a id="visiblelength" name="visiblelength"></a> visibleLength

▸ **visibleLength**(): `number`

获取当前视图中可见数据的长度。

**`example`**
```
// 获取数据后，可以获取视图的可见长度。
let viewVisibleLength = productView.visibleLength();
```

#### Returns

`number`

当前视图中可见数据的长度。
