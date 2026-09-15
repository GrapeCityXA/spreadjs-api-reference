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

表示时间线（Timeline）的样式配置。

**`example`**
```javascript
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
var style = new GC.Spread.Sheets.Slicers.TimelineStyle();
style.wholeSlicerStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('red', 'blue', '12pt Calibri'));
style.headerStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('yellow', 'green', '14pt Calibri'));
style.timeLevelStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo(undefined, 'white', '14pt Calibri'));
timeline.style(style);
```

## Methods

### <a id="fromjson" name="fromjson"></a> fromJSON

▸ **fromJSON**(`data`): `void`

从指定的 JSON 数据中加载对象状态（实现反序列化）。

**`example`**
```javascript
// 此示例使用 fromJSON 方法。
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
| `data` | `Object` | 用于反序列化的时间线切片器主题数据。 |

#### Returns

`void`

___

### <a id="headerstyle" name="headerstyle"></a> headerStyle

▸ **headerStyle**(`value?`): `any`

获取或设置切片器头部的样式，包括颜色、字体和边框等属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", new Date("1968/6/8"), "80", "180"],
    ["4", "NewYork", new Date("1972/7/3"), "72", "168"],
    ["4", "NewYork", new Date("1964/3/2"), "71", "179"],
    ["5", "Washington", new Date("1972/8/8"),"80", "171"],
    ["6", "Washington", new Date("1986/2/2"), "89", "161"],
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]
];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var pivotTable = sheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
var timeline = sheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var style = new GC.Spread.Sheets.Slicers.TimelineStyle();
style.headerStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('yellow', 'green', '14pt Calibri'));
timeline.style(style);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) | 可选参数。切片器头部的样式配置对象。 |

#### Returns

`any`

- 如果未设置值，则返回当前切片器头部的样式；否则返回当前切片器样式对象。

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置该时间线样式的名称。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", new Date("1968/6/8"), "80", "180"],
    ["4", "NewYork", new Date("1972/7/3"), "72", "168"],
    ["4", "NewYork", new Date("1964/3/2"), "71", "179"],
    ["5", "Washington", new Date("1972/8/8"),"80", "171"],
    ["6", "Washington", new Date("1986/2/2"), "89", "161"],
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]
];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
var pivotTable = sheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
var timeline = sheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
console.log(timeline.name()); // 'timeline1'
timeline.name("birthday");
console.log(timeline.name()); // 'birthday'
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 可选参数。时间线切片器样式的名称。 |

#### Returns

`any`

- 如果未设置参数值，则返回当前时间线样式的名称；否则返回当前时间线切片器样式对象本身。

___

### <a id="periodlabel1style" name="periodlabel1style"></a> periodLabel1Style

▸ **periodLabel1Style**(`value?`): `any`

获取或设置时间线周期标签1的样式（仅支持配置字体相关样式）。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", new Date("1968/6/8"), "80", "180"],
    ["4", "NewYork", new Date("1972/7/3"), "72", "168"],
    ["4", "NewYork", new Date("1964/3/2"), "71", "179"],
    ["5", "Washington", new Date("1972/8/8"),"80", "171"],
    ["6", "Washington", new Date("1986/2/2"), "89", "161"],
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]
];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var pivotTable = sheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
var timeline = sheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var style = new GC.Spread.Sheets.Slicers.TimelineStyle();
style.periodLabel1Style(new GC.Spread.Sheets.Slicers.SlicerStyleInfo(undefined, 'blue', '12pt Calibri'));
timeline.style(style);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) | 可选参数。时间线周期标签1的样式配置对象。 |

#### Returns

`any`

- 如果未设置参数值，则返回当前时间线周期标签1的样式；否则返回当前时间线切片器样式对象本身。

___

### <a id="periodlabel2style" name="periodlabel2style"></a> periodLabel2Style

▸ **periodLabel2Style**(`value?`): `any`

获取或设置时间线周期标签2的样式（仅支持配置字体相关样式）。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", new Date("1968/6/8"), "80", "180"],
    ["4", "NewYork", new Date("1972/7/3"), "72", "168"],
    ["4", "NewYork", new Date("1964/3/2"), "71", "179"],
    ["5", "Washington", new Date("1972/8/8"),"80", "171"],
    ["6", "Washington", new Date("1986/2/2"), "89", "161"],
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]
];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var pivotTable = sheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
var timeline = sheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var style = new GC.Spread.Sheets.Slicers.TimelineStyle();
style.periodLabel2Style(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('red', 'blue', '12pt Calibri'));

timeline.style(style);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) | 可选参数。时间线周期标签2的样式配置对象。 |

#### Returns

`any`

- 如果未设置参数值，则返回当前时间线周期标签2的样式；否则返回当前时间线切片器样式对象本身。

___

### <a id="selectedtimeblockspacestyle" name="selectedtimeblockspacestyle"></a> selectedTimeBlockSpaceStyle

▸ **selectedTimeBlockSpaceStyle**(`value?`): `any`

获取或设置时间线中已选中时间块区域的样式（仅支持配置颜色相关样式）。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", new Date("1968/6/8"), "80", "180"],
    ["4", "NewYork", new Date("1972/7/3"), "72", "168"],
    ["4", "NewYork", new Date("1964/3/2"), "71", "179"],
    ["5", "Washington", new Date("1972/8/8"),"80", "171"],
    ["6", "Washington", new Date("1986/2/2"), "89", "161"],
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]
];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var pivotTable = sheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
var timeline = sheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);

var style = new GC.Spread.Sheets.Slicers.TimelineStyle();
style.selectedTimeBlockSpaceStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('red', undefined, '12pt Calibri'));

timeline.style(style);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) | 可选参数。时间线中已选中时间块区域的样式配置对象。 |

#### Returns

`any`

- 如果未设置参数值，则返回当前时间线中已选中时间块区域的样式；否则返回当前时间线切片器样式对象本身。

___

### <a id="selectedtimeblockstyle" name="selectedtimeblockstyle"></a> selectedTimeBlockStyle

▸ **selectedTimeBlockStyle**(`value?`): `any`

获取或设置已选中时间块的样式，包括颜色和边框等属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", new Date("1968/6/8"), "80", "180"],
    ["4", "NewYork", new Date("1972/7/3"), "72", "168"],
    ["4", "NewYork", new Date("1964/3/2"), "71", "179"],
    ["5", "Washington", new Date("1972/8/8"),"80", "171"],
    ["6", "Washington", new Date("1986/2/2"), "89", "161"],
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]
];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var pivotTable = sheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
var timeline = sheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var style = new GC.Spread.Sheets.Slicers.TimelineStyle();
var border = new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green");
style.selectedTimeBlockStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('red', undefined, '12pt Calibri', border, border, border, border));
timeline.style(style);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) | 可选参数。已选中时间块的样式配置对象。 |

#### Returns

`any`

- 如果未设置参数值，则返回当前已选中时间块的样式；否则返回当前时间线切片器样式对象本身。

___

### <a id="selectionlabelstyle" name="selectionlabelstyle"></a> selectionLabelStyle

▸ **selectionLabelStyle**(`value?`): `any`

获取或设置时间线选择标签的样式（仅支持配置字体相关样式）。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", new Date("1968/6/8"), "80", "180"],
    ["4", "NewYork", new Date("1972/7/3"), "72", "168"],
    ["4", "NewYork", new Date("1964/3/2"), "71", "179"],
    ["5", "Washington", new Date("1972/8/8"),"80", "171"],
    ["6", "Washington", new Date("1986/2/2"), "89", "161"],
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]
];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var pivotTable = sheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
var timeline = sheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var style = new GC.Spread.Sheets.Slicers.TimelineStyle();
style.selectionLabelStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo(undefined, 'blue', '12pt Calibri'));
timeline.style(style);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) | 可选参数。时间线选择标签的样式配置对象。 |

#### Returns

`any`

- 如果未设置参数值，则返回当前时间线选择标签的样式；否则返回当前时间线切片器样式对象本身。

___

### <a id="timelevelstyle" name="timelevelstyle"></a> timeLevelStyle

▸ **timeLevelStyle**(`value?`): `any`

获取或设置时间线时间层级的样式（仅支持配置字体相关样式）。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", new Date("1968/6/8"), "80", "180"],
    ["4", "NewYork", new Date("1972/7/3"), "72", "168"],
    ["4", "NewYork", new Date("1964/3/2"), "71", "179"],
    ["5", "Washington", new Date("1972/8/8"),"80", "171"],
    ["6", "Washington", new Date("1986/2/2"), "89", "161"],
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]
];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var pivotTable = sheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
var timeline = sheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var style = new GC.Spread.Sheets.Slicers.TimelineStyle();
style.timeLevelStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo(undefined, 'blue', '14pt Calibri'));
timeline.style(style);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) | 可选参数。时间线时间层级的样式配置对象。 |

#### Returns

`any`

- 如果未设置参数值，则返回当前时间线时间层级的样式；否则返回当前时间线切片器样式对象本身。

___

### <a id="tojson" name="tojson"></a> toJSON

▸ **toJSON**(): `Object`

将当前对象的状态序列化为 JSON 数据（保存对象状态）。

**`example`**
```javascript
// 此示例使用 toJSON 方法。
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

