# Class: PivotTableItemSlicer

[Spread](../modules/GC.Spread.md).[Pivot](../modules/GC.Spread.Pivot.md).PivotTableItemSlicer

## Table of contents

### Constructors

- [constructor](GC.Spread.Pivot.PivotTableItemSlicer.md#constructor)

### Methods

- [allowMove](GC.Spread.Pivot.PivotTableItemSlicer.md#allowmove)
- [allowResize](GC.Spread.Pivot.PivotTableItemSlicer.md#allowresize)
- [captionName](GC.Spread.Pivot.PivotTableItemSlicer.md#captionname)
- [columnCount](GC.Spread.Pivot.PivotTableItemSlicer.md#columncount)
- [connectPivotTable](GC.Spread.Pivot.PivotTableItemSlicer.md#connectpivottable)
- [disableResizingAndMoving](GC.Spread.Pivot.PivotTableItemSlicer.md#disableresizingandmoving)
- [disconnectPivotTable](GC.Spread.Pivot.PivotTableItemSlicer.md#disconnectpivottable)
- [dynamicMove](GC.Spread.Pivot.PivotTableItemSlicer.md#dynamicmove)
- [dynamicSize](GC.Spread.Pivot.PivotTableItemSlicer.md#dynamicsize)
- [endColumn](GC.Spread.Pivot.PivotTableItemSlicer.md#endcolumn)
- [endColumnOffset](GC.Spread.Pivot.PivotTableItemSlicer.md#endcolumnoffset)
- [endRow](GC.Spread.Pivot.PivotTableItemSlicer.md#endrow)
- [endRowOffset](GC.Spread.Pivot.PivotTableItemSlicer.md#endrowoffset)
- [getAllConnectedPivotTables](GC.Spread.Pivot.PivotTableItemSlicer.md#getallconnectedpivottables)
- [getAllPivotTables](GC.Spread.Pivot.PivotTableItemSlicer.md#getallpivottables)
- [getConnectedPivotTableNameList](GC.Spread.Pivot.PivotTableItemSlicer.md#getconnectedpivottablenamelist)
- [getStyleName](GC.Spread.Pivot.PivotTableItemSlicer.md#getstylename)
- [height](GC.Spread.Pivot.PivotTableItemSlicer.md#height)
- [isConnectedPivotTable](GC.Spread.Pivot.PivotTableItemSlicer.md#isconnectedpivottable)
- [isLocked](GC.Spread.Pivot.PivotTableItemSlicer.md#islocked)
- [isSelected](GC.Spread.Pivot.PivotTableItemSlicer.md#isselected)
- [isVisible](GC.Spread.Pivot.PivotTableItemSlicer.md#isvisible)
- [itemHeight](GC.Spread.Pivot.PivotTableItemSlicer.md#itemheight)
- [multiSelect](GC.Spread.Pivot.PivotTableItemSlicer.md#multiselect)
- [name](GC.Spread.Pivot.PivotTableItemSlicer.md#name)
- [nameInFormula](GC.Spread.Pivot.PivotTableItemSlicer.md#nameinformula)
- [position](GC.Spread.Pivot.PivotTableItemSlicer.md#position)
- [refresh](GC.Spread.Pivot.PivotTableItemSlicer.md#refresh)
- [sheet](GC.Spread.Pivot.PivotTableItemSlicer.md#sheet)
- [showHeader](GC.Spread.Pivot.PivotTableItemSlicer.md#showheader)
- [showNoDataItems](GC.Spread.Pivot.PivotTableItemSlicer.md#shownodataitems)
- [showNoDataItemsInLast](GC.Spread.Pivot.PivotTableItemSlicer.md#shownodataitemsinlast)
- [sortState](GC.Spread.Pivot.PivotTableItemSlicer.md#sortstate)
- [sourceName](GC.Spread.Pivot.PivotTableItemSlicer.md#sourcename)
- [startColumn](GC.Spread.Pivot.PivotTableItemSlicer.md#startcolumn)
- [startColumnOffset](GC.Spread.Pivot.PivotTableItemSlicer.md#startcolumnoffset)
- [startRow](GC.Spread.Pivot.PivotTableItemSlicer.md#startrow)
- [startRowOffset](GC.Spread.Pivot.PivotTableItemSlicer.md#startrowoffset)
- [style](GC.Spread.Pivot.PivotTableItemSlicer.md#style)
- [visuallyNoDataItems](GC.Spread.Pivot.PivotTableItemSlicer.md#visuallynodataitems)
- [width](GC.Spread.Pivot.PivotTableItemSlicer.md#width)
- [x](GC.Spread.Pivot.PivotTableItemSlicer.md#x)
- [y](GC.Spread.Pivot.PivotTableItemSlicer.md#y)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new PivotTableItemSlicer**()

透视表切片器

## Methods

### <a id="allowmove" name="allowmove"></a> allowMove

▸ **allowMove**(`value?`): `any`

获取或设置切片器的是否允许移动选项

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
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

如果缺省参数，则返回切片器的是否移动选项值；否则，返回切片器对象。

___

### <a id="allowresize" name="allowresize"></a> allowResize

▸ **allowResize**(`value?`): `any`

获取或设置切片器的是否允许调整大小选项

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
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

如果缺省参数，则返回切片器的是否允许调整大小选项值；否则，返回切片器对象。

___

### <a id="captionname" name="captionname"></a> captionName

▸ **captionName**(`value?`): `any`

获取或设置切片器的标题名称

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.captionName();
console.log(oldValue);
slicer.captionName('Slicer_Caption');
var newValue = slicer.captionName();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果缺省参数，则返回切片器的标题名称；否则，返回切片器对象。

___

### <a id="columncount" name="columncount"></a> columnCount

▸ **columnCount**(`value?`): `any`

获取或设置切片器的列数

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.columnCount();
console.log(oldValue);
slicer.columnCount(3);
var newValue = slicer.columnCount();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果缺省参数，则返回切片器的列数；否则，返回切片器对象。

___

### <a id="connectpivottable" name="connectpivottable"></a> connectPivotTable

▸ **connectPivotTable**(`ptName`): `void`

绑定透视表

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);

slicer.connectPivotTable('pivotTable1');
slicer.isConnectedPivotTable('pivotTable1');
slicer.disconnectPivotTable('pivotTable1');
slicer.isConnectedPivotTable('pivotTable1');
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

获取或设置切片器的禁止移动或调整大小选项

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.disableResizingAndMoving();
console.log(oldValue);
slicer.disableResizingAndMoving(true);
var newValue = slicer.disableResizingAndMoving();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果缺省参数，则返回切片器的禁止移动和调整大小选项值；否则，返回切片器对象。

___

### <a id="disconnectpivottable" name="disconnectpivottable"></a> disconnectPivotTable

▸ **disconnectPivotTable**(`ptName`): `void`

解绑透视表

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);

slicer.connectPivotTable('pivotTable1');
slicer.isConnectedPivotTable('pivotTable1');
slicer.disconnectPivotTable('pivotTable1');
slicer.isConnectedPivotTable('pivotTable1');
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

获取或设置切片器的动态移动选项

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
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

如果缺省参数，则返回切片器的动态移动选项值；否则，返回切片器对象。

___

### <a id="dynamicsize" name="dynamicsize"></a> dynamicSize

▸ **dynamicSize**(`value?`): `any`

获取或设置切片器的动态大小选项

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
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

如果缺省参数，则返回切片器的动态大小选项值；否则，返回切片器对象。

___

### <a id="endcolumn" name="endcolumn"></a> endColumn

▸ **endColumn**(`value?`): `any`

获取或设置切片器的结束列

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.endColumn();
console.log(oldValue);
slicer.endColumn(20);
var newValue = slicer.endColumn();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果缺省参数，则返回切片器的结束列；否则，返回切片器对象。

___

### <a id="endcolumnoffset" name="endcolumnoffset"></a> endColumnOffset

▸ **endColumnOffset**(`value?`): `any`

获取或设置切片器的结束列偏移值

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.endColumnOffset();
console.log(oldValue);
slicer.endColumnOffset(5);
var newValue = slicer.endColumnOffset();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果缺省参数，则返回切片器的结束列偏移量；否则，返回切片器对象。

___

### <a id="endrow" name="endrow"></a> endRow

▸ **endRow**(`value?`): `any`

获取或设置切片器的结束行

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.endRow();
console.log(oldValue);
slicer.endRow(20);
var newValue = slicer.endRow();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果缺省参数，则返回切片器的结束行；否则，返回切片器对象。

___

### <a id="endrowoffset" name="endrowoffset"></a> endRowOffset

▸ **endRowOffset**(`value?`): `any`

获取或设置切片器的结束行偏移量

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
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

如果缺省参数，则返回切片器的结束行偏移量；否则，返回切片器对象。

___

### <a id="getallconnectedpivottables" name="getallconnectedpivottables"></a> getAllConnectedPivotTables

▸ **getAllConnectedPivotTables**(): [`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)[]

获取所有绑定的透视表

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);

slicer.connectPivotTable('pivotTable1');
slicer.isConnectedPivotTable('pivotTable1');
console.log(slicer.getAllConnectedPivotTables());
slicer.disconnectPivotTable('pivotTable1');
slicer.isConnectedPivotTable('pivotTable1');
console.log(slicer.getAllConnectedPivotTables());
```

#### Returns

[`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)[]

与切片器绑定的透视表数组

___

### <a id="getallpivottables" name="getallpivottables"></a> getAllPivotTables

▸ **getAllPivotTables**(): [`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)[]

获取所有透视表，无论是否绑定

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);

slicer.connectPivotTable('pivotTable1');
slicer.isConnectedPivotTable('pivotTable1');
console.log(slicer.getAllPivotTables());
slicer.disconnectPivotTable('pivotTable1');
slicer.isConnectedPivotTable('pivotTable1');
console.log(slicer.getAllPivotTables());
```

#### Returns

[`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)[]

与切片器使用相同数据源的透视表

___

### <a id="getconnectedpivottablenamelist" name="getconnectedpivottablenamelist"></a> getConnectedPivotTableNameList

▸ **getConnectedPivotTableNameList**(): `string`[]

获取所有绑定的透视表名称

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);

slicer.connectPivotTable('pivotTable1');
slicer.isConnectedPivotTable('pivotTable1');
console.log(slicer.getConnectedPivotTableNameList());
slicer.disconnectPivotTable('pivotTable1');
slicer.isConnectedPivotTable('pivotTable1');
console.log(slicer.getConnectedPivotTableNameList());
```

#### Returns

`string`[]

与切片器绑定的数据透视表名称列表

___

### <a id="getstylename" name="getstylename"></a> getStyleName

▸ **getStyleName**(): `undefined` \| `string`

获取或设置数据透视表项目切片器的样式名称。

#### Returns

`undefined` \| `string`

返回数据透视表项目切片器样式名称。
___

### <a id="height" name="height"></a> height

▸ **height**(`value?`): `any`

获取或设置切片器的高度

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.height();
console.log(oldValue);
slicer.height(200);
var newValue = slicer.height();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果缺省参数，则返回切片器的高度；否则，返回切片器对象。

___

### <a id="isconnectedpivottable" name="isconnectedpivottable"></a> isConnectedPivotTable

▸ **isConnectedPivotTable**(`ptName`): `boolean`

透视表是否与切片器绑定

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);

slicer.connectPivotTable('pivotTable1');
slicer.isConnectedPivotTable('pivotTable1');
slicer.disconnectPivotTable('pivotTable1');
slicer.isConnectedPivotTable('pivotTable1');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ptName` | `string` | 透视表的名称 |

#### Returns

`boolean`

数据透视表是否与切片器绑定

___

### <a id="islocked" name="islocked"></a> isLocked

▸ **isLocked**(`value?`): `any`

获取或设置切片器的锁定状态

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
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

如果缺省参数，返回切片器的锁定属性值；否则，返回切片器对象。

___

### <a id="isselected" name="isselected"></a> isSelected

▸ **isSelected**(`value?`): `any`

获取或设置切片器的选择状态

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.isSelected();
console.log(oldValue);
slicer.isSelected(true);
var newValue = slicer.isSelected();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果缺省参数，则返回切片器的选择状态；否则，返回切片器对象。

___

### <a id="isvisible" name="isvisible"></a> isVisible

▸ **isVisible**(`value?`): `any`

获取或设置切片器的可视状态

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
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

如果缺省参数，则返回切片器的可视状态；否则，返回切片器对象。

___

### <a id="itemheight" name="itemheight"></a> itemHeight

▸ **itemHeight**(`value?`): `any`

获取或设置切片器中项目的高度

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.itemHeight();
console.log(oldValue);
slicer.itemHeight(34);
var newValue = slicer.itemHeight();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果缺省参数，则返回切片器的项目高度；否则，返回切片器对象。

___

### <a id="multiselect" name="multiselect"></a> multiSelect

▸ **multiSelect**(`value?`): `any`

获取或设置切片器的是否允许多选选项

**`example`**
```
var spread = GC.Spread.Sheets.findControl('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: "1968/6/8" },
    { Name: "Betty", City: "NewYork", Birthday: "1972/7/3" },
    { Name: "Alice", City: "Washington", Birthday: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.multiSelect();
console.log(oldValue);
slicer.multiSelect(true);
var newValue = slicer.multiSelect();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果缺省参数，则返回切片器的是否允许多选选项值；否则，返回切片器对象。

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置切片器的名称

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.name();
console.log(oldValue);
slicer.name('SlicerA');
var newValue = slicer.name();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果缺省参数，则返回切片器的名称；否则，返回切片器对象。

___

### <a id="nameinformula" name="nameinformula"></a> nameInFormula

▸ **nameInFormula**(): `string`

获取切片器在公式中使用的名称

#### Returns

`string`

返回切片器在公式中使用的名称

___

### <a id="position" name="position"></a> position

▸ **position**(`value?`): `any`

获取或设置切片器的位置

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.position();
console.log(oldValue);
slicer.position(new GC.Spread.Sheets.Point(100, 200));
var newValue = slicer.position();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`Point`](GC.Spread.Sheets.Point.md) |

#### Returns

`any`

如果缺省参数，则返回切片器的位置；否则，返回切片器对象。

___

### <a id="refresh" name="refresh"></a> refresh

▸ **refresh**(): `void`

刷新切片器

#### Returns

`void`

___

### <a id="sheet" name="sheet"></a> sheet

▸ **sheet**(): [`Worksheet`](GC.Spread.Sheets.Worksheet.md)

获取切片器所在工作表

#### Returns

[`Worksheet`](GC.Spread.Sheets.Worksheet.md)

返回工作表

___

### <a id="showheader" name="showheader"></a> showHeader

▸ **showHeader**(`value?`): `any`

获取或设置切片器的是否显示标题选项

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
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

如果缺省参数，则返回切片器的是否显示标题选项值；否则，返回切片器对象。

___

### <a id="shownodataitems" name="shownodataitems"></a> showNoDataItems

▸ **showNoDataItems**(`value?`): `any`

获取或设置切片器是否显示无数据项选项

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.showNoDataItems();
console.log(oldValue);
slicer.showNoDataItems(false);
var newValue = slicer.showNoDataItems();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果缺省参数，则返回切片器的是否显示无数据项选项值；否则，返回切片器对象。

___

### <a id="shownodataitemsinlast" name="shownodataitemsinlast"></a> showNoDataItemsInLast

▸ **showNoDataItemsInLast**(`value?`): `any`

获取或设置切片器是否在最后显示无数据项选项

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.showNoDataItemsInLast();
console.log(oldValue);
slicer.showNoDataItemsInLast(false);
var newValue = slicer.showNoDataItemsInLast();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果缺省参数，则返回切片器的是否在最后显示无数据项选项值；否则，返回切片器对象。

___

### <a id="sortstate" name="sortstate"></a> sortState

▸ **sortState**(`value?`): `any`

获取或设置切片器的排序状态

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.sortState();
console.log(oldValue);
slicer.sortState(GC.Spread.Sheets.SortState.descending);
var newValue = slicer.sortState();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SortState`](../enums/GC.Spread.Sheets.SortState.md) |

#### Returns

`any`

如果缺省参数，则返回切片器的排序状态值；否则，返回切片器对象。

___

### <a id="sourcename" name="sourcename"></a> sourceName

▸ **sourceName**(): `string`

获取切片器的 SourceName 属性。SourceName 属性是指与切片器关联的源数据字段的名称。

#### Returns

`string`

返回与切片器关联的源数据字段的名称

___

### <a id="startcolumn" name="startcolumn"></a> startColumn

▸ **startColumn**(`value?`): `any`

获取或设置切片器的起始列

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.startColumn();
console.log(oldValue);
slicer.startColumn(10);
var newValue = slicer.startColumn();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果缺省参数，则返回切片器的起始列；否则，返回切片器对象。

___

### <a id="startcolumnoffset" name="startcolumnoffset"></a> startColumnOffset

▸ **startColumnOffset**(`value?`): `any`

获取或设置切片器的起始列偏移量

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
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

如果缺省参数，则返回切片器的起始列偏移量；否则，返回切片器对象。

___

### <a id="startrow" name="startrow"></a> startRow

▸ **startRow**(`value?`): `any`

获取或设置切片器的起始行

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.startRow();
console.log(oldValue);
slicer.startRow(10);
var newValue = slicer.startRow();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果缺省参数，则返回切片器的起始行；否则，返回切片器对象。

___

### <a id="startrowoffset" name="startrowoffset"></a> startRowOffset

▸ **startRowOffset**(`value?`): `any`

获取或设置切片器的起始行偏移量

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.startRowOffset();
console.log(oldValue);
slicer.startRowOffset(15);
var newValue = slicer.startRowOffset();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果缺省参数，则返回切片器的起始行偏移量；否则，返回切片器对象。

___

### <a id="style" name="style"></a> style

▸ **style**(`value?`): `any`

获取或设置切片器的样式

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);

var style = new GC.Spread.Sheets.Slicers.SlicerStyle();
style.wholeSlicerStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('red', 'blue', '16pt Calibri'));
style.headerStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo(undefined, 'green'));
style.selectedItemWithDataStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo(undefined, undefined, undefined, new GC.Spread.Sheets.LineBorder('pink', GC.Spread.Sheets.LineStyle.double)));

var oldValue = slicer.style();
console.log(oldValue);
slicer.style(style);
var newValue = slicer.style();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md) |

#### Returns

`any`

如果缺省参数，则返回切片器的样式；否则，返回切片器对象。

___

### <a id="visuallynodataitems" name="visuallynodataitems"></a> visuallyNoDataItems

▸ **visuallyNoDataItems**(`value?`): `any`

获取或设置切片器中视觉上无数据的项选项

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.visuallyNoDataItems();
console.log(oldValue);
slicer.visuallyNoDataItems(false);
var newValue = slicer.visuallyNoDataItems();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果缺省参数，则返回切片器中视觉上无数据的项选项值；否则，返回切片器对象。

___

### <a id="width" name="width"></a> width

▸ **width**(`value?`): `any`

获取或设置切片器的宽度

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.width();
console.log(oldValue);
slicer.width(200);
var newValue = slicer.width();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果缺省参数，则返回切片器的宽度；否则，返回切片器对象。

___

### <a id="x" name="x"></a> x

▸ **x**(`value?`): `any`

获取或设置切片器的横轴坐标

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.x();
console.log(oldValue);
slicer.x(100);
var newValue = slicer.x();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果缺省参数，则返回切片器的横轴坐标；否则，返回切片器对象。

___

### <a id="y" name="y"></a> y

▸ **y**(`value?`): `any`

获取或设置切片器的纵轴坐标

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.y();
console.log(oldValue);
slicer.y(100);
var newValue = slicer.y();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果缺省参数，则返回切片器的纵轴坐标；否则，返回切片器对象。
