# Class: GeneralSlicerData

[Spread](../modules/GC.Spread.md).[Slicers](../modules/GC.Spread.Slicers.md).GeneralSlicerData

## Hierarchy

- **`GeneralSlicerData`**

  ↳ [`TableSlicerData`](GC.Spread.Sheets.Slicers.TableSlicerData.md)

## Table of contents

### Constructors

- [constructor](GC.Spread.Slicers.GeneralSlicerData.md#constructor)

### Properties

- [columnNames](GC.Spread.Slicers.GeneralSlicerData.md#columnnames)
- [data](GC.Spread.Slicers.GeneralSlicerData.md#data)

### Methods

- [aggregateData](GC.Spread.Slicers.GeneralSlicerData.md#aggregatedata)
- [attachListener](GC.Spread.Slicers.GeneralSlicerData.md#attachlistener)
- [clearPreview](GC.Spread.Slicers.GeneralSlicerData.md#clearpreview)
- [detachListener](GC.Spread.Slicers.GeneralSlicerData.md#detachlistener)
- [doFilter](GC.Spread.Slicers.GeneralSlicerData.md#dofilter)
- [doUnfilter](GC.Spread.Slicers.GeneralSlicerData.md#dounfilter)
- [getColumnIndex](GC.Spread.Slicers.GeneralSlicerData.md#getcolumnindex)
- [getData](GC.Spread.Slicers.GeneralSlicerData.md#getdata)
- [getExclusiveData](GC.Spread.Slicers.GeneralSlicerData.md#getexclusivedata)
- [getExclusiveRowIndex](GC.Spread.Slicers.GeneralSlicerData.md#getexclusiverowindex)
- [getFilteredIndexes](GC.Spread.Slicers.GeneralSlicerData.md#getfilteredindexes)
- [getFilteredOutIndexes](GC.Spread.Slicers.GeneralSlicerData.md#getfilteredoutindexes)
- [getFilteredOutRanges](GC.Spread.Slicers.GeneralSlicerData.md#getfilteredoutranges)
- [getFilteredOutRowIndexes](GC.Spread.Slicers.GeneralSlicerData.md#getfilteredoutrowindexes)
- [getFilteredRanges](GC.Spread.Slicers.GeneralSlicerData.md#getfilteredranges)
- [getFilteredRowIndexes](GC.Spread.Slicers.GeneralSlicerData.md#getfilteredrowindexes)
- [getRowIndexes](GC.Spread.Slicers.GeneralSlicerData.md#getrowindexes)
- [inPreview](GC.Spread.Slicers.GeneralSlicerData.md#inpreview)
- [onColumnNameChanged](GC.Spread.Slicers.GeneralSlicerData.md#oncolumnnamechanged)
- [onColumnsRemoved](GC.Spread.Slicers.GeneralSlicerData.md#oncolumnsremoved)
- [onDataChanged](GC.Spread.Slicers.GeneralSlicerData.md#ondatachanged)
- [onFiltered](GC.Spread.Slicers.GeneralSlicerData.md#onfiltered)
- [onRowsAdded](GC.Spread.Slicers.GeneralSlicerData.md#onrowsadded)
- [onRowsRemoved](GC.Spread.Slicers.GeneralSlicerData.md#onrowsremoved)
- [resumeFilteredEvents](GC.Spread.Slicers.GeneralSlicerData.md#resumefilteredevents)
- [suspendFilteredEvents](GC.Spread.Slicers.GeneralSlicerData.md#suspendfilteredevents)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new GeneralSlicerData**(`data`, `columnNames`)

通用切片器数据

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `any`[][] | 切片器数据;它是一个矩阵数组 |
| `columnNames` | `string`[] | 切片器数据的列名 |

## Properties

### <a id="columnnames" name="columnnames"></a> columnNames

• **columnNames**: `string`[]

通用切片器数据的列名称

___

### <a id="data" name="data"></a> data

• **data**: `any`[][]

通用切片器的数据源

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

___

### <a id="clearpreview" name="clearpreview"></a> clearPreview

▸ **clearPreview**(): `void`

清除预览筛选状态

#### Returns

`void`

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

___

### <a id="dofilter" name="dofilter"></a> doFilter

▸ **doFilter**(`columnName`, `conditional`, `isPreview?`): `void`

筛选与指定列名和排他数据索引对应的数据

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnName` | `string` | 列名 |
| `conditional` | [`ISlicerConditional`](../interfaces/GC.Spread.Slicers.ISlicerConditional.md) | 条件筛选 conditional.exclusiveRowIndexes: 数字数组类型,可见的排他行索引 conditional.ranges: {min:number, max:number} 数组类型,可见区域 |
| `isPreview?` | `boolean` | 是否设置预览 |

#### Returns

`void`

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

___

### <a id="getfilteredoutrowindexes" name="getfilteredoutrowindexes"></a> getFilteredOutRowIndexes

▸ **getFilteredOutRowIndexes**(): `number`[]

获取筛选出的行索引

#### Returns

`number`[]

筛选出的行索引

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

___

### <a id="getfilteredrowindexes" name="getfilteredrowindexes"></a> getFilteredRowIndexes

▸ **getFilteredRowIndexes**(): `number`[]

获取筛选出的行索引

#### Returns

`number`[]

筛选出的行索引

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

___

### <a id="inpreview" name="inpreview"></a> inPreview

▸ **inPreview**(): `boolean`

获取切片器是否处于预览状态

#### Returns

`boolean`

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

___

### <a id="onfiltered" name="onfiltered"></a> onFiltered

▸ **onFiltered**(): `void`

发生在对切片器数据筛选之后

#### Returns

`void`

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

___

### <a id="resumefilteredevents" name="resumefilteredevents"></a> resumeFilteredEvents

▸ **resumeFilteredEvents**(): `void`

恢复onFiltered事件

#### Returns

`void`

___

### <a id="suspendfilteredevents" name="suspendfilteredevents"></a> suspendFilteredEvents

▸ **suspendFilteredEvents**(): `void`

挂起onFiltered事件

#### Returns

`void`
