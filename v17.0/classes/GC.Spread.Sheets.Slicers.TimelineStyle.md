# Class: TimelineStyle

[Sheets](../modules/GC.Spread.Sheets.md).[Slicers](../modules/GC.Spread.Sheets.Slicers.md).TimelineStyle

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Slicers.TimelineStyle.md#constructor)

### Methods

- [headerStyle](GC.Spread.Sheets.Slicers.TimelineStyle.md#headerstyle)
- [name](GC.Spread.Sheets.Slicers.TimelineStyle.md#name)
- [periodLabel1Style](GC.Spread.Sheets.Slicers.TimelineStyle.md#periodlabel1style)
- [periodLabel2Style](GC.Spread.Sheets.Slicers.TimelineStyle.md#periodlabel2style)
- [selectedTimeBlockSpaceStyle](GC.Spread.Sheets.Slicers.TimelineStyle.md#selectedtimeblockspacestyle)
- [selectedTimeBlockStyle](GC.Spread.Sheets.Slicers.TimelineStyle.md#selectedtimeblockstyle)
- [selectionLabelStyle](GC.Spread.Sheets.Slicers.TimelineStyle.md#selectionlabelstyle)
- [timeLevelStyle](GC.Spread.Sheets.Slicers.TimelineStyle.md#timelevelstyle)
- [unselectedTimeBlockStyle](GC.Spread.Sheets.Slicers.TimelineStyle.md#unselectedtimeblockstyle)
- [wholeSlicerStyle](GC.Spread.Sheets.Slicers.TimelineStyle.md#wholeslicerstyle)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new TimelineStyle**()

时间线样式设置

## Methods

### <a id="headerstyle" name="headerstyle"></a> headerStyle

▸ **headerStyle**(`value?`): `any`

获取或设置切片器头部的样式

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", new Date("1968/6/8"), "80", "180"],
    ["4", "NewYork", new Date("1972/7/3"), "72", "168"],
    ["4", "NewYork", new Date("1964/3/2"), "71", "179"],
    ["5", "Washington", new Date("1972/8/8"),"80", "171"],
    ["6", "Washington", new Date("1986/2/2"), "89", "161"],
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var pivotTable = sheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
var timeline = sheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);

var style = new GC.Spread.Sheets.Slicers.TimelineStyle()
style.wholeSlicerStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('red', 'blue', '12pt Calibri'));
style.headerStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo(undefined, 'green', '14pt Calibri'));
style.timeLevelStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('yellow'));

timeline.style(style);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) |

#### Returns

`any`

如果未设置任何值，则返回切片器头部的样式；否则，返回切片器样式

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置样式的名称

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置任何值，则返回样式的名称；否则，返回切片器样式

___

### <a id="periodlabel1style" name="periodlabel1style"></a> periodLabel1Style

▸ **periodLabel1Style**(`value?`): `any`

获取或设置时间线周期标签1的样式

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", new Date("1968/6/8"), "80", "180"],
    ["4", "NewYork", new Date("1972/7/3"), "72", "168"],
    ["4", "NewYork", new Date("1964/3/2"), "71", "179"],
    ["5", "Washington", new Date("1972/8/8"),"80", "171"],
    ["6", "Washington", new Date("1986/2/2"), "89", "161"],
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var pivotTable = sheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
var timeline = sheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);

var style = new GC.Spread.Sheets.Slicers.TimelineStyle()
style.periodLabel1Style(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('red', 'blue', '12pt Calibri'));

timeline.style(style);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) |

#### Returns

`any`

如果未设置值，则返回时间线周期标签1样式；否则，返回切片器样式

___

### <a id="periodlabel2style" name="periodlabel2style"></a> periodLabel2Style

▸ **periodLabel2Style**(`value?`): `any`

获取或设置时间线周期标签2的样式

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", new Date("1968/6/8"), "80", "180"],
    ["4", "NewYork", new Date("1972/7/3"), "72", "168"],
    ["4", "NewYork", new Date("1964/3/2"), "71", "179"],
    ["5", "Washington", new Date("1972/8/8"),"80", "171"],
    ["6", "Washington", new Date("1986/2/2"), "89", "161"],
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var pivotTable = sheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
var timeline = sheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);

var style = new GC.Spread.Sheets.Slicers.TimelineStyle()
style.periodLabel2Style(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('red', 'blue', '12pt Calibri'));

timeline.style(style);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) |

#### Returns

`any`

如果未设置值，则返回时间线周期标签2样式；否则，返回切片器样式

___

### <a id="selectedtimeblockspacestyle" name="selectedtimeblockspacestyle"></a> selectedTimeBlockSpaceStyle

▸ **selectedTimeBlockSpaceStyle**(`value?`): `any`

获取或设置所选时间线块空间的样式

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", new Date("1968/6/8"), "80", "180"],
    ["4", "NewYork", new Date("1972/7/3"), "72", "168"],
    ["4", "NewYork", new Date("1964/3/2"), "71", "179"],
    ["5", "Washington", new Date("1972/8/8"),"80", "171"],
    ["6", "Washington", new Date("1986/2/2"), "89", "161"],
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var pivotTable = sheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
var timeline = sheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);

