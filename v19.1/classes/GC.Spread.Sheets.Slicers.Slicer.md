# Class: Slicer

[Sheets](../modules/GC.Spread.Sheets.md).[Slicers](../modules/GC.Spread.Sheets.Slicers.md).Slicer

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Slicers.Slicer.md#constructor)

### Methods

- [allowMove](GC.Spread.Sheets.Slicers.Slicer.md#allowmove)
- [allowResize](GC.Spread.Sheets.Slicers.Slicer.md#allowresize)
- [captionName](GC.Spread.Sheets.Slicers.Slicer.md#captionname)
- [columnCount](GC.Spread.Sheets.Slicers.Slicer.md#columncount)
- [columnName](GC.Spread.Sheets.Slicers.Slicer.md#columnname)
- [disableResizingAndMoving](GC.Spread.Sheets.Slicers.Slicer.md#disableresizingandmoving)
- [dynamicMove](GC.Spread.Sheets.Slicers.Slicer.md#dynamicmove)
- [dynamicSize](GC.Spread.Sheets.Slicers.Slicer.md#dynamicsize)
- [endColumn](GC.Spread.Sheets.Slicers.Slicer.md#endcolumn)
- [endColumnOffset](GC.Spread.Sheets.Slicers.Slicer.md#endcolumnoffset)
- [endRow](GC.Spread.Sheets.Slicers.Slicer.md#endrow)
- [endRowOffset](GC.Spread.Sheets.Slicers.Slicer.md#endrowoffset)
- [height](GC.Spread.Sheets.Slicers.Slicer.md#height)
- [isLocked](GC.Spread.Sheets.Slicers.Slicer.md#islocked)
- [isSelected](GC.Spread.Sheets.Slicers.Slicer.md#isselected)
- [isVisible](GC.Spread.Sheets.Slicers.Slicer.md#isvisible)
- [itemHeight](GC.Spread.Sheets.Slicers.Slicer.md#itemheight)
- [multiSelect](GC.Spread.Sheets.Slicers.Slicer.md#multiselect)
- [name](GC.Spread.Sheets.Slicers.Slicer.md#name)
- [nameInFormula](GC.Spread.Sheets.Slicers.Slicer.md#nameinformula)
- [position](GC.Spread.Sheets.Slicers.Slicer.md#position)
- [refresh](GC.Spread.Sheets.Slicers.Slicer.md#refresh)
- [sheet](GC.Spread.Sheets.Slicers.Slicer.md#sheet)
- [showHeader](GC.Spread.Sheets.Slicers.Slicer.md#showheader)
- [showNoDataItems](GC.Spread.Sheets.Slicers.Slicer.md#shownodataitems)
- [showNoDataItemsInLast](GC.Spread.Sheets.Slicers.Slicer.md#shownodataitemsinlast)
- [sortState](GC.Spread.Sheets.Slicers.Slicer.md#sortstate)
- [sourceName](GC.Spread.Sheets.Slicers.Slicer.md#sourcename)
- [startColumn](GC.Spread.Sheets.Slicers.Slicer.md#startcolumn)
- [startColumnOffset](GC.Spread.Sheets.Slicers.Slicer.md#startcolumnoffset)
- [startRow](GC.Spread.Sheets.Slicers.Slicer.md#startrow)
- [startRowOffset](GC.Spread.Sheets.Slicers.Slicer.md#startrowoffset)
- [style](GC.Spread.Sheets.Slicers.Slicer.md#style)
- [toImageSrc](GC.Spread.Sheets.Slicers.Slicer.md#toimagesrc)
- [toImageSrcAsync](GC.Spread.Sheets.Slicers.Slicer.md#toimagesrcasync)
- [visuallyNoDataItems](GC.Spread.Sheets.Slicers.Slicer.md#visuallynodataitems)
- [width](GC.Spread.Sheets.Slicers.Slicer.md#width)
- [x](GC.Spread.Sheets.Slicers.Slicer.md#x)
- [y](GC.Spread.Sheets.Slicers.Slicer.md#y)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Slicer**()

表示一个表格项目切片器。

## Methods

### <a id="allowmove" name="allowmove"></a> allowMove

▸ **allowMove**(`value?`): `any`

获取或设置切片器的allowMove属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.allowMove();
console.log(oldValue);
slicer.allowMove(false);
var newValue = slicer.allowMove();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的allowMove属性。切片器的allowMove属性指定是否允许用户移动切片器，启用或禁用重新定位功能。 |

#### Returns

`any`

如果未设置值，返回切片器的allowMove属性；否则返回切片器。

___

### <a id="allowresize" name="allowresize"></a> allowResize

▸ **allowResize**(`value?`): `any`

获取或设置切片器的allowResize属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.allowResize();
console.log(oldValue);
slicer.allowResize(false);
var newValue = slicer.allowResize();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的allowResize属性。切片器的allowResize属性指定是否允许用户调整切片器的大小，启用或禁用调整大小功能。 |

#### Returns

`any`

如果未设置值，返回切片器的allowResize属性；否则返回切片器。

___

### <a id="captionname" name="captionname"></a> captionName

▸ **captionName**(`value?`): `any`

获取或设置切片器的captionName属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.captionName();
console.log(oldValue);
slicer.captionName('Slicer_Caption');
var newValue = slicer.captionName();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 切片器的captionName属性。切片器的captionName属性显示在切片器的标题中。 |

#### Returns

`any`

如果未设置值，返回切片器的captionName属性；否则返回切片器。

___

### <a id="columncount" name="columncount"></a> columnCount

▸ **columnCount**(`value?`): `any`

获取或设置切片器的columnCount属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.columnCount();
console.log(oldValue);
slicer.columnCount(3);
var newValue = slicer.columnCount();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的columnCount属性。切片器的columnCount属性指定切片器的列数。 |

#### Returns

`any`

如果未设置值，返回切片器的columnCount属性；否则返回切片器。

___

### <a id="columnname" name="columnname"></a> columnName

▸ **columnName**(): `string`

获取切片器的columnName属性。切片器的columnName属性指定切片器关联的源数据字段中的列的名称。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
console.log(slicer.columnName());
```

#### Returns

`string`

返回

___

### <a id="disableresizingandmoving" name="disableresizingandmoving"></a> disableResizingAndMoving

▸ **disableResizingAndMoving**(`value?`): `any`

获取或设置切片器的disableResizingAndMoving属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.disableResizingAndMoving();
console.log(oldValue);
slicer.disableResizingAndMoving(true);
var newValue = slicer.disableResizingAndMoving();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的disableResizingAndMoving属性。切片器的disableResizingAndMoving属性指定是否允许用户调整切片器的大小或移动切片器，限制其大小或位置的任何更改。 |

#### Returns

`any`

如果未设置值，返回切片器的disableResizingAndMoving属性；否则返回切片器。

___

### <a id="dynamicmove" name="dynamicmove"></a> dynamicMove

▸ **dynamicMove**(`value?`): `any`

获取或设置切片器的dynamicMove属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.dynamicMove();
console.log(oldValue);
slicer.dynamicMove(false);
var newValue = slicer.dynamicMove();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的dynamicMove属性。切片器的dynamicMove属性指定切片器控制是否配置为动态调整其位置或大小，基于关联数据或PivotTable布局的变化。 |

#### Returns

`any`

如果未设置值，返回切片器的dynamicMove属性；否则返回切片器。

___

### <a id="dynamicsize" name="dynamicsize"></a> dynamicSize

▸ **dynamicSize**(`value?`): `any`

获取或设置切片器的dynamicSize属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.dynamicSize();
console.log(oldValue);
slicer.dynamicSize(false);
var newValue = slicer.dynamicSize();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的dynamicSize属性。切片器的dynamicSize属性指定切片器控制是否配置为动态调整其大小，基于关联数据或PivotTable布局的变化。 |

#### Returns

`any`

如果未设置值，返回切片器的dynamicSize属性；否则返回切片器。

___

### <a id="endcolumn" name="endcolumn"></a> endColumn

▸ **endColumn**(`value?`): `any`

获取或设置切片器的endColumn属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.endColumn();
console.log(oldValue);
slicer.endColumn(20);
var newValue = slicer.endColumn();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的endColumnOffset。切片器的endColumnOffset属性指定了切片器右边缘与其所在列起始位置之间的水平偏移量（即距离）。 |

#### Returns

`any`

如果未设置值，返回切片器的endColumn属性；否则返回切片器。

___

### <a id="endcolumnoffset" name="endcolumnoffset"></a> endColumnOffset

▸ **endColumnOffset**(`value?`): `any`

获取或设置切片器的endColumnOffset属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.endColumnOffset();
console.log(oldValue);
slicer.endColumnOffset(5);
var newValue = slicer.endColumnOffset();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的endColumnOffset属性。切片器的endColumnOffset属性指定切片器结束的列索引或工作表中的位置，其中切片器结束或受限。 |

#### Returns

`any`

如果未设置值，返回切片器的endColumnOffset属性；否则返回切片器。

___

### <a id="endrow" name="endrow"></a> endRow

▸ **endRow**(`value?`): `any`

获取或设置切片器的endRow属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.endRow();
console.log(oldValue);
slicer.endRow(20);
var newValue = slicer.endRow();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的endRow属性。切片器的endRow属性指定切片器结束的行索引或工作表中的位置，其中切片器结束或受限。 |

#### Returns

`any`

如果未设置值，返回切片器的endRow属性；否则返回切片器。

___

### <a id="endrowoffset" name="endrowoffset"></a> endRowOffset

▸ **endRowOffset**(`value?`): `any`

获取或设置切片器的endRowOffset属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.endRowOffset();
console.log(oldValue);
slicer.endRowOffset(5);
var newValue = slicer.endRowOffset();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的endRowOffset。切片器的endRowOffset属性指定了垂直偏移量，即切片器下边缘与包含该下边缘的行的上边缘之间的距离。 |

#### Returns

`any`

如果未设置值，返回切片器的endRowOffset属性；否则返回切片器。

___

### <a id="height" name="height"></a> height

▸ **height**(`value?`): `any`

获取或设置切片器的height属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.height();
console.log(oldValue);
slicer.height(200);
var newValue = slicer.height();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的height属性。切片器的height属性指定切片器控制的高度或垂直维度，确定其在y轴上的大小。 |

#### Returns

`any`

如果未设置值，返回切片器的height属性；否则返回切片器。

___

### <a id="islocked" name="islocked"></a> isLocked

▸ **isLocked**(`value?`): `any`

获取或设置切片器的isLocked属性。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
activeSheet.options.isProtected = true;
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: "1968/6/8" },
    { Name: "Betty", City: "NewYork", Birthday: "1972/7/3" },
    { Name: "Alice", City: "Washington", Birthday: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.isLocked();
console.log(oldValue);
slicer.isLocked(false);
var newValue = slicer.isLocked();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的isLocked属性。切片器的isLocked属性指定切片器当前是否锁定或解锁，指示用户是否可以在工作表受保护时更改其设置或选择。 |

#### Returns

`any`

如果未设置值，返回切片器的isLocked属性；否则返回切片器。

___

### <a id="isselected" name="isselected"></a> isSelected

▸ **isSelected**(`value?`): `any`

获取或设置切片器的isSelected属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.isSelected();
console.log(oldValue);
slicer.isSelected(true);
var newValue = slicer.isSelected();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的isSelected属性。切片器的isSelected属性指定切片器中当前是否选择或突出显示特定项目。 |

#### Returns

`any`

如果未设置值，返回切片器的isSelected属性；否则返回切片器。

___

### <a id="isvisible" name="isvisible"></a> isVisible

▸ **isVisible**(`value?`): `any`

获取或设置切片器的isVisible属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.isVisible();
console.log(oldValue);
slicer.isVisible(false);
var newValue = slicer.isVisible();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的isVisible属性。切片器的isVisible属性指定切片器当前是否可见或隐藏。 |

#### Returns

`any`

如果未设置值，返回切片器的isVisible属性；否则返回切片器。

___

### <a id="itemheight" name="itemheight"></a> itemHeight

▸ **itemHeight**(`value?`): `any`

获取或设置切片器的itemHeight属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.itemHeight();
console.log(oldValue);
slicer.itemHeight(34);
var newValue = slicer.itemHeight();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的itemHeight属性。切片器的itemHeight属性指定切片器控制中每个项目或行的高度。 |

#### Returns

`any`

如果未设置值，返回切片器的itemHeight属性；否则返回切片器。

___

### <a id="multiselect" name="multiselect"></a> multiSelect

▸ **multiSelect**(`value?`): `any`

获取或设置切片器的multiSelect属性。

**`example`**
```javascript
var spread = GC.Spread.Sheets.findControl('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: "1968/6/8" },
    { Name: "Betty", City: "NewYork", Birthday: "1972/7/3" },
    { Name: "Alice", City: "Washington", Birthday: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.multiSelect();
console.log(oldValue);
slicer.multiSelect(true);
var newValue = slicer.multiSelect();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的multiSelect属性。切片器的multiSelect属性指定是否可以在切片器中同时选择多个项目。 |

#### Returns

`any`

如果未设置值，返回切片器的multiSelect属性；否则返回切片器。

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置切片器的name属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.name();
console.log(oldValue);
slicer.name('SlicerA');
var newValue = slicer.name();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 切片器的name属性。切片器的name属性指定分配给切片器的唯一标识符或标签，允许在工作簿或编程交互中进行识别和引用。 |

#### Returns

`any`

如果未设置值，返回切片器的name属性；否则返回切片器。

___

### <a id="nameinformula" name="nameinformula"></a> nameInFormula

▸ **nameInFormula**(): `string`

获取切片器的nameInFormula属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
console.log(slicer.nameInFormula());
```

#### Returns

`string`

返回切片器的nameInFormula属性。

___

### <a id="position" name="position"></a> position

▸ **position**(`value?`): `any`

获取或设置切片器的position属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.position();
console.log(oldValue);
slicer.position(new GC.Spread.Sheets.Point(100, 200));
var newValue = slicer.position();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`Point`](GC.Spread.Sheets.Point.md) | 切片器的position属性。切片器的position属性指定切片器在工作表中的位置。 |

#### Returns

`any`

如果未设置值，返回切片器的position属性；否则返回切片器。

___

### <a id="refresh" name="refresh"></a> refresh

▸ **refresh**(): `void`

刷新切片器。

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
// 添加自定义切片器样式
let slicerStyle = spread.customSlicerThemes.add("custom0");
let wholeSlicerStyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
wholeSlicerStyle.backColor = "blue";
slicerStyle.wholeSlicerStyle(wholeSlicerStyle);
// 添加一个切片器
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
slicer.style("custom0");
// 修改自定义切片器样式
spread.customSlicerThemes.all()[0].headerStyle().backColor('red');
// 刷新切片器
slicer.refresh();
```

#### Returns

`void`

___

### <a id="sheet" name="sheet"></a> sheet

▸ **sheet**(): [`Worksheet`](GC.Spread.Sheets.Worksheet.md)

获取切片器的工作表。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
console.log(slicer.sheet().name());
```

#### Returns

[`Worksheet`](GC.Spread.Sheets.Worksheet.md)

返回切片器的工作表。

___

### <a id="showheader" name="showheader"></a> showHeader

▸ **showHeader**(`value?`): `any`

获取或设置切片器的showHeader属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.showHeader();
console.log(oldValue);
slicer.showHeader(false);
var newValue = slicer.showHeader();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的showHeader属性。切片器的showHeader属性指定是否显示切片器中的标题，包括标题和过滤相关控件。 |

#### Returns

`any`

如果未设置值，返回切片器的showHeader属性；否则返回切片器。

___

### <a id="shownodataitems" name="shownodataitems"></a> showNoDataItems

▸ **showNoDataItems**(`value?`): `any`

获取或设置切片器的showNoDataItems，NoDataItems指的是在当前筛选器和数据上下文下被判定为没有对应数据的切片器项（可能是由于其他切片器应用的筛选导致的）。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var condition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.textCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.TextCompareType.contains,expected: '*New*'});
table.rowFilter().addFilterItem(2, condition);
table.rowFilter().filter();
console.log(slicer.showNoDataItems());
slicer.showNoDataItems(false);
console.log(slicer.showNoDataItems());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的showNoDataItems属性。切片器的showNoDataItems属性指定是否显示切片器控制中与连接的PivotTable或数据源中没有关联数据的项目。 |

#### Returns

`any`

如果未设置值，返回切片器的showNoDataItems属性；否则返回切片器。

___

### <a id="shownodataitemsinlast" name="shownodataitemsinlast"></a> showNoDataItemsInLast

▸ **showNoDataItemsInLast**(`value?`): `any`

获取或设置切片器的showNoDataItemsInLast属性。这将决定无数据项（NoDataItems）是放在切片器的开头还是末尾。无数据项指的是在当前筛选器和数据上下文下被判定为没有对应数据的切片器项（可能是由于其他切片器应用的筛选导致的）。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.showNoDataItemsInLast();
console.log(oldValue);
slicer.showNoDataItemsInLast(false);
var newValue = slicer.showNoDataItemsInLast();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的showNoDataItemsInLast属性。切片器的showNoDataItemsInLast属性指定是否在切片器控制列表的末尾显示没有关联数据的项目。 |

#### Returns

`any`

如果未设置值，返回切片器的showNoDataItemsInLast属性；否则返回切片器。

___

### <a id="sortstate" name="sortstate"></a> sortState

▸ **sortState**(`value?`): `any`

获取或设置切片器的sortState属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.sortState();
console.log(oldValue);
slicer.sortState(GC.Spread.Sheets.SortState.descending);
var newValue = slicer.sortState();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SortState`](../enums/GC.Spread.Sheets.SortState.md) | 切片器的sortState属性。切片器的sortState属性指定应用于切片器中项目的当前排序状态，指示它们是否按升序、降序或未排序。 |

#### Returns

`any`

如果未设置值，返回切片器的sortState属性；否则返回切片器。

___

### <a id="sourcename" name="sourcename"></a> sourceName

▸ **sourceName**(): `string`

获取切片器的sourceName属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
console.log(slicer.sourceName());
```

#### Returns

`string`

返回切片器的sourceName属性。

___

### <a id="startcolumn" name="startcolumn"></a> startColumn

▸ **startColumn**(`value?`): `any`

获取或设置切片器的startColumn属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.startColumn();
console.log(oldValue);
slicer.startColumn(10);
var newValue = slicer.startColumn();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的startColumn属性。切片器的startColumn属性指定切片器锚定的起始列索引或工作表中的位置。 |

#### Returns

`any`

如果未设置值，返回切片器的startColumn属性；否则返回切片器。

___

### <a id="startcolumnoffset" name="startcolumnoffset"></a> startColumnOffset

▸ **startColumnOffset**(`value?`): `any`

获取或设置切片器的起始列偏移量。起始列偏移量指定切片器左上角相对于其锚定的工作表单元格左上角的水平偏移（沿列方向）。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.startColumnOffset();
console.log(oldValue);
slicer.startColumnOffset(15);
var newValue = slicer.startColumnOffset();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的startColumnOffset属性。切片器的startColumnOffset属性指定切片器锚定的起始列索引或工作表中的位置。 |

#### Returns

`any`

如果未设置值，返回切片器的startColumnOffset属性；否则返回切片器。

___

### <a id="startrow" name="startrow"></a> startRow

▸ **startRow**(`value?`): `any`

获取或设置切片器的startRow属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.startRow();
console.log(oldValue);
slicer.startRow(10);
var newValue = slicer.startRow();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的startRow属性。切片器的startRow属性指定切片器锚定的起始行索引或工作表中的位置。 |

#### Returns

`any`

如果未设置值，返回切片器的startRow属性；否则返回切片器。

___

### <a id="startrowoffset" name="startrowoffset"></a> startRowOffset

▸ **startRowOffset**(`value?`): `any`

获取或设置切片器的startRowOffset。startRowOffset指定切片器左上角相对于其所锚定的工作表单元格左上角的垂直偏移量（沿行方向）。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.startRowOffset();
console.log(oldValue);
slicer.startRowOffset(15);
var newValue = slicer.startRowOffset();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的startRowOffset属性。切片器的startRowOffset属性指定切片器锚定的起始行索引或工作表中的位置。 |

#### Returns

`any`

如果未设置值，返回切片器的startRowOffset属性；否则返回切片器。

___

### <a id="style" name="style"></a> style

▸ **style**(`value?`): `any`

获取或设置切片器的style属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");

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
| `value?` | `string` \| [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md) | 切片器的style属性。切片器的style属性指定应用于切片器控制的可视化外观和格式化样式，定义其整体外观和呈现。 |

#### Returns

`any`

如果未设置值，返回切片器的style属性；否则返回切片器。

___

### <a id="toimagesrc" name="toimagesrc"></a> toImageSrc

▸ **toImageSrc**(): `string`

获取切片器的Image src属性。

**`example`**
```javascript
let slicerImageSrc = sheet.slicers.all()[0].toImageSrc();
```

#### Returns

`string`

返回切片器的Image src属性。

___

### <a id="toimagesrcasync" name="toimagesrcasync"></a> toImageSrcAsync

▸ **toImageSrcAsync**(): `Promise`<`string`\>

获取切片器的Image src属性。

**`example`**
```javascript
let slicerImageSrc = await sheet.slicers.all()[0].toImageSrcAsync();
```

#### Returns

`Promise`<`string`\>

返回切片器的Image src属性。

___

### <a id="visuallynodataitems" name="visuallynodataitems"></a> visuallyNoDataItems

▸ **visuallyNoDataItems**(`value?`): `any`

获取或设置切片器的visuallyNoDataItems。NoDataItems表示在当前筛选器和数据上下文中被判定为没有对应数据的切片器项（可能是由于其他切片器应用的筛选）。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.visuallyNoDataItems();
console.log(oldValue);
slicer.visuallyNoDataItems(false);
var newValue = slicer.visuallyNoDataItems();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 切片器的visuallyNoDataItems属性。切片器的visuallyNoDataItems属性指定切片器控制中与连接的PivotTable或数据源中没有关联数据的项目。 |

#### Returns

`any`

如果未设置值，返回切片器的visuallyNoDataItems属性；否则返回切片器。

___

### <a id="width" name="width"></a> width

▸ **width**(`value?`): `any`

获取或设置切片器的width属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.width();
console.log(oldValue);
slicer.width(200);
var newValue = slicer.width();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的width属性。切片器的width属性指定切片器的水平维度或宽度，确定其在x轴上的大小。 |

#### Returns

`any`

如果未设置值，返回切片器的width属性；否则返回切片器。

___

### <a id="x" name="x"></a> x

▸ **x**(`value?`): `any`

获取或设置切片器的x属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.x();
console.log(oldValue);
slicer.x(100);
var newValue = slicer.x();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的x属性。切片器的x属性指定切片器在工作表中的水平位置或坐标。 |

#### Returns

`any`

如果未设置值，返回切片器的x属性；否则返回切片器。

___

### <a id="y" name="y"></a> y

▸ **y**(`value?`): `any`

获取或设置切片器的y属性。

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
var slicer = activeSheet.slicers.add("slicer", "table1", "Name");
var oldValue = slicer.y();
console.log(oldValue);
slicer.y(100);
var newValue = slicer.y();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 切片器的y属性。切片器的y属性指定切片器在工作表中的垂直位置或坐标。 |

#### Returns

`any`

如果未设置值，返回切片器的y属性；否则返回切片器。
