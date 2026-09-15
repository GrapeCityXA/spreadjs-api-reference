# Class: PivotTableManager

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).PivotTableManager

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.PivotTableManager.md#constructor)

### Methods

- [add](GC.Spread.Sheets.PivotTableManager.md#add)
- [all](GC.Spread.Sheets.PivotTableManager.md#all)
- [findPivotTable](GC.Spread.Sheets.PivotTableManager.md#findpivottable)
- [get](GC.Spread.Sheets.PivotTableManager.md#get)
- [getRangePivotAreas](GC.Spread.Sheets.PivotTableManager.md#getrangepivotareas)
- [remove](GC.Spread.Sheets.PivotTableManager.md#remove)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new PivotTableManager**(`sheet`)

透视表管理器

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheet` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 表单 |

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`name`, `sourceData`, `row`, `col`, `layout?`, `theme?`, `options?`): [`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)

**`description`** Add a pivot table to current worksheet.

**`代码示例`**
```
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
sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 透视表名称，它在整个工作簿中应该是唯一的 |
| `sourceData` | `string` \| `any`[][] | 用于透视表的数据源。它支持三种类型：表名、透视表名或绝对引用范围的公式 |
| `row` | `number` | 透视表起始行位置 |
| `col` | `number` | 透视表起始列位置 |
| `layout?` | [`PivotTableLayoutType`](../enums/GC.Spread.Pivot.PivotTableLayoutType.md) | 透视表布局类型 |
| `theme?` | [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md) | 透视表主题样式 |
| `options?` | [`IPivotTableOption`](../modules/GC.Spread.Pivot.md#ipivottableoption) |  透视表的选项. |

#### Returns

[`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)

透视表实例

___

### <a id="all" name="all"></a> all

▸ **all**(): [`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)[]

**`description`** 获取当前工作表中的所有透视表

**`代码示例`**
```
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
var pivotTables = pivotTableManager.all();
console.log(pivotTables);
```

#### Returns

[`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)[]

返回当前工作表中的所有透视表

___

### <a id="findpivottable" name="findpivottable"></a> findPivotTable

▸ **findPivotTable**(`r`, `c`): [`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)

**`description`** 按单元格位置获取数据透视表

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `r` | `number` | 单元格行索引 |
| `c` | `number` | 单元格列索引 |

#### Returns

[`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)

返回透视表实例

___

### <a id="get" name="get"></a> get

▸ **get**(`name`): [`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)

**`description`** 按名称获取数据透视表

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 数据透视表名称 |

#### Returns

[`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)

返回透视表实例

___

### <a id="getrangepivotareas" name="getrangepivotareas"></a> getRangePivotAreas

▸ **getRangePivotAreas**(`range`): [`IPivotAreasCollection`](../modules/GC.Spread.Pivot.md#ipivotareascollection)

**`description`** 按指定的表单范围获取透视表区域

**`代码示例`**
```
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
var myPivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme);
myPivotTable.add("Buyer", "Buyer", GC.Spread.Pivot.PivotTableFieldType.rowField);
myPivotTable.add("Type", "Type", GC.Spread.Pivot.PivotTableFieldType.columnField)
myPivotTable.add("Amount", "Sum of Amount", GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
var pivotAreas = sheet.pivotTables.getRangePivotAreas(new GC.Spread.Sheets.Range(3, 2, 2, 2))[myPivotTable.name()];
var style = new GC.Spread.Sheets.Style();
style.backColor = 'red';
myPivotTable.setStyle(pivotAreas[0], style);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](GC.Spread.Sheets.Range.md) | 表单区域 |

#### Returns

[`IPivotAreasCollection`](../modules/GC.Spread.Pivot.md#ipivotareascollection)

包含所有数据透视表的区域

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`name`): `any`

**`description`** 从表单中删除数据透视表

**`代码示例`**
```
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
sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme);
sheet.pivotTables.remove("pivotTable_1");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 数据透视表名称 |

#### Returns

`any`
