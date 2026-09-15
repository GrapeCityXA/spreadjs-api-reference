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

透视表时间线切片器

## Methods

### <a id="allowmove" name="allowmove"></a> allowMove

▸ **allowMove**(`value?`): `any`

获取或设置切片器的allowMove

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值，返回切片器的allowMove;否则，返回切片器

___

### <a id="allowresize" name="allowresize"></a> allowResize

▸ **allowResize**(`value?`): `any`

获取或设置切片器的allowResize

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值，返回切片器的allowResize;否则，返回切片器

___

### <a id="captionname" name="captionname"></a> captionName

▸ **captionName**(`value?`): `any`

获取或设置切片器的captionName

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果没有设置值，返回切片器的captionName;否则，返回切片器

___

### <a id="connectpivottable" name="connectpivottable"></a> connectPivotTable

▸ **connectPivotTable**(`ptName`): `void`

用切器关联的透视表

**`example`**
```
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
| `ptName` | `string` | 透视表的名称 |

#### Returns

`void`

___

### <a id="disableresizingandmoving" name="disableresizingandmoving"></a> disableResizingAndMoving

▸ **disableResizingAndMoving**(`value?`): `any`

获取或设置切片器的 disableResizingAndMoving

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值，返回切片器的disableResizingAndMoving;否则，返回切片器

___

### <a id="disconnectpivottable" name="disconnectpivottable"></a> disconnectPivotTable

▸ **disconnectPivotTable**(`ptName`): `void`

获取或设置切片器的disconnectPivotTable

**`example`**
```
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
| `ptName` | `string` | 透视表的名称 |

#### Returns

`void`

___

### <a id="dynamicmove" name="dynamicmove"></a> dynamicMove

▸ **dynamicMove**(`value?`): `any`

获取或设置切片器的dynamicMove

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值，返回切片器的dynamicMove;否则，返回切片器

___

### <a id="dynamicsize" name="dynamicsize"></a> dynamicSize

▸ **dynamicSize**(`value?`): `any`

获取或设置切片器的dynamicSize

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值，返回切片器的dynamicSize;否则，返回切片器

___

### <a id="endcolumn" name="endcolumn"></a> endColumn

▸ **endColumn**(`value?`): `any`

获取或设置切片器的endColumn

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值，返回切片器的endColumn;否则，返回切片器

___

### <a id="endcolumnoffset" name="endcolumnoffset"></a> endColumnOffset

▸ **endColumnOffset**(`value?`): `any`

获取或设置切片器的endColumnOffset

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值，返回切片器的endColumnOffset;否则，返回切片器

___

### <a id="endrow" name="endrow"></a> endRow

▸ **endRow**(`value?`): `any`

获取或设置切片器的endRow

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值，返回切片器的endRow;否则，返回切片器

___

### <a id="endrowoffset" name="endrowoffset"></a> endRowOffset

▸ **endRowOffset**(`value?`): `any`

获取或设置切片器的endRowOffset

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值，返回切片器的endRowOffset;否则，返回切片器

___

### <a id="getallconnectedpivottables" name="getallconnectedpivottables"></a> getAllConnectedPivotTables

