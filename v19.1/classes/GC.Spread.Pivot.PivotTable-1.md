# Class: PivotTable

[Spread](../modules/GC.Spread.md).[Pivot](../modules/GC.Spread.Pivot.md).PivotTable

## Table of contents

### Constructors

- [constructor](GC.Spread.Pivot.PivotTable-1.md#constructor)

### Properties

- [options](GC.Spread.Pivot.PivotTable-1.md#options)
- [views](GC.Spread.Pivot.PivotTable-1.md#views)

### Methods

- [add](GC.Spread.Pivot.PivotTable-1.md#add)
- [addCalcField](GC.Spread.Pivot.PivotTable-1.md#addcalcfield)
- [addCalcItem](GC.Spread.Pivot.PivotTable-1.md#addcalcitem)
- [addConditionalRule](GC.Spread.Pivot.PivotTable-1.md#addconditionalrule)
- [autoFitColumn](GC.Spread.Pivot.PivotTable-1.md#autofitcolumn)
- [autoSortState](GC.Spread.Pivot.PivotTable-1.md#autosortstate)
- [clearOverwriteList](GC.Spread.Pivot.PivotTable-1.md#clearoverwritelist)
- [collapse](GC.Spread.Pivot.PivotTable-1.md#collapse)
- [connectSlicer](GC.Spread.Pivot.PivotTable-1.md#connectslicer)
- [dataPosition](GC.Spread.Pivot.PivotTable-1.md#dataposition)
- [deserialize](GC.Spread.Pivot.PivotTable-1.md#deserialize)
- [disconnectSlicer](GC.Spread.Pivot.PivotTable-1.md#disconnectslicer)
- [getAllSlicers](GC.Spread.Pivot.PivotTable-1.md#getallslicers)
- [getCalcFields](GC.Spread.Pivot.PivotTable-1.md#getcalcfields)
- [getCalcItems](GC.Spread.Pivot.PivotTable-1.md#getcalcitems)
- [getConditionalRules](GC.Spread.Pivot.PivotTable-1.md#getconditionalrules)
- [getField](GC.Spread.Pivot.PivotTable-1.md#getfield)
- [getFieldsByArea](GC.Spread.Pivot.PivotTable-1.md#getfieldsbyarea)
- [getItemsByField](GC.Spread.Pivot.PivotTable-1.md#getitemsbyfield)
- [getNodeInfo](GC.Spread.Pivot.PivotTable-1.md#getnodeinfo)
- [getNodeValue](GC.Spread.Pivot.PivotTable-1.md#getnodevalue)
- [getOverwriteList](GC.Spread.Pivot.PivotTable-1.md#getoverwritelist)
- [getPivotAreaRanges](GC.Spread.Pivot.PivotTable-1.md#getpivotarearanges)
- [getPivotDetails](GC.Spread.Pivot.PivotTable-1.md#getpivotdetails)
- [getRange](GC.Spread.Pivot.PivotTable-1.md#getrange)
- [getSource](GC.Spread.Pivot.PivotTable-1.md#getsource)
- [getSourceFields](GC.Spread.Pivot.PivotTable-1.md#getsourcefields)
- [getStyle](GC.Spread.Pivot.PivotTable-1.md#getstyle)
- [getThemeName](GC.Spread.Pivot.PivotTable-1.md#getthemename)
- [group](GC.Spread.Pivot.PivotTable-1.md#group)
- [isConnectedSlicer](GC.Spread.Pivot.PivotTable-1.md#isconnectedslicer)
- [labelFilter](GC.Spread.Pivot.PivotTable-1.md#labelfilter)
- [layoutType](GC.Spread.Pivot.PivotTable-1.md#layouttype)
- [name](GC.Spread.Pivot.PivotTable-1.md#name)
- [position](GC.Spread.Pivot.PivotTable-1.md#position)
- [refresh](GC.Spread.Pivot.PivotTable-1.md#refresh)
- [remove](GC.Spread.Pivot.PivotTable-1.md#remove)
- [removeCalcField](GC.Spread.Pivot.PivotTable-1.md#removecalcfield)
- [removeCalcItem](GC.Spread.Pivot.PivotTable-1.md#removecalcitem)
- [removeConditionalRule](GC.Spread.Pivot.PivotTable-1.md#removeconditionalrule)
- [resumeLayout](GC.Spread.Pivot.PivotTable-1.md#resumelayout)
- [serialize](GC.Spread.Pivot.PivotTable-1.md#serialize)
- [setNodeValue](GC.Spread.Pivot.PivotTable-1.md#setnodevalue)
- [setStyle](GC.Spread.Pivot.PivotTable-1.md#setstyle)
- [showDataAs](GC.Spread.Pivot.PivotTable-1.md#showdataas)
- [showNoData](GC.Spread.Pivot.PivotTable-1.md#shownodata)
- [sort](GC.Spread.Pivot.PivotTable-1.md#sort)
- [subtotalPosition](GC.Spread.Pivot.PivotTable-1.md#subtotalposition)
- [subtotalType](GC.Spread.Pivot.PivotTable-1.md#subtotaltype)
- [subtotalVisible](GC.Spread.Pivot.PivotTable-1.md#subtotalvisible)
- [suspendLayout](GC.Spread.Pivot.PivotTable-1.md#suspendlayout)
- [theme](GC.Spread.Pivot.PivotTable-1.md#theme)
- [ungroup](GC.Spread.Pivot.PivotTable-1.md#ungroup)
- [updateCalcItem](GC.Spread.Pivot.PivotTable-1.md#updatecalcitem)
- [updateField](GC.Spread.Pivot.PivotTable-1.md#updatefield)
- [updateFieldName](GC.Spread.Pivot.PivotTable-1.md#updatefieldname)
- [updateSource](GC.Spread.Pivot.PivotTable-1.md#updatesource)
- [valueFilter](GC.Spread.Pivot.PivotTable-1.md#valuefilter)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new PivotTable**(`name`, `sheet?`, `row?`, `col?`, `layout?`, `style?`, `options?`, `layoutModel?`)

表示一个数据透视表。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 数据透视表的名称。 |
| `sheet?` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 所属的工作表。 |
| `row?` | `number` | 数据透视表的起始行号。 |
| `col?` | `number` | 数据透视表的起始列号。 |
| `layout?` | [`PivotTableLayoutType`](../enums/GC.Spread.Pivot.PivotTableLayoutType.md) | 数据透视表的布局类型。 |
| `style?` | `string` \| [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md) | 数据透视表的主题样式或样式名称。 |
| `options?` | [`IPivotTableOption`](../modules/GC.Spread.Pivot.md#ipivottableoption) | - |
| `layoutModel?` | `any` | - |

## Properties

### <a id="options" name="options"></a> options

• **options**: [`IPivotTableOption`](../modules/GC.Spread.Pivot.md#ipivottableoption)

数据透视表的选项配置。

**`property`** {boolean} [allowMultipleFiltersPerField] 指示是否在单个字段中使用多个筛选器。

**`property`** {boolean} [fillDownLabels] 指示是否显示重复的标签项。

**`property`** {boolean} [insertBlankLineAfterEachItem] 指示是否在每个项目末尾插入空白行。

**`property`** {GC.Spread.Pivot.GrandTotalPosition} [grandTotalPosition] 指示总计行/列的显示位置（行、列或两者）。

**`property`** {GC.Spread.Pivot.SubtotalsPosition} [subtotalsPosition] 指示分类汇总显示在顶部、底部或不显示。

**`property`** {GC.Spread.Pivot.DisplayFields} [displayFieldsInPageFilterArea] 指示页面筛选区域中字段的显示顺序（先横向后纵向或先纵向后横向）。

**`property`** {number} [reportFilterFieldsPerColumn] 每页筛选字段的列数。

**`property`** {boolean} [bandRows] 指示是否显示行带状样式。

**`property`** {boolean} [bandColumns] 指示是否显示列带状样式。

**`property`** {boolean} [showRowHeader] 指示是否显示行标题样式。

**`property`** {boolean} [showColumnHeader] 指示是否显示列标题样式。

**`property`** {boolean} [showDrill] 指示是否显示展开/折叠按钮。

**`property`** {boolean} [showMissing] 指示是否应用缺失值显示规则。

**`property`** {boolean} [missingCaption] 指示当实际值为空时显示的内容。

**`property`** {boolean} [rowLabelIndent] 指示各级标题的缩进。

**`property`** {boolean} [printDrill] 打印时是否显示展开/折叠按钮。

**`property`** {boolean} [itemPrintTitles] 每页是否重复行标签。

**`property`** {boolean} [fieldPrintTitles] 设置打印标题。

**`property`** {boolean} [showFilter] 指示是否显示筛选按钮。

**`property`** {boolean} [showToolTip] 指示是否显示工具提示。

**`property`** {boolean} [mergeItem] 指示是否合并并居中带有标签的单元格。

**`property`** {boolean} [isShowErrorValue] 指示是否应用错误值显示规则。

**`property`** {boolean} [errorValueInfo] 指示当实际值为错误时显示的内容。

**`property`** {string} [rowHeaderCaption] 紧凑布局中替代“行标签”的显示文本。

**`property`** {string} [colHeaderCaption] 紧凑布局中替代“列标签”的显示文本。

**`property`** {boolean} [showHeaders] 指示是否显示字段标题。

**`property`** {GC.Spread.Pivot.CalcItemAggregation} [calcItemAggregation] 指示数据透视表总计是否包含计算项的值。

**`property`** {boolean} [enableDataValueEditing] 指示是否允许编辑数据区域的单元格值。

___

### <a id="views" name="views"></a> views

• **views**: [`IPivotTableViewManager`](../interfaces/GC.Spread.Pivot.IPivotTableViewManager.md)

数据透视表的视图管理器。

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`sourceName`, `displayName`, `area`, `subtotal?`, `index?`): `void`

**`description`** 向数据透视表添加字段。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                  ["01-一月","妈妈","燃油",74],
                  ["15-一月","妈妈","食品",235],
                  ["17-一月","爸爸","运动",20],
                  ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var subtotal = GC.Pivot.SubtotalType.count;
pivotTable.add("购买者", "购买者", 1, subtotal, 0); // 向数据透视表添加字段，显示名称为“购买者”，位于行区域
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sourceName` | `string` | 字段的源名称（来自数据源）。 |
| `displayName` | `string` | 字段的显示名称。 |
| `area` | `number` | 字段要添加到的区域（行、列、值等区域的枚举值）。 |
| `subtotal?` | [`SubtotalType`](../enums/GC.Pivot.SubtotalType.md) | 添加到值区域时的汇总类型（可选）。 |
| `index?` | `number` | 字段在目标区域中的索引位置（可选）。 |

#### Returns

`void`

___

### <a id="addcalcfield" name="addcalcfield"></a> addCalcField

▸ **addCalcField**(`fieldName`, `formula`): `void`

**`description`** 添加计算字段（只能添加到值区域）。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                  ["01-一月","妈妈","燃油",74],
                  ["15-一月","妈妈","食品",235],
                  ["17-一月","爸爸","运动",20],
                  ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var pivotTable = sheet.pivotTables.add("myPivotTable", 'sourceData', 1, 1, layout, theme);
pivotTable.addCalcField("各项占比", "=金额/454");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 计算字段的名称。 |
| `formula` | `string` | 计算字段的公式（如“=字段1+字段2”）。 |

#### Returns

`void`

___

### <a id="addcalcitem" name="addcalcitem"></a> addCalcItem

▸ **addCalcItem**(`sourceName`, `calcItemName`, `formula`): `void`

**`description`** 添加计算项（基于现有字段的自定义计算）。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                 ["01-一月","妈妈","燃油",74],
                 ["15-一月","妈妈","食品",235],
                 ["17-一月","爸爸","运动",20],
                 ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var pivotTable = sheet.pivotTables.get("pivotTable_1");
pivotTable.add("购买者","购买者",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("类型","类型",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("金额","金额汇总",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.addCalcItem("购买者", "合计项", "=购买者[妈妈]+购买者[爸爸]");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sourceName` | `string` | 源字段的名称。 |
| `calcItemName` | `string` | 计算项的名称。 |
| `formula` | `string` | 计算项的公式（如“=字段[项1]+字段[项2]”）。 |

#### Returns

`void`

___

### <a id="addconditionalrule" name="addconditionalrule"></a> addConditionalRule

▸ **addConditionalRule**(`pivotArea`, `conditionalRule`): `void`

**`description`** 为指定数据透视区域设置条件格式规则。

**`example`**
```javascript
// 此示例使用三色刻度规则
var pivotTable = activeSheet.pivotTables.all()[0];
var rule = new GC.Spread.Sheets.ConditionalFormatting.ScaleRule();
rule.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.threeScaleRule);
rule.midColor("#12ff34"); // 中间色
rule.midType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number); // 中间值类型
rule.midValue(50000); // 中间值
rule.maxColor("#EE3344"); // 最大值颜色
rule.maxType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number); // 最大值类型
rule.maxValue(400000); // 最大值
rule.minColor("#AAff34"); // 最小值颜色
rule.minType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number); // 最小值类型
rule.minValue(5000); // 最小值
var AmericaPivotArea = {
       dataOnly: true,
       references: [{
           fieldName: "Country",
           items: ["America"]
       }]
   }
var BritainPivotArea = {
       dataOnly: true,
       references: [{
           fieldName: "Country",
           items: ["Britain"]
       }]
   }
pivotTable.addConditionalRule([AmericaPivotArea, BritainPivotArea], rule);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pivotArea` | [`IPivotArea`](../modules/GC.Spread.Pivot.md#ipivotarea)[] | 数据透视区域数组（包含字段和项的引用）。 |
| `conditionalRule` | [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md) | 要应用的条件格式规则。 |

#### Returns

`void`

___

### <a id="autofitcolumn" name="autofitcolumn"></a> autoFitColumn

▸ **autoFitColumn**(): `void`

**`description`** 自动调整列宽以适应字段内容。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                  ["01-一月","妈妈","燃油",74],
                  ["15-一月","妈妈","食品",235],
                  ["17-一月","爸爸","运动",20],
                  ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme);
pivotTable.add("类型", "类型", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("日期", "日期", GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("金额", "金额汇总", GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.autoFitColumn(); // 自动调整列宽
```

#### Returns

`void`

___

### <a id="autosortstate" name="autosortstate"></a> autoSortState

▸ **autoSortState**(`fieldName`, `enabled?`): `boolean` \| `void`

**`description`** 获取或设置数据透视表字段的排序选项。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.workbook(document.getElementById("ss"));
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = spread.getSheet(0).pivotTables.add("pivotTable_1",sourceData,1,1,layout,theme,options);
pivotTable.add("Buyer","Buyer",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Type","Type",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.sort("Type", { sortType: GC.Pivot.SortType.asc, sortValueFieldName: "Sum of Amount"});
pivotTable.autoSortState("Buyer", false);
pivotTable.sort("Buyer", { sortType: GC.Pivot.SortType.asc });
pivotTable.sort("Buyer", { customSortCallback: function(fieldItemNameArray) {
    return fieldItemNameArray.sort((a, b) => a.length - b.length);
    }
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 要设置排序选项的字段名称。 |
| `enabled?` | `boolean` | 指示字段是否处于自动排序状态。 |

#### Returns

`boolean` \| `void`

___

### <a id="clearoverwritelist" name="clearoverwritelist"></a> clearOverwriteList

▸ **clearOverwriteList**(): `void`

**`description`** 清除覆盖值列表（用于自定义单元格值的缓存）。

#### Returns

`void`

___

### <a id="collapse" name="collapse"></a> collapse

▸ **collapse**(`fieldName`, `item`, `isCollapse?`): `boolean` \| `void`

**`description`** 获取或设置字段的折叠状态。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                  ["01-一月","妈妈","燃油",74],
                  ["15-一月","妈妈","食品",235],
                  ["17-一月","爸爸","运动",20],
                  ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var subtotal = GC.Pivot.SubtotalType.count;
pivotTable.add("购买者", "购买者", 1, subtotal, 0);
pivotTable.add("类型", "类型", 1, subtotal, 1);
var 当前状态 = pivotTable.collapse("购买者", "妈妈"); // 获取“妈妈”项的折叠状态
pivotTable.collapse("购买者", "妈妈", !当前状态); // 切换折叠状态
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 目标字段的名称。 |
| `item` | `string` | 要折叠/展开的项的名称。 |
| `isCollapse?` | `boolean` | 折叠状态（true=折叠，false=展开；未指定时返回当前状态）。 |

#### Returns

`boolean` \| `void`

当前折叠状态（无参数时返回）。

___

### <a id="connectslicer" name="connectslicer"></a> connectSlicer

▸ **connectSlicer**(`name`): `void`

**`description`** 将切片器连接到数据透视表（建立筛选关联）。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 切片器的名称。 |

#### Returns

`void`

___

### <a id="dataposition" name="dataposition"></a> dataPosition

▸ **dataPosition**(`positionType?`, `positionIndex?`): `void` \| [`IDataPosition`](../modules/GC.Pivot.md#idataposition)

**`description`** 获取或设置值字段在数据透视表中的位置（行区域或列区域）。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                  ["01-一月","妈妈","燃料",74],
                  ["15-一月","妈妈","食品",235],
                  ["17-一月","爸爸","体育",20],
                  ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.dataPosition(1,0) //将值移动到行区域，索引为0
pivotTable.dataPosition();//{positionType:1,positionIndex:0}
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `positionType?` | [`DataPosition`](../enums/GC.Pivot.DataPosition.md) | 位置类型（行区域或列区域的枚举值）。 |
| `positionIndex?` | `number` | 在目标区域中的索引位置。 |

#### Returns

`void` \| [`IDataPosition`](../modules/GC.Pivot.md#idataposition)

数据位置信息（无参数时返回当前设置）。

___

### <a id="deserialize" name="deserialize"></a> deserialize

▸ **deserialize**(`serializeInfo`): `void`

**`description`** 将序列化的数据透视表数据恢复到已存在的数据透视表中

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                  ["01-一月","妈妈","燃料",74],
                  ["15-一月","妈妈","食品",235],
                  ["17-一月","爸爸","运动",20],
                  ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme);
pivotTable.add("购买者","购买者",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("类型","类型",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("金额","金额汇总",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
var serialization = pivotTable.serialize();
pivotTable.remove('类型');
pivotTable.deserialize(serialization);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `serializeInfo` | [`ISerializeInfo`](../modules/GC.Spread.Pivot.md#iserializeinfo) | 序列化的数据透视表数据 |

#### Returns

`void`

___

### <a id="disconnectslicer" name="disconnectslicer"></a> disconnectSlicer

▸ **disconnectSlicer**(`name`): `void`

断开切片器与数据透视表的连接

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |

#### Returns

`void`

___

### <a id="getallslicers" name="getallslicers"></a> getAllSlicers

▸ **getAllSlicers**(): [`PivotTableItemSlicer`](GC.Spread.Pivot.PivotTableItemSlicer.md)[]

获取与数据透视表连接的所有切片器

#### Returns

[`PivotTableItemSlicer`](GC.Spread.Pivot.PivotTableItemSlicer.md)[]

与数据透视表连接的切片器数组

___

### <a id="getcalcfields" name="getcalcfields"></a> getCalcFields

▸ **getCalcFields**(): [`ICalcFieldInfo`](../modules/GC.Spread.Pivot.md#icalcfieldinfo)[]

**`description`** 获取所有计算字段的信息

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                  ["01-一月","妈妈","燃料",74],
                  ["15-一月","妈妈","食品",235],
                  ["17-一月","爸爸","运动",20],
                  ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var pivotTable = sheet.pivotTables.add("pivotTable1", 'sourceData', 1, 1, layout, theme);
pivotTable.addCalcField("各部分百分比", "=金额/454");
pivotTable.getCalcFields();
```

#### Returns

[`ICalcFieldInfo`](../modules/GC.Spread.Pivot.md#icalcfieldinfo)[]

返回所有计算字段的信息数组

___

### <a id="getcalcitems" name="getcalcitems"></a> getCalcItems

▸ **getCalcItems**(`sourceName?`): [`ICalcItemInfo`](../modules/GC.Spread.Pivot.md#icalciteminfo)[]

**`description`** 获取计算项信息

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                 ["01-一月","妈妈","燃料",74],
                 ["15-一月","妈妈","食品",235],
                 ["17-一月","爸爸","运动",20],
                 ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var pivotTable = sheet.pivotTables.get("pivotTable_1");
pivotTable.add("购买者","购买者",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("类型","类型",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("金额","金额汇总",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.addCalcItem("购买者", "公式1", "=购买者[妈妈]+购买者[爸爸]");
pivotTable.getCalcItems("购买者");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sourceName?` | `string` | 源字段名称 |

#### Returns

[`ICalcItemInfo`](../modules/GC.Spread.Pivot.md#icalciteminfo)[]

计算项信息数组

___

### <a id="getconditionalrules" name="getconditionalrules"></a> getConditionalRules

▸ **getConditionalRules**(`pivotArea`): [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)[]

获取数据透视区域使用的规则

**`example`**
```javascript
//本示例使用getRule方法
var pivotTable = activeSheet.pivotTables.all()[0];
var rule = new GC.Spread.Sheets.ConditionalFormatting.ScaleRule();
rule.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.threeScaleRule);
rule.midColor("#12ff34");
rule.midType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
rule.midValue(50000);
rule.maxColor("#EE3344");
rule.maxType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
rule.maxValue(400000);
rule.minColor("#AAff34");
rule.minType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
rule.minValue(5000);
var AmericaPivotArea = {
       dataOnly: true
       references: [{
           fieldName: "国家",
           items: ["美国"]
       }]
   }
var BritainPivotArea = {
       dataOnly: true
       references: [{
           fieldName: "国家",
           items: ["英国"]
       }]
   }
pivotTable.addConditionalRule([AmericaPivotArea, BritainPivotArea], rule);
var ruleTest = pivotTable.getConditionalRules(BritainPivotArea);
alert(ruleTest[0].midValue());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pivotArea` | [`IPivotArea`](../modules/GC.Spread.Pivot.md#ipivotarea) | 数据透视表中的数据透视区域 |

#### Returns

[`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)[]

数据透视区域的规则数组

___

### <a id="getfield" name="getfield"></a> getField

▸ **getField**(`fieldName`): [`IFieldInfo`](../modules/GC.Spread.Pivot.md#ifieldinfo)

**`description`** 按字段名从数据透视表中获取字段信息

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                  ["01-一月","妈妈","燃料",74],
                  ["15-一月","妈妈","食品",235],
                  ["17-一月","爸爸","运动",20],
                  ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.add("购买者","购买者",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("类型","类型",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("金额","金额汇总",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.getField("类型");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 字段名称 |

#### Returns

[`IFieldInfo`](../modules/GC.Spread.Pivot.md#ifieldinfo)

返回字段信息对象

___

### <a id="getfieldsbyarea" name="getfieldsbyarea"></a> getFieldsByArea

▸ **getFieldsByArea**(`area?`): [`IFieldInfo`](../modules/GC.Spread.Pivot.md#ifieldinfo)[]

**`description`** 从数据透视表或某个数据透视区域获取所有字段信息

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                  ["01-一月","妈妈","燃料",74],
                  ["15-一月","妈妈","食品",235],
                  ["17-一月","爸爸","运动",20],
                  ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.add("购买者","购买者",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("类型","类型",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("金额","金额汇总",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.getFieldsByArea(GC.Spread.PivotTableFieldType.columnField);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `area?` | [`PivotTableFieldType`](../enums/GC.Spread.Pivot.PivotTableFieldType.md) | 区域索引（可选） |

#### Returns

[`IFieldInfo`](../modules/GC.Spread.Pivot.md#ifieldinfo)[]

返回数据透视区域的所有字段信息数组

___

### <a id="getitemsbyfield" name="getitemsbyfield"></a> getItemsByField

▸ **getItemsByField**(`fieldName`, `sorted?`): `any`

**`description`** 按字段名从数据透视表中获取所有项

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 数据透视表字段的名称 |
| `sorted?` | `boolean` | 是否按排序顺序返回项（可选） |

#### Returns

`any`

返回数据透视表字段的所有项数组

___

### <a id="getnodeinfo" name="getnodeinfo"></a> getNodeInfo

▸ **getNodeInfo**(`row`, `col`): [`IPivotNodeInfo`](../modules/GC.Spread.Pivot.md#ipivotnodeinfo)

从工作表行和列构建覆盖信息

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 单元格所在的工作表行号 |
| `col` | `number` | 单元格所在的工作表列号 |

#### Returns

[`IPivotNodeInfo`](../modules/GC.Spread.Pivot.md#ipivotnodeinfo)

需要获取的节点信息对象

___

### <a id="getnodevalue" name="getnodevalue"></a> getNodeValue

▸ **getNodeValue**(`nodeInfo`): `number`

根据节点信息获取值

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `nodeInfo` | [`IPivotNodeInfo`](../modules/GC.Spread.Pivot.md#ipivotnodeinfo) | 要获取的节点信息 |

#### Returns

`number`

节点信息的值

___

### <a id="getoverwritelist" name="getoverwritelist"></a> getOverwriteList

▸ **getOverwriteList**(): [`IPivotOverwriteNodeInfo`](../modules/GC.Spread.Pivot.md#ipivotoverwritenodeinfo)[]

获取数据透视缓存的所有覆盖信息

#### Returns

[`IPivotOverwriteNodeInfo`](../modules/GC.Spread.Pivot.md#ipivotoverwritenodeinfo)[]

覆盖信息列表

___

### <a id="getpivotarearanges" name="getpivotarearanges"></a> getPivotAreaRanges

▸ **getPivotAreaRanges**(`pivotArea`): [`Range`](GC.Spread.Sheets.Range.md)[]

**`description`** 获取与特定数据透视区域对应的工作表范围

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                 ["01-一月","妈妈","燃料",74],
                 ["15-一月","妈妈","食品",235],
                 ["17-一月","爸爸","运动",20],
                 ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.add("购买者", "购买者", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("类型", "类型", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("日期", "日期", GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("金额", "金额", GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
var pivotArea = {
    dataOnly: false,
    references: [
        {
            fieldName: "购买者",
            items: ["妈妈", "爸爸"]
        }
    ]
};
let ranges = pivotTable.getPivotAreaRanges(pivotArea);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pivotArea` | [`IPivotArea`](../modules/GC.Spread.Pivot.md#ipivotarea) | 特定的数据透视区域 |

#### Returns

[`Range`](GC.Spread.Sheets.Range.md)[]

与特定数据透视区域对应的工作表范围

___

### <a id="getpivotdetails" name="getpivotdetails"></a> getPivotDetails

▸ **getPivotDetails**(`pivotItemInfo`): `void` \| `any`[][]

**`description`** 获取数据透视表详细信息

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                 ["01-一月","妈妈","燃料",74],
                 ["15-一月","妈妈","食品",235],
                 ["17-一月","爸爸","运动",20],
                 ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var pivotTable = sheet.pivotTables.get("pivotTable_1");
pivotTable.add("购买者","购买者",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("类型","类型",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("金额","金额汇总",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.getPivotDetails([{fieldName:"购买者", fieldItem:"凯莉"}]);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pivotItemInfo` | [`IPivotItemInfo`](../interfaces/GC.Spread.Pivot.IPivotItemInfo.md)[] | 数据透视详细信息列表 |

#### Returns

`void` \| `any`[][]

___

### <a id="getrange" name="getrange"></a> getRange

▸ **getRange**(): [`IPivotTableRange`](../modules/GC.Spread.Pivot.md#ipivottablerange)

**`description`** 获取数据透视表的范围，由页和内容组成。这些范围是只读的，更改范围不会产生任何效果。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                 ["01-一月","妈妈","燃料",74],
                 ["15-一月","妈妈","食品",235],
                 ["17-一月","爸爸","运动",20],
                 ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var pivotTable = sheet.pivotTables.add("pivotTable1", 'sourceData', 1, 1, layout, theme);
pivotTable.add("购买者", "购买者", GC.Spread.Pivot.PivotTableFieldType.filterField);
pivotTable.add("类型", "类型", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("日期", "日期", GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("金额", "金额", GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
var ranges = pivotTable.getRange();
console.log(ranges.page, ranges.content);
```

#### Returns

[`IPivotTableRange`](../modules/GC.Spread.Pivot.md#ipivottablerange)

返回当前数据透视表的范围

___

### <a id="getsource" name="getsource"></a> getSource

▸ **getSource**(): `string`

**`description`** 获取数据透视表的数据引用

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                 ["01-一月","妈妈","燃料",74],
                 ["15-一月","妈妈","食品",235],
                 ["17-一月","爸爸","运动",20],
                 ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme);
var pivotTable = sheet.pivotTables.get("pivotTable_1");
pivotTable.getSource();
```

#### Returns

`string`

___

### <a id="getsourcefields" name="getsourcefields"></a> getSourceFields

▸ **getSourceFields**(): [`ISourceFieldInfo`](../modules/GC.Spread.Pivot.md#isourcefieldinfo)[]

**`description`** 获取数据透视表的源字段信息

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                 ["01-一月","妈妈","燃料",74],
                 ["15-一月","妈妈","食品",235],
                 ["17-一月","爸爸","运动",20],
                 ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var pivotTable = sheet.pivotTables.get("pivotTable_1");
pivotTable.addCalcField("calcField", "=金额*2");
pivotTable.getSourceFields();
```

#### Returns

[`ISourceFieldInfo`](../modules/GC.Spread.Pivot.md#isourcefieldinfo)[]

___

### <a id="getstyle" name="getstyle"></a> getStyle

▸ **getStyle**(`pivotArea`): [`Style`](GC.Spread.Sheets.Style.md)

**`description`** 根据特定的数据透视区域获取样式

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                 ["01-一月","妈妈","燃料",74],
                 ["15-一月","妈妈","食品",235],
                 ["17-一月","爸爸","运动",20],
                 ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.add("购买者", "购买者", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("类型", "类型", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("日期", "日期", GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("金额", "金额", GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
var pivotArea = {
    dataOnly: false,
    references: [
        {
            fieldName: "购买者",
            items: ["妈妈", "爸爸"]
        }
    ]
};
var style = new GC.Spread.Sheets.Style();
redBack.backColor = '#ff0000';
pivotTable.setStyle(pivotArea, style);
pivotTable.getStyle(pivotArea);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pivotArea` | [`IPivotArea`](../modules/GC.Spread.Pivot.md#ipivotarea) | 特定的数据透视区域 |

#### Returns

[`Style`](GC.Spread.Sheets.Style.md)

GC.Spread.Sheets.Style

___

### <a id="getthemename" name="getthemename"></a> getThemeName

▸ **getThemeName**(): `undefined` \| `string`

获取或设置数据透视表的样式名称

#### Returns

`undefined` \| `string`

返回数据透视表样式名称

___

### <a id="group" name="group"></a> group

▸ **group**(`groupInfo`): `void`

**`description`** 对字段的项进行分组

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                  ["01-一月","妈妈","燃料",74],
                  ["15-一月","妈妈","食品",235],
                  ["17-一月","爸爸","运动",20],
                  ["19-一月","大卫","书籍",120],
                  ["20-一月","爸爸","食品",160],
                  ["21-一月","大卫","运动",15],
                  ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 8, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var groupInfo = {
    originFieldName: "购买者",
    textGroup: {
        fieldName: "家庭成员",
        groupItems: {
             "parent": ["妈妈", "爸爸"],
             "children": ["大卫", "凯莉"]
        }
    }
};
pivotTable.group(groupInfo);
pivotTable.add("家庭成员", "家庭成员", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("购买者", "购买者", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("金额", "金额汇总", GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
sheet.resumePaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `groupInfo` | [`IDateGroupsInfo`](../modules/GC.Spread.Pivot.md#idategroupsinfo) \| [`INumberGroupInfo`](../modules/GC.Spread.Pivot.md#inumbergroupinfo) \| [`ITextGroupInfo`](../modules/GC.Spread.Pivot.md#itextgroupinfo) | 表示分组信息 |

#### Returns

`void`

___

### <a id="isconnectedslicer" name="isconnectedslicer"></a> isConnectedSlicer

▸ **isConnectedSlicer**(`name`): `boolean`

判断切片器是否与数据透视表连接

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 切片器名称 |

#### Returns

`boolean`

切片器是否与数据透视表连接

___

### <a id="labelfilter" name="labelfilter"></a> labelFilter

▸ **labelFilter**(`fieldName`, `filterInfo?`): `void` \| [`IPivotConditionFilterInfo`](../modules/GC.Spread.Pivot.md#ipivotconditionfilterinfo) \| [`IPivotTextFilterInfo`](../modules/GC.Spread.Pivot.md#ipivottextfilterinfo)

获取或设置字段的标签筛选器信息

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                  ["01-一月","妈妈","燃料",74],
                  ["15-一月","妈妈","食品",235],
                  ["17-一月","爸爸","运动",20],
                  ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.suspendLayout();
pivotTable.options.showRowHeader = true;
pivotTable.options.showColumnHeader = true;
pivotTable.add("购买者", "购买者", GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("类型", "类型", GC.Spread.Pivot.PivotTableFieldType.rowField);
var condition = { conType: GC.Pivot.PivotConditionType.caption, operator: GC.Pivot.PivotCaptionFilterOperator.contains, val: ["妈妈"] };
var filterInfo = { condition };
pivotTable.labelFilter("购买者", filterInfo);
pivotTable.add("金额", "金额汇总", GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.resumeLayout();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 表示数据透视表的目标字段名称 |
| `filterInfo?` | ``null`` \| [`IPivotConditionFilterInfo`](../modules/GC.Spread.Pivot.md#ipivotconditionfilterinfo) \| [`IPivotTextFilterInfo`](../modules/GC.Spread.Pivot.md#ipivottextfilterinfo) | 设置时表示标签筛选器信息 |

#### Returns

`void` \| [`IPivotConditionFilterInfo`](../modules/GC.Spread.Pivot.md#ipivotconditionfilterinfo) \| [`IPivotTextFilterInfo`](../modules/GC.Spread.Pivot.md#ipivottextfilterinfo)

返回数据透视表标签筛选器信息

___

### <a id="layouttype" name="layouttype"></a> layoutType

▸ **layoutType**(`type?`): [`PivotTableLayoutType`](../enums/GC.Spread.Pivot.PivotTableLayoutType.md)

**`description`** 获取或设置数据透视表的布局类型

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                  ["01-一月","妈妈","燃料",74],
                  ["15-一月","妈妈","食品",235],
                  ["17-一月","爸爸","运动",20],
                  ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var pivotTableLayoutType = GC.Spread.Pivot.PivotTableLayoutType.compact;
pivotTable.layoutType(pivotTableLayoutType);
pivotTable.layoutType();//GC.Spread.Pivot.PivotTableLayoutType.compact
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type?` | [`PivotTableLayoutType`](../enums/GC.Spread.Pivot.PivotTableLayoutType.md) | 表示数据透视表布局类型 |

#### Returns

[`PivotTableLayoutType`](../enums/GC.Spread.Pivot.PivotTableLayoutType.md)

如果不传入参数，则获取当前布局类型

___

### <a id="name" name="name"></a> name

▸ **name**(`name?`): `string` \| `void`

**`description`** 获取或设置数据透视表名称

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                  ["01-一月","妈妈","燃料",74],
                  ["15-一月","妈妈","食品",235],
                  ["17-一月","爸爸","运动",20],
                  ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.name("pivotTable_2")
console.log(pivotTable.name()); //pivotTable_2
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name?` | `string` | 表示数据透视表名称 |

#### Returns

`string` \| `void`

___

### <a id="position" name="position"></a> position

▸ **position**(`row?`, `col?`, `sheetName?`): `void` \| [`IPivotTablePosition`](../modules/GC.Spread.Pivot.md#ipivottableposition)

**`description`** 获取或设置数据透视表的起始位置，当有足够的单元格放置数据透视表时，其位置将自动更改

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var toSheet = spread.getSheet(2);
var sourceData = [["日期","购买者","类型","金额"],
                  ["01-一月","妈妈","燃料",74],
                  ["15-一月","妈妈","食品",235],
                  ["17-一月","爸爸","运动",20],
                  ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.position(10,10,toSheet.name());
pivotTable.position(); //{row:10,col:10, sheetName: "Sheet3"}
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row?` | `number` | 表示数据透视表的起始行 |
| `col?` | `number` | 表示数据透视表的起始列 |
| `sheetName?` | `string` | 数据透视表所在的工作表名称 |

#### Returns

`void` \| [`IPivotTablePosition`](../modules/GC.Spread.Pivot.md#ipivottableposition)

___

### <a id="refresh" name="refresh"></a> refresh

▸ **refresh**(): `void`

**`description`** 刷新字段布局，重新计算工作表中的所有字段数据

#### Returns

`void`

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`fieldName`): `void`

**`description`** 按名称删除字段

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                  ["01-一月","妈妈","燃料",74],
                  ["15-一月","妈妈","食品",235],
                  ["17-一月","爸爸","运动",20],
                  ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.add("购买者", "购买者", 1, GC.Pivot.SubtotalType.count, 0);
pivotTable.remove("购买者");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 要删除的字段名称 |

#### Returns

`void`

___

### <a id="removecalcfield" name="removecalcfield"></a> removeCalcField

▸ **removeCalcField**(`fieldName`): `void`

**`description`** 删除计算字段

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                  ["01-一月","妈妈","燃料",74],
                  ["15-一月","妈妈","食品",235],
                  ["17-一月","爸爸","运动",20],
                  ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var pivotTable = sheet.pivotTables.add("pivotTable1", 'sourceData', 1, 1, layout, theme);
pivotTable.addCalcField("各部分百分比", "=金额/454");
var calcFieldsInfo = pivotTable.getCalcFields();
pivotTable.removeCalcField(calcFieldsInfo[0].fieldName);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 计算字段名称 |

#### Returns

`void`

___

### <a id="removecalcitem" name="removecalcitem"></a> removeCalcItem

▸ **removeCalcItem**(`sourceName`, `calcItemName`): `void`

**`description`** 删除计算项

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                 ["01-一月","妈妈","燃料",74],
                 ["15-一月","妈妈","食品",235],
                 ["17-一月","爸爸","运动",20],
                 ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var pivotTable = sheet.pivotTables.get("pivotTable_1");
pivotTable.add("购买者","购买者",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("类型","类型",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("金额","金额汇总",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.addCalcItem("购买者", "公式1", "=购买者[妈妈]+购买者[爸爸]");
pivotTable.removeCalcItem("购买者", "公式1");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sourceName` | `string` | 源字段名称 |
| `calcItemName` | `string` | 源字段计算项名称 |

#### Returns

`void`

___

### <a id="removeconditionalrule" name="removeconditionalrule"></a> removeConditionalRule

▸ **removeConditionalRule**(`conditionalRule`): `void`

删除数据透视表的规则

**`example`**
```javascript
//本示例使用getRule方法
var pivotTable = activeSheet.pivotTables.all()[0];
var rule = new GC.Spread.Sheets.ConditionalFormatting.ScaleRule();
rule.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.threeScaleRule);
rule.midColor("#12ff34");
rule.midType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
rule.midValue(50000);
rule.maxColor("#EE3344");
rule.maxType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
rule.maxValue(400000);
rule.minColor("#AAff34");
rule.minType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
rule.minValue(5000);
var AmericaPivotArea = {
       dataOnly: true,
       references: [{
           fieldName: "Country",
           items: ["America"]
       }]
   }
var BritainPivotArea = {
       dataOnly: true,
       references: [{
           fieldName: "Country",
           items: ["Britain"]
       }]
   }
pivotTable.addConditionalRule([AmericaPivotArea, BritainPivotArea], rule);
pivotTable.removeConditionalRule(rule);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `conditionalRule` | [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md) | 设置到数据透视表的规则 |

#### Returns

`void`

___

### <a id="resumelayout" name="resumelayout"></a> resumeLayout

▸ **resumeLayout**(): `void`

**`description`** 停止暂缓更新字段，结束suspendLayout的效果，必须与suspendLayout成对使用

#### Returns

`void`

___

### <a id="serialize" name="serialize"></a> serialize

▸ **serialize**(): [`ISerializeInfo`](../modules/GC.Spread.Pivot.md#iserializeinfo)

**`description`** 获取序列化的数据透视表数据

#### Returns

[`ISerializeInfo`](../modules/GC.Spread.Pivot.md#iserializeinfo)

序列化的数据透视表数据

___

### <a id="setnodevalue" name="setnodevalue"></a> setNodeValue

▸ **setNodeValue**(`nodeInfo`, `value?`): `void`

向数据透视缓存设置覆盖值

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `nodeInfo` | [`IPivotNodeInfo`](../modules/GC.Spread.Pivot.md#ipivotnodeinfo) | 要设置的节点信息 |
| `value?` | `number` | 要设置到节点信息的值，若value为null或undefined，则移除该节点信息的值 |

#### Returns

`void`

___

### <a id="setstyle" name="setstyle"></a> setStyle

▸ **setStyle**(`pivotArea`, `style`): `void`

**`description`** 向特定数据透视区域设置或移除样式

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                 ["01-一月","妈妈","燃料",74],
                 ["15-一月","妈妈","食品",235],
                 ["17-一月","爸爸","运动",20],
                 ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.add("购买者", "购买者", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("类型", "类型", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("日期", "日期", GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("金额", "金额", GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
var pivotArea = {
    dataOnly: false,
    references: [
        {
            fieldName: "购买者",
            items: ["妈妈", "爸爸"]
        }
    ]
};
var style = new GC.Spread.Sheets.Style();
style.backColor = '#ff0000';
pivotTable.setStyle(pivotArea, style);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pivotArea` | [`IPivotArea`](../modules/GC.Spread.Pivot.md#ipivotarea) | 特定的数据透视区域 |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 要设置到特定数据透视区域的样式，null或undefined表示移除该区域的样式 |

#### Returns

`void`

___

### <a id="showdataas" name="showdataas"></a> showDataAs

▸ **showDataAs**(`fieldName`, `showDataAsInfo?`): `void` \| [`IPivotShowDataAsInfo`](../modules/GC.Spread.Pivot.md#ipivotshowdataasinfo)

**`description`** 获取或设置值字段的"数据显示为"信息

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 要应用"数据显示为"设置的值字段名称 |
| `showDataAsInfo?` | [`IPivotShowDataAsInfo`](../modules/GC.Spread.Pivot.md#ipivotshowdataasinfo) | 应用于值字段的"数据显示为"信息 |

#### Returns

`void` \| [`IPivotShowDataAsInfo`](../modules/GC.Spread.Pivot.md#ipivotshowdataasinfo)

___

### <a id="shownodata" name="shownodata"></a> showNoData

▸ **showNoData**(`cacheFieldName`, `isShow`): `boolean`

**`description`** 设置或获取字段"显示无数据项"的信息

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                 ["01-一月","妈妈","燃料",74],
                 ["15-一月","妈妈","食品",235],
                 ["17-一月","爸爸","运动",20],
                 ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var pivotTable = sheet.pivotTables.get("pivotTable_1");
pivotTable.add("日期","日期",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("购买者","购买者",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("类型","类型",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("金额","金额汇总",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.showNoData("购买者", true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cacheFieldName` | `string` | - |
| `isShow` | `boolean` | 标志是否显示无数据的项 |

#### Returns

`boolean`

___

### <a id="sort" name="sort"></a> sort

▸ **sort**(`fieldName`, `sortInfo`): `void` \| [`IPivotViewSortInfo`](../modules/GC.Pivot.md#ipivotviewsortinfo)

**`description`** 获取或设置数据透视表字段的排序

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceData = [["日期","购买者","类型","金额"],
                  ["01-一月","妈妈","燃料",74],
                  ["15-一月","妈妈","食品",235],
                  ["17-一月","爸爸","运动",20],
                  ["21-一月","凯莉","书籍",125]];
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = spread.getSheet(0).pivotTables.add("pivotTable_1", sourceData, 1, 1, layout, theme, options);
pivotTable.add("购买者","购买者",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("类型","类型",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("金额", "总金额", GC.Spread.Pivot.PivotTableFieldType.valueField);
pivotTable.sort("类型", { sortType: GC.Pivot.SortType.asc, sortValueFieldName: "总金额"});
pivotTable.sort("购买者", { sortType: GC.Pivot.SortType.asc });
pivotTable.sort("购买者", { customSortCallback: function(fieldItemNameArray) {
    return fieldItemNameArray.sort((a, b) => a.length - b.length);
    }
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 目标字段名称 |
| `sortInfo` | [`IPivotViewSortInfo`](../modules/GC.Pivot.md#ipivotviewsortinfo) | 排序信息 |

#### Returns

`void` \| [`IPivotViewSortInfo`](../modules/GC.Pivot.md#ipivotviewsortinfo)

___

### <a id="subtotalposition" name="subtotalposition"></a> subtotalPosition

▸ **subtotalPosition**(`fieldName`, `position`): `void` \| [`SubtotalsPosition`](../enums/GC.Spread.Pivot.SubtotalsPosition.md)

**`description`** 设置或获取字段显示分类汇总的位置信息

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                 ["01-一月","妈妈","燃料",74],
                 ["15-一月","妈妈","食品",235],
                 ["17-一月","爸爸","运动",20],
                 ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var pivotTable = sheet.pivotTables.get("pivotTable_1");
pivotTable.add("日期","日期",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("购买者","购买者",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("类型","类型",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("金额","金额汇总",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.subtotalPosition("购买者", GC.Spread.Pivot.SubtotalsPosition.top);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 字段名称 |
| `position` | [`SubtotalsPosition`](../enums/GC.Spread.Pivot.SubtotalsPosition.md) | 指示设置分类汇总的位置，仅支持顶部和底部 |

#### Returns

`void` \| [`SubtotalsPosition`](../enums/GC.Spread.Pivot.SubtotalsPosition.md)

___

### <a id="subtotaltype" name="subtotaltype"></a> subtotalType

▸ **subtotalType**(`fieldName`, `type?`): `void` \| [`SubtotalType`](../enums/GC.Pivot.SubtotalType.md)

获取或设置字段的分类汇总类型

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.add("购买者","购买者",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("类型","类型",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("金额","金额汇总",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
var subtotalType = GC.Pivot.SubtotalType.average;
pivotTable.subtotalType("购买者", subtotalType); // 为名称是"购买者"的字段设置分类汇总类型
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 数据透视表的目标字段名称 |
| `type?` | [`SubtotalType`](../enums/GC.Pivot.SubtotalType.md) | 要设置的分类汇总类型 |

#### Returns

`void` \| [`SubtotalType`](../enums/GC.Pivot.SubtotalType.md)

___

### <a id="subtotalvisible" name="subtotalvisible"></a> subtotalVisible

▸ **subtotalVisible**(`fieldName`, `isVisible`): `boolean`

**`description`** 设置或获取字段是否显示分类汇总信息

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                 ["01-一月","妈妈","燃料",74],
                 ["15-一月","妈妈","食品",235],
                 ["17-一月","爸爸","运动",20],
                 ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var pivotTable = sheet.pivotTables.get("pivotTable_1");
pivotTable.add("日期","日期",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("购买者","购买者",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("类型","类型",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("金额","金额汇总",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.subtotalVisible("购买者", false);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 字段名称 |
| `isVisible` | `boolean` | 指示是否显示该字段的分类汇总信息 |

#### Returns

`boolean`

___

### <a id="suspendlayout" name="suspendlayout"></a> suspendLayout

▸ **suspendLayout**(): `void`

**`description`** 暂停更新字段，直到调用resumeFieldsLayout，必须与resumeFieldsLayout成对使用

#### Returns

`void`

___

### <a id="theme" name="theme"></a> theme

▸ **theme**(`theme?`): `void` \| [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md)

获取或设置数据透视表主题

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                  ["01-一月","妈妈","燃料",74],
                  ["15-一月","妈妈","食品",235],
                  ["17-一月","爸爸","运动",20],
                  ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.theme("light3");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `theme?` | `string` \| [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md) | 指示数据透视表内部主题名称或数据透视表主题实例 |

#### Returns

`void` \| [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md)

如果不传入参数，则获取当前主题

___

### <a id="ungroup" name="ungroup"></a> ungroup

▸ **ungroup**(`fieldName`): `void`

**`description`** 根据字段名称取消字段分组

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 3 });
var sheet = spread.getActiveSheet();
sheet.suspendPaint();
var sourceDataArray = [["日期", "购买者", "类型", "金额"],
["01-一月", "妈妈", "燃料", 74],
["15-一月", "妈妈", "食品", 235],
["17-一月", "爸爸", "运动", 20],
["19-一月", "大卫", "书籍", 120],
["20-一月", "爸爸", "食品", 160],
["21-一月", "大卫", "运动", 15],
["21-一月", "凯莉", "书籍", 125]];
sheet.setArray(3, 0, sourceDataArray);
sheet.tables.add('Table1', 3, 0, 8, 4);
sheet.setColumnWidth(6, 130);
sheet.setColumnWidth(8, 100);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("PivotTable1", 'Table1', 3, 6, layout, theme, option);
var groupInfo = {
    originFieldName: "购买者",
    textGroup: {
        "parent": ["妈妈", "爸爸"],
        "children": ["大卫", "凯莉"]
    }
};
pivotTable.group("家庭成员", groupInfo);
pivotTable.add("家庭成员", "家庭成员", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("购买者", "购买者", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("金额", "金额汇总", GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
sheet.resumePaint();

pivotTable.ungroup("家庭成员");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 要取消分组的字段名称 |

#### Returns

`void`

___

### <a id="updatecalcitem" name="updatecalcitem"></a> updateCalcItem

▸ **updateCalcItem**(`sourceName`, `calcItemName`, `formula`, `priority`): `void`

**`description`** 更新计算项信息

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                 ["01-一月","妈妈","燃料",74],
                 ["15-一月","妈妈","食品",235],
                 ["17-一月","爸爸","运动",20],
                 ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var pivotTable = sheet.pivotTables.get("pivotTable_1");
pivotTable.add("购买者","购买者",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("类型","类型",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("金额","金额汇总",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.addCalcItem("购买者", "公式1", "=购买者[妈妈]+购买者[爸爸]");
pivotTable.updateCalcItem("购买者", "公式1", "=购买者[妈妈]+购买者[凯莉]", 1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sourceName` | `string` | 源字段名称 |
| `calcItemName` | `string` | 源字段计算项名称 |
| `formula` | `string` | 此计算项的新公式 |
| `priority` | `number` | 此计算项的新优先级 |

#### Returns

`void`

___

### <a id="updatefield" name="updatefield"></a> updateField

▸ **updateField**(`name`, `area`, `index?`): `void`

**`description`** 更新字段区域和索引

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                  ["01-一月","妈妈","燃料",74],
                  ["15-一月","妈妈","食品",235],
                  ["17-一月","爸爸","运动",20],
                  ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.add("购买者","购买者",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("类型","类型",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("金额","金额汇总",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.updateField("购买者", GC.Spread.Pivot.PivotTableFieldType.columnField, 0); // 名称为"购买者"的字段移动到列区域，字段索引为2
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 字段名称 |
| `area` | [`PivotTableFieldType`](../enums/GC.Spread.Pivot.PivotTableFieldType.md) | 指示字段要放置的区域 |
| `index?` | `number` | 指示要设置的索引位置 |

#### Returns

`void`

___

### <a id="updatefieldname" name="updatefieldname"></a> updateFieldName

▸ **updateFieldName**(`oldName`, `newName`): `void`

**`description`** 更新现有字段名称

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                  ["01-一月","妈妈","燃料",74],
                  ["15-一月","妈妈","食品",235],
                  ["17-一月","爸爸","运动",20],
                  ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.add("购买者","购买者",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.updateFieldName("购买者", "新购买者");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `oldName` | `string` | 数据透视表中字段的旧显示名称 |
| `newName` | `string` | 数据透视表中字段的新显示名称 |

#### Returns

`void`

___

### <a id="updatesource" name="updatesource"></a> updateSource

▸ **updateSource**(`source?`): `void`

**`description`** 刷新数据透视表数据源

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                 ["01-一月","妈妈","燃料",74],
                 ["15-一月","妈妈","食品",235],
                 ["17-一月","爸爸","运动",20],
                 ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var pivotTable = sheet.pivotTables.get("pivotTable_1");
pivotTable.add("购买者","购买者",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("类型","类型",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("金额","金额汇总",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
sourceSheet.setValue(1,3,1000);
pivotTable.updateSource();
var newSourceData = [["销售员","产品类型","产品","销售额"],
                 ["孙琳","饮料","苹果汁",74],
                 ["金石鹏","饮料","牛奶",235],
                 ["张尚","甜点","巧克力",20],
                 ["孙杨","甜点","牛肉干",125]];
sourceSheet.setArray(10, 0, newSourceData);
sourceSheet.tables.add('newSourceData', 10, 0, 5, 4);
pivotTable.updateSource('newSourceData');
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `source?` | `string` |

#### Returns

`void`

___

### <a id="valuefilter" name="valuefilter"></a> valueFilter

▸ **valueFilter**(`fieldName`, `filterInfo?`): `void` \| [`IPivotConditionFilterInfo`](../modules/GC.Spread.Pivot.md#ipivotconditionfilterinfo)

获取或设置字段的值筛选器信息

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                  ["01-一月","妈妈","燃料",74],
                  ["15-一月","妈妈","食品",235],
                  ["17-一月","爸爸","运动",20],
                  ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.suspendLayout();
pivotTable.options.showRowHeader = true;
pivotTable.options.showColumnHeader = true;
pivotTable.add("购买者", "购买者", GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("类型", "类型", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("金额", "金额汇总", GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
let condition = { conType: GC.Pivot.PivotConditionType.value, operator: GC.Pivot.PivotValueFilterOperator.between, val: [0, 100] };
let filterInfo = { condition: condition, conditionByName: "金额汇总" };
pivotTable.valueFilter("购买者", filterInfo);
pivotTable.resumeLayout();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 数据透视表的目标字段名称 |
| `filterInfo?` | ``null`` \| [`IPivotConditionFilterInfo`](../modules/GC.Spread.Pivot.md#ipivotconditionfilterinfo) | 设置时指示值筛选器信息 |

#### Returns

`void` \| [`IPivotConditionFilterInfo`](../modules/GC.Spread.Pivot.md#ipivotconditionfilterinfo)

返回数据透视表值筛选信息
