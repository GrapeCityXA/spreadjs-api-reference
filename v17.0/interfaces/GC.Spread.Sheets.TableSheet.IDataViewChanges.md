# Interface: IDataViewChanges

[Sheets](../modules/GC.Spread.Sheets.md).[TableSheet](../modules/GC.Spread.Sheets.TableSheet.md).IDataViewChanges

## Table of contents

### Properties

- [dataItem](GC.Spread.Sheets.TableSheet.IDataViewChanges.md#dataitem)
- [index](GC.Spread.Sheets.TableSheet.IDataViewChanges.md#index)
- [oldDataItem](GC.Spread.Sheets.TableSheet.IDataViewChanges.md#olddataitem)
- [type](GC.Spread.Sheets.TableSheet.IDataViewChanges.md#type)

## Properties

### <a id="dataitem" name="dataitem"></a> dataItem

• **dataItem**: `any`

The current row data.

___

### <a id="index" name="index"></a> index

• **index**: `number`

The view index of table sheet.

___

### <a id="olddataitem" name="olddataitem"></a> oldDataItem

• `Optional` **oldDataItem**: `any`

The original row data, only used for "update".

___

### <a id="type" name="type"></a> type

• **type**: `string`

The change type, could be one of "insert", "update" or "delete".
