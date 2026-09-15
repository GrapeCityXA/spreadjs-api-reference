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

获取或设置切片器的allowMove

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值,返回切片器的allowMove;否则,返回切片器

___

### <a id="allowresize" name="allowresize"></a> allowResize

▸ **allowResize**(`value?`): `any`

获取或设置切片器的allowResize

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值,返回切片器的allowResize;否则,返回切片器

___

### <a id="captionname" name="captionname"></a> captionName

▸ **captionName**(`value?`): `any`

获取或设置切片器的captionName

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果没有设置值,返回切片器的captionName;否则,返回切片器

___

### <a id="columncount" name="columncount"></a> columnCount

▸ **columnCount**(`value?`): `any`

获取或设置切片器的columnCount

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值,返回切片器的columnCount;否则,返回切片器

___

### <a id="connectpivottable" name="connectpivottable"></a> connectPivotTable

▸ **connectPivotTable**(`ptName`): `void`

用切器关联的透视表

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ptName` | `string` | 透视表的名称 |

#### Returns

`void`

___

### <a id="disableresizingandmoving" name="disableresizingandmoving"></a> disableResizingAndMoving

▸ **disableResizingAndMoving**(`value?`): `any`

获取或设置切片器的disableResizingAndMoving

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值,返回切片器的disableResizingAndMoving;否则,返回切片器

___

### <a id="disconnectpivottable" name="disconnectpivottable"></a> disconnectPivotTable

▸ **disconnectPivotTable**(`ptName`): `void`

获取或设置切片器的disconnectPivotTable

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

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值,返回切片器的dynamicMove;否则,返回切片器

___

### <a id="dynamicsize" name="dynamicsize"></a> dynamicSize

▸ **dynamicSize**(`value?`): `any`

获取或设置切片器的dynamicSize

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值,返回切片器的dynamicSize;否则,返回切片器

___

### <a id="endcolumn" name="endcolumn"></a> endColumn

▸ **endColumn**(`value?`): `any`

获取或设置切片器的endColumn

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值,返回切片器的endColumn;否则,返回切片器

___

### <a id="endcolumnoffset" name="endcolumnoffset"></a> endColumnOffset

▸ **endColumnOffset**(`value?`): `any`

获取或设置切片器的endColumnOffset

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值,返回切片器的endColumnOffset;否则,返回切片器

___

### <a id="endrow" name="endrow"></a> endRow

▸ **endRow**(`value?`): `any`

获取或设置切片器的endRow

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值,返回切片器的endRow;否则,返回切片器

___

### <a id="endrowoffset" name="endrowoffset"></a> endRowOffset

▸ **endRowOffset**(`value?`): `any`

获取或设置切片器的endRowOffset

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值,返回切片器的endRowOffset;否则,返回切片器

___

### <a id="getallconnectedpivottables" name="getallconnectedpivottables"></a> getAllConnectedPivotTables

▸ **getAllConnectedPivotTables**(): [`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)[]

获得所有关联的透视表

#### Returns

[`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)[]

与切片器相连的透视表

___

### <a id="getallpivottables" name="getallpivottables"></a> getAllPivotTables

▸ **getAllPivotTables**(): [`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)[]

获取所有透视表,无论是否关联

#### Returns

[`PivotTable`](GC.Spread.Pivot.PivotTable-1.md)[]

与切片器相同数据源的透视表

___

### <a id="getconnectedpivottablenamelist" name="getconnectedpivottablenamelist"></a> getConnectedPivotTableNameList

▸ **getConnectedPivotTableNameList**(): `string`[]

获得所有关联的透视表名称

#### Returns

`string`[]

name 与切片器连接的数据透视表列表

___

### <a id="height" name="height"></a> height

▸ **height**(`value?`): `any`

获取或设置切片器的高度

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值,返回切片器的高度;否则,返回切片器

___

### <a id="isconnectedpivottable" name="isconnectedpivottable"></a> isConnectedPivotTable

▸ **isConnectedPivotTable**(`ptName`): `boolean`

