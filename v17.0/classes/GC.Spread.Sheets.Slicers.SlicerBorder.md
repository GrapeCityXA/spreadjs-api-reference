# Class: SlicerBorder

[Sheets](../modules/GC.Spread.Sheets.md).[Slicers](../modules/GC.Spread.Sheets.Slicers.md).SlicerBorder

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Slicers.SlicerBorder.md#constructor)

### Methods

- [borderColor](GC.Spread.Sheets.Slicers.SlicerBorder.md#bordercolor)
- [borderStyle](GC.Spread.Sheets.Slicers.SlicerBorder.md#borderstyle)
- [borderWidth](GC.Spread.Sheets.Slicers.SlicerBorder.md#borderwidth)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new SlicerBorder**(`borderWidth`, `borderStyle`, `borderColor`)

切片器边框

**`代码示例`**
```
//本示例设置边框样式
//create a table
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
//样式信息
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.backColor("red");
hstyle.borderBottom(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green"));
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredSelectedItemWithDataStyle(hstyle);
//向表单添加一个切片器并返回切片器实例
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
//改变切片器的属性
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `borderWidth` | `number` | 边框宽度 |
| `borderStyle` | `string` | 边框样式 |
| `borderColor` | `string` | 边框颜色 |

## Methods

### <a id="bordercolor" name="bordercolor"></a> borderColor

▸ **borderColor**(`value?`): `any`

获取或设置边框颜色

**`example`**
```
//create a table
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
//style info
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
var border = new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green");

console.log(border.borderWidth()); // green
border.borderWidth('red');
console.log(border.borderWidth()); // red

hstyle.borderBottom(border);
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredSelectedItemWithDataStyle(hstyle);
//add a slicer to the sheet and return the slicer instance.
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
slicer.style(style1);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置任何值，则返回边框颜色 否则，返回切片器边框

___

### <a id="borderstyle" name="borderstyle"></a> borderStyle

▸ **borderStyle**(`value?`): `any`

获取或设置边框样式

**`example`**
```
//create a table
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
//style info
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
var border = new GC.Spread.Sheets.Slicers.SlicerBorder(3, 'dashed', "green");

console.log(border.borderStyle()); // 'dashed'
border.borderStyle('mediumDashDot');
console.log(border.borderStyle()); // 'mediumDashDot'

hstyle.borderBottom(border);
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredSelectedItemWithDataStyle(hstyle);
//add a slicer to the sheet and return the slicer instance.
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
slicer.style(style1);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置任何值，则返回边框样式 否则，返回切片器边框

___

### <a id="borderwidth" name="borderwidth"></a> borderWidth

▸ **borderWidth**(`value?`): `any`

获取或设置边框宽度

**`example`**
```
//create a table
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
//style info
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
var border = new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green");

console.log(border.borderWidth()); // 3
border.borderWidth(5);
console.log(border.borderWidth()); // 5

hstyle.borderBottom(border);
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredSelectedItemWithDataStyle(hstyle);
//add a slicer to the sheet and return the slicer instance.
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
slicer.style(style1);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置任何值，则返回边框宽度 否则，返回切片器边框
