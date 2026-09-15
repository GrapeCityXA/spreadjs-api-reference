# Class: TableSlicerData

[Sheets](../modules/GC.Spread.Sheets.md).[Slicers](../modules/GC.Spread.Sheets.Slicers.md).TableSlicerData

## Hierarchy

- [`GeneralSlicerData`](GC.Spread.Slicers.GeneralSlicerData.md)

  ↳ **`TableSlicerData`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Slicers.TableSlicerData.md#constructor)

### Properties

- [columnNames](GC.Spread.Sheets.Slicers.TableSlicerData.md#columnnames)
- [data](GC.Spread.Sheets.Slicers.TableSlicerData.md#data)

### Methods

- [aggregateData](GC.Spread.Sheets.Slicers.TableSlicerData.md#aggregatedata)
- [attachListener](GC.Spread.Sheets.Slicers.TableSlicerData.md#attachlistener)
- [clearPreview](GC.Spread.Sheets.Slicers.TableSlicerData.md#clearpreview)
- [detachListener](GC.Spread.Sheets.Slicers.TableSlicerData.md#detachlistener)
- [doFilter](GC.Spread.Sheets.Slicers.TableSlicerData.md#dofilter)
- [doUnfilter](GC.Spread.Sheets.Slicers.TableSlicerData.md#dounfilter)
- [getColumnIndex](GC.Spread.Sheets.Slicers.TableSlicerData.md#getcolumnindex)
- [getData](GC.Spread.Sheets.Slicers.TableSlicerData.md#getdata)
- [getExclusiveData](GC.Spread.Sheets.Slicers.TableSlicerData.md#getexclusivedata)
- [getExclusiveRowIndex](GC.Spread.Sheets.Slicers.TableSlicerData.md#getexclusiverowindex)
- [getFilteredIndexes](GC.Spread.Sheets.Slicers.TableSlicerData.md#getfilteredindexes)
- [getFilteredOutIndexes](GC.Spread.Sheets.Slicers.TableSlicerData.md#getfilteredoutindexes)
- [getFilteredOutRanges](GC.Spread.Sheets.Slicers.TableSlicerData.md#getfilteredoutranges)
- [getFilteredOutRowIndexes](GC.Spread.Sheets.Slicers.TableSlicerData.md#getfilteredoutrowindexes)
- [getFilteredRanges](GC.Spread.Sheets.Slicers.TableSlicerData.md#getfilteredranges)
- [getFilteredRowIndexes](GC.Spread.Sheets.Slicers.TableSlicerData.md#getfilteredrowindexes)
- [getRowIndexes](GC.Spread.Sheets.Slicers.TableSlicerData.md#getrowindexes)
- [getSlicerData](GC.Spread.Sheets.Slicers.TableSlicerData.md#getslicerdata)
- [getTable](GC.Spread.Sheets.Slicers.TableSlicerData.md#gettable)
- [inPreview](GC.Spread.Sheets.Slicers.TableSlicerData.md#inpreview)
- [onColumnNameChanged](GC.Spread.Sheets.Slicers.TableSlicerData.md#oncolumnnamechanged)
- [onColumnsRemoved](GC.Spread.Sheets.Slicers.TableSlicerData.md#oncolumnsremoved)
- [onDataChanged](GC.Spread.Sheets.Slicers.TableSlicerData.md#ondatachanged)
- [onFiltered](GC.Spread.Sheets.Slicers.TableSlicerData.md#onfiltered)
- [onRowsAdded](GC.Spread.Sheets.Slicers.TableSlicerData.md#onrowsadded)
- [onRowsRemoved](GC.Spread.Sheets.Slicers.TableSlicerData.md#onrowsremoved)
- [refresh](GC.Spread.Sheets.Slicers.TableSlicerData.md#refresh)
- [resumeFilteredEvents](GC.Spread.Sheets.Slicers.TableSlicerData.md#resumefilteredevents)
- [suspendFilteredEvents](GC.Spread.Sheets.Slicers.TableSlicerData.md#suspendfilteredevents)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new TableSlicerData**(`table`)

表格切片器数据

**`代码示例`**
```
//本示例为表格创建切片器
//创建表格
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: "1968/6/8" },
    { Name: "Betty", City: "NewYork", Birthday: "1972/7/3" },
    { Name: "Alice", City: "Washington", Birthday: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var slicerData = new GC.Spread.Sheets.Slicers.TableSlicerData(table)
//给项切片器设置项切片器数据
var slicer = new GC.Spread.Sheets.Slicers.ItemSlicer("slicer", slicerData, "Name");
//将项切片器添加到dom树
//The "slicerHost" is the div you want to add the slicer's dom to.
$("#slicerHost").append(slicer.getDOMElement());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `table` | [`Table`](GC.Spread.Sheets.Tables.Table.md) | 表格 |

#### Overrides

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[constructor](GC.Spread.Slicers.GeneralSlicerData.md#constructor)

## Properties

### <a id="columnnames" name="columnnames"></a> columnNames

• **columnNames**: `string`[]

通用切片器数据的列名称

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[columnNames](GC.Spread.Slicers.GeneralSlicerData.md#columnnames)

___

### <a id="data" name="data"></a> data

• **data**: `any`[][]

通用切片器的数据源

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[data](GC.Spread.Slicers.GeneralSlicerData.md#data)

## Methods

### <a id="aggregatedata" name="aggregatedata"></a> aggregateData

▸ **aggregateData**(`columnName`, `aggregateType`, `range?`): `number`

通过指定的列名聚合数据

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnName` | `string` | 列名 |
| `aggregateType` | [`SlicerAggregateType`](../enums/GC.Spread.Slicers.SlicerAggregateType.md) | 聚合类型 |
| `range?` | [`ISlicerRangeConditional`](../interfaces/GC.Spread.Slicers.ISlicerRangeConditional.md) | 特定区域 range.min: 数值类型,最小值 range.max: 数值类型,最大值 |

#### Returns

`number`

聚合数据

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[aggregateData](GC.Spread.Slicers.GeneralSlicerData.md#aggregatedata)

___

### <a id="attachlistener" name="attachlistener"></a> attachListener

▸ **attachListener**(`listener`): `void`

附加切片器

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | [`ISlicerListener`](../interfaces/GC.Spread.Slicers.ISlicerListener.md) | 切片器 |

#### Returns

`void`

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[attachListener](GC.Spread.Slicers.GeneralSlicerData.md#attachlistener)

___

### <a id="clearpreview" name="clearpreview"></a> clearPreview

▸ **clearPreview**(): `void`

清除预览筛选状态

#### Returns

`void`

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[clearPreview](GC.Spread.Slicers.GeneralSlicerData.md#clearpreview)

___

### <a id="detachlistener" name="detachlistener"></a> detachListener

▸ **detachListener**(`listener`): `void`

移除切片器

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | [`ISlicerListener`](../interfaces/GC.Spread.Slicers.ISlicerListener.md) | 切片器 |

#### Returns

`void`

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[detachListener](GC.Spread.Slicers.GeneralSlicerData.md#detachlistener)

___

### <a id="dofilter" name="dofilter"></a> doFilter

▸ **doFilter**(`columnName`, `conditional`, `isPreview?`): `void`

筛选与指定列名和排他数据索引对应的数据

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnName` | `string` | 列名 |
| `conditional` | [`ISlicerConditional`](../interfaces/GC.Spread.Slicers.ISlicerConditional.md) | 有条件的筛选 conditional.exclusiveRowIndexes: 数字数组类型,可见的排他行索引 conditional.ranges: {min:number, max:number} 数组类型,可见区域 |
| `isPreview?` | `boolean` | - |

#### Returns

`void`

#### Overrides

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[doFilter](GC.Spread.Slicers.GeneralSlicerData.md#dofilter)

___

### <a id="dounfilter" name="dounfilter"></a> doUnfilter

▸ **doUnfilter**(`columnName`): `void`

取消筛选与指定列名称相对应的数据

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnName` | `string` | 列名 |

#### Returns

`void`

#### Overrides

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[doUnfilter](GC.Spread.Slicers.GeneralSlicerData.md#dounfilter)

___

### <a id="getcolumnindex" name="getcolumnindex"></a> getColumnIndex

▸ **getColumnIndex**(`columnName`): `number`

通过指定的列名获取列索引

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnName` | `string` | 列名 |

#### Returns

`number`

列索引

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[getColumnIndex](GC.Spread.Slicers.GeneralSlicerData.md#getcolumnindex)

___

### <a id="getdata" name="getdata"></a> getData

▸ **getData**(`columnName`, `range?`): `string`[]

通过指定的列名获取数据

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnName` | `string` | 列名 |
| `range?` | [`ISlicerRangeConditional`](../interfaces/GC.Spread.Slicers.ISlicerRangeConditional.md) | 特定区域 range.min: 数值类型,最小值 range.max: 数值类型,最大值 |

#### Returns

`string`[]

与指定列名相对应的数据

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[getData](GC.Spread.Slicers.GeneralSlicerData.md#getdata)

___

### <a id="getexclusivedata" name="getexclusivedata"></a> getExclusiveData

▸ **getExclusiveData**(`columnName`): `any`[]

通过指定的列名获取排除数据

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnName` | `string` | 列名 |

#### Returns

`any`[]

与指定列名相对应的排除数据

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[getExclusiveData](GC.Spread.Slicers.GeneralSlicerData.md#getexclusivedata)

___

### <a id="getexclusiverowindex" name="getexclusiverowindex"></a> getExclusiveRowIndex

▸ **getExclusiveRowIndex**(`columnName`, `rowIndex`): `number`

通过指定的列名和数据索引获取排除数据索引

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnName` | `string` | 列名 |
| `rowIndex` | `number` | 数据索引 |

#### Returns

`number`

与指定的列名和数据索引对应的排除数据索引

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[getExclusiveRowIndex](GC.Spread.Slicers.GeneralSlicerData.md#getexclusiverowindex)

___

### <a id="getfilteredindexes" name="getfilteredindexes"></a> getFilteredIndexes

▸ **getFilteredIndexes**(`columnName`): `number`[]

通过指定的列名获取筛选后的排除数据索引

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnName` | `string` | 列名 |

#### Returns

`number`[]

与指定的列名相对应的筛选后的排除数据索引

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[getFilteredIndexes](GC.Spread.Slicers.GeneralSlicerData.md#getfilteredindexes)

___

### <a id="getfilteredoutindexes" name="getfilteredoutindexes"></a> getFilteredOutIndexes

▸ **getFilteredOutIndexes**(`columnName`, `filteredOutDataType`): `number`[]

通过指定的列名获取筛选出的排除数据索引

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnName` | `string` | 列名 |
| `filteredOutDataType` | [`FilteredOutDataType`](../enums/GC.Spread.Slicers.FilteredOutDataType.md) | 应包括在结果中的筛选出的排除数据索引的类型 |

#### Returns

`number`[]

与指定的列名相对应的筛选出的排除数据索引

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[getFilteredOutIndexes](GC.Spread.Slicers.GeneralSlicerData.md#getfilteredoutindexes)

___

### <a id="getfilteredoutranges" name="getfilteredoutranges"></a> getFilteredOutRanges

▸ **getFilteredOutRanges**(`columnName`): [`ISlicerRangeConditional`](../interfaces/GC.Spread.Slicers.ISlicerRangeConditional.md)[]

获取其他列筛选出的区域

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnName` | `string` | 列名 |

#### Returns

[`ISlicerRangeConditional`](../interfaces/GC.Spread.Slicers.ISlicerRangeConditional.md)[]

与指定的列名称相对应的其他列所筛选的区域

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[getFilteredOutRanges](GC.Spread.Slicers.GeneralSlicerData.md#getfilteredoutranges)

___

### <a id="getfilteredoutrowindexes" name="getfilteredoutrowindexes"></a> getFilteredOutRowIndexes

▸ **getFilteredOutRowIndexes**(): `number`[]

获取筛选出的行索引

#### Returns

`number`[]

筛选出的行索引

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[getFilteredOutRowIndexes](GC.Spread.Slicers.GeneralSlicerData.md#getfilteredoutrowindexes)

___

### <a id="getfilteredranges" name="getfilteredranges"></a> getFilteredRanges

▸ **getFilteredRanges**(`columnName`): [`ISlicerRangeConditional`](../interfaces/GC.Spread.Slicers.ISlicerRangeConditional.md)[]

通过指定的列名获取筛选区域

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnName` | `string` | 列名 |

#### Returns

[`ISlicerRangeConditional`](../interfaces/GC.Spread.Slicers.ISlicerRangeConditional.md)[]

与指定的列名相对应的筛选区域

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[getFilteredRanges](GC.Spread.Slicers.GeneralSlicerData.md#getfilteredranges)

___

### <a id="getfilteredrowindexes" name="getfilteredrowindexes"></a> getFilteredRowIndexes

▸ **getFilteredRowIndexes**(): `number`[]

获取筛选出的行索引

#### Returns

`number`[]

筛选出的行索引

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[getFilteredRowIndexes](GC.Spread.Slicers.GeneralSlicerData.md#getfilteredrowindexes)

___

### <a id="getrowindexes" name="getrowindexes"></a> getRowIndexes

▸ **getRowIndexes**(`columnName`, `exclusiveRowIndex`): `number`[]

通过指定的列名和排除数据索引获取数据索引

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnName` | `string` | 列名 |
| `exclusiveRowIndex` | `number` | 排除数据的索引 |

#### Returns

`number`[]

与指定的列名和排除数据索引相对应的数据索引

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[getRowIndexes](GC.Spread.Slicers.GeneralSlicerData.md#getrowindexes)

___

### <a id="getslicerdata" name="getslicerdata"></a> getSlicerData

▸ **getSlicerData**(): [`TableSlicerData`](GC.Spread.Sheets.Slicers.TableSlicerData.md)

获取表格的切片器数据

#### Returns

[`TableSlicerData`](GC.Spread.Sheets.Slicers.TableSlicerData.md)

表格的切片器数据

___

### <a id="gettable" name="gettable"></a> getTable

▸ **getTable**(): [`Table`](GC.Spread.Sheets.Tables.Table.md)

获取表格切片器数据的表格

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md)

表格切片器数据的表格

___

### <a id="inpreview" name="inpreview"></a> inPreview

▸ **inPreview**(): `boolean`

获取切片器是否处于预览状态

#### Returns

`boolean`

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[inPreview](GC.Spread.Slicers.GeneralSlicerData.md#inpreview)

___

### <a id="oncolumnnamechanged" name="oncolumnnamechanged"></a> onColumnNameChanged

▸ **onColumnNameChanged**(`oldName`, `newName`): `void`

更改通用切片器数据的列名

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `oldName` | `string` | 旧列名 |
| `newName` | `string` | 新列名 |

#### Returns

`void`

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[onColumnNameChanged](GC.Spread.Slicers.GeneralSlicerData.md#oncolumnnamechanged)

___

### <a id="oncolumnsremoved" name="oncolumnsremoved"></a> onColumnsRemoved

▸ **onColumnsRemoved**(`colIndex`, `colCount`): `void`

删除通用切片器数据的列

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `colIndex` | `number` | 起始列索引 |
| `colCount` | `number` | 删除的列数 |

#### Returns

`void`

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[onColumnsRemoved](GC.Spread.Slicers.GeneralSlicerData.md#oncolumnsremoved)

___

### <a id="ondatachanged" name="ondatachanged"></a> onDataChanged

▸ **onDataChanged**(`changedDataItems`): `void`

更改通用切片器数据的数据源中的数据项

#### Parameters

| Name | Type |
| :------ | :------ |
| `changedDataItems` | [`ISlicerDataItem`](../interfaces/GC.Spread.Slicers.ISlicerDataItem.md) |

#### Returns

`void`

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[onDataChanged](GC.Spread.Slicers.GeneralSlicerData.md#ondatachanged)

___

### <a id="onfiltered" name="onfiltered"></a> onFiltered

▸ **onFiltered**(): `void`

发生在对切片器数据筛选之后

#### Returns

`void`

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[onFiltered](GC.Spread.Slicers.GeneralSlicerData.md#onfiltered)

___

### <a id="onrowsadded" name="onrowsadded"></a> onRowsAdded

▸ **onRowsAdded**(`rowIndex`, `rowCount`): `void`

在通用切片器数据的数据源中添加行

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rowIndex` | `number` | 起始行的索引 |
| `rowCount` | `number` | 要添加的行数 |

#### Returns

`void`

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[onRowsAdded](GC.Spread.Slicers.GeneralSlicerData.md#onrowsadded)

___

### <a id="onrowsremoved" name="onrowsremoved"></a> onRowsRemoved

▸ **onRowsRemoved**(`rowIndex`, `rowCount`): `void`

删除通用切片器数据的数据源中的行

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rowIndex` | `number` | 起始行的索引 |
| `rowCount` | `number` | 删除的行数 |

#### Returns

`void`

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[onRowsRemoved](GC.Spread.Slicers.GeneralSlicerData.md#onrowsremoved)

___

### <a id="refresh" name="refresh"></a> refresh

▸ **refresh**(): `void`

刷新表格切片器数据

#### Returns

`void`

___

### <a id="resumefilteredevents" name="resumefilteredevents"></a> resumeFilteredEvents

▸ **resumeFilteredEvents**(): `void`

恢复onFiltered事件

#### Returns

`void`

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[resumeFilteredEvents](GC.Spread.Slicers.GeneralSlicerData.md#resumefilteredevents)

___

### <a id="suspendfilteredevents" name="suspendfilteredevents"></a> suspendFilteredEvents

▸ **suspendFilteredEvents**(): `void`

挂起onFiltered事件

#### Returns

`void`

#### Inherited from

[GeneralSlicerData](GC.Spread.Slicers.GeneralSlicerData.md).[suspendFilteredEvents](GC.Spread.Slicers.GeneralSlicerData.md#suspendfilteredevents)
