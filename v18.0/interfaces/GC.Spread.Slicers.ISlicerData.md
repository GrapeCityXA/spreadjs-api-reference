# Interface: ISlicerData

[Spread](../modules/GC.Spread.md).[Slicers](../modules/GC.Spread.Slicers.md).ISlicerData

## Table of contents

### Methods

- [attachListener](GC.Spread.Slicers.ISlicerData.md#attachlistener)
- [clearPreview](GC.Spread.Slicers.ISlicerData.md#clearpreview)
- [detachListener](GC.Spread.Slicers.ISlicerData.md#detachlistener)
- [doFilter](GC.Spread.Slicers.ISlicerData.md#dofilter)
- [doUnfilter](GC.Spread.Slicers.ISlicerData.md#dounfilter)
- [getColumnIndex](GC.Spread.Slicers.ISlicerData.md#getcolumnindex)
- [getData](GC.Spread.Slicers.ISlicerData.md#getdata)
- [getExclusiveData](GC.Spread.Slicers.ISlicerData.md#getexclusivedata)
- [getExclusiveRowIndex](GC.Spread.Slicers.ISlicerData.md#getexclusiverowindex)
- [getFilteredIndexes](GC.Spread.Slicers.ISlicerData.md#getfilteredindexes)
- [getFilteredOutIndexes](GC.Spread.Slicers.ISlicerData.md#getfilteredoutindexes)
- [getFilteredOutRanges](GC.Spread.Slicers.ISlicerData.md#getfilteredoutranges)
- [getFilteredRanges](GC.Spread.Slicers.ISlicerData.md#getfilteredranges)
- [getRowIndexes](GC.Spread.Slicers.ISlicerData.md#getrowindexes)

## Methods

### <a id="attachlistener" name="attachlistener"></a> attachListener

▸ **attachListener**(`listener`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | [`ISlicerListener`](GC.Spread.Slicers.ISlicerListener.md) |

#### Returns

`void`

___

### <a id="clearpreview" name="clearpreview"></a> clearPreview

▸ **clearPreview**(): `void`

#### Returns

`void`

___

### <a id="detachlistener" name="detachlistener"></a> detachListener

▸ **detachListener**(`listener`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | [`ISlicerListener`](GC.Spread.Slicers.ISlicerListener.md) |

#### Returns

`void`

___

### <a id="dofilter" name="dofilter"></a> doFilter

▸ **doFilter**(`columnName`, `slicerConditional`, `isPreview?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `columnName` | `string` |
| `slicerConditional` | [`ISlicerConditional`](GC.Spread.Slicers.ISlicerConditional.md) |
| `isPreview?` | `boolean` |

#### Returns

`void`

___

### <a id="dounfilter" name="dounfilter"></a> doUnfilter

▸ **doUnfilter**(`columnName`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `columnName` | `string` |

#### Returns

`void`

___

### <a id="getcolumnindex" name="getcolumnindex"></a> getColumnIndex

▸ **getColumnIndex**(`columnName`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `columnName` | `string` |

#### Returns

`number`

___

### <a id="getdata" name="getdata"></a> getData

▸ **getData**(`columnName`, `range?`): `any`[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `columnName` | `string` |
| `range?` | [`ISlicerRangeConditional`](GC.Spread.Slicers.ISlicerRangeConditional.md) |

#### Returns

`any`[]

___

### <a id="getexclusivedata" name="getexclusivedata"></a> getExclusiveData

▸ **getExclusiveData**(`columnName`): `any`[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `columnName` | `string` |

#### Returns

`any`[]

___

### <a id="getexclusiverowindex" name="getexclusiverowindex"></a> getExclusiveRowIndex

▸ **getExclusiveRowIndex**(`columnName`, `rowIndex`): `number`

#### Parameters

| Name | Type |
| :------ | :------ |
| `columnName` | `string` |
| `rowIndex` | `number` |

#### Returns

`number`

___

### <a id="getfilteredindexes" name="getfilteredindexes"></a> getFilteredIndexes

▸ **getFilteredIndexes**(`columnName`, `isPreview?`): `number`[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `columnName` | `string` |
| `isPreview?` | `boolean` |

#### Returns

`number`[]

___

### <a id="getfilteredoutindexes" name="getfilteredoutindexes"></a> getFilteredOutIndexes

▸ **getFilteredOutIndexes**(`columnName`, `filteredOutDataType`, `isPreview?`): `number`[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `columnName` | `string` |
| `filteredOutDataType` | [`FilteredOutDataType`](../enums/GC.Spread.Slicers.FilteredOutDataType.md) |
| `isPreview?` | `boolean` |

#### Returns

`number`[]

___

### <a id="getfilteredoutranges" name="getfilteredoutranges"></a> getFilteredOutRanges

▸ **getFilteredOutRanges**(`columnName`): [`ISlicerRangeConditional`](GC.Spread.Slicers.ISlicerRangeConditional.md)[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `columnName` | `string` |

#### Returns

[`ISlicerRangeConditional`](GC.Spread.Slicers.ISlicerRangeConditional.md)[]

___

### <a id="getfilteredranges" name="getfilteredranges"></a> getFilteredRanges

▸ **getFilteredRanges**(`columnName`): [`ISlicerRangeConditional`](GC.Spread.Slicers.ISlicerRangeConditional.md)[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `columnName` | `string` |

#### Returns

[`ISlicerRangeConditional`](GC.Spread.Slicers.ISlicerRangeConditional.md)[]

___

### <a id="getrowindexes" name="getrowindexes"></a> getRowIndexes

▸ **getRowIndexes**(`columnName`, `exclusiveRowIndex`): `number`[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `columnName` | `string` |
| `exclusiveRowIndex` | `number` |

#### Returns

`number`[]
