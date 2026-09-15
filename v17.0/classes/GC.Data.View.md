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

视图

**`property`** {string} name - 列的唯一名称

**`property`** {string} [value] - 列的值可以是数据库中表的字段名称，也可以是使用字段名称的公式

**`property`** {string | string[]} [caption] - 列标题

**`property`** {number | string} [width] - 列的宽度，以像素为单位的支持 pixel 或 star

**`property`** {GC.Data.StyleOptions} [style] - 列样式选项

**`property`** {(GC.Data.CellValueRuleOptions | GC.Data.SpecificTextRuleOptions | GC.Data.FormulaRuleOptions | GC.Data.DateOccurringRuleOptions | GC.Data.Top10RuleOptions | GC.Data.UniqueRuleOptions | GC.Data.DuplicateRuleOptions | GC.Data.AverageRuleOptions | GC.Data.TwoScaleRuleOptions | GC.Data.ThreeScaleRuleOptions | GC.Data.DataBarRuleOptions | GC.Data.IconSetRuleOptions)[]} [conditionalFormats] - 条件规则数组

**`property`** {GC.Data.NumberValidatorOptions | GC.Data.DateValidatorOptions | GC.Data.TimeValidatorOptions | GC.Data.TextLengthValidatorOptions | GC.Data.FormulaValidatorOptions | GC.Data.FormulaListValidatorOptions | GC.Data.ListValidatorOptions} [validators] - 默认数据验证器

**`property`** {boolean} [isPrimaryKey] - 将该列标记为主键列

**`property`** {boolean} [readonly] - 将列标记为只读

**`property`** {boolean} [required] - 插入新行时需要标记列

**`property`** {Object} [defaultValue] - 插入新行时提供默认值，可以是常量或公式

**`property`** {GC.Data.HeaderStyleOptions} [style] - 列标题样式选项

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The view name. |
| `columnInfos?` | `string`[] \| [`IColumn`](../modules/GC.Data.md#icolumn)[] | - |
| `includeDefaultColumns?` | `boolean` | - |
| `options?` | [`ViewOptions`](../modules/GC.Data.md#viewoptions) | - |

## Properties

### <a id="autofilter" name="autofilter"></a> autoFilter

• **autoFilter**: `boolean`

数据更改后是否再次过滤其默认值为true

___

### <a id="autosort" name="autosort"></a> autoSort

• **autoSort**: `boolean`

数据更改后是否重新排序其默认值为true

## Methods

### <a id="addcolumn" name="addcolumn"></a> addColumn

▸ **addColumn**(`column`): `void`

将列添加到当前视图中

**`代码示例`**
```
// 向视图中添加列
var productTable = dataManager.addTable("products", {
     remote: {
        read: {
            url: "https://demodata.grapecity.com/northwind/api/v1/products"
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
| `column` | `string` \| [`IColumn`](../modules/GC.Data.md#icolumn) | 列字符串或对象当参数是字符串时，列名和值就是字符串 |

#### Returns

`void`

___

### <a id="addstylerule" name="addstylerule"></a> addStyleRule

▸ **addStyleRule**(`name`, `style?`, `rule?`): `void`

在视图中添加一个样式规则

**`代码示例`**
```
// 添加样式规则
view.addStyleRule("dirtyRowStyle", { backColor: "yellow" }, {
   direction: GC.Data.StateRuleDirection.row,
   state: GC.Data.RowColumnStates.dirty
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 样式规则名称 |
| `style?` | [`StyleOptions`](../modules/GC.Data.md#styleoptions) | - |
| `rule?` | [`FormulaRule`](../modules/GC.Data.md#formularule) \| [`StateRule`](../modules/GC.Data.md#staterule) | - |

#### Returns

`void`

___

### <a id="clearstylerules" name="clearstylerules"></a> clearStyleRules

▸ **clearStyleRules**(): `void`

从视图中清除所有的样式规则

**`代码示例`**
```
// 移除样式规则
view.clearStyleRules();
```

#### Returns

`void`

___

### <a id="fetch" name="fetch"></a> fetch

▸ **fetch**(`reload?`): `Promise`<`any`\>

从其宿主表和相关表请求视图数据

**`代码示例`**
```
// 使用自定义视图设置集算表
var tablesheet = spread.addSheetTab(0, "TableSheet1", GC.Spread.Sheets.SheetType.tableSheet);
var dataManager = new GC.Data.DataManager();
var productTable = dataManager.addTable("productTable", {
    remote: {
        read: {
            url: "https://demodata.grapecity.com/northwind/api/v1/products"
        }
    }
});
var productView = productTable.addView("productView", [
    "id", "name", "reorderLevel", "unitPrice", "unitsInStock", "unitsOnOrder"
]);
productView.fetch().then(function () {
    // 用视图设置数据源
    tablesheet.setDataView(productView);
});
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `reload?` | `boolean` |

#### Returns

`Promise`<`any`\>

你可以通过 Promise.then() 获取数据

___

### <a id="getcolumn" name="getcolumn"></a> getColumn

▸ **getColumn**(`index?`): [`IColumn`](../modules/GC.Data.md#icolumn) \| [`IColumn`](../modules/GC.Data.md#icolumn)[]

获取当前视图的列

**`代码示例`**
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

按指定的索引返回列，或者在省略参数时返回所有列

___

### <a id="getstylerule" name="getstylerule"></a> getStyleRule

▸ **getStyleRule**(`name?`): `undefined` \| [`StyleRule`](../modules/GC.Data.md#stylerule) \| [`StyleRules`](../modules/GC.Data.md#stylerules)

获取一个样式规则，或者获取所有样式规则

**`example`**
```
// get a style rule
view.getStyleRule("dirtyRowStyle");
// get all style rule
view.getStyleRule();
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `name?` | `string` |

#### Returns

`undefined` \| [`StyleRule`](../modules/GC.Data.md#stylerule) \| [`StyleRules`](../modules/GC.Data.md#stylerules)

返回一个样式规则，或者返回所有样式规则

___


### <a id="length" name="length"></a> length

▸ **length**(): `number`

获取视图宿主表的数据源长度

**`代码示例`**
```
// 在获取数据后，可以得到视图数据源的长度
let dataSourceLength = productView.length();
```

#### Returns

`number`

宿主表数据源长度

___

### <a id="removecolumn" name="removecolumn"></a> removeColumn

▸ **removeColumn**(`column`): `void`

从当前视图中删除列

**`代码示例`**
```
// 删除一列
productWithSupplierView.removeColumn("discontinued");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `column` | `string` | The column value. |

#### Returns

`void`

___

### <a id="removestylerule" name="removestylerule"></a> removeStyleRule

▸ **removeStyleRule**(`name`): `void`

从视图中按名称添加一个样式规则

**`代码示例`**
```
// 移除样式规则
view.removeStyleRule("dirtyRowStyle");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 样式规则名称 |

#### Returns

`void`

___

### <a id="visiblelength" name="visiblelength"></a> visibleLength

▸ **visibleLength**(): `number`

获取当前视图中的可见数据长度

**`代码示例`**
```
// 在获取数据后，可以得到视图的visibleLength
let viewVisibleLength = productView.visibleLength();
```

#### Returns

`number`

当前视图中的可见数据长度
