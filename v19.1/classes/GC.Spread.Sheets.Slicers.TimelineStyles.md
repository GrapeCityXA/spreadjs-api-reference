# Class: TimelineStyles

[Sheets](../modules/GC.Spread.Sheets.md).[Slicers](../modules/GC.Spread.Sheets.Slicers.md).TimelineStyles

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Slicers.TimelineStyles.md#constructor)

### Methods

- [dark1](GC.Spread.Sheets.Slicers.TimelineStyles.md#dark1)
- [dark2](GC.Spread.Sheets.Slicers.TimelineStyles.md#dark2)
- [dark3](GC.Spread.Sheets.Slicers.TimelineStyles.md#dark3)
- [dark4](GC.Spread.Sheets.Slicers.TimelineStyles.md#dark4)
- [dark5](GC.Spread.Sheets.Slicers.TimelineStyles.md#dark5)
- [dark6](GC.Spread.Sheets.Slicers.TimelineStyles.md#dark6)
- [light1](GC.Spread.Sheets.Slicers.TimelineStyles.md#light1)
- [light2](GC.Spread.Sheets.Slicers.TimelineStyles.md#light2)
- [light3](GC.Spread.Sheets.Slicers.TimelineStyles.md#light3)
- [light4](GC.Spread.Sheets.Slicers.TimelineStyles.md#light4)
- [light5](GC.Spread.Sheets.Slicers.TimelineStyles.md#light5)
- [light6](GC.Spread.Sheets.Slicers.TimelineStyles.md#light6)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new TimelineStyles**()

表示内置时间线样式集合。

## Methods

### <a id="dark1" name="dark1"></a> dark1

▸ `Static` **dark1**(): [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

获取dark1样式。

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
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var pivotTable = activeSheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
pivotTable.add('Birthday', 'Birthday', 1);

var timeline = activeSheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.light1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var style = new GC.Spread.Sheets.Slicers.SlicerStyles.dark1();
timeline.style(style);
```

#### Returns

[`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

___

### <a id="dark2" name="dark2"></a> dark2

▸ `Static` **dark2**(): [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

获取dark2样式。

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
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var pivotTable = activeSheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
pivotTable.add('Birthday', 'Birthday', 1);

var timeline = activeSheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.light1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var style = new GC.Spread.Sheets.Slicers.SlicerStyles.dark2();
timeline.style(style);
```

#### Returns

[`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

___

### <a id="dark3" name="dark3"></a> dark3

▸ `Static` **dark3**(): [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

获取dark3样式。

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
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var pivotTable = activeSheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
pivotTable.add('Name', 'Name', 1);

var timeline = activeSheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.light1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var style = new GC.Spread.Sheets.Slicers.SlicerStyles.dark3();
timeline.style(style);
```

#### Returns

[`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

___

### <a id="dark4" name="dark4"></a> dark4

▸ `Static` **dark4**(): [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

获取dark4样式。

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
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var pivotTable = activeSheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
pivotTable.add('Birthday', 'Birthday', 1);

var timeline = activeSheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.light1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var style = new GC.Spread.Sheets.Slicers.SlicerStyles.dark4();
timeline.style(style);
```

#### Returns

[`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

___

### <a id="dark5" name="dark5"></a> dark5

▸ `Static` **dark5**(): [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

获取dark5样式。

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
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var pivotTable = activeSheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
pivotTable.add('Birthday', 'Birthday', 1);

var timeline = activeSheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.light1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var style = new GC.Spread.Sheets.Slicers.SlicerStyles.dark5();
timeline.style(style);
```

#### Returns

[`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

___

### <a id="dark6" name="dark6"></a> dark6

▸ `Static` **dark6**(): [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

获取dark6样式。

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
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var pivotTable = activeSheet.pivotTables.add('pivotTable1', table.name(), 11, 1);
pivotTable.add('Birthday', 'Birthday', 1);

var timeline = activeSheet.slicers.add('timeline1', 'pivotTable1', 'Birthday', GC.Spread.Sheets.Slicers.TimelineStyles.light1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var style = new GC.Spread.Sheets.Slicers.SlicerStyles.dark6();
timeline.style(style);
```

#### Returns

[`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

___

### <a id="light1" name="light1"></a> light1

▸ `Static` **light1**(): [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

获取light1样式。

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
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]];
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
var style = new GC.Spread.Sheets.Slicers.SlicerStyles.light1();
timeline.style(style);
```

#### Returns

[`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

___

### <a id="light2" name="light2"></a> light2

▸ `Static` **light2**(): [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

获取light2样式。

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
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]];
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
var style = new GC.Spread.Sheets.Slicers.SlicerStyles.light2();
timeline.style(style);
```

#### Returns

[`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

___

### <a id="light3" name="light3"></a> light3

▸ `Static` **light3**(): [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

获取light3样式。

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
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]];
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
var style = new GC.Spread.Sheets.Slicers.SlicerStyles.light3();
timeline.style(style);
```

#### Returns

[`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

___

### <a id="light4" name="light4"></a> light4

▸ `Static` **light4**(): [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

获取light4样式。

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
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]];
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
var style = new GC.Spread.Sheets.Slicers.SlicerStyles.light4();
timeline.style(style);
```

#### Returns

[`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

___

### <a id="light5" name="light5"></a> light5

▸ `Static` **light5**(): [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

获取light5样式。

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
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]];
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
var style = new GC.Spread.Sheets.Slicers.SlicerStyles.light5();
timeline.style(style);
```

#### Returns

[`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

___

### <a id="light6" name="light6"></a> light6

▸ `Static` **light6**(): [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

获取light6样式。

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
    ["7", "Washington", new Date("2012/2/15"), "71", "240"]];
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
var style = new GC.Spread.Sheets.Slicers.SlicerStyles.light6();
timeline.style(style);
```

#### Returns

[`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)
