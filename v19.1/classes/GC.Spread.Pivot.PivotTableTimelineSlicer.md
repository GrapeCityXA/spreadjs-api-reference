# Class: PivotTableTimelineSlicer

[Spread](../modules/GC.Spread.md).[Pivot](../modules/GC.Spread.Pivot.md).PivotTableTimelineSlicer

## Table of contents

### Constructors

- [constructor](GC.Spread.Pivot.PivotTableTimelineSlicer.md#constructor)

### Methods

- [allowMove](GC.Spread.Pivot.PivotTableTimelineSlicer.md#allowmove)
- [allowResize](GC.Spread.Pivot.PivotTableTimelineSlicer.md#allowresize)
- [captionName](GC.Spread.Pivot.PivotTableTimelineSlicer.md#captionname)
- [connectPivotTable](GC.Spread.Pivot.PivotTableTimelineSlicer.md#connectpivottable)
- [disableResizingAndMoving](GC.Spread.Pivot.PivotTableTimelineSlicer.md#disableresizingandmoving)
- [disconnectPivotTable](GC.Spread.Pivot.PivotTableTimelineSlicer.md#disconnectpivottable)
- [dynamicMove](GC.Spread.Pivot.PivotTableTimelineSlicer.md#dynamicmove)
- [dynamicSize](GC.Spread.Pivot.PivotTableTimelineSlicer.md#dynamicsize)
- [endColumn](GC.Spread.Pivot.PivotTableTimelineSlicer.md#endcolumn)
- [endColumnOffset](GC.Spread.Pivot.PivotTableTimelineSlicer.md#endcolumnoffset)
- [endRow](GC.Spread.Pivot.PivotTableTimelineSlicer.md#endrow)
- [endRowOffset](GC.Spread.Pivot.PivotTableTimelineSlicer.md#endrowoffset)
- [getAllConnectedPivotTables](GC.Spread.Pivot.PivotTableTimelineSlicer.md#getallconnectedpivottables)
- [getAllPivotTables](GC.Spread.Pivot.PivotTableTimelineSlicer.md#getallpivottables)
- [getConnectedPivotTableNameList](GC.Spread.Pivot.PivotTableTimelineSlicer.md#getconnectedpivottablenamelist)
- [getStyleName](GC.Spread.Pivot.PivotTableTimelineSlicer.md#getstylename)
- [height](GC.Spread.Pivot.PivotTableTimelineSlicer.md#height)
- [isConnectedPivotTable](GC.Spread.Pivot.PivotTableTimelineSlicer.md#isconnectedpivottable)
- [isLocked](GC.Spread.Pivot.PivotTableTimelineSlicer.md#islocked)
- [isSelected](GC.Spread.Pivot.PivotTableTimelineSlicer.md#isselected)
- [isVisible](GC.Spread.Pivot.PivotTableTimelineSlicer.md#isvisible)
- [level](GC.Spread.Pivot.PivotTableTimelineSlicer.md#level)
- [name](GC.Spread.Pivot.PivotTableTimelineSlicer.md#name)
- [nameInFormula](GC.Spread.Pivot.PivotTableTimelineSlicer.md#nameinformula)
- [position](GC.Spread.Pivot.PivotTableTimelineSlicer.md#position)
- [refresh](GC.Spread.Pivot.PivotTableTimelineSlicer.md#refresh)
- [scrollPosition](GC.Spread.Pivot.PivotTableTimelineSlicer.md#scrollposition)
- [sheet](GC.Spread.Pivot.PivotTableTimelineSlicer.md#sheet)
- [showHeader](GC.Spread.Pivot.PivotTableTimelineSlicer.md#showheader)
- [showHorizontalScrollbar](GC.Spread.Pivot.PivotTableTimelineSlicer.md#showhorizontalscrollbar)
- [showSelectionLabel](GC.Spread.Pivot.PivotTableTimelineSlicer.md#showselectionlabel)
- [showTimeLevel](GC.Spread.Pivot.PivotTableTimelineSlicer.md#showtimelevel)
- [sourceName](GC.Spread.Pivot.PivotTableTimelineSlicer.md#sourcename)
- [startColumn](GC.Spread.Pivot.PivotTableTimelineSlicer.md#startcolumn)
- [startColumnOffset](GC.Spread.Pivot.PivotTableTimelineSlicer.md#startcolumnoffset)
- [startRow](GC.Spread.Pivot.PivotTableTimelineSlicer.md#startrow)
- [startRowOffset](GC.Spread.Pivot.PivotTableTimelineSlicer.md#startrowoffset)
- [style](GC.Spread.Pivot.PivotTableTimelineSlicer.md#style)
- [width](GC.Spread.Pivot.PivotTableTimelineSlicer.md#width)
- [x](GC.Spread.Pivot.PivotTableTimelineSlicer.md#x)
- [y](GC.Spread.Pivot.PivotTableTimelineSlicer.md#y)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new PivotTableTimelineSlicer**()

表示一个数据透视表时间轴切片器。

## Methods

### <a id="allowmove" name="allowmove"></a> allowMove

▸ **allowMove**(`value?`): `any`

获取或设置切片器的 allowMove 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.allowMove();
console.log(oldValue);
slicer.allowMove(false);
var newValue = slicer.allowMove();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的 allowMove 属性。 allowMove 属性指定是否允许用户移动时间轴，启用或禁用重新定位功能。 |

#### Returns

`any`

如果未设置值，则返回切片器的 allowMove 属性；否则，返回切片器。

___

### <a id="allowresize" name="allowresize"></a> allowResize

▸ **allowResize**(`value?`): `any`

获取或设置切片器的 allowResize 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.allowResize();
console.log(oldValue);
slicer.allowResize(false);
var newValue = slicer.allowResize();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的 allowResize 属性。 allowResize 属性指定是否允许用户调整时间轴的大小，启用或禁用调整大小功能。 |

#### Returns

`any`

如果未设置值，则返回切片器的 allowResize 属性；否则，返回切片器。

___

### <a id="captionname" name="captionname"></a> captionName

▸ **captionName**(`value?`): `any`

获取或设置切片器的 captionName 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.captionName();
console.log(oldValue);
slicer.captionName('timeline_caption');
var newValue = slicer.captionName();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 切片器的 captionName 属性。 captionName 属性显示在时间轴切片器的标题中。 |

#### Returns

`any`

如果未设置值，则返回切片器的 captionName 属性；否则，返回切片器。

___

### <a id="connectpivottable" name="connectpivottable"></a> connectPivotTable

▸ **connectPivotTable**(`ptName`): `void`

连接数据透视表与切片器

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);

timeline.connectPivotTable('pivotTable1');
timeline.isConnectedPivotTable('pivotTable1');
timeline.disconnectPivotTable('pivotTable1');
timeline.isConnectedPivotTable('pivotTable1');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ptName` | `string` | 数据透视表的名称 |

#### Returns

`void`

___

### <a id="disableresizingandmoving" name="disableresizingandmoving"></a> disableResizingAndMoving

▸ **disableResizingAndMoving**(`value?`): `any`

获取或设置切片器的 disableResizingAndMoving 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.disableResizingAndMoving();
console.log(oldValue);
slicer.disableResizingAndMoving(false);
var newValue = slicer.disableResizingAndMoving();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的 disableResizingAndMoving 属性。 disableResizingAndMoving 属性指定是否允许用户调整时间轴切片器的大小或位置，限制任何更改。 |

#### Returns

`any`

如果未设置值，则返回切片器的 disableResizingAndMoving 属性；否则，返回切片器。

___

### <a id="disconnectpivottable" name="disconnectpivottable"></a> disconnectPivotTable

▸ **disconnectPivotTable**(`ptName`): `void`

断开数据透视表与切片器

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);

timeline.connectPivotTable('pivotTable1');
timeline.isConnectedPivotTable('pivotTable1');
timeline.disconnectPivotTable('pivotTable1');
timeline.isConnectedPivotTable('pivotTable1');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ptName` | `string` | 数据透视表的名称 |

#### Returns

`void`

___

### <a id="dynamicmove" name="dynamicmove"></a> dynamicMove

▸ **dynamicMove**(`value?`): `any`

获取或设置切片器的 dynamicMove 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.dynamicMove();
console.log(oldValue);
slicer.dynamicMove(false);
var newValue = slicer.dynamicMove();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的 dynamicMove 属性。 dynamicMove 属性指定是否允许时间轴切片器根据关联数据或数据透视表布局动态调整其位置或大小。 |

#### Returns

`any`

如果未设置值，则返回切片器的 dynamicMove 属性；否则，返回切片器。

___

### <a id="dynamicsize" name="dynamicsize"></a> dynamicSize

▸ **dynamicSize**(`value?`): `any`

获取或设置切片器的 dynamicSize 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.dynamicSize();
console.log(oldValue);
slicer.dynamicSize(false);
var newValue = slicer.dynamicSize();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的 dynamicSize 属性。 dynamicSize 属性指定是否允许时间轴根据关联数据或数据透视表布局动态调整其大小。 |

#### Returns

`any`

如果未设置值，则返回切片器的 dynamicSize 属性；否则，返回切片器。

___

### <a id="endcolumn" name="endcolumn"></a> endColumn

▸ **endColumn**(`value?`): `any`

获取或设置切片器的 endColumn 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.endColumn();
console.log(oldValue);
slicer.endColumn(9);
var newValue = slicer.endColumn();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的 endColumn 属性。 endColumn 属性指定时间轴切片器在工作表中的结束列索引或位置。 |

#### Returns

`any`

如果未设置值，则返回切片器的 endColumn 属性；否则，返回切片器。

___

### <a id="endcolumnoffset" name="endcolumnoffset"></a> endColumnOffset

▸ **endColumnOffset**(`value?`): `any`

获取或设置切片器的 endColumnOffset 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.endColumnOffset();
console.log(oldValue);
slicer.endColumnOffset(10);
var newValue = slicer.endColumnOffset();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的 endColumnOffset 属性。 endColumnOffset 属性指定时间轴切片器在工作表中的结束列偏移量或位置。 |

#### Returns

`any`

如果未设置值，则返回切片器的 endColumnOffset 属性；否则，返回切片器。

___

### <a id="endrow" name="endrow"></a> endRow

▸ **endRow**(`value?`): `any`

获取或设置切片器的 endRow 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.endRow();
console.log(oldValue);
slicer.endRow(7);
var newValue = slicer.endRow();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的 endRow 属性。 endRow 属性指定时间轴切片器在工作表中的结束行索引或位置。 |

#### Returns

`any`

如果未设置值，则返回切片器的 endRow 属性；否则，返回切片器。

___

### <a id="endrowoffset" name="endrowoffset"></a> endRowOffset

▸ **endRowOffset**(`value?`): `any`

获取或设置切片器的 endRowOffset 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.endRowOffset();
console.log(oldValue);
slicer.endRowOffset(5);
var newValue = slicer.endRowOffset();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的 endRowOffset 属性。 endRowOffset 属性指定时间轴切片器在工作表中的结束行偏移量或位置。 |

#### Returns

`any`

如果未设置值，则返回切片器的 endRowOffset 属性；否则，返回切片器。

___

### <a id="getallconnectedpivottables" name="getallconnectedpivottables"></a> getAllConnectedPivotTables

▸ **getAllConnectedPivotTables**(): [`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)[]

获取所有连接的数据透视表

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);

timeline.connectPivotTable('pivotTable1');
timeline.isConnectedPivotTable('pivotTable1');
console.log(timeline.getAllPivotTables());
timeline.disconnectPivotTable('pivotTable1');
timeline.isConnectedPivotTable('pivotTable1');
console.log(timeline.getAllPivotTables());
```

#### Returns

[`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)[]

连接到切片器的数据透视表。

___

### <a id="getallpivottables" name="getallpivottables"></a> getAllPivotTables

▸ **getAllPivotTables**(): [`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)[]

获取所有连接或未连接的数据透视表。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);

timeline.connectPivotTable('pivotTable1');
timeline.isConnectedPivotTable('pivotTable1');
console.log(timeline.getAllPivotTables());
timeline.disconnectPivotTable('pivotTable1');
timeline.isConnectedPivotTable('pivotTable1');
console.log(timeline.getAllPivotTables());
```

#### Returns

[`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)[]

源与切片器相同的数据透视表。

___

### <a id="getconnectedpivottablenamelist" name="getconnectedpivottablenamelist"></a> getConnectedPivotTableNameList

▸ **getConnectedPivotTableNameList**(): `string`[]

获取所有连接的数据透视表的名称。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);

timeline.connectPivotTable('pivotTable1');
timeline.isConnectedPivotTable('pivotTable1');
console.log(timeline.getAllPivotTables());
timeline.disconnectPivotTable('pivotTable1');
timeline.isConnectedPivotTable('pivotTable1');
console.log(timeline.getAllPivotTables());
```

#### Returns

`string`[]

连接到切片器的数据透视表的名称列表。

___

### <a id="getstylename" name="getstylename"></a> getStyleName

▸ **getStyleName**(): `undefined` \| `string`

获取或设置切片器的时间轴样式名称。

#### Returns

`undefined` \| `string`

返回时间轴切片器的样式名称。

___

### <a id="height" name="height"></a> height

▸ **height**(`value?`): `any`

获取或设置切片器的高度。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.height();
console.log(oldValue);
slicer.height(120);
var newValue = slicer.height();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的高度。 height 属性指定时间轴切片器的高度或大小。 |

#### Returns

`any`

如果未设置值，则返回切片器的高度；否则，返回切片器。

___

### <a id="isconnectedpivottable" name="isconnectedpivottable"></a> isConnectedPivotTable

▸ **isConnectedPivotTable**(`ptName`): `boolean`

检查是否连接到切片器的数据透视表。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);

timeline.connectPivotTable('pivotTable1');
timeline.isConnectedPivotTable('pivotTable1');
timeline.disconnectPivotTable('pivotTable1');
timeline.isConnectedPivotTable('pivotTable1');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ptName` | `string` | 数据透视表的名称。 |

#### Returns

`boolean`

是否连接到时间轴切片器。

___

### <a id="islocked" name="islocked"></a> isLocked

▸ **isLocked**(`value?`): `any`

获取或设置切片器的 isLocked 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.isLocked();
console.log(oldValue);
slicer.isLocked(false);
var newValue = slicer.isLocked();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的 isLocked 属性。 isLocked 属性指定时间轴切片器是否当前锁定或解锁，指示当工作表受保护时，用户是否可以更改其设置或选择。 |

#### Returns

`any`

如果未设置值，则返回切片器的 isLocked；否则返回切片器。

___

### <a id="isselected" name="isselected"></a> isSelected

▸ **isSelected**(`value?`): `any`

获取或设置切片器的 isSelected 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.isSelected();
console.log(oldValue);
slicer.isSelected(false);
var newValue = slicer.isSelected();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的 isSelected 属性。 isSelected 属性指定时间轴切片器中是否当前选择或突出显示特定时间范围。 |

#### Returns

`any`

如果未设置值，则返回切片器的 isSelected 属性；否则，返回切片器。

___

### <a id="isvisible" name="isvisible"></a> isVisible

▸ **isVisible**(`value?`): `any`

获取或设置切片器的 isVisible 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.isVisible();
console.log(oldValue);
slicer.isVisible(false);
var newValue = slicer.isVisible();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的 isVisible 属性。 isVisible 属性指定时间轴切片器是否当前可见或隐藏。 |

#### Returns

`any`

如果未设置值，则返回切片器的 isVisible 属性；否则，返回切片器。

___

### <a id="level" name="level"></a> level

▸ **level**(`value?`): `any`

获取或设置切片器的 level 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.level();
console.log(oldValue);
slicer.level(GC.Spread.Sheets.Slicers.TimelineLevel.years);
var newValue = slicer.level();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`TimelineLevel`](../enums/GC.Spread.Sheets.Slicers.TimelineLevel.md) | 切片器的 level 属性。 level 属性指定时间轴切片器当前操作的时态粒度或时间单位（例如，年、季度、月），确定基于日期的过滤和选择的时间范围。 |

#### Returns

`any`

如果未设置值，则返回切片器的 level 属性；否则，返回切片器。

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置切片器的 name 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.name();
console.log(oldValue);
slicer.name('timeline2');
var newValue = slicer.name();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 切片器的 name 属性。 name 属性指定时间轴切片器的唯一标识符或标签，允许在工作簿或程序化交互中进行识别和引用。 |

#### Returns

`any`

如果未设置值，则返回切片器的 name 属性；否则，返回切片器。

___

### <a id="nameinformula" name="nameinformula"></a> nameInFormula

▸ **nameInFormula**(): `string`

获取切片器的 nameInFormula 属性。

#### Returns

`string`

返回切片器的 nameInFormula 属性。

___

### <a id="position" name="position"></a> position

▸ **position**(`value?`): `any`

获取或设置切片器的位置。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.position();
console.log(oldValue);
slicer.position(new GC.Spread.Sheets.Point(10, 20));
var newValue = slicer.position();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`Point`](GC.Spread.Sheets.Point.md) | 切片器的位置。时间线切片器的 position 属性指定时间线在工作表中的放置位置。 |

#### Returns

`any`

如果未设置值，则返回切片器的位置；否则返回切片器。

___

### <a id="refresh" name="refresh"></a> refresh

▸ **refresh**(): `void`

刷新切片器。

#### Returns

`void`

___

### <a id="scrollposition" name="scrollposition"></a> scrollPosition

▸ **scrollPosition**(`value?`): `any`

获取或设置切片器的 scrollPosition 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.showHeader();
console.log(oldValue);
slicer.showHeader(new Date('1973/7/3'));
var newValue = slicer.showHeader();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `Date` | 切片器的 scrollPosition 属性。 scrollPosition 属性指定时间轴切片器当前滚动位置或偏移量，指示可见时间范围在整体时间轴数据中的起始点。 |

#### Returns

`any`

如果未设置值，则返回切片器的 scrollPosition 属性；否则，返回切片器。

___

### <a id="sheet" name="sheet"></a> sheet

▸ **sheet**(): [`Worksheet`](GC.Spread.Sheets.Worksheet.md)

获取切片器的工作表。

#### Returns

[`Worksheet`](GC.Spread.Sheets.Worksheet.md)

返回切片器的工作表。

___

### <a id="showheader" name="showheader"></a> showHeader

▸ **showHeader**(`value?`): `any`

获取或设置切片器的 showHeader 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.showHeader();
console.log(oldValue);
slicer.showHeader(false);
var newValue = slicer.showHeader();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的 showHeader 属性。 showHeader 属性指定时间轴切片器是否显示标题和过滤相关控件。 |

#### Returns

`any`

如果未设置值，则返回切片器的 showHeader 属性；否则，返回切片器。

___

### <a id="showhorizontalscrollbar" name="showhorizontalscrollbar"></a> showHorizontalScrollbar

▸ **showHorizontalScrollbar**(`value?`): `any`

获取或设置切片器的 showHorizontalScrollbar 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.showHorizontalScrollbar();
console.log(oldValue);
slicer.showHorizontalScrollbar(false);
var newValue = slicer.showHorizontalScrollbar();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的 showHorizontalScrollbar 属性。 showHorizontalScrollbar 属性指定时间轴切片器是否显示水平滚动条，允许用户导航内容。 |

#### Returns

`any`

如果未设置值，则返回切片器的 showHorizontalScrollbar 属性；否则，返回切片器。

___

### <a id="showselectionlabel" name="showselectionlabel"></a> showSelectionLabel

▸ **showSelectionLabel**(`value?`): `any`

获取或设置切片器的 showSelectionLabel 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.showSelectionLabel();
console.log(oldValue);
slicer.showSelectionLabel(false);
var newValue = slicer.showSelectionLabel();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的 showSelectionLabel 属性。 showSelectionLabel 属性指定时间轴切片器是否显示选定时间范围的标签，提供用户关于当前选择的时间范围的信息。 |

#### Returns

`any`

如果未设置值，则返回切片器的 showSelectionLabel 属性；否则，返回切片器。

___

### <a id="showtimelevel" name="showtimelevel"></a> showTimeLevel

▸ **showTimeLevel**(`value?`): `any`

获取或设置切片器的 showTimeLevel 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.showTimeLevel();
console.log(oldValue);
slicer.showTimeLevel(false);
var newValue = slicer.showTimeLevel();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的 showTimeLevel 属性。 showTimeLevel 属性指定时间轴切片器是否显示不同的时间级别（例如，年、季度、月）作为选项，供用户选择和过滤数据。 |

#### Returns

`any`

如果未设置值，则返回切片器的 showTimeLevel 属性；否则，返回切片器。

___

### <a id="sourcename" name="sourcename"></a> sourceName

▸ **sourceName**(): `string`

获取切片器的 sourceName 属性。

#### Returns

`string`

返回切片器的 sourceName 属性。 sourceName 属性指定时间轴切片器关联的数据源字段的名称。

___

### <a id="startcolumn" name="startcolumn"></a> startColumn

▸ **startColumn**(`value?`): `any`

获取或设置切片器的 startColumn 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.startColumn();
console.log(oldValue);
slicer.startColumn(5);
var newValue = slicer.startColumn();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的 startColumn 属性。 startColumn 属性指定时间轴切片器在工作表中的起始列索引或位置。 |

#### Returns

`any`

如果未设置值，则返回切片器的 startColumn 属性；否则，返回切片器。

___

### <a id="startcolumnoffset" name="startcolumnoffset"></a> startColumnOffset

▸ **startColumnOffset**(`value?`): `any`

获取或设置切片器的 startColumnOffset 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.startColumnOffset();
console.log(oldValue);
slicer.startColumnOffset(15);
var newValue = slicer.startColumnOffset();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的 startColumnOffset 属性。 startColumnOffset 属性指定时间轴切片器在工作表中的水平偏移量或距离，从起始列索引开始，确定时间轴在表格中的位置。 |

#### Returns

`any`

如果未设置值，则返回切片器的 startColumnOffset 属性；否则，返回切片器。

___

### <a id="startrow" name="startrow"></a> startRow

▸ **startRow**(`value?`): `any`

获取或设置切片器的 startRow 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.startRow();
console.log(oldValue);
slicer.startRow(3);
var newValue = slicer.startRow();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的 startRow 属性。 startRow 属性指定时间轴切片器在工作表中的起始行索引或位置。 |

#### Returns

`any`

如果未设置值，则返回切片器的 startRow 属性；否则，返回切片器。

___

### <a id="startrowoffset" name="startrowoffset"></a> startRowOffset

▸ **startRowOffset**(`value?`): `any`

获取或设置切片器的 startRowOffset 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.startRowOffset();
console.log(oldValue);
slicer.startRowOffset(10);
var newValue = slicer.startRowOffset();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的 startRowOffset 属性。 startRowOffset 属性指定时间轴切片器在工作表中的垂直偏移量或距离，从起始行索引开始，确定时间轴在表格中的位置。 |

#### Returns

`any`

如果未设置值，则返回切片器的 startRowOffset 属性；否则，返回切片器。

___

### <a id="style" name="style"></a> style

▸ **style**(`value?`): [`PivotTableTimelineSlicer`](GC.Spread.Pivot.PivotTableTimelineSlicer.md) \| [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

获取或设置切片器的样式。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: "1968/6/8" },
    { Name: "Betty", City: "NewYork", Birthday: "1972/7/3" },
    { Name: "Alice", City: "Washington", Birthday: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);

var style = new GC.Spread.Sheets.Slicers.TimelineStyle()
style.wholeSlicerStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('red', 'blue', '12pt Calibri'));
style.headerStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo(undefined, 'green', '14pt Calibri'));
style.timeLevelStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('yellow'));

var oldValue = slicer.style();
console.log(oldValue);
timeline.style(style);
var newValue = slicer.style();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` \| [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md) | 切片器的 style 属性。 style 属性指定时间轴切片器的视觉外观和格式化样式，定义其整体外观和展示。 |

#### Returns

[`PivotTableTimelineSlicer`](GC.Spread.Pivot.PivotTableTimelineSlicer.md) \| [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

如果未设置样式，则返回切片器的样式；否则，返回切片器。

___

### <a id="width" name="width"></a> width

▸ **width**(`value?`): `any`

获取或设置切片器的 width 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.width();
console.log(oldValue);
slicer.width(150);
var newValue = slicer.width();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的 width 属性。 width 属性指定时间轴切片器的水平维度或宽度，确定其在 x 轴上的大小。 |

#### Returns

`any`

如果未设置值，则返回切片器的 width 属性；否则，返回切片器。

___

### <a id="x" name="x"></a> x

▸ **x**(`value?`): `any`

获取或设置切片器的 x 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.x();
console.log(oldValue);
slicer.x(30);
var newValue = slicer.x();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的 x 属性。 x 属性指定时间轴切片器在工作表中的水平位置或坐标，确定其在 x 轴上的位置。 |

#### Returns

`any`

如果未设置值，则返回切片器的 x 属性；否则，返回切片器。

___

### <a id="y" name="y"></a> y

▸ **y**(`value?`): `any`

获取或设置切片器的 y 属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: new Date("1968/6/8") },
    { Name: "Betty", City: "NewYork", Birthday: new Date("1972/7/3") },
    { Name: "Alice", City: "Washington", Birthday: new Date("2012/2/15") },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var timeline = activeSheet.slicers.add("timeline", "pivotTable1", "Birthday", GC.Spread.Sheets.Slicers.TimelineStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTimeline);
var oldValue = slicer.y();
console.log(oldValue);
slicer.y(50);
var newValue = slicer.y();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的 y 属性。 y 属性指定时间轴切片器在工作表中的垂直位置或坐标，确定其在 y 轴上的位置。 |

#### Returns

`any`

如果未设置值，则返回切片器的 y 属性；否则，返回切片器。