- 时间线切片器的主题数据（JSON 格式对象）。

___

### <a id="unselectedtimeblockstyle" name="unselectedtimeblockstyle"></a> unselectedTimeBlockStyle

▸ **unselectedTimeBlockStyle**(`value?`): `any`

获取或设置未选中时间块的样式，包括颜色和边框等属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", new Date("1968/6/8"), "80", "180"],
    ["4", "NewYork", new Date("1972/7/3"), "72", "168"],
    ["4", "NewYork", new Date("1964/3/2"), "71", "179"],
    ["5", "Washington", new Date("1972/8/8"),"80", "171"],
    ["6", "Washington", new Date("1986/2/2"), "89", "161"],
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]
];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var pivotTable = sheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
var timeline = sheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
pivotTable.labelFilter("Birthday", { condition: { operator: 18, conType: 1, val: [] } });
var style = new GC.Spread.Sheets.Slicers.TimelineStyle();
style.unselectedTimeBlockStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('red', undefined, '12pt Calibri'));
timeline.style(style);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) | 可选参数。未选中时间块的样式配置对象。 |

#### Returns

`any`

- 如果未设置参数值，则返回当前未选中时间块的样式；否则返回当前时间线切片器样式对象本身。

___

### <a id="wholeslicerstyle" name="wholeslicerstyle"></a> wholeSlicerStyle

▸ **wholeSlicerStyle**(`value?`): `any`

获取或设置整个时间线切片器的整体样式。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", new Date("1968/6/8"), "80", "180"],
    ["4", "NewYork", new Date("1972/7/3"), "72", "168"],
    ["4", "NewYork", new Date("1964/3/2"), "71", "179"],
    ["5", "Washington", new Date("1972/8/8"),"80", "171"],
    ["6", "Washington", new Date("1986/2/2"), "89", "161"],
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]
];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var pivotTable = activeSheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
pivotTable.add('Birthday', 'Birthday', 1);

var timeline = activeSheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var style = new GC.Spread.Sheets.Slicers.TimelineStyle();
style.wholeSlicerStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('red', 'blue', '12pt Calibri'));
style.headerStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo(undefined, 'green', '14pt Calibri'));
style.timeLevelStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('yellow'));

timeline.style(style);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) | 可选参数。整个时间线切片器的样式配置对象。 |

#### Returns

`any`

- 如果未设置参数值，则返回当前整个时间线切片器的样式；否则返回当前时间线切片器样式对象本身。
