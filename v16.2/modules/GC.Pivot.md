# Namespace: Pivot

[GC](GC.md).Pivot

## Table of contents

### Enumerations

- [DataPosition](../enums/GC.Pivot.DataPosition.md)
- [DateGroupType](../enums/GC.Pivot.DateGroupType.md)
- [PivotAdvancedDateFilterBy](../enums/GC.Pivot.PivotAdvancedDateFilterBy.md)
- [PivotCaptionFilterOperator](../enums/GC.Pivot.PivotCaptionFilterOperator.md)
- [PivotConditionType](../enums/GC.Pivot.PivotConditionType.md)
- [PivotDataType](../enums/GC.Pivot.PivotDataType.md)
- [PivotDateFilterOperator](../enums/GC.Pivot.PivotDateFilterOperator.md)
- [PivotShowDataAs](../enums/GC.Pivot.PivotShowDataAs.md)
- [PivotShowDataAsBaseItemType](../enums/GC.Pivot.PivotShowDataAsBaseItemType.md)
- [PivotSourceFieldType](../enums/GC.Pivot.PivotSourceFieldType.md)
- [PivotTop10FilterOperator](../enums/GC.Pivot.PivotTop10FilterOperator.md)
- [PivotTop10FilterType](../enums/GC.Pivot.PivotTop10FilterType.md)
- [PivotValueFilterOperator](../enums/GC.Pivot.PivotValueFilterOperator.md)
- [SortType](../enums/GC.Pivot.SortType.md)
- [SubtotalType](../enums/GC.Pivot.SubtotalType.md)

### Interfaces

- [ICustomSortCallBack](../interfaces/GC.Pivot.ICustomSortCallBack.md)
- [IPivotCustomSortInfo](../interfaces/GC.Pivot.IPivotCustomSortInfo.md)

### Type aliases

