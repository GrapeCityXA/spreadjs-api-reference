# Class: TimelineStyle

[Sheets](../modules/GC.Spread.Sheets.md).[Slicers](../modules/GC.Spread.Sheets.Slicers.md).TimelineStyle

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Slicers.TimelineStyle.md#constructor)

### Methods

- [fromJSON](GC.Spread.Sheets.Slicers.TimelineStyle.md#fromjson)
- [headerStyle](GC.Spread.Sheets.Slicers.TimelineStyle.md#headerstyle)
- [name](GC.Spread.Sheets.Slicers.TimelineStyle.md#name)
- [periodLabel1Style](GC.Spread.Sheets.Slicers.TimelineStyle.md#periodlabel1style)
- [periodLabel2Style](GC.Spread.Sheets.Slicers.TimelineStyle.md#periodlabel2style)
- [selectedTimeBlockSpaceStyle](GC.Spread.Sheets.Slicers.TimelineStyle.md#selectedtimeblockspacestyle)
- [selectedTimeBlockStyle](GC.Spread.Sheets.Slicers.TimelineStyle.md#selectedtimeblockstyle)
- [selectionLabelStyle](GC.Spread.Sheets.Slicers.TimelineStyle.md#selectionlabelstyle)
- [timeLevelStyle](GC.Spread.Sheets.Slicers.TimelineStyle.md#timelevelstyle)
- [toJSON](GC.Spread.Sheets.Slicers.TimelineStyle.md#tojson)
- [unselectedTimeBlockStyle](GC.Spread.Sheets.Slicers.TimelineStyle.md#unselectedtimeblockstyle)
- [wholeSlicerStyle](GC.Spread.Sheets.Slicers.TimelineStyle.md#wholeslicerstyle)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new TimelineStyle**()

Represents the timeline style settings.

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", new Date("1968/6/8")],
    ["4", "NewYork", new Date("1972/7/3")],
    ["4", "NewYork", new Date("1964/3/2")]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);

var pivotTable = sheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
var timeline = sheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);

var style = new GC.Spread.Sheets.Slicers.TimelineStyle()
style.wholeSlicerStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('red', 'blue', '12pt Calibri'));
style.headerStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo(undefined, 'green', '14pt Calibri'));
style.timeLevelStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('yellow'));

timeline.style(style);
```

## Methods

### <a id="fromjson" name="fromjson"></a> fromJSON

▸ **fromJSON**(`data`): `void`

Loads the object state from the specified JSON string.

**`example`**
```
//This example uses the fromJSON method.
const light1 = GC.Spread.Sheets.Slicers.TimelineStyles.light1();
// 导出
const jsonStr = JSON.stringify(light1.toJSON());
// 导入
const newTheme = new GC.Spread.Sheets.Slicers.TimelineStyle();
newTheme.fromJSON(JSON.parse(jsonStr));
newTheme.name('custom1');
alert(jsonStr);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `Object` | The timeline slicer theme data from deserialization. |

#### Returns

`void`

___

### <a id="headerstyle" name="headerstyle"></a> headerStyle

▸ **headerStyle**(`value?`): `any`

Gets or sets the style of the slicer header.

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

If no value is set, returns the style of the slicer header; otherwise, returns the slicer style.

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

Gets or sets the name of the style.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

If no value is set, returns the name of the style; otherwise, returns the slicer style.

___

### <a id="periodlabel1style" name="periodlabel1style"></a> periodLabel1Style

▸ **periodLabel1Style**(`value?`): `any`

Gets or sets the style of the timeline period label 1.

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

If no value is set, returns the style of the timeline period label 1; otherwise, returns the slicer style.

___

### <a id="periodlabel2style" name="periodlabel2style"></a> periodLabel2Style

▸ **periodLabel2Style**(`value?`): `any`

Gets or sets the style of the timeline period label 2.

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

If no value is set, returns the style of the timeline period label 2; otherwise, returns the slicer style.

___

### <a id="selectedtimeblockspacestyle" name="selectedtimeblockspacestyle"></a> selectedTimeBlockSpaceStyle

▸ **selectedTimeBlockSpaceStyle**(`value?`): `any`

Gets or sets the style of the timeline selected time block space.

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

If no value is set, returns the style of the timeline selected time block space; otherwise, returns the slicer style.

___

### <a id="selectedtimeblockstyle" name="selectedtimeblockstyle"></a> selectedTimeBlockStyle

▸ **selectedTimeBlockStyle**(`value?`): `any`

Gets or sets the style of the selected time block.

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

If no value is set, returns the style of the selected time block; otherwise, returns the slicer style.

___

### <a id="selectionlabelstyle" name="selectionlabelstyle"></a> selectionLabelStyle

▸ **selectionLabelStyle**(`value?`): `any`

Gets or sets the style of the timeline selection label.

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

If no value is set, returns the style of the timeline selection label; otherwise, returns the slicer style.

___

### <a id="timelevelstyle" name="timelevelstyle"></a> timeLevelStyle

▸ **timeLevelStyle**(`value?`): `any`

Gets or sets the style of the timeline time level.

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

If no value is set, returns the style of the timeline time level; otherwise, returns the slicer style.

___

### <a id="tojson" name="tojson"></a> toJSON

▸ **toJSON**(): `Object`

Saves the object state to a JSON string.

**`example`**
```
//This example uses the toJSON method.
const light1 = GC.Spread.Sheets.Slicers.TimelineStyles.light1();
// 导出
const jsonStr = JSON.stringify(light1.toJSON());
// 导入
const newTheme = new GC.Spread.Sheets.Slicers.TimelineStyle();
newTheme.fromJSON(JSON.parse(jsonStr));
newTheme.name('custom1');
alert(jsonStr);
```

#### Returns

`Object`

The timeline slicer theme data.

___

### <a id="unselectedtimeblockstyle" name="unselectedtimeblockstyle"></a> unselectedTimeBlockStyle

▸ **unselectedTimeBlockStyle**(`value?`): `any`

Gets or sets the style of the unselected time block.

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

If no value is set, returns the style of the unselected time block; otherwise, returns the slicer style.

___

### <a id="wholeslicerstyle" name="wholeslicerstyle"></a> wholeSlicerStyle

▸ **wholeSlicerStyle**(`value?`): `any`

Gets or sets the style of the whole slicer.

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

If no value is set, returns the style of the whole slicer; otherwise, returns the slicer style.