var style = new GC.Spread.Sheets.Slicers.TimelineStyle()
style.selectedTimeBlockSpaceStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('red', 'blue', '12pt Calibri'));

timeline.style(style);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) |

#### Returns

`any`

如果未设置值，则返回时间线块空间的样式；否则，返回切片器样式

___

### <a id="selectedtimeblockstyle" name="selectedtimeblockstyle"></a> selectedTimeBlockStyle

▸ **selectedTimeBlockStyle**(`value?`): `any`

获取或设置选定时间块的样式

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", new Date("1968/6/8"), "80", "180"],
    ["4", "NewYork", new Date("1972/7/3"), "72", "168"],
    ["4", "NewYork", new Date("1964/3/2"), "71", "179"],
    ["5", "Washington", new Date("1972/8/8"),"80", "171"],
    ["6", "Washington", new Date("1986/2/2"), "89", "161"],
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var pivotTable = sheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
var timeline = sheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);

var style = new GC.Spread.Sheets.Slicers.TimelineStyle()
style.periodLabel2Style(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('red', 'blue', '12pt Calibri'));

timeline.style(style);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) |

#### Returns

`any`

如果未设置值，则返回时间线块的样式；否则，返回切片器样式

___

### <a id="selectionlabelstyle" name="selectionlabelstyle"></a> selectionLabelStyle

▸ **selectionLabelStyle**(`value?`): `any`

获取或设置时间线选择标签的样式

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", new Date("1968/6/8"), "80", "180"],
    ["4", "NewYork", new Date("1972/7/3"), "72", "168"],
    ["4", "NewYork", new Date("1964/3/2"), "71", "179"],
    ["5", "Washington", new Date("1972/8/8"),"80", "171"],
    ["6", "Washington", new Date("1986/2/2"), "89", "161"],
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var pivotTable = sheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
var timeline = sheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);

var style = new GC.Spread.Sheets.Slicers.TimelineStyle()
style.selectionLabelStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('red', 'blue', '12pt Calibri'));

timeline.style(style);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) |

#### Returns

`any`

如果未设置值，则返回时间线选择标签的样式；否则，返回切片器样式

___

### <a id="timelevelstyle" name="timelevelstyle"></a> timeLevelStyle

▸ **timeLevelStyle**(`value?`): `any`

获取或设置时间级别的样式

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", new Date("1968/6/8"), "80", "180"],
    ["4", "NewYork", new Date("1972/7/3"), "72", "168"],
    ["4", "NewYork", new Date("1964/3/2"), "71", "179"],
    ["5", "Washington", new Date("1972/8/8"),"80", "171"],
    ["6", "Washington", new Date("1986/2/2"), "89", "161"],
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var pivotTable = sheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
var timeline = sheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);

var style = new GC.Spread.Sheets.Slicers.TimelineStyle()
style.timeLevelStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('red', 'blue', '12pt Calibri'));

timeline.style(style);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) |

#### Returns

`any`

如果未设置值，则返回时间级别的样式；否则，返回切片器样式

___

### <a id="unselectedtimeblockstyle" name="unselectedtimeblockstyle"></a> unselectedTimeBlockStyle

▸ **unselectedTimeBlockStyle**(`value?`): `any`

获取或设置未选时间块的样式

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", new Date("1968/6/8"), "80", "180"],
    ["4", "NewYork", new Date("1972/7/3"), "72", "168"],
    ["4", "NewYork", new Date("1964/3/2"), "71", "179"],
    ["5", "Washington", new Date("1972/8/8"),"80", "171"],
    ["6", "Washington", new Date("1986/2/2"), "89", "161"],
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var pivotTable = sheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
var timeline = sheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);

var style = new GC.Spread.Sheets.Slicers.TimelineStyle()
style.unselectedTimeBlockStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('red', 'blue', '12pt Calibri'));

timeline.style(style);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) |

#### Returns

`any`

如果未设置值，则返回未选时间块的样式；否则，返回切片器样式

___

### <a id="wholeslicerstyle" name="wholeslicerstyle"></a> wholeSlicerStyle

▸ **wholeSlicerStyle**(`value?`): `any`

获取或设置整个切片器的样式

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", new Date("1968/6/8"), "80", "180"],
    ["4", "NewYork", new Date("1972/7/3"), "72", "168"],
    ["4", "NewYork", new Date("1964/3/2"), "71", "179"],
    ["5", "Washington", new Date("1972/8/8"),"80", "171"],
    ["6", "Washington", new Date("1986/2/2"), "89", "161"],
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var pivotTable = sheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
var timeline = sheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);

var style = new GC.Spread.Sheets.Slicers.TimelineStyle()
style.wholeSlicerStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('red', 'blue', '12pt Calibri'));
style.headerStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo(undefined, 'green', '14pt Calibri'));
style.timeLevelStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('yellow'));

timeline.style(style);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) |

#### Returns

`any`

如果未设置任何值，则返回整个切片器的样式；否则，返回切片器样式
