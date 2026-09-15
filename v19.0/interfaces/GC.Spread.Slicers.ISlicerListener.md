# Interface: ISlicerListener

[Spread](../modules/GC.Spread.md).[Slicers](../modules/GC.Spread.Slicers.md).ISlicerListener

## Table of contents

### Methods

- [onColumnNameChanged](GC.Spread.Slicers.ISlicerListener.md#oncolumnnamechanged)
- [onColumnRemoved](GC.Spread.Slicers.ISlicerListener.md#oncolumnremoved)
- [onDataChanged](GC.Spread.Slicers.ISlicerListener.md#ondatachanged)
- [onFiltered](GC.Spread.Slicers.ISlicerListener.md#onfiltered)
- [onRowsChanged](GC.Spread.Slicers.ISlicerListener.md#onrowschanged)

## Methods

### <a id="oncolumnnamechanged" name="oncolumnnamechanged"></a> onColumnNameChanged

▸ **onColumnNameChanged**(`oldName`, `newName`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `oldName` | `string` |
| `newName` | `string` |

#### Returns

`void`

___

### <a id="oncolumnremoved" name="oncolumnremoved"></a> onColumnRemoved

▸ **onColumnRemoved**(`columnName`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `columnName` | `string` |

#### Returns

`void`

___

### <a id="ondatachanged" name="ondatachanged"></a> onDataChanged

▸ **onDataChanged**(`data`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `data` | [`ISlicerDataItem`](GC.Spread.Slicers.ISlicerDataItem.md)[] |

#### Returns

`void`

___

### <a id="onfiltered" name="onfiltered"></a> onFiltered

▸ **onFiltered**(`data`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `data` | [`ISlicerFilteredData`](GC.Spread.Slicers.ISlicerFilteredData.md) |

#### Returns

`void`

___

### <a id="onrowschanged" name="onrowschanged"></a> onRowsChanged

▸ **onRowsChanged**(`rowIndex`, `rowCount`, `isAdd`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `rowIndex` | `number` |
| `rowCount` | `number` |
| `isAdd` | `boolean` |

#### Returns

`void`