检查透视表是否与切片器关联

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ptName` | `string` | 透视表的名称 |

#### Returns

`boolean`

___

### <a id="islocked" name="islocked"></a> isLocked

▸ **isLocked**(`value?`): `any`

获取或设置切片器的isLocked

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值,返回切片器的isLocked;否则,返回切片器

___

### <a id="isselected" name="isselected"></a> isSelected

▸ **isSelected**(`value?`): `any`

获取或设置切片器的isSelected

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值,返回切片器的isSelected;否则,返回切片器

___

### <a id="isvisible" name="isvisible"></a> isVisible

▸ **isVisible**(`value?`): `any`

获取或设置切片器的isVisible

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值,返回切片器的isVisible;否则,返回切片器

___

### <a id="itemheight" name="itemheight"></a> itemHeight

▸ **itemHeight**(`value?`): `any`

获取或设置切片器的itemHeight

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值,返回切片器的itemHeight;否则,返回切片器

___

### <a id="multiselect" name="multiselect"></a> multiSelect

▸ **multiSelect**(`value?`): `any`

获取或设置切片器的multiSelect

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值,返回切片器的multiSelect;否则,返回切片器

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置切片器的name

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果没有设置值,返回切片器的名称;否则,返回切片器

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

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`Point`](GC.Spread.Sheets.Point.md) |

#### Returns

`any`

如果没有设置值,返回切片器的position;否则,返回切片器

___

### <a id="refresh" name="refresh"></a> refresh

▸ **refresh**(): `void`

刷新切片器

#### Returns

`void`

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

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值,返回切片器的showHeader;否则,返回切片器

___

### <a id="shownodataitems" name="shownodataitems"></a> showNoDataItems

▸ **showNoDataItems**(`value?`): `any`

获取或设置切片器的showNoDataItems

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值,返回切片器的showNoDataItems;否则,返回切片器

___

### <a id="shownodataitemsinlast" name="shownodataitemsinlast"></a> showNoDataItemsInLast

▸ **showNoDataItemsInLast**(`value?`): `any`

获取或设置切片器的showNoDataItemsInLast

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值,返回切片器的showNoDataItemsInLast;否则,返回切片器

___

### <a id="sortstate" name="sortstate"></a> sortState

▸ **sortState**(`value?`): `any`

获取或设置切片器的sortState

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SortState`](../enums/GC.Spread.Sheets.SortState.md) |

#### Returns

`any`

如果没有设置值,返回切片器的sortState;否则,返回切片器

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

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值,返回切片器的startColumn;否则,返回切片器

___

### <a id="startcolumnoffset" name="startcolumnoffset"></a> startColumnOffset

▸ **startColumnOffset**(`value?`): `any`

获取或设置切片器的startColumnOffset

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值,返回切片器的startColumnOffset;否则,返回切片器

___

### <a id="startrow" name="startrow"></a> startRow

▸ **startRow**(`value?`): `any`

获取或设置切片器的startRow

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值,返回切片器的startRow;否则,返回切片器

___

### <a id="startrowoffset" name="startrowoffset"></a> startRowOffset

▸ **startRowOffset**(`value?`): `any`

获取或设置切片器的startRowOffset

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值,返回切片器的startRowOffset;否则,返回切片器

___

### <a id="style" name="style"></a> style

▸ **style**(`value?`): `any`

获取或设置切片器的style

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md) |

#### Returns

`any`

如果没有设置值,返回切片器的style;否则,返回切片器

___

### <a id="visuallynodataitems" name="visuallynodataitems"></a> visuallyNoDataItems

▸ **visuallyNoDataItems**(`value?`): `any`

获取或设置切片器的visuallyNoDataItems

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值,返回切片器的visuallyNoDataItems;否则,返回切片器

___

### <a id="width" name="width"></a> width

▸ **width**(`value?`): `any`

获取或设置切片器的width

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值,返回切片器的width;否则,返回切片器

___

### <a id="x" name="x"></a> x

▸ **x**(`value?`): `any`

获取或设置切片器的x

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值,返回切片器的x;否则,返回切片器

___

### <a id="y" name="y"></a> y

▸ **y**(`value?`): `any`

获取或设置切片器的y

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值,返回切片器的y;否则,返回切片器
