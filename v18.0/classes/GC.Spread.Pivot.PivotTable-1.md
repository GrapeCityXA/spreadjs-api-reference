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

数据透视表

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 数据透视表的名称 |
| `sheet?` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 透视表所在工作表 |
| `row?` | `number` | 数据透视表的起始行 |
| `col?` | `number` | 数据透视表的起始列 |
| `layout?` | [`PivotTableLayoutType`](../enums/GC.Spread.Pivot.PivotTableLayoutType.md) | 数据透视表布局类型 |
| `style?` | [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md) | 数据透视表主题样式 |
| `options?` | [`IPivotTableOption`](../modules/GC.Spread.Pivot.md#ipivottableoption) | - |
| `layoutModel?` | `any` | - |

## Properties

### <a id="options" name="options"></a> options

• **options**: [`IPivotTableOption`](../modules/GC.Spread.Pivot.md#ipivottableoption)

透视表选项：

<!-- TODO这里的选项类型有误 -->

**`property`** {boolean} [allowMultipleFiltersPerField] 是否允许在一个字段中使用多个过滤器

**`property`** {boolean} [fillDownLabels] 是否显示重复标签项

**`property`** {boolean} [insertBlankLineAfterEachItem] 是否在每个项目末尾插入空白行

**`property`** {GC.Spread.Pivot.GrandTotalPosition} [grandTotalPosition] 是否在行、列或两者中显示总计

**`property`** {GC.Spread.Pivot.SubtotalsPosition} [subtotalsPosition] 是否在顶部、底部或不显示小计

**`property`** {GC.Spread.Pivot.DisplayFields} [displayFieldsInPageFilterArea] 表示页面区域中的字段显示方式是 先横向后纵向 还是 先纵向后横向

**`property`** {number} [reportFilterFieldsPerColumn] 每列中报表筛选字段的数量

**`property`** {boolean} [bandRows] 是否显示带状行

**`property`** {boolean} [bandColumns] 是否显示带状列

**`property`** {boolean} [showRowHeader] 是否显示行标题样式

**`property`** {boolean} [showColumnHeader] 是否显示列标题样式

**`property`** {boolean} [showDrill] 是否显示展开/折叠按钮

**`property`** {boolean} [showMissing] 是否使 missingCaption 选项生效

**`property`** {boolean} [missingCaption] 当实际值为空时应显示的值

**`property`** {boolean} [rowLabelIndent] 每一级标题的缩进量

**`property`** {boolean} [printDrill] 是否在数据透视表上显示时打印展开/折叠按钮

**`property`** {boolean} [itemPrintTitles] 是否在每个数据透视表上重复行标签

**`property`** {boolean} [fieldPrintTitles] 设置打印标题

**`property`** {boolean} [showFilter] 是否显示过滤按钮

**`property`** {boolean} [showToolTip] 是否显示ToolTip

**`property`** {boolean} [mergeItem] 是否将带有标签的单元格合并并居中

**`property`** {boolean} [isShowErrorValue] 是否使 errorValueInfo 选项生效

**`property`** {boolean} [errorValueInfo] 当实际值错误时应显示的值

**`property`** {string} [rowHeaderCaption] 在紧凑布局中替换行标签时显示的值

**`property`** {string} [colHeaderCaption] 在紧凑布局中替换列标签时显示的值

**`property`** {boolean} [showHeaders] 是否显示字段标题

**`property`** {GC.Spread.Pivot.CalcItemAggregation} [calcItemAggregation] 数据透视表总计是否包含 calcItem 的值

**`property`** {boolean} [enableDataValueEditing] 是否允许编辑数据透视表数据区域的单元格值

___

### <a id="views" name="views"></a> views

• **views**: [`IPivotTableViewManager`](../interfaces/GC.Spread.Pivot.IPivotTableViewManager.md)

数据透视表视图管理器

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`sourceName`, `displayName`, `area`, `subtotal?`, `index?`): `void`

向数据透视表添加字段

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var subtotal = GC.Pivot.SubtotalType.count;
pivotTable.add("Buyer", "Buyer", 1, subtotal, 0) //向透视表行区域中添加一个字段，字段名为displayName
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sourceName` | `string` | 字段的数据源名称 |
| `displayName` | `string` | 字段的显示名称 |
| `area` | `number` | 添加字段的区域索引值 |
| `subtotal?` | [`SubtotalType`](../enums/GC.Pivot.SubtotalType.md) | - |
| `index?` | `number` | - |

#### Returns

`void`

___

### <a id="addcalcfield" name="addcalcfield"></a> addCalcField

▸ **addCalcField**(`fieldName`, `formula`): `void`

添加计算字段，计算字段只能添加到透视表的值区域。

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var pivotTable = sheet.pivotTables.add("myPivotTable", 'sourceData', 1, 1, layout, theme);
pivotTable.addCalcField("PercentOfEach", "=Amount/454");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 计算字段名 |
| `formula` | `string` | 计算公式 |

#### Returns

`void`

___

### <a id="addcalcitem" name="addcalcitem"></a> addCalcItem

▸ **addCalcItem**(`sourceName`, `calcItemName`, `formula`): `void`

添加计算项

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                 ["01-Jan","Mom","Fuel",74],
                 ["15-Jan","Mom","Food",235],
                 ["17-Jan","Dad","Sports",20],
                 ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var pivotTable = sheet.pivotTables.get("pivotTable_1");
pivotTable.add("Buyer","Buyer",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Type","Type",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("Amount","Sum of Amount",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.addCalcItem("Buyer", "formula1", "=Buyer[Mom]+Buyer[Dad]");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sourceName` | `string` | 源字段名称 |
| `calcItemName` | `string` | 源字段的计算项名称 |
| `formula` | `string` | 源字段的计算公式 |

#### Returns

`void`

___

### <a id="addconditionalrule" name="addconditionalrule"></a> addConditionalRule

▸ **addConditionalRule**(`pivotArea`, `conditionalRule`): `void`

在数据透视表中添加规则

**`代码示例`**
``` javascript
// 本示例使用了getRule方法
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
        fieldName: "Country",
        items: ["America"]
    }]
}
var BritainPivotArea = {
    dataOnly: true
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
| `pivotArea` | [`IPivotArea`](../modules/GC.Spread.Pivot.md#ipivotarea)[] | 数据透视表中的区域 |
| `conditionalRule` | [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md) | 数据透视表中添加的规则 |

#### Returns

`void`

___

### <a id="autofitcolumn" name="autofitcolumn"></a> autoFitColumn

▸ **autoFitColumn**(): `void`

为每个字段项设置最小可视列宽

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme);
pivotTable.add("Type", "Type", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Date", "Date", GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("Amount", "Sum of Amount", GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.autoFitColumn();
```

#### Returns

`void`

___

### <a id="clearoverwritelist" name="clearoverwritelist"></a> clearOverwriteList

▸ **clearOverwriteList**(): `void`

清除覆盖信息列表

#### Returns

`void`

___

### <a id="collapse" name="collapse"></a> collapse

▸ **collapse**(`fieldName`, `item`, `isCollapse?`): `boolean` \| `void`

获取或设置透视表字段的折叠信息

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.add("Buyer", "Buyer", 1, subtotal, 0);
pivotTable.add("Type", "Type", 1, subtotal, 1);
var collapseValue = pivotTable.collapse("Buyer","Mom");
pivotTable.collapse("Buyer","Mom", !collapseValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 目标字段名称 |
| `item` | `string` | 折叠项名称 |
| `isCollapse?` | `boolean` | - |

#### Returns

`boolean` \| `void`

是否折叠

___

### <a id="connectslicer" name="connectslicer"></a> connectSlicer

▸ **connectSlicer**(`name`): `void`

绑定切片器

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 切片器名称 |

#### Returns

`void`

___

### <a id="dataposition" name="dataposition"></a> dataPosition

▸ **dataPosition**(`positionType?`, `positionIndex?`): `void` \| [`IDataPosition`](../modules/GC.Pivot.md#idataposition)

获取或设置值的位置

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.dataPosition(1,0) // 将值移动到行区域，索引为0
pivotTable.dataPosition();// {positionType:1,positionIndex:0}
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `positionType?` | [`DataPosition`](../enums/GC.Pivot.DataPosition.md) |
| `positionIndex?` | `number` |

#### Returns

`void` \| [`IDataPosition`](../modules/GC.Pivot.md#idataposition)

返回数据透视表的数据位置信息或空值

___

### <a id="deserialize" name="deserialize"></a> deserialize

▸ **deserialize**(`serializeInfo`): `void`

将序列化的透视表数据还原到现有透视表

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme);
pivotTable.add("Buyer","Buyer",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Type","Type",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("Amount","Sum of Amount",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
var serialization = pivotTable.serialize();
pivotTable.remove('Type');
pivotTable.deserialize(serialization);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `serializeInfo` | [`ISerializeInfo`](../modules/GC.Spread.Pivot.md#iserializeinfo) | 序列化的透视表数据 |

#### Returns

`void`

___

### <a id="disconnectslicer" name="disconnectslicer"></a> disconnectSlicer

▸ **disconnectSlicer**(`name`): `void`

解绑切片器

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |

#### Returns

`void`

___

### <a id="getallslicers" name="getallslicers"></a> getAllSlicers

▸ **getAllSlicers**(): [`PivotTableItemSlicer`](GC.Spread.Pivot.PivotTableItemSlicer.md)[]

获取所有绑定的切片器

#### Returns

[`PivotTableItemSlicer`](GC.Spread.Pivot.PivotTableItemSlicer.md)[]

返回所有与透视表绑定的切片器

___

### <a id="getcalcfields" name="getcalcfields"></a> getCalcFields

▸ **getCalcFields**(): [`ICalcFieldInfo`](../modules/GC.Spread.Pivot.md#icalcfieldinfo)[]

获取所有计算字段的信息

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var pivotTable = sheet.pivotTables.add("pivotTable1", 'sourceData', 1, 1, layout, theme);
pivotTable.addCalcField("PercentOfEach", "=Amount/454");
pivotTable.getCalcFields();
```

#### Returns

[`ICalcFieldInfo`](../modules/GC.Spread.Pivot.md#icalcfieldinfo)[]

返回所有计算字段的信息

___

### <a id="getcalcitems" name="getcalcitems"></a> getCalcItems

▸ **getCalcItems**(`sourceName?`): [`ICalcItemInfo`](../modules/GC.Spread.Pivot.md#icalciteminfo)[]

获取计算项信息

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                 ["01-Jan","Mom","Fuel",74],
                 ["15-Jan","Mom","Food",235],
                 ["17-Jan","Dad","Sports",20],
                 ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var pivotTable = sheet.pivotTables.get("pivotTable_1");
pivotTable.add("Buyer","Buyer",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Type","Type",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("Amount","Sum of Amount",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.addCalcItem("Buyer", "formula1", "=Buyer[Mom]+Buyer[Dad]");
pivotTable.getCalcItems("Buyer");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sourceName?` | `string` | 源字段名称 |

#### Returns

[`ICalcItemInfo`](../modules/GC.Spread.Pivot.md#icalciteminfo)[]

___

### <a id="getconditionalrules" name="getconditionalrules"></a> getConditionalRules

▸ **getConditionalRules**(`pivotArea`): [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)[]

获取使用数据透视区域的规则

**`代码示例`**
``` javascript
// 本示例使用了getRule方法
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
        fieldName: "Country",
        items: ["America"]
    }]
}
var BritainPivotArea = {
    dataOnly: true
    references: [{
        fieldName: "Country",
        items: ["Britain"]
    }]
}
pivotTable.addConditionalRule([AmericaPivotArea, BritainPivotArea], rule);
var ruleTest = pivotTable.getConditionalRules(BritainPivotArea);
alert(ruleTest[0].midValue());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pivotArea` | [`IPivotArea`](../modules/GC.Spread.Pivot.md#ipivotarea) | 数据透视表中的区域 |

#### Returns

[`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)[]

透视区域中的规则

___

### <a id="getfield" name="getfield"></a> getField

▸ **getField**(`fieldName`): [`IFieldInfo`](../modules/GC.Spread.Pivot.md#ifieldinfo)

按字段名从透视表获取字段信息

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.add("Buyer","Buyer",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Type","Type",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("Amount","Sum of Amount",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.getField("Type");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 字段名称 |

#### Returns

[`IFieldInfo`](../modules/GC.Spread.Pivot.md#ifieldinfo)

返回字段信息

___

### <a id="getfieldsbyarea" name="getfieldsbyarea"></a> getFieldsByArea

▸ **getFieldsByArea**(`area?`): [`IFieldInfo`](../modules/GC.Spread.Pivot.md#ifieldinfo)[]

从数据透视表或数据透视表区域获取所有字段信息

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.add("Buyer","Buyer",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Type","Type",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("Amount","Sum of Amount",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.getFieldsByArea(GC.Spread.PivotTableFieldType.columnField);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `area?` | [`PivotTableFieldType`](../enums/GC.Spread.Pivot.PivotTableFieldType.md) |

#### Returns

[`IFieldInfo`](../modules/GC.Spread.Pivot.md#ifieldinfo)[]

返回数据透视表区域中的所有字段信息

___

### <a id="getitemsbyfield" name="getitemsbyfield"></a> getItemsByField

▸ **getItemsByField**(`fieldName`): `any`

按字段名从数据透视表中获取所有项

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 透视表字段的字段名 |

#### Returns

`any`

返回透视表字段的所有项

___

### <a id="getnodeinfo" name="getnodeinfo"></a> getNodeInfo

▸ **getNodeInfo**(`row`, `col`): [`IPivotNodeInfo`](../modules/GC.Spread.Pivot.md#ipivotnodeinfo)

从工作表的行和列组合覆盖信息。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 单元格的行索引 |
| `col` | `number` | 单元格的列索引 |

#### Returns

[`IPivotNodeInfo`](../modules/GC.Spread.Pivot.md#ipivotnodeinfo)

想要获取的节点信息

___

### <a id="getnodevalue" name="getnodevalue"></a> getNodeValue

▸ **getNodeValue**(`nodeInfo`): `number`

通过节点信息获取值

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `nodeInfo` | [`IPivotNodeInfo`](../modules/GC.Spread.Pivot.md#ipivotnodeinfo) | The node info want to get. |

#### Returns

`number`

节点信息的值

___

### <a id="getoverwritelist" name="getoverwritelist"></a> getOverwriteList

▸ **getOverwriteList**(): [`IPivotOverwriteNodeInfo`](../modules/GC.Spread.Pivot.md#ipivotoverwritenodeinfo)[]

获取数据透视缓存的所有覆盖信息

#### Returns

[`IPivotOverwriteNodeInfo`](../modules/GC.Spread.Pivot.md#ipivotoverwritenodeinfo)[]

返回覆盖信息数组

___

### <a id="getpivotarearanges" name="getpivotarearanges"></a> getPivotAreaRanges

▸ **getPivotAreaRanges**(`pivotArea`): [`Range`](GC.Spread.Sheets.Range.md)[]

获取指定数据透视区域对应的工作表区域

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                 ["01-Jan","Mom","Fuel",74],
                 ["15-Jan","Mom","Food",235],
                 ["17-Jan","Dad","Sports",20],
                 ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.add("Buyer", "Buyer", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Type", "Type", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Date", "Date", GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("Amount", "Amount", GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
var pivotArea = {
    dataOnly: false,
    references: [
        {
            fieldName: "Buyer",
            items: ["Mom", "Dad"]
        }
    ]
};
let ranges = pivotTable.getPivotAreaRanges(pivotArea);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pivotArea` | [`IPivotArea`](../modules/GC.Spread.Pivot.md#ipivotarea) | 指定透视表区域 |

#### Returns

[`Range`](GC.Spread.Sheets.Range.md)[]

指定数据透视区域相对应的工作表区域

___

### <a id="getpivotdetails" name="getpivotdetails"></a> getPivotDetails

▸ **getPivotDetails**(`pivotItemInfo`): `void` \| `any`[][]

获取数据透视表详细信息

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                 ["01-Jan","Mom","Fuel",74],
                 ["15-Jan","Mom","Food",235],
                 ["17-Jan","Dad","Sports",20],
                 ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var pivotTable = sheet.pivotTables.get("pivotTable_1");
pivotTable.add("Buyer","Buyer",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Type","Type",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("Amount","Sum of Amount",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.getPivotDetails([{fieldName:"Buyer", fieldItem:"Kelly"}]);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pivotItemInfo` | [`IPivotItemInfo`](../interfaces/GC.Spread.Pivot.IPivotItemInfo.md)[] | 透视详细信息列表 |

#### Returns

`void` \| `any`[][]

___

### <a id="getrange" name="getrange"></a> getRange

▸ **getRange**(): [`IPivotTableRange`](../modules/GC.Spread.Pivot.md#ipivottablerange)

获取数据透视表的范围，包括页面和内容部分。它们是只读的，更改范围不会产生任何效果。

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                 ["01-Jan","Mom","Fuel",74],
                 ["15-Jan","Mom","Food",235],
                 ["17-Jan","Dad","Sports",20],
                 ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var pivotTable = sheet.pivotTables.add("pivotTable1", 'sourceData', 1, 1, layout, theme);
pivotTable.add("Buyer", "Buyer", GC.Spread.Pivot.PivotTableFieldType.filterField);
pivotTable.add("Type", "Type", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Date", "Date", GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("Amount", "Amount", GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
var ranges = pivotTable.getRange();
console.log(ranges.page, ranges.content);
```

#### Returns

[`IPivotTableRange`](../modules/GC.Spread.Pivot.md#ipivottablerange)

返回当前透视表范围

___

### <a id="getsource" name="getsource"></a> getSource

▸ **getSource**(): `string`

获取数据透视表数据引用

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                 ["01-Jan","Mom","Fuel",74],
                 ["15-Jan","Mom","Food",235],
                 ["17-Jan","Dad","Sports",20],
                 ["21-Jan","Kelly","Books",125]];
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

获取数据透视表源字段信息

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                 ["01-Jan","Mom","Fuel",74],
                 ["15-Jan","Mom","Food",235],
                 ["17-Jan","Dad","Sports",20],
                 ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var pivotTable = sheet.pivotTables.get("pivotTable_1");
pivotTable.addCalcField("calcField", "=Amount*2");
pivotTable.getSourceFields();
```

#### Returns

[`ISourceFieldInfo`](../modules/GC.Spread.Pivot.md#isourcefieldinfo)[]

___

### <a id="getstyle" name="getstyle"></a> getStyle

▸ **getStyle**(`pivotArea`): [`Style`](GC.Spread.Sheets.Style.md)

获取特定数据透视区域的样式

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                 ["01-Jan","Mom","Fuel",74],
                 ["15-Jan","Mom","Food",235],
                 ["17-Jan","Dad","Sports",20],
                 ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.add("Buyer", "Buyer", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Type", "Type", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Date", "Date", GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("Amount", "Amount", GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
var pivotArea = {
    dataOnly: false,
    references: [
        {
            fieldName: "Buyer",
            items: ["Mom", "Dad"]
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
| `pivotArea` | [`IPivotArea`](../modules/GC.Spread.Pivot.md#ipivotarea) | 指定透视表区域 |

#### Returns

[`Style`](GC.Spread.Sheets.Style.md)

GC.Spread.Sheets.Style

___

### <a id="getthemename" name="getthemename"></a> getThemeName

▸ **getThemeName**(): `undefined` \| `string`

获取或设置数据透视表的样式名称。

#### Returns

`undefined` \| `string`

返回数据透视表样式名称。

___

### <a id="group" name="group"></a> group

▸ **group**(`groupInfo`): `void`

对字段项进行分组

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["19-Jan","David","Books",120],
                  ["20-Jan","Dad","Food",160],
                  ["21-Jan","David","Sports",15],
                  ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 8, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var groupInfo = {
    originFieldName: "Buyer",
    textGroup: {
        fieldName: "FamilyMembers",
        groupItems: {
             "parent": ["Mom", "Dad"],
             "children": ["David", "Kelly"]
        }
    }
};
pivotTable.group(groupInfo);
pivotTable.add("FamilyMembers", "FamilyMembers", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Buyer", "Buyer", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Amount", "Sum of Amount", GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
sheet.resumePaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `groupInfo` | [`IDateGroupsInfo`](../modules/GC.Spread.Pivot.md#idategroupsinfo) \| [`INumberGroupInfo`](../modules/GC.Spread.Pivot.md#inumbergroupinfo) \| [`ITextGroupInfo`](../modules/GC.Spread.Pivot.md#itextgroupinfo) | 分组信息 |

#### Returns

`void`

___

### <a id="isconnectedslicer" name="isconnectedslicer"></a> isConnectedSlicer

▸ **isConnectedSlicer**(`name`): `boolean`

切片器是否与透视表绑定

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 切片器名称 |

#### Returns

`boolean`

切片器是否与透视表绑定

___

### <a id="labelfilter" name="labelfilter"></a> labelFilter

▸ **labelFilter**(`fieldName`, `filterInfo?`): `void` \| [`IPivotConditionFilterInfo`](../modules/GC.Spread.Pivot.md#ipivotconditionfilterinfo) \| [`IPivotTextFilterInfo`](../modules/GC.Spread.Pivot.md#ipivottextfilterinfo)

获取或设置字段的标签筛选信息

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.suspendLayout();
pivotTable.options.showRowHeader = true;
pivotTable.options.showColumnHeader = true;
pivotTable.add("Buyer", "Buyer", GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("Type", "Type", GC.Spread.Pivot.PivotTableFieldType.rowField);
var condition = { conType: GC.Pivot.PivotConditionType.caption, operator: GC.Pivot.PivotCaptionFilterOperator.contains, val: ["Mom"] };
var filterInfo = { condition };
pivotTable.labelFilter("Buyer", filterInfo);
pivotTable.add("Amount", "Sum of Amount", GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.resumeLayout();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 数据透视表的目标字段名称 |
| `filterInfo?` | ``null`` \| [`IPivotConditionFilterInfo`](../modules/GC.Spread.Pivot.md#ipivotconditionfilterinfo) \| [`IPivotTextFilterInfo`](../modules/GC.Spread.Pivot.md#ipivottextfilterinfo) | - |

#### Returns

`void` \| [`IPivotConditionFilterInfo`](../modules/GC.Spread.Pivot.md#ipivotconditionfilterinfo) \| [`IPivotTextFilterInfo`](../modules/GC.Spread.Pivot.md#ipivottextfilterinfo)

返回数据透视表标签筛选信息

___

### <a id="layouttype" name="layouttype"></a> layoutType

▸ **layoutType**(`type?`): [`PivotTableLayoutType`](../enums/GC.Spread.Pivot.PivotTableLayoutType.md)

获取或设置数据透视表的布局类型

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var pivotTableLayoutType = GC.Spread.Pivot.PivotTableLayoutType.compact;
pivotTable.layoutType(pivotTableLayoutType);
pivotTable.layoutType(); //GC.Spread.Pivot.PivotTableLayoutType.compact
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `type?` | [`PivotTableLayoutType`](../enums/GC.Spread.Pivot.PivotTableLayoutType.md) |

#### Returns

[`PivotTableLayoutType`](../enums/GC.Spread.Pivot.PivotTableLayoutType.md)

如果没有传入参数，则获取当前布局类型

___

### <a id="name" name="name"></a> name

▸ **name**(`name?`): `string` \| `void`

获取或设置数据透视表名称

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
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
| `name?` | `string` | 数据透视表名称 |

#### Returns

`string` \| `void`

___

### <a id="position" name="position"></a> position

▸ **position**(`row?`, `col?`, `sheetName?`): `void` \| [`IPivotTablePosition`](../modules/GC.Spread.Pivot.md#ipivottableposition)

获取或设置数据透视表的起始位置，当有足够单元格放置数据透视表时，其位置会自动更改。

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var toSheet = spread.getSheet(2);
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
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

| Name | Type |
| :------ | :------ |
| `row?` | `number` |
| `col?` | `number` |
| `sheetName?` | `string` |

#### Returns

`void` \| [`IPivotTablePosition`](../modules/GC.Spread.Pivot.md#ipivottableposition)

___

### <a id="refresh" name="refresh"></a> refresh

▸ **refresh**(): `void`

刷新字段布局，重新计算表中的所有字段数据

#### Returns

`void`

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`fieldName`): `void`

按名称删除字段

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.add("Buyer", "Buyer", 1, GC.Pivot.SubtotalType.count, 0);
pivotTable.remove("Buyer");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 将被删除的字段名 |

#### Returns

`void`

___

### <a id="removecalcfield" name="removecalcfield"></a> removeCalcField

▸ **removeCalcField**(`fieldName`): `void`

移除计算字段

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var pivotTable = sheet.pivotTables.add("pivotTable1", 'sourceData', 1, 1, layout, theme);
pivotTable.addCalcField("Amount", "PercentOfEach", "=Amount/454");
var calcFieldsInfo = pivotTable.getCalcFields();
pivotTable.removeCalcField(calcFieldsInfo[i].fieldName);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 计算字段名 |

#### Returns

`void`

___

### <a id="removecalcitem" name="removecalcitem"></a> removeCalcItem

▸ **removeCalcItem**(`sourceName`, `calcItemName`): `void`

移除计算项

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                 ["01-Jan","Mom","Fuel",74],
                 ["15-Jan","Mom","Food",235],
                 ["17-Jan","Dad","Sports",20],
                 ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var pivotTable = sheet.pivotTables.get("pivotTable_1");
pivotTable.add("Buyer","Buyer",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Type","Type",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("Amount","Sum of Amount",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.addCalcItem("Buyer", "formula1", "=Buyer[Mom]+Buyer[Dad]");
pivotTable.removeCalcItem("Buyer", "formula1");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sourceName` | `string` | 源字段名称 |
| `calcItemName` | `string` | 源字段的计算项名称 |

#### Returns

`void`

___

### <a id="removeconditionalrule" name="removeconditionalrule"></a> removeConditionalRule

▸ **removeConditionalRule**(`conditionalRule`): `void`

删除透视表的条件格式

**`代码示例`**
``` javascript
//本示例使用了getRule方法
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
           fieldName: "Country",
           items: ["America"]
       }]
   }
var BritainPivotArea = {
       dataOnly: true
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
| `conditionalRule` | [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md) | 透视表设置的条件格式 |

#### Returns

`void`

___

### <a id="resumelayout" name="resumelayout"></a> resumeLayout

▸ **resumeLayout**(): `void`

停止更新字段, 直至 suspendLayout 结束, 并且必须与 suspendLayout 成对使用。

#### Returns

`void`

___

### <a id="serialize" name="serialize"></a> serialize

▸ **serialize**(): [`ISerializeInfo`](../modules/GC.Spread.Pivot.md#iserializeinfo)

获取序列化的透视表数据

#### Returns

[`ISerializeInfo`](../modules/GC.Spread.Pivot.md#iserializeinfo)

序列化数据透视表数据

___

### <a id="setnodevalue" name="setnodevalue"></a> setNodeValue

▸ **setNodeValue**(`nodeInfo`, `value?`): `void`

将覆盖值设置到数据透视缓存中。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `nodeInfo` | [`IPivotNodeInfo`](../modules/GC.Spread.Pivot.md#ipivotnodeinfo) | 要设置的节点信息 |
| `value?` | `number` | - |

#### Returns

`void`

___

### <a id="setstyle" name="setstyle"></a> setStyle

▸ **setStyle**(`pivotArea`, `style`): `void`

设置或删除特定透视表区域的样式

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                 ["01-Jan","Mom","Fuel",74],
                 ["15-Jan","Mom","Food",235],
                 ["17-Jan","Dad","Sports",20],
                 ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.add("Buyer", "Buyer", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Type", "Type", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Date", "Date", GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("Amount", "Amount", GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
var pivotArea = {
    dataOnly: false,
    references: [
        {
            fieldName: "Buyer",
            items: ["Mom", "Dad"]
        }
    ]
};
var style = new GC.Spread.Sheets.Style();
redBack.backColor = '#ff0000';
pivotTable.setStyle(pivotArea, style);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pivotArea` | [`IPivotArea`](../modules/GC.Spread.Pivot.md#ipivotarea) | 指定透视表区域 |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 设置指定透视区域的样式，参数为null或undefined时可删除指定透视区域的样式 |

#### Returns

`void`

___

### <a id="showdataas" name="showdataas"></a> showDataAs

▸ **showDataAs**(`fieldName`, `showDataAsInfo?`): `void` \| [`IPivotShowDataAsInfo`](../modules/GC.Spread.Pivot.md#ipivotshowdataasinfo)

获取或设置值字段的 显示为 的信息。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 应用 显示为 信息的字段名 |
| `showDataAsInfo?` | [`IPivotShowDataAsInfo`](../modules/GC.Spread.Pivot.md#ipivotshowdataasinfo) | - |

#### Returns

`void` \| [`IPivotShowDataAsInfo`](../modules/GC.Spread.Pivot.md#ipivotshowdataasinfo)

___

### <a id="shownodata" name="shownodata"></a> showNoData

▸ **showNoData**(`cacheFieldName`, `isShow`): `boolean`

设置或获取字段 显示为无数据 的信息

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                 ["01-Jan","Mom","Fuel",74],
                 ["15-Jan","Mom","Food",235],
                 ["17-Jan","Dad","Sports",20],
                 ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var pivotTable = sheet.pivotTables.get("pivotTable_1");
pivotTable.add("Date","Date",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Buyer","Buyer",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Type","Type",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("Amount","Sum of Amount",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.showNoData("Buyer", true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cacheFieldName` | `string` | - |
| `isShow` | `boolean` | 该标志表示是否需要显示没有数据的项 |

#### Returns

`boolean`

___

### <a id="sort" name="sort"></a> sort

▸ **sort**(`fieldName`, `sortInfo`): `void` \| [`IPivotViewSortInfo`](../modules/GC.Pivot.md#ipivotviewsortinfo)

获取或设置透视表的字段排序

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.workbook(document.getElementById("ss"));
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = spread.getSheet(0).pivotTables.add("pivotTable_1",sourceData,1,1,layout,theme,option);
pivotTable.add("Buyer","Buyer",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Type","Type",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("Type", { sortType: GC.Pivot.SortType.asc, sortValueFieldName: "Sum of Amount"});
pivotTable.sort("Buyer", { sortType: GC.Pivot.SortType.asc });
pivotTable.sort("Buyer", { customSortCallback: function(fieldItemNameArray) {
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

获取或设置subtotal的位置信息

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                 ["01-Jan","Mom","Fuel",74],
                 ["15-Jan","Mom","Food",235],
                 ["17-Jan","Dad","Sports",20],
                 ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var pivotTable = sheet.pivotTables.get("pivotTable_1");
pivotTable.add("Date","Date",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Buyer","Buyer",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Type","Type",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("Amount","Sum of Amount",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.subtotalPosition("Buyer", GC.Spread.Pivot.SubtotalsPosition.top);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 字段名称 |
| `position` | [`SubtotalsPosition`](../enums/GC.Spread.Pivot.SubtotalsPosition.md) | 是否设置小计位置，仅支持顶部或底部 |

#### Returns

`void` \| [`SubtotalsPosition`](../enums/GC.Spread.Pivot.SubtotalsPosition.md)

___

### <a id="subtotaltype" name="subtotaltype"></a> subtotalType

▸ **subtotalType**(`fieldName`, `type?`): `void`

获取或设置字段的小计类型

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
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
pivotTable.add("Buyer","Buyer",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Type","Type",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("Amount","Sum of Amount",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
var subtotalType = GC.Pivot.SubtotalType.average;
pivotTable.subtotalType("Buyer", subtotalType) // 将名称字段的小计类型设置为"fieldName"
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 数据透视表的目标字段名称 |
| `type?` | [`SubtotalType`](../enums/GC.Pivot.SubtotalType.md) | 小计类型 |

#### Returns

`void` \| [`SubtotalType`](../enums/GC.Pivot.SubtotalType.md)

___

### <a id="subtotalvisible" name="subtotalvisible"></a> subtotalVisible

▸ **subtotalVisible**(`fieldName`, `isVisible`): `boolean`

设置或获取该字段是否显示小计。

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                 ["01-Jan","Mom","Fuel",74],
                 ["15-Jan","Mom","Food",235],
                 ["17-Jan","Dad","Sports",20],
                 ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var pivotTable = sheet.pivotTables.get("pivotTable_1");
pivotTable.add("Date","Date",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Buyer","Buyer",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Type","Type",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("Amount","Sum of Amount",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.subtotalVisible("Buyer", false);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 字段名称。 |
| `isVisible` | `boolean` | - |

#### Returns

`boolean`

___

### <a id="suspendlayout" name="suspendlayout"></a> suspendLayout

▸ **suspendLayout**(): `void`

停止更新字段直至 resumeFieldsLayout, 必须与 resumeFieldsLayout 成对使用。

#### Returns

`void`

___

### <a id="theme" name="theme"></a> theme

▸ **theme**(`theme?`): `void` \| [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md)

获取或设置数据透视表主题

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.theme("light3");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `theme?` | `string` \| [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md) |

#### Returns

`void` \| [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md)

如果没有传入参数，则获取当前主题。

___

### <a id="ungroup" name="ungroup"></a> ungroup

▸ **ungroup**(`fieldName`): `void`

按字段名称取消对字段的分组

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 3 });
var sheet = spread.getActiveSheet();
sheet.suspendPaint();
var sourceDataArray = [["Date", "Buyer", "Type", "Amount"],
                       ["01-Jan", "Mom", "Fuel", 74],
                       ["15-Jan", "Mom", "Food", 235],
                       ["17-Jan", "Dad", "Sports", 20],
                       ["19-Jan", "David", "Books", 120],
                       ["20-Jan", "Dad", "Food", 160],
                       ["21-Jan", "David", "Sports", 15],
                       ["21-Jan", "Kelly", "Books", 125]];
sheet.setArray(3, 0, sourceDataArray);
sheet.tables.add('Table1', 3, 0, 8, 4);
sheet.setColumnWidth(6, 130);
sheet.setColumnWidth(8, 100);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("PivotTable1", 'Table1', 3, 6, layout, theme, option);
var groupInfo = {
    originFieldName: "Buyer",
    textGroup: {
        "parent": ["Mom", "Dad"],
        "children": ["David", "Kelly"]
    }
};
pivotTable.group("FamilyMembers", groupInfo);
pivotTable.add("FamilyMembers", "FamilyMembers", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Buyer", "Buyer", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Amount", "Sum of Amount", GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
sheet.resumePaint();

pivotTable.ungroup("FamilyMembers");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 取消分组的字段名称 |

#### Returns

`void`

___

### <a id="updatecalcitem" name="updatecalcitem"></a> updateCalcItem

▸ **updateCalcItem**(`sourceName`, `calcItemName`, `formula`, `priority`): `void`

更新计算项

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                 ["01-Jan","Mom","Fuel",74],
                 ["15-Jan","Mom","Food",235],
                 ["17-Jan","Dad","Sports",20],
                 ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var pivotTable = sheet.pivotTables.get("pivotTable_1");
pivotTable.add("Buyer","Buyer",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Type","Type",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("Amount","Sum of Amount",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.addCalcItem("Buyer", "formula1", "=Buyer[Mom]+Buyer[Dad]");
pivotTable.updateCalcItem("Buyer", "formula1", "=Buyer[Mom]+Buyer[Kelly]", 1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sourceName` | `string` | 源字段名称 |
| `calcItemName` | `string` | 源字段的计算项名称 |
| `formula` | `string` | 此计算项的新公式 |
| `priority` | `number` | 此计算项的新优先级 |

#### Returns

`void`

___

### <a id="updatefield" name="updatefield"></a> updateField

▸ **updateField**(`name`, `area`, `index?`): `void`

更新字段区域和索引

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.add("Buyer","Buyer",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Type","Type",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("Amount","Sum of Amount",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
pivotTable.updateField("Buyer", GC.Spread.Pivot.PivotTableFieldType.columnField, 0) // 将名称为“Buyer”的字段移动到列区域，字段索引为 2。
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 字段名称 |
| `area` | [`PivotTableFieldType`](../enums/GC.Spread.Pivot.PivotTableFieldType.md) | 放置字段的区域 |
| `index?` | `number` | - |

#### Returns

`void`

___

### <a id="updatefieldname" name="updatefieldname"></a> updateFieldName

▸ **updateFieldName**(`oldName`, `newName`): `void`

更新现有字段名

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.add("Buyer","Buyer",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.updateFieldName("Buyer", "newBuyer")
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

▸ **updateSource**(): `void`

刷新数据透视表数据源

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                 ["01-Jan","Mom","Fuel",74],
                 ["15-Jan","Mom","Food",235],
                 ["17-Jan","Dad","Sports",20],
                 ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var pivotTable = sheet.pivotTables.get("pivotTable_1");
pivotTable.add("Buyer","Buyer",GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Type","Type",GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("Amount","Sum of Amount",GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
sourceSheet.setValue(1,3,1000);
pivotTable.updateSource();
var newSourceData = [["Salesman","ProductType","Product","Sales"],
                 ["SunLin","Drinks","Apple Juice",74],
                 ["JinShiPeng","Drinks","Milk",235],
                 ["ZhangShang","Dessert","Chocolate",20],
                 ["SunYang","Dessert","Beef Jerky",125]];
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

获取或设置字段的值筛选信息

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.suspendLayout();
pivotTable.options.showRowHeader = true;
pivotTable.options.showColumnHeader = true;
pivotTable.add("Buyer", "Buyer", GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("Type", "Type", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Amount", "Sum of Amount", GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
let condition = { conType: GC.Pivot.PivotConditionType.value, operator: GC.Pivot.PivotValueFilterOperator.between, val: [0, 100] };
let filterInfo = { condition: condition, conditionByName: "Sum of Amount" };
pivotTable.valueFilter("Buyer", filterInfo);
pivotTable.resumeLayout();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fieldName` | `string` | 数据透视表的目标字段名称 |
| `filterInfo?` | ``null`` \| [`IPivotConditionFilterInfo`](../modules/GC.Spread.Pivot.md#ipivotconditionfilterinfo) | - |

#### Returns

`void` \| [`IPivotConditionFilterInfo`](../modules/GC.Spread.Pivot.md#ipivotconditionfilterinfo)

返回透视表值信息
