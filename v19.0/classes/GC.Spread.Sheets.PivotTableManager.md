# Class: PivotTableManager

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).PivotTableManager

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.PivotTableManager.md#constructor)

### Methods

- [add](GC.Spread.Sheets.PivotTableManager.md#add)
- [all](GC.Spread.Sheets.PivotTableManager.md#all)
- [customList](GC.Spread.Sheets.PivotTableManager.md#customlist)
- [findPivotTable](GC.Spread.Sheets.PivotTableManager.md#findpivottable)
- [get](GC.Spread.Sheets.PivotTableManager.md#get)
- [getRangePivotAreas](GC.Spread.Sheets.PivotTableManager.md#getrangepivotareas)
- [remove](GC.Spread.Sheets.PivotTableManager.md#remove)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new PivotTableManager**(`sheet`)

表示一个数据透视表管理器，可以管理工作表中的所有数据透视表。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheet` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 工作表。 |

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`name`, `sourceData`, `row`, `col`, `layout?`, `theme?`, `options?`): [`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)

**`description`** 向当前工作表添加数据透视表。

**`example`**
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
| `name` | `string` | 数据透视表名称，在整个工作簿中应该是唯一的。 |
| `sourceData` | `string` | 用于数据透视表的源数据。支持三种类型：表名、集算表名或绝对引用范围的公式。 |
| `row` | `number` | 数据透视表的起始行位置。 |
| `col` | `number` | 数据透视表的起始列位置。 |
| `layout?` | [`PivotTableLayoutType`](../enums/GC.Spread.Pivot.PivotTableLayoutType.md) | 数据透视表布局。 |
| `theme?` | `string` \| [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md) | 数据透视表主题样式名称。 |
| `options?` | [`IPivotTableOption`](../modules/GC.Spread.Pivot.md#ipivottableoption) | 数据透视表选项。 |

#### Returns

[`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)

新的数据透视表实例。

___

### <a id="all" name="all"></a> all

▸ **all**(): [`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)[]

**`description`** 获取当前工作表中的所有数据透视表。

**`example`**
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

返回当前工作表中的所有数据透视表。

___

### <a id="customlist" name="customlist"></a> customList

▸ **customList**(`customList?`): `void` \| `string`[]

**`description`** 获取或设置一个自定义排序列表。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `customList?` | `string`[] | 设置一个自定义排序列表。 |

#### Returns

`void` \| `string`[]

返回自定义排序列表。

___

### <a id="findpivottable" name="findpivottable"></a> findPivotTable

▸ **findPivotTable**(`r`, `c`): [`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)

**`description`** 通过单元格位置获取数据透视表。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `r` | `number` | 单元格行索引。 |
| `c` | `number` | 单元格列索引。 |

#### Returns

[`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)

返回数据透视表实例。

___

### <a id="get" name="get"></a> get

▸ **get**(`name`): [`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)

**`description`** 通过名称获取数据透视表。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 数据透视表名称。 |

#### Returns

[`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)

返回数据透视表实例。

___

### <a id="getrangepivotareas" name="getrangepivotareas"></a> getRangePivotAreas

▸ **getRangePivotAreas**(`range`): [`IPivotAreasCollection`](../modules/GC.Spread.Pivot.md#ipivotareascollection)

**`description`** 通过指定的工作表范围获取数据透视表区域。

**`example`**
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
| `range` | [`Range`](GC.Spread.Sheets.Range.md) | 工作表范围。 |

#### Returns

[`IPivotAreasCollection`](../modules/GC.Spread.Pivot.md#ipivotareascollection)

包含在范围内的所有数据透视表区域。

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`name`): `any`

**`description`** 从工作表中删除数据透视表。

**`example`**
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
| `name` | `string` | 数据透视表名称。 |

#### Returns

`any`