- [IDataPosition](GC.Pivot.md#idataposition)
- [IPivotCaptionConditionFilterInfo](GC.Pivot.md#ipivotcaptionconditionfilterinfo)
- [IPivotDateConditionFilterInfo](GC.Pivot.md#ipivotdateconditionfilterinfo)
- [IPivotTop10ConditionFilterInfo](GC.Pivot.md#ipivottop10conditionfilterinfo)
- [IPivotValueConditionInfo](GC.Pivot.md#ipivotvalueconditioninfo)
- [IPivotViewSortInfo](GC.Pivot.md#ipivotviewsortinfo)
- [IStringGroupItems](GC.Pivot.md#istringgroupitems)
- [IValueInfo](GC.Pivot.md#ivalueinfo)

## Type aliases

### <a id="idataposition" name="idataposition"></a> IDataPosition

Ƭ **IDataPosition**: `Object`

**`property`** {boolean} [display]

**`property`** {GC.Pivot.DataPosition}

**`property`** {number}

#### Type declaration

| Name | Type |
| :------ | :------ |
| `display?` | `boolean` |
| `positionIndex` | `number` |
| `positionType` | [`DataPosition`](../enums/GC.Pivot.DataPosition.md) |

___

### <a id="ipivotcaptionconditionfilterinfo" name="ipivotcaptionconditionfilterinfo"></a> IPivotCaptionConditionFilterInfo

Ƭ **IPivotCaptionConditionFilterInfo**: `Object`

**`property`** {GC.Pivot.PivotConditionType} conType

**`property`** {string[]} val

**`property`** {GC.Pivot.PivotCaptionFilterOperator} operator

#### Type declaration

| Name | Type |
| :------ | :------ |
| `conType` | [`PivotConditionType`](../enums/GC.Pivot.PivotConditionType.md) |
| `operator` | [`PivotCaptionFilterOperator`](../enums/GC.Pivot.PivotCaptionFilterOperator.md) |
| `val` | `string`[] |

___

### <a id="ipivotdateconditionfilterinfo" name="ipivotdateconditionfilterinfo"></a> IPivotDateConditionFilterInfo

Ƭ **IPivotDateConditionFilterInfo**: `Object`

**`property`** {GC.Pivot.PivotConditionType} conType

**`property`** {Date[]} val

**`property`** {GC.Pivot.PivotDateFilterOperator} operator

**`property`** {boolean} isWholeDay

**`property`** {boolean} isDynamicEndDate

**`property`** {boolean} isParallel

**`property`** {GC.Pivot.PivotAdvancedDateFilterBy} by

#### Type declaration

| Name | Type |
| :------ | :------ |
| `by?` | [`PivotAdvancedDateFilterBy`](../enums/GC.Pivot.PivotAdvancedDateFilterBy.md) |
| `conType` | [`PivotConditionType`](../enums/GC.Pivot.PivotConditionType.md) |
| `isDynamicEndDate?` | `boolean` |
| `isParallel?` | `boolean` |
| `isWholeDay` | `boolean` |
| `operator` | [`PivotDateFilterOperator`](../enums/GC.Pivot.PivotDateFilterOperator.md) |
| `val` | `Date`[] |

___

### <a id="ipivottop10conditionfilterinfo" name="ipivottop10conditionfilterinfo"></a> IPivotTop10ConditionFilterInfo

Ƭ **IPivotTop10ConditionFilterInfo**: `Object`

**`property`** {GC.Pivot.PivotConditionType} conType

**`property`** {number} val

**`property`** {GC.Pivot.PivotTop10FilterType} type

**`property`** {GC.Pivot.PivotTop10FilterOperator} operator

#### Type declaration

| Name | Type |
| :------ | :------ |
| `conType` | [`PivotConditionType`](../enums/GC.Pivot.PivotConditionType.md) |
| `operator` | [`PivotTop10FilterOperator`](../enums/GC.Pivot.PivotTop10FilterOperator.md) |
| `type` | [`PivotTop10FilterType`](../enums/GC.Pivot.PivotTop10FilterType.md) |
| `val` | `number` |

___

### <a id="ipivotvalueconditioninfo" name="ipivotvalueconditioninfo"></a> IPivotValueConditionInfo

Ƭ **IPivotValueConditionInfo**: `Object`

**`property`** {GC.Pivot.PivotConditionType} conType

**`property`** {number[]} val

**`property`** {GC.Pivot.PivotValueFilterOperator} operator

#### Type declaration

| Name | Type |
| :------ | :------ |
| `conType` | [`PivotConditionType`](../enums/GC.Pivot.PivotConditionType.md) |
| `operator` | [`PivotValueFilterOperator`](../enums/GC.Pivot.PivotValueFilterOperator.md) |
| `val` | `number`[] |

___

### <a id="ipivotviewsortinfo" name="ipivotviewsortinfo"></a> IPivotViewSortInfo

Ƭ **IPivotViewSortInfo**: `Object`

**`property`** {GC.Pivot.SortType} sortType sort field by ascending or descending or custom.

**`property`** {string} sortValueFieldName sort field by specified value area field's value.

**`property`** {GC.Spread.Pivot.IPivotReference[]} sortByPivotReferences sort field by specified row or column. sortValueFieldName is must if use this property.

**`property`** {GC.Pivot.ICustomSortCallBack} customSortCallback sort field by custom way. should return the ordered field items array.

#### Type declaration

| Name | Type |
| :------ | :------ |
| `customSortCallback?` | [`ICustomSortCallBack`](../interfaces/GC.Pivot.ICustomSortCallBack.md) |
| `sortByPivotReferences?` | [`IPivotReference`](GC.Spread.Pivot.md#ipivotreference)[] |
| `sortType?` | [`SortType`](../enums/GC.Pivot.SortType.md) |
| `sortValueFieldName?` | `string` |

___

### <a id="istringgroupitems" name="istringgroupitems"></a> IStringGroupItems

Ƭ **IStringGroupItems**: `Object`

**`property`** {Object.<string, string[] | number[]>}  -The -组字段项名称和匹配项文本

#### Index signature

▪ [groupItemName: `string`]: (`string` \| `number`)[]

___

### <a id="ivalueinfo" name="ivalueinfo"></a> IValueInfo

Ƭ **IValueInfo**: `Object`

**`property`** {string} sourceName value field source name.

**`property`** {GC.Pivot.SubtotalType} subtotalType value field subtotal type.

#### Type declaration

| Name | Type |
| :------ | :------ |
| `sourceName` | `string` |
| `subtotalType` | [`SubtotalType`](../enums/GC.Pivot.SubtotalType.md) |