▸ **getAllConnectedPivotTables**(): [`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)[]

获得所有关联的透视表

**`example`**
```
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

与切片器相连的透视表

___

### <a id="getallpivottables" name="getallpivottables"></a> getAllPivotTables

▸ **getAllPivotTables**(): [`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)[]

获取所有透视表，无论是否关联

**`example`**
```
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

与切片器相同数据源的透视表

___

### <a id="getconnectedpivottablenamelist" name="getconnectedpivottablenamelist"></a> getConnectedPivotTableNameList

▸ **getConnectedPivotTableNameList**(): `string`[]

获得所有关联的透视表名称

**`example`**
```
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

name 与切片器连接的数据透视表列表

___

### <a id="getstylename" name="getstylename"></a> getStyleName

▸ **getStyleName**(): `undefined` \| `string`

获取或设置数据透视表时间线切片器的样式名称。

#### Returns

`undefined` \| `string`

返回数据透视表时间线切片器样式名称。

___

### <a id="height" name="height"></a> height

▸ **height**(`value?`): `any`

获取或设置切片器的高度

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值，返回切片器的高度；否则，返回切片器

___

### <a id="isconnectedpivottable" name="isconnectedpivottable"></a> isConnectedPivotTable

▸ **isConnectedPivotTable**(`ptName`): `boolean`

检查透视表是否与切片器关联

**`example`**
```
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
| `ptName` | `string` | 透视表的名称 |

#### Returns

`boolean`

数据透视表是否与时间线切片器连接

___

### <a id="islocked" name="islocked"></a> isLocked

▸ **isLocked**(`value?`): `any`

获取或设置切片器的isLocked

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值，返回切片器的isLocked;否则，返回切片器

___

### <a id="isselected" name="isselected"></a> isSelected

▸ **isSelected**(`value?`): `any`

获取或设置切片器的isSelected

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值，返回切片器的isSelected;否则，返回切片器

___

### <a id="isvisible" name="isvisible"></a> isVisible

▸ **isVisible**(`value?`): `any`

获取或设置切片器的isVisible

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值，返回切片器的isVisible;否则，返回切片器

___

### <a id="level" name="level"></a> level

▸ **level**(`value?`): `any`

获取或设置切片器的level

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | [`TimelineLevel`](../enums/GC.Spread.Sheets.Slicers.TimelineLevel.md) |

#### Returns

`any`

如果未设置值，则返回切片器的level;否则，返回切片器

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置切片器的name

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果没有设置值，返回切片器的名称；否则，返回切片器

___

### <a id="nameinformula" name="nameinformula"></a> nameInFormula

▸ **nameInFormula**(): `string`

切片器的nameInFormula

#### Returns

`string`

返回nameInFormula

___

### <a id="position" name="position"></a> position

▸ **position**(`value?`): `any`

获取或设置切片器的position

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | [`Point`](GC.Spread.Sheets.Point.md) |

#### Returns

`any`

如果没有设置值，返回切片器的position;否则，返回切片器

___

### <a id="refresh" name="refresh"></a> refresh

▸ **refresh**(): `void`

刷新切片器

#### Returns

`void`

___

### <a id="scrollposition" name="scrollposition"></a> scrollPosition

▸ **scrollPosition**(`value?`): `any`

获取或设置切片器的scrollPosition

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `Date` |

#### Returns

`any`

如果未设置值，则返回切片器的scrollPosition;否则，返回切片器

___

### <a id="sheet" name="sheet"></a> sheet

▸ **sheet**(): [`Worksheet`](GC.Spread.Sheets.Worksheet.md)

获取表单

#### Returns

[`Worksheet`](GC.Spread.Sheets.Worksheet.md)

返回表单

___

### <a id="showheader" name="showheader"></a> showHeader

▸ **showHeader**(`value?`): `any`

获取或设置切片器的showHeader

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值，返回切片器的showHeader;否则，返回切片器

___

### <a id="showhorizontalscrollbar" name="showhorizontalscrollbar"></a> showHorizontalScrollbar

▸ **showHorizontalScrollbar**(`value?`): `any`

获取或设置切片器的showHorizontalScrollbar

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置值，则返回切片器的showHorizontalScrollbar;否则，返回切片器

___

### <a id="showselectionlabel" name="showselectionlabel"></a> showSelectionLabel

▸ **showSelectionLabel**(`value?`): `any`

获取或设置切片器的showSelectionLabel

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置值，则返回切片器的showSelectionLabel;否则，返回切片器

___

### <a id="showtimelevel" name="showtimelevel"></a> showTimeLevel

▸ **showTimeLevel**(`value?`): `any`

获取或设置切片器的showTimeLevel

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置值，则返回切片器的showTimeLevel;否则，返回切片器

___

### <a id="sourcename" name="sourcename"></a> sourceName

▸ **sourceName**(): `string`

获取sourceName

#### Returns

`string`

返回sourceName

___

### <a id="startcolumn" name="startcolumn"></a> startColumn

▸ **startColumn**(`value?`): `any`

获取或设置切片器的startColumn

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值，返回切片器的startColumn;否则，返回切片器

___

### <a id="startcolumnoffset" name="startcolumnoffset"></a> startColumnOffset

▸ **startColumnOffset**(`value?`): `any`

获取或设置切片器的startColumnOffset

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值，返回切片器的startColumnOffset;否则，返回切片器

___

### <a id="startrow" name="startrow"></a> startRow

▸ **startRow**(`value?`): `any`

获取或设置切片器的startRow

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值，返回切片器的startRow;否则，返回切片器

___

### <a id="startrowoffset" name="startrowoffset"></a> startRowOffset

▸ **startRowOffset**(`value?`): `any`

获取或设置切片器的startRowOffset

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值，返回切片器的startRowOffset;否则，返回切片器

___

### <a id="style" name="style"></a> style

▸ **style**(`value?`): `any`

获取或设置切片器的style

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md) |

#### Returns

`any`

如果没有设置值，返回切片器的style;否则，返回切片器

___

### <a id="width" name="width"></a> width

▸ **width**(`value?`): `any`

获取或设置切片器的width

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值，返回切片器的width;否则，返回切片器

___

### <a id="x" name="x"></a> x

▸ **x**(`value?`): `any`

获取或设置切片器的x

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值，返回切片器的x;否则，返回切片器

___

### <a id="y" name="y"></a> y

▸ **y**(`value?`): `any`

获取或设置切片器的y

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值，返回切片器的y;否则，返回切片器
