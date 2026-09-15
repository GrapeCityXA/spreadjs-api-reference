# Interface: IDataViewChanges

[Sheets](../modules/GC.Spread.Sheets.md).[TableSheet](../modules/GC.Spread.Sheets.TableSheet.md).IDataViewChanges

## Table of contents

### Properties

- [column](GC.Spread.Sheets.TableSheet.IDataViewChanges.md#column)
- [data](GC.Spread.Sheets.TableSheet.IDataViewChanges.md#data)
- [dataItem](GC.Spread.Sheets.TableSheet.IDataViewChanges.md#dataitem)
- [index](GC.Spread.Sheets.TableSheet.IDataViewChanges.md#index)
- [oldDataItem](GC.Spread.Sheets.TableSheet.IDataViewChanges.md#olddataitem)
- [originalColumn](GC.Spread.Sheets.TableSheet.IDataViewChanges.md#originalcolumn)
- [type](GC.Spread.Sheets.TableSheet.IDataViewChanges.md#type)

## Properties

### <a id="column" name="column"></a> column

• `Optional` **column**: [`IColumn`](../modules/GC.Data.md#icolumn)

当前列。

___

### <a id="data" name="data"></a> data

• `Optional` **data**: `any`[]

当前添加列的默认值。

___

### <a id="dataitem" name="dataitem"></a> dataItem

• **dataItem**: `any`

当前行数据。

___

### <a id="index" name="index"></a> index

• **index**: `number`

表格视图的索引。

___

### <a id="olddataitem" name="olddataitem"></a> oldDataItem

• `Optional` **oldDataItem**: `any`

原始行数据，仅用于"update"（更新）操作。

___

### <a id="originalcolumn" name="originalcolumn"></a> originalColumn

• `Optional` **originalColumn**: [`IColumn`](../modules/GC.Data.md#icolumn)

原始列，仅用于"update column"（更新列）操作。

___

### <a id="type" name="type"></a> type

• **type**: `string`

变更类型，可以是以下之一："insert"（插入）、"update"（更新）、"delete"（删除）、"addColumn"（添加列）、"updateColumn"（更新列）、"removeColumn"（删除列）。
