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

表示数据透视切片器

## Methods

### <a id="allowmove" name="allowmove"></a> allowMove

▸ **allowMove**(`value?`): `any`

获取或设置切片器的允许移动属性

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { 姓名: "Bob", 城市: "纽约", 生日: "1968/6/8" },
    { 姓名: "Betty", 城市: "纽约", 生日: "1972/7/3" },
    { 姓名: "Alice", 城市: "华盛顿", 生日: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "姓名", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.allowMove();
console.log(oldValue);
slicer.allowMove(false);
var newValue = slicer.allowMove();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的允许移动属性值。该属性指定是否允许用户移动切片器，启用或禁用重新定位功能 |

#### Returns

`any`

未设置值时返回允许移动状态；否则返回切片器实例

___

### <a id="allowresize" name="allowresize"></a> allowResize

▸ **allowResize**(`value?`): `any`

获取或设置切片器的允许调整大小属性

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { 姓名: "Bob", 城市: "纽约", 生日: "1968/6/8" },
    { 姓名: "Betty", 城市: "纽约", 生日: "1972/7/3" },
    { 姓名: "Alice", 城市: "华盛顿", 生日: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "姓名", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.allowResize();
console.log(oldValue);
slicer.allowResize(false);
var newValue = slicer.allowResize();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的允许调整大小属性值。该属性指定是否允许用户调整切片器的大小，启用或禁用调整大小功能 |

#### Returns

`any`

未设置值时返回允许调整大小状态；否则返回切片器实例

___

### <a id="captionname" name="captionname"></a> captionName

▸ **captionName**(`value?`): `any`

获取或设置切片器的标题名称

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { 姓名: "Bob", 城市: "纽约", 生日: "1968/6/8" },
    { 姓名: "Betty", 城市: "纽约", 生日: "1972/7/3" },
    { 姓名: "Alice", 城市: "华盛顿", 生日: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "姓名", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.captionName();
console.log(oldValue);
slicer.captionName('切片器标题');
var newValue = slicer.captionName();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 切片器的标题名称，显示在切片器的标题栏中 |

#### Returns

`any`

未设置值时返回当前标题名称；否则返回切片器实例

___

### <a id="columncount" name="columncount"></a> columnCount

▸ **columnCount**(`value?`): `any`

获取或设置切片器的列数

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { 姓名: "Bob", 城市: "纽约", 生日: "1968/6/8" },
    { 姓名: "Betty", 城市: "纽约", 生日: "1972/7/3" },
    { 姓名: "Alice", 城市: "华盛顿", 生日: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "姓名", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.columnCount();
console.log(oldValue);
slicer.columnCount(3);
var newValue = slicer.columnCount();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的列数 |

#### Returns

`any`

未设置值时返回当前列数；否则返回切片器实例

___

### <a id="connectpivottable" name="connectpivottable"></a> connectPivotTable

▸ **connectPivotTable**(`ptName`): `void`

将数据透视表与切片器连接

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { 姓名: "Bob", 城市: "纽约", 生日: "1968/6/8" },
    { 姓名: "Betty", 城市: "纽约", 生日: "1972/7/3" },
    { 姓名: "Alice", 城市: "华盛顿", 生日: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "姓名", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);

slicer.connectPivotTable('pivotTable1');
slicer.isConnectedPivotTable('pivotTable1');
slicer.disconnectPivotTable('pivotTable1');
slicer.isConnectedPivotTable('pivotTable1');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ptName` | `string` | 数据透视表名称 |

#### Returns

`void`

___

### <a id="disableresizingandmoving" name="disableresizingandmoving"></a> disableResizingAndMoving

▸ **disableResizingAndMoving**(`value?`): `any`

获取或设置切片器的禁用调整大小和移动属性

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { 姓名: "Bob", 城市: "纽约", 生日: "1968/6/8" },
    { 姓名: "Betty", 城市: "纽约", 生日: "1972/7/3" },
    { 姓名: "Alice", 城市: "华盛顿", 生日: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "姓名", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.disableResizingAndMoving();
console.log(oldValue);
slicer.disableResizingAndMoving(true);
var newValue = slicer.disableResizingAndMoving();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的禁用调整大小和移动属性值。该属性指定是否禁止用户调整切片器的大小或移动其位置 |

#### Returns

`any`

未设置值时返回禁用状态；否则返回切片器实例

___

### <a id="disconnectpivottable" name="disconnectpivottable"></a> disconnectPivotTable

▸ **disconnectPivotTable**(`ptName`): `void`

将数据透视表与切片器断开连接

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { 姓名: "Bob", 城市: "纽约", 生日: "1968/6/8" },
    { 姓名: "Betty", 城市: "纽约", 生日: "1972/7/3" },
    { 姓名: "Alice", 城市: "华盛顿", 生日: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "姓名", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);

slicer.connectPivotTable('pivotTable1');
slicer.isConnectedPivotTable('pivotTable1');
slicer.disconnectPivotTable('pivotTable1');
slicer.isConnectedPivotTable('pivotTable1');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ptName` | `string` | 数据透视表名称 |

#### Returns

`void`

___

### <a id="dynamicmove" name="dynamicmove"></a> dynamicMove

▸ **dynamicMove**(`value?`): `any`

获取或设置切片器的动态移动属性

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { 姓名: "Bob", 城市: "纽约", 生日: "1968/6/8" },
    { 姓名: "Betty", 城市: "纽约", 生日: "1972/7/3" },
    { 姓名: "Alice", 城市: "华盛顿", 生日: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "姓名", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.dynamicMove();
console.log(oldValue);
slicer.dynamicMove(false);
var newValue = slicer.dynamicMove();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的动态移动属性值。该属性指定切片器是否配置为根据关联数据或数据透视表布局的变化动态调整其位置或大小 |

#### Returns

`any`

未设置值时返回动态移动状态；否则返回切片器实例

___

### <a id="dynamicsize" name="dynamicsize"></a> dynamicSize

▸ **dynamicSize**(`value?`): `any`

获取或设置切片器的动态大小属性

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { 姓名: "Bob", 城市: "纽约", 生日: "1968/6/8" },
    { 姓名: "Betty", 城市: "纽约", 生日: "1972/7/3" },
    { 姓名: "Alice", 城市: "华盛顿", 生日: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "姓名", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.dynamicSize();
console.log(oldValue);
slicer.dynamicSize(false);
var newValue = slicer.dynamicSize();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的动态大小属性值。该属性指定切片器是否配置为根据关联数据或数据透视表布局的变化动态调整其大小 |

#### Returns

`any`

未设置值时返回动态大小状态；否则返回切片器实例

___

### <a id="endcolumn" name="endcolumn"></a> endColumn

▸ **endColumn**(`value?`): `any`

获取或设置切片器的结束列

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { 姓名: "Bob", 城市: "纽约", 生日: "1968/6/8" },
    { 姓名: "Betty", 城市: "纽约", 生日: "1972/7/3" },
    { 姓名: "Alice", 城市: "华盛顿", 生日: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "姓名", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.endColumn();
console.log(oldValue);
slicer.endColumn(20);
var newValue = slicer.endColumn();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的结束列属性值。该属性指定切片器在工作表中结束或限定的列索引或位置 |

#### Returns

`any`

未设置值时返回结束列索引；否则返回切片器实例

___

### <a id="endcolumnoffset" name="endcolumnoffset"></a> endColumnOffset

▸ **endColumnOffset**(`value?`): `any`

获取或设置切片器的结束列偏移量

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { 姓名: "Bob", 城市: "纽约", 生日: "1968/6/8" },
    { 姓名: "Betty", 城市: "纽约", 生日: "1972/7/3" },
    { 姓名: "Alice", 城市: "华盛顿", 生日: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "姓名", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.endColumnOffset();
console.log(oldValue);
slicer.endColumnOffset(5);
var newValue = slicer.endColumnOffset();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的结束列偏移量属性值。该属性指定切片器在工作表中结束位置与结束列索引之间的水平偏移量或距离 |

#### Returns

`any`

未设置值时返回结束列偏移量；否则返回切片器实例

___

### <a id="endrow" name="endrow"></a> endRow

▸ **endRow**(`value?`): `any`

获取或设置切片器的结束行

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { 姓名: "Bob", 城市: "纽约", 生日: "1968/6/8" },
    { 姓名: "Betty", 城市: "纽约", 生日: "1972/7/3" },
    { 姓名: "Alice", 城市: "华盛顿", 生日: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "姓名", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.endRow();
console.log(oldValue);
slicer.endRow(20);
var newValue = slicer.endRow();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的结束行属性值。该属性指定切片器在工作表中结束或限定的行索引或位置 |

#### Returns

`any`

未设置值时返回结束行索引；否则返回切片器实例

___

### <a id="endrowoffset" name="endrowoffset"></a> endRowOffset

▸ **endRowOffset**(`value?`): `any`

获取或设置切片器的结束行偏移量

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { 姓名: "Bob", 城市: "纽约", 生日: "1968/6/8" },
    { 姓名: "Betty", 城市: "纽约", 生日: "1972/7/3" },
    { 姓名: "Alice", 城市: "华盛顿", 生日: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "姓名", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.endRowOffset();
console.log(oldValue);
slicer.endRowOffset(5);
var newValue = slicer.endRowOffset();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的结束行偏移量属性值。该属性指定切片器在工作表中结束位置与结束行索引之间的垂直偏移量或距离 |

#### Returns

`any`

未设置值时返回结束行偏移量；否则返回切片器实例

___

### <a id="getallconnectedpivottables" name="getallconnectedpivottables"></a> getAllConnectedPivotTables

▸ **getAllConnectedPivotTables**(): [`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)[]

获取所有已连接的数据透视表

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { 姓名: "Bob", 城市: "纽约", 生日: "1968/6/8" },
    { 姓名: "Betty", 城市: "纽约", 生日: "1972/7/3" },
    { 姓名: "Alice", 城市: "华盛顿", 生日: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "姓名", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);

slicer.connectPivotTable('pivotTable1');
slicer.isConnectedPivotTable('pivotTable1');
console.log(slicer.getAllConnectedPivotTables());
slicer.disconnectPivotTable('pivotTable1');
slicer.isConnectedPivotTable('pivotTable1');
console.log(slicer.getAllConnectedPivotTables());
```

#### Returns

[`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)[]

与切片器连接的数据透视表数组

___

### <a id="getallpivottables" name="getallpivottables"></a> getAllPivotTables

▸ **getAllPivotTables**(): [`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)[]

获取所有数据透视表（无论是否连接）

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { 姓名: "Bob", 城市: "纽约", 生日: "1968/6/8" },
    { 姓名: "Betty", 城市: "纽约", 生日: "1972/7/3" },
    { 姓名: "Alice", 城市: "华盛顿", 生日: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "姓名", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);

slicer.connectPivotTable('pivotTable1');
slicer.isConnectedPivotTable('pivotTable1');
console.log(slicer.getAllPivotTables());
slicer.disconnectPivotTable('pivotTable1');
slicer.isConnectedPivotTable('pivotTable1');
console.log(slicer.getAllPivotTables());
```

#### Returns

[`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)[]

与切片器数据源相同的数据透视表数组

___

### <a id="getconnectedpivottablenamelist" name="getconnectedpivottablenamelist"></a> getConnectedPivotTableNameList

▸ **getConnectedPivotTableNameList**(): `string`[]

获取所有已连接数据透视表的名称列表

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { 姓名: "Bob", 城市: "纽约", 生日: "1968/6/8" },
    { 姓名: "Betty", 城市: "纽约", 生日: "1972/7/3" },
    { 姓名: "Alice", 城市: "华盛顿", 生日: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "姓名", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);

slicer.connectPivotTable('pivotTable1');
slicer.isConnectedPivotTable('pivotTable1');
console.log(slicer.getConnectedPivotTableNameList());
slicer.disconnectPivotTable('pivotTable1');
slicer.isConnectedPivotTable('pivotTable1');
console.log(slicer.getConnectedPivotTableNameList());
```

#### Returns

`string`[]

与切片器连接的数据透视表名称数组

___

### <a id="getstylename" name="getstylename"></a> getStyleName

▸ **getStyleName**(): `undefined` \| `string`

获取或设置数据透视表项切片器的样式名称

#### Returns

`undefined` \| `string`

返回数据透视表项切片器的样式名称

___

### <a id="height" name="height"></a> height

▸ **height**(`value?`): `any`

获取或设置切片器的高度

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { 姓名: "Bob", 城市: "纽约", 生日: "1968/6/8" },
    { 姓名: "Betty", 城市: "纽约", 生日: "1972/7/3" },
    { 姓名: "Alice", 城市: "华盛顿", 生日: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "姓名", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.height();
console.log(oldValue);
slicer.height(200);
var newValue = slicer.height();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的高度。该属性指定切片器的垂直尺寸（沿 y 轴的高度） |

#### Returns

`any`

未设置值时返回切片器高度；否则返回切片器实例

___

### <a id="isconnectedpivottable" name="isconnectedpivottable"></a> isConnectedPivotTable

▸ **isConnectedPivotTable**(`ptName`): `boolean`

检查数据透视表是否与切片器连接

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { 姓名: "Bob", 城市: "纽约", 生日: "1968/6/8" },
    { 姓名: "Betty", 城市: "纽约", 生日: "1972/7/3" },
    { 姓名: "Alice", 城市: "华盛顿", 生日: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "姓名", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);

slicer.connectPivotTable('pivotTable1');
slicer.isConnectedPivotTable('pivotTable1'); // 返回 true
slicer.disconnectPivotTable('pivotTable1');
slicer.isConnectedPivotTable('pivotTable1'); // 返回 false
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ptName` | `string` | 数据透视表名称 |

#### Returns

`boolean`

是否已连接

___

### <a id="islocked" name="islocked"></a> isLocked

▸ **isLocked**(`value?`): `any`

获取或设置切片器的锁定状态

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { 姓名: "Bob", 城市: "纽约", 生日: "1968/6/8" },
    { 姓名: "Betty", 城市: "纽约", 生日: "1972/7/3" },
    { 姓名: "Alice", 城市: "华盛顿", 生日: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "姓名", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.isLocked();
console.log(oldValue); // 初始值为 false
slicer.isLocked(true); // 锁定切片器
var newValue = slicer.isLocked();
console.log(newValue); // 返回 true
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否锁定切片器（工作表受保护时限制用户修改） |

#### Returns

`any`

未设置值时返回锁定状态；否则返回切片器实例

___

### <a id="isselected" name="isselected"></a> isSelected

▸ **isSelected**(`value?`): `any`

获取或设置切片器的选中状态

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { 姓名: "Bob", 城市: "纽约", 生日: "1968/6/8" },
    { 姓名: "Betty", 城市: "纽约", 生日: "1972/7/3" },
    { 姓名: "Alice", 城市: "华盛顿", 生日: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "姓名", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.isSelected(); // 初始值为 false
slicer.isSelected(true); // 设置为选中状态
var newValue = slicer.isSelected();
console.log(newValue); // 返回 true
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否选中切片器（用于程序控制可视化状态） |

#### Returns

`any`

未设置值时返回选中状态；否则返回切片器实例

___

### <a id="isvisible" name="isvisible"></a> isVisible

▸ **isVisible**(`value?`): `any`

获取或设置切片器的可见性

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { 姓名: "Bob", 城市: "纽约", 生日: "1968/6/8" },
    { 姓名: "Betty", 城市: "纽约", 生日: "1972/7/3" },
    { 姓名: "Alice", 城市: "华盛顿", 生日: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "姓名", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.isVisible(); // 初始值为 true
slicer.isVisible(false); // 隐藏切片器
var newValue = slicer.isVisible();
console.log(newValue); // 返回 false
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否显示切片器 |

#### Returns

`any`

未设置值时返回可见性状态；否则返回切片器实例

___

### <a id="itemheight" name="itemheight"></a> itemHeight

▸ **itemHeight**(`value?`): `any`

获取或设置切片器中项目的行高

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { 姓名: "Bob", 城市: "纽约", 生日: "1968/6/8" },
    { 姓名: "Betty", 城市: "纽约", 生日: "1972/7/3" },
    { 姓名: "Alice", 城市: "华盛顿", 生日: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "姓名", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.itemHeight(); // 初始值可能为默认行高（如 22）
slicer.itemHeight(34); // 设置行高为 34 像素
var newValue = slicer.itemHeight();
console.log(newValue); // 返回 34
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器内每个项目的高度（像素值） |

#### Returns

`any`

未设置值时返回项目高度；否则返回切片器实例

___

### <a id="multiselect" name="multiselect"></a> multiSelect

▸ **multiSelect**(`value?`): `any`

获取或设置切片器的多选功能

**`example`**
```javascript
var spread = GC.Spread.Sheets.findControl('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { 姓名: "Bob", 城市: "纽约", 生日: "1968/6/8" },
    { 姓名: "Betty", 城市: "纽约", 生日: "1972/7/3" },
    { 姓名: "Alice", 城市: "华盛顿", 生日: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "姓名", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.multiSelect(); // 初始值为 false（单选）
slicer.multiSelect(true); // 启用多选
var newValue = slicer.multiSelect();
console.log(newValue); // 返回 true
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否允许同时选择多个项目 |

#### Returns

`any`

未设置值时返回当前多选状态

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置切片器的名称

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { 姓名: "Bob", 城市: "纽约", 生日: "1968/6/8" },
    { 姓名: "Betty", 城市: "纽约", 生日: "1972/7/3" },
    { 姓名: "Alice", 城市: "华盛顿", 生日: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "姓名", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.name(); // 初始名称如 "Slicer1"
slicer.name('SlicerA'); // 重命名为 "SlicerA"
var newValue = slicer.name();
console.log(newValue); // 返回 "SlicerA"
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 切片器的唯一标识符（用于程序引用） |

#### Returns

`any`

未设置值时返回当前名称；否则返回切片器实例

___

### <a id="nameinformula" name="nameinformula"></a> nameInFormula

▸ **nameInFormula**(): `string`

获取切片器在公式中的引用名称

#### Returns

`string`

切片器的公式引用名称（如 "_SlicerA"）

___

### <a id="position" name="position"></a> position

▸ **position**(`value?`): `any`

获取或设置切片器的位置

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { 姓名: "Bob", 城市: "纽约", 生日: "1968/6/8" },
    { 姓名: "Betty", 城市: "纽约", 生日: "1972/7/3" },
    { 姓名: "Alice", 城市: "华盛顿", 生日: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var pivotTable = activeSheet.pivotTables.add("pivotTable1", "table1", 6, 1);
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "姓名", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.position(); // 初始位置如 {x: 0, y: 0}
slicer.position(new GC.Spread.Sheets.Point(100, 200)); // 移动到坐标 (100, 200)
var newValue = slicer.position();
console.log(newValue.x, newValue.y); // 输出 100 200
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`Point`](GC.Spread.Sheets.Point.md) | 切片器在工作表中的坐标位置（x, y 像素值） |

#### Returns

`any`

未设置值时返回当前位置；否则返回切片器实例

___

### <a id="refresh" name="refresh"></a> refresh

▸ **refresh**(): `void`

刷新切片器。

#### Returns

`void`

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

获取或设置切片器的显示标题。

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.showHeader();
console.log(oldValue);
slicer.showHeader(false);
var newValue = slicer.showHeader();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的显示标题。切片器的 showHeader 属性指定是否在切片器中显示包含标题和筛选相关控件的标头。 |

#### Returns

`any`

如果未设置值，则返回切片器的显示标题；否则返回切片器。

___

### <a id="shownodataitems" name="shownodataitems"></a> showNoDataItems

▸ **showNoDataItems**(`value?`): `any`

获取或设置切片器是否显示无数据项。

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.showNoDataItems();
console.log(oldValue);
slicer.showNoDataItems(false);
var newValue = slicer.showNoDataItems();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的无数据项显示设置。该属性指定是否在切片器控件中显示关联数据透视表或数据源中无关联数据的项。 |

#### Returns

`any`

若未设置值，则返回当前无数据项显示状态；否则返回切片器实例以支持链式调用。

___

### <a id="shownodataitemsinlast" name="shownodataitemsinlast"></a> showNoDataItemsInLast

▸ **showNoDataItemsInLast**(`value?`): `any`

获取或设置切片器是否将无数据项显示在列表末尾。

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.showNoDataItemsInLast();
console.log(oldValue);
slicer.showNoDataItemsInLast(false);
var newValue = slicer.showNoDataItemsInLast();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的无数据项位置设置。该属性指定在展示项时，是否将无关联数据的项显示在切片器控件列表的末尾。 |

#### Returns

`any`

若未设置值，则返回当前无数据项位置状态；否则返回切片器实例以支持链式调用。

___

### <a id="sortstate" name="sortstate"></a> sortState

▸ **sortState**(`value?`): `any`

获取或设置切片器的排序状态。

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.sortState();
console.log(oldValue);
slicer.sortState(GC.Spread.Sheets.SortState.descending);
var newValue = slicer.sortState();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SortState`](../enums/GC.Spread.Sheets.SortState.md) | 切片器的排序状态。该属性指定应用于切片器内项的当前排序方式，包括升序、降序或不排序。 |

#### Returns

`any`

若未设置值，则返回当前排序状态；否则返回切片器实例以支持链式调用。

___

### <a id="sourcename" name="sourcename"></a> sourceName

▸ **sourceName**(): `string`

获取切片器的源字段名称。
切片器的sourceName属性指定与该切片器关联的源数据字段名称。

#### Returns

`string`

返回切片器的源字段名称。

___

### <a id="startcolumn" name="startcolumn"></a> startColumn

▸ **startColumn**(`value?`): `any`

获取或设置切片器的起始列位置。

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.startColumn();
console.log(oldValue);
slicer.startColumn(10);
var newValue = slicer.startColumn();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的起始列索引。该属性指定切片器在工作表中锚定的起始列位置。 |

#### Returns

`any`

若未设置值，则返回当前起始列索引；否则返回切片器实例以支持链式调用。

___

### <a id="startcolumnoffset" name="startcolumnoffset"></a> startColumnOffset

▸ **startColumnOffset**(`value?`): `any`

获取或设置切片器的起始列偏移量。

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.startColumnOffset();
console.log(oldValue);
slicer.startColumnOffset(15);
var newValue = slicer.startColumnOffset();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的起始列偏移量。该属性指定切片器在工作表中相对于起始列索引的水平偏移距离（以像素为单位）。 |

#### Returns

`any`

若未设置值，则返回当前起始列偏移量；否则返回切片器实例以支持链式调用。

___

### <a id="startrow" name="startrow"></a> startRow

▸ **startRow**(`value?`): `any`

获取或设置切片器的起始行。

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.startRow();
console.log(oldValue);
slicer.startRow(10);
var newValue = slicer.startRow();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的起始行。切片器的startRow属性指定了切片器在工作表中锚定的起始行索引或位置。 |

#### Returns

`any`

如果未设置值，则返回切片器的起始行；否则返回切片器。

___

### <a id="startrowoffset" name="startrowoffset"></a> startRowOffset

▸ **startRowOffset**(`value?`): `any`

获取或设置切片器的起始行偏移量。

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.startRowOffset();
console.log(oldValue);
slicer.startRowOffset(15);
var newValue = slicer.startRowOffset();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的起始行偏移量。切片器的startRowOffset属性指定了切片器在工作表中相对于起始行索引的垂直偏移量或距离。 |

#### Returns

`any`

如果未设置值，则返回切片器的起始行偏移量；否则返回切片器。

___

### <a id="style" name="style"></a> style

▸ **style**(`value?`): `any`

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

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` \| [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md) | 切片器的样式或样式名称。切片器的style属性指定了应用于切片器的视觉外观和格式样式，定义了其整体外观和展示效果。 |

#### Returns

`any`

如果未设置样式，则返回切片器的样式；否则返回切片器。

___

### <a id="visuallynodataitems" name="visuallynodataitems"></a> visuallyNoDataItems

▸ **visuallyNoDataItems**(`value?`): `any`

获取或设置切片器对无数据项的视觉处理方式。

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.visuallyNoDataItems();
console.log(oldValue);
slicer.visuallyNoDataItems(false);
var newValue = slicer.visuallyNoDataItems();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的无数据项视觉处理方式。切片器的visuallyNoDataItems属性指定了切片器控件中对无关联数据项的视觉表示或处理方式。 |

#### Returns

`any`

如果未设置值，则返回切片器的无数据项视觉处理方式；否则返回切片器。

___

### <a id="width" name="width"></a> width

▸ **width**(`value?`): `any`

获取或设置切片器的宽度。

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.width();
console.log(oldValue);
slicer.width(200);
var newValue = slicer.width();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的宽度。切片器的width属性指定了切片器的水平尺寸或宽度，决定了其在x轴上的大小。 |

#### Returns

`any`

如果未设置值，则返回切片器的宽度；否则返回切片器。

___

### <a id="x" name="x"></a> x

▸ **x**(`value?`): `any`

获取或设置切片器的x坐标。

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.x();
console.log(oldValue);
slicer.x(100);
var newValue = slicer.x();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的x坐标。切片器的x属性指定了切片器在工作表中左上角的水平位置或坐标。 |

#### Returns

`any`

如果未设置值，则返回切片器的x坐标；否则返回切片器。

___

### <a id="y" name="y"></a> y

▸ **y**(`value?`): `any`

获取或设置切片器的y坐标。

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
var slicer = activeSheet.slicers.add("slicer", "pivotTable1", "Name", GC.Spread.Sheets.Slicers.SlicerStyles.dark1(), GC.Spread.Sheets.Slicers.SlicerType.pivotTable);
var oldValue = slicer.y();
console.log(oldValue);
slicer.y(100);
var newValue = slicer.y();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的y坐标。切片器的y属性指定了切片器在工作表中左上角的垂直位置或坐标。 |

#### Returns

`any`

如果未设置值，则返回切片器的y坐标；否则返回切片器。
