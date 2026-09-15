# Namespace: Pivot

[GC](GC.md).[Spread](GC.Spread.md).Pivot

## Table of contents

### Namespaces

- [PivotTable](GC.Spread.Pivot.PivotTable.md)

### Enumerations

- [CalcItemAggregation](../enums/GC.Spread.Pivot.CalcItemAggregation.md)
- [DisplayFields](../enums/GC.Spread.Pivot.DisplayFields.md)
- [GrandTotalPosition](../enums/GC.Spread.Pivot.GrandTotalPosition.md)
- [PivotAreaAxisType](../enums/GC.Spread.Pivot.PivotAreaAxisType.md)
- [PivotAreaReference](../enums/GC.Spread.Pivot.PivotAreaReference.md)
- [PivotAreaType](../enums/GC.Spread.Pivot.PivotAreaType.md)
- [PivotPanelLayoutType](../enums/GC.Spread.Pivot.PivotPanelLayoutType.md)
- [PivotPanelSection](../enums/GC.Spread.Pivot.PivotPanelSection.md)
- [PivotTableFieldType](../enums/GC.Spread.Pivot.PivotTableFieldType.md)
- [PivotTableLayoutType](../enums/GC.Spread.Pivot.PivotTableLayoutType.md)
- [SubtotalsPosition](../enums/GC.Spread.Pivot.SubtotalsPosition.md)

### Classes

- [CustomPivotTableThemeManager](../classes/GC.Spread.Pivot.CustomPivotTableThemeManager.md)
- [PivotPanel](../classes/GC.Spread.Pivot.PivotPanel.md)
- [PivotTable](../classes/GC.Spread.Pivot.PivotTable-1.md)
- [PivotTableItemSlicer](../classes/GC.Spread.Pivot.PivotTableItemSlicer.md)
- [PivotTableStyle](../classes/GC.Spread.Pivot.PivotTableStyle.md)
- [PivotTableTheme](../classes/GC.Spread.Pivot.PivotTableTheme.md)
- [PivotTableThemes](../classes/GC.Spread.Pivot.PivotTableThemes.md)
- [PivotTableTimelineSlicer](../classes/GC.Spread.Pivot.PivotTableTimelineSlicer.md)

### Interfaces

- [IPivotItemInfo](../interfaces/GC.Spread.Pivot.IPivotItemInfo.md)
- [IPivotTableViewManager](../interfaces/GC.Spread.Pivot.IPivotTableViewManager.md)

### Type aliases

- [ICalcFieldInfo](GC.Spread.Pivot.md#icalcfieldinfo)
- [ICalcItemInfo](GC.Spread.Pivot.md#icalciteminfo)
- [IDateGroupInfo](GC.Spread.Pivot.md#idategroupinfo)
- [IDateGroupsInfo](GC.Spread.Pivot.md#idategroupsinfo)
- [IFieldInfo](GC.Spread.Pivot.md#ifieldinfo)
- [INumberGroupInfo](GC.Spread.Pivot.md#inumbergroupinfo)
- [IPivotArea](GC.Spread.Pivot.md#ipivotarea)
- [IPivotAreaOffset](GC.Spread.Pivot.md#ipivotareaoffset)
- [IPivotAreasCollection](GC.Spread.Pivot.md#ipivotareascollection)
- [IPivotConditionFilterInfo](GC.Spread.Pivot.md#ipivotconditionfilterinfo)
- [IPivotNodeInfo](GC.Spread.Pivot.md#ipivotnodeinfo)
- [IPivotOverwriteNodeInfo](GC.Spread.Pivot.md#ipivotoverwritenodeinfo)
- [IPivotReference](GC.Spread.Pivot.md#ipivotreference)
- [IPivotShowDataAsInfo](GC.Spread.Pivot.md#ipivotshowdataasinfo)
- [IPivotStyle](GC.Spread.Pivot.md#ipivotstyle)
- [IPivotTableOption](GC.Spread.Pivot.md#ipivottableoption)
- [IPivotTablePosition](GC.Spread.Pivot.md#ipivottableposition)
- [IPivotTableRange](GC.Spread.Pivot.md#ipivottablerange)
- [IPivotTableView](GC.Spread.Pivot.md#ipivottableview)
- [IPivotTextFilterInfo](GC.Spread.Pivot.md#ipivottextfilterinfo)
- [ISerializeFieldInfo](GC.Spread.Pivot.md#iserializefieldinfo)
- [ISerializeInfo](GC.Spread.Pivot.md#iserializeinfo)
- [ISerializeShowDataAsInfo](GC.Spread.Pivot.md#iserializeshowdataasinfo)
- [ISourceFieldInfo](GC.Spread.Pivot.md#isourcefieldinfo)
- [ITextCollectionCondition](GC.Spread.Pivot.md#itextcollectioncondition)
- [ITextGroupInfo](GC.Spread.Pivot.md#itextgroupinfo)

## Type aliases

### <a id="icalcfieldinfo" name="icalcfieldinfo"></a> ICalcFieldInfo

Ƭ **ICalcFieldInfo**: `Object`

**`property`** {string} fieldName  calc字段的字段名

**`property`** {string} formula  calc字段的公式

#### Type declaration

| Name | Type |
| :------ | :------ |
| `fieldName` | `string` |
| `formula` | `string` |

___

### <a id="icalciteminfo" name="icalciteminfo"></a> ICalcItemInfo

Ƭ **ICalcItemInfo**: `Object`

**`property`** {string} sourceName PivotTable的sourceField名称

**`property`** {string} calcItemName PivotTable源字段的名称计算项名称

**`property`** {string} formula PivotTable的sourceField的calcItem的公式

**`property`** {number} priority PivotTable源字段calcItem的优先级

#### Type declaration

| Name | Type |
| :------ | :------ |
| `calcItemName` | `string` |
| `formula` | `string` |
| `priority` | `number` |
| `sourceName` | `string` |

___

### <a id="idategroupinfo" name="idategroupinfo"></a> IDateGroupInfo

Ƭ **IDateGroupInfo**: `Object`

**`property`** {GC.Pivot.DateGroupType} by 日期组的日期单位

**`property`** {Date} [start]  组的开始日期

**`property`** {Date} [end] 组的结束日期

#### Type declaration

| Name | Type |
| :------ | :------ |
| `by` | [`DateGroupType`](../enums/GC.Pivot.DateGroupType.md) |
| `end?` | `Date` |
| `start?` | `Date` |

___

### <a id="idategroupsinfo" name="idategroupsinfo"></a> IDateGroupsInfo

Ƭ **IDateGroupsInfo**: `Object`

**`property`** {string} originFieldName 源字段名称

**`property`** {GC.Spread.Pivot.IDateGroupInfo[]} dateGroups 日期组信息

#### Type declaration

| Name | Type |
| :------ | :------ |
| `dateGroups` | [`IDateGroupInfo`](GC.Spread.Pivot.md#idategroupinfo)[] |
| `originFieldName` | `string` |

___

### <a id="ifieldinfo" name="ifieldinfo"></a> IFieldInfo

Ƭ **IFieldInfo**: `Object`

**`property`** {string} fieldName 字段名

**`property`** {string} sourceName 源名称

**`property`** {GC.Pivot.PivotDataType} dataType  字段对应源数据类型

**`property`** {GC.Spread.Pivot.PivotTableFieldType} pivotArea 字段类型，影响不同区域中的字段

**`property`** {number} pivotIndex 字段区域中的索引

**`property`** {Date|number} [start] 数字类型数据字段的最小值或日期类型字段的最旧值

**`property`** {Date|number} [end]  数字型数据字段的最大值或日期型字段的最新值

#### Type declaration

| Name | Type |
| :------ | :------ |
| `dataType` | [`PivotDataType`](../enums/GC.Pivot.PivotDataType.md) |
| `end?` | `Date` \| `number` |
| `fieldName` | `string` |
| `pivotArea` | [`PivotTableFieldType`](../enums/GC.Spread.Pivot.PivotTableFieldType.md) |
| `pivotIndex` | `number` |
| `sourceName` | `string` |
| `start?` | `Date` \| `number` |

___

### <a id="inumbergroupinfo" name="inumbergroupinfo"></a> INumberGroupInfo

Ƭ **INumberGroupInfo**: `Object`

**`property`** {string} originFieldName 源字段名称

**`property`** {object}  numberGroup 数值组

**`property`** {number}  [numberGroup.start]  数值组的起始数值

**`property`** {number}  [numberGroup.end]  数值组的结束数值

**`property`** {number}  numberGroup.by   数值组的步长

#### Type declaration

| Name | Type |
| :------ | :------ |
| `numberGroup` | { `by`: `number` ; `end?`: `number` ; `start?`: `number`  } |
| `numberGroup.by` | `number` |
| `numberGroup.end?` | `number` |
| `numberGroup.start?` | `number` |
| `originFieldName` | `string` |

___

### <a id="ipivotarea" name="ipivotarea"></a> IPivotArea

Ƭ **IPivotArea**: `Object`

**`property`** {GC.Spread.Pivot.PivotAreaType} [type]

**`property`** {string} [fieldName]

**`property`** {boolean} [labelOnly]

**`property`** {boolean} [dataOnly]

**`property`** {boolean} [grandRow]

**`property`** {boolean} [grandCol]

**`property`** {GC.Spread.Pivot.IPivotReference[]} [references]

**`property`** {GC.Spread.Pivot.IPivotAreaOffset} [offset]

#### Type declaration

| Name | Type |
| :------ | :------ |
| `dataOnly?` | `boolean` |
| `fieldName?` | `string` |
| `grandCol?` | `boolean` |
| `grandRow?` | `boolean` |
| `labelOnly?` | `boolean` |
| `references?` | [`IPivotReference`](GC.Spread.Pivot.md#ipivotreference)[] |
| `type?` | [`PivotAreaType`](../enums/GC.Spread.Pivot.PivotAreaType.md) |

___

### <a id="ipivotareaoffset" name="ipivotareaoffset"></a> IPivotAreaOffset

Ƭ **IPivotAreaOffset**: `Object`

**`property`** {number} row

**`property`** {number} col

**`property`** {number} [rowCount]

**`property`** {number} [colCount]

#### Type declaration

| Name | Type |
| :------ | :------ |
| `col` | `number` |
| `colCount?` | `number` |
| `row` | `number` |
| `rowCount?` | `number` |

___

### <a id="ipivotareascollection" name="ipivotareascollection"></a> IPivotAreasCollection

Ƭ **IPivotAreasCollection**: `Object`

**`property`** {Object.<string, GC.Spread.Pivot.IPivotArea[]>} - key 键表示透视表名称，值表示选定的透视区域

#### Index signature

▪ [pivotTableName: `string`]: [`IPivotArea`](GC.Spread.Pivot.md#ipivotarea)[]

___

### <a id="ipivotconditionfilterinfo" name="ipivotconditionfilterinfo"></a> IPivotConditionFilterInfo

Ƭ **IPivotConditionFilterInfo**: `Object`

**`property`** {string} conditionByName

**`property`** {GC.Pivot.IPivotCaptionConditionFilterInfo | GC.Pivot.IPivotDateConditionFilterInfo | GC.Pivot.IPivotTop10ConditionFilterInfo | GC.Pivot.IPivotValueConditionInfo} condition

#### Type declaration

| Name | Type |
| :------ | :------ |
| `condition` | [`IPivotCaptionConditionFilterInfo`](GC.Pivot.md#ipivotcaptionconditionfilterinfo) \| [`IPivotDateConditionFilterInfo`](GC.Pivot.md#ipivotdateconditionfilterinfo) \| [`IPivotTop10ConditionFilterInfo`](GC.Pivot.md#ipivottop10conditionfilterinfo) \| [`IPivotValueConditionInfo`](GC.Pivot.md#ipivotvalueconditioninfo) |
| `conditionByName` | `string` |

___

### <a id="ipivotnodeinfo" name="ipivotnodeinfo"></a> IPivotNodeInfo

Ƭ **IPivotNodeInfo**: `Object`

**`property`** {GC.Spread.Pivot.IPivotItemInfo[]} fieldInfos 节点信息的标签字段信息。

**`property`** {GC.Pivot.IValueInfo} valueInfo 节点信息的值字段信息。

#### Type declaration

| Name | Type |
| :------ | :------ |
| `fieldInfos` | [`IPivotItemInfo`](../interfaces/GC.Spread.Pivot.IPivotItemInfo.md)[] |
| `valueInfo` | [`IValueInfo`](GC.Pivot.md#ivalueinfo) |

___

### <a id="ipivotoverwritenodeinfo" name="ipivotoverwritenodeinfo"></a> IPivotOverwriteNodeInfo

Ƭ **IPivotOverwriteNodeInfo**: `Object`

**`property`** {GC.Spread.Pivot.IPivotItemInfo[]} fieldInfos 节点信息的标签字段信息。

**`property`** {GC.Pivot.IValueInfo} valueInfo 节点信息的值字段信息。

**`property`** {number} value 节点信息的值。

#### Type declaration

| Name | Type |
| :------ | :------ |
| `fieldInfos` | [`IPivotItemInfo`](../interfaces/GC.Spread.Pivot.IPivotItemInfo.md)[] |
| `value` | `number` |
| `valueInfo` | [`IValueInfo`](GC.Pivot.md#ivalueinfo) |

___

### <a id="ipivotreference" name="ipivotreference"></a> IPivotReference

Ƭ **IPivotReference**: `Object`

**`property`** {string} fieldName

**`property`** {boolean} [subtotal]

**`property`** {string[]} [items]

#### Type declaration

| Name | Type |
| :------ | :------ |
| `fieldName` | `string` |
| `items?` | `string`[] |
| `subtotal?` | `boolean` |

___

### <a id="ipivotshowdataasinfo" name="ipivotshowdataasinfo"></a> IPivotShowDataAsInfo

Ƭ **IPivotShowDataAsInfo**: `Object`

**`property`** {string} baseFieldName

**`property`** {GC.Pivot.PivotShowDataAsBaseItemType} baseFieldItemType

**`property`** {string} baseFieldItem

#### Type declaration

| Name | Type |
| :------ | :------ |
| `baseFieldItem?` | `string` |
| `baseFieldItemType?` | [`PivotShowDataAsBaseItemType`](../enums/GC.Pivot.PivotShowDataAsBaseItemType.md) |
| `baseFieldName?` | `string` |
| `showDataAs` | [`PivotShowDataAs`](../enums/GC.Pivot.PivotShowDataAs.md) |

___

### <a id="ipivotstyle" name="ipivotstyle"></a> IPivotStyle

Ƭ **IPivotStyle**: `Object`

**`property`** {GC.Spread.Pivot.IPivotArea} pivotArea 数据透视表中的数据透视区域

**`property`** {GC.Spread.Sheets.Style}  style 数据透视区域样式

#### Type declaration

| Name | Type |
| :------ | :------ |
| `pivotArea?` | [`IPivotArea`](GC.Spread.Pivot.md#ipivotarea) |
| `style?` | [`Style`](../classes/GC.Spread.Sheets.Style.md) |

___

### <a id="ipivottableoption" name="ipivottableoption"></a> IPivotTableOption

Ƭ **IPivotTableOption**: `Object`

**`property`** {boolean} [allowMultipleFiltersPerField]

**`property`** {boolean} [fillDownLabels]

**`property`** {boolean} [insertBlankLineAfterEachItem]

**`property`** {GC.Spread.Pivot.GrandTotalPosition} grandTotalPosition

**`property`** {GC.Spread.Pivot.SubtotalsPosition} subtotalsPosition

**`property`** {GC.Spread.Pivot.DisplayFields} displayFieldsInPageFilterArea

**`property`** {number} reportFilterFieldsPerColumn

**`property`** {boolean} [bandRows]

**`property`** {boolean} [bandColumns]

**`property`** {boolean} [showRowHeader]

**`property`** {boolean} [showColumnHeader]

**`property`** {boolean} [showDrill]

**`property`** {boolean} [showMissing]

**`property`** {string | number} missingCaption

**`property`** {number} rowLabelIndent

**`property`** {boolean} [printDrill]

**`property`** {boolean} [itemPrintTitles]

**`property`** {boolean} [fieldPrintTitles]

**`property`** {boolean} [showFilter]

**`property`** {boolean} [showToolTip]

**`property`** {boolean} [mergeItem]

**`property`** {boolean} [isShowErrorValue]

**`property`** {string} [errorValueInfo]

**`property`** {string} [rowHeaderCaption]

**`property`** {string} [colHeaderCaption]

**`property`** {string} [showHeaders]

**`property`** {GC.Spread.Pivot.CalcItemAggregation} [calcItemAggregation]

**`property`** {boolean} [enableDataValueEditing]

#### Type declaration

| Name | Type |
| :------ | :------ |
| `allowMultipleFiltersPerField?` | `boolean` |
| `bandColumns?` | `boolean` |
| `bandRows?` | `boolean` |
| `calcItemAggregation?` | [`CalcItemAggregation`](../enums/GC.Spread.Pivot.CalcItemAggregation.md) |
| `colHeaderCaption?` | `string` |
| `displayFieldsInPageFilterArea?` | [`DisplayFields`](../enums/GC.Spread.Pivot.DisplayFields.md) |
| `enableDataValueEditing?` | `boolean` |
| `errorValueInfo?` | `string` |
| `fieldPrintTitles?` | `boolean` |
| `fillDownLabels?` | `boolean` |
| `grandTotalPosition?` | [`GrandTotalPosition`](../enums/GC.Spread.Pivot.GrandTotalPosition.md) |
| `insertBlankLineAfterEachItem?` | `boolean` |
| `isShowErrorValue?` | `boolean` |
| `itemPrintTitles?` | `boolean` |
| `mergeItem?` | `boolean` |
| `missingCaption?` | `string` \| `number` |
| `printDrill?` | `boolean` |
| `reportFilterFieldsPerColumn?` | `number` |
| `rowHeaderCaption?` | `string` |
| `rowLabelIndent?` | `number` |
| `showColumnHeader?` | `boolean` |
| `showDrill?` | `boolean` |
| `showFilter?` | `boolean` |
| `showHeaders?` | `boolean` |
| `showMissing?` | `boolean` |
| `showRowHeader?` | `boolean` |
| `showToolTip?` | `boolean` |
| `subtotalsPosition?` | [`SubtotalsPosition`](../enums/GC.Spread.Pivot.SubtotalsPosition.md) |

___

### <a id="ipivottableposition" name="ipivottableposition"></a> IPivotTablePosition

Ƭ **IPivotTablePosition**: `Object`

**`property`** {number} row 数据透视表起始行

**`property`** {number} col 数据透视表起始列

**`property`** {number} [sheetName] 透视表在哪张表单上

#### Type declaration

| Name | Type |
| :------ | :------ |
| `col` | `number` |
| `row` | `number` |
| `sheetName?` | `string` |

___

### <a id="ipivottablerange" name="ipivottablerange"></a> IPivotTableRange

Ƭ **IPivotTableRange**: `Object`

**`property`** {GC.Spread.Sheets.Range} page 筛选面积范围

**`property`** {GC.Spread.Sheets.Range} content 内容区域范围

#### Type declaration

| Name | Type |
| :------ | :------ |
| `content` | [`Range`](../classes/GC.Spread.Sheets.Range.md) |
| `page` | [`Range`](../classes/GC.Spread.Sheets.Range.md) |

___

### <a id="ipivottableview" name="ipivottableview"></a> IPivotTableView

Ƭ **IPivotTableView**: `Object`

**`property`** {string} name

**`property`** {GC.Spread.Pivot.ISerializeInfo} config

#### Type declaration

| Name | Type |
| :------ | :------ |
| `config` | [`ISerializeInfo`](GC.Spread.Pivot.md#iserializeinfo) |
| `name` | `string` |

___

### <a id="ipivottextfilterinfo" name="ipivottextfilterinfo"></a> IPivotTextFilterInfo

Ƭ **IPivotTextFilterInfo**: `Object`

**`property`** {GC.Spread.Pivot.ITextCollectionCondition} textItem

#### Type declaration

| Name | Type |
| :------ | :------ |
| `textItem` | [`ITextCollectionCondition`](GC.Spread.Pivot.md#itextcollectioncondition) |

___

### <a id="iserializefieldinfo" name="iserializefieldinfo"></a> ISerializeFieldInfo

Ƭ **ISerializeFieldInfo**: `Object`

**`property`** {string} conditionBySourceName

**`property`** {string} displayName

**`property`** {GC.Pivot.SubtotalType} [subtotal]

**`property`** {GC.Spread.Pivot.IPivotTextFilterInfo | GC.Spread.Pivot.IPivotConditionFilterInfo} [labelFilter]

**`property`** {GC.Spread.Pivot.IPivotConditionFilterInfo} [valueFilter]

**`property`** {GC.Pivot.IPivotViewSortInfo} [sortInfo]

#### Type declaration

| Name | Type |
| :------ | :------ |
| `displayName` | `string` |
| `labelFilter?` | [`IPivotTextFilterInfo`](GC.Spread.Pivot.md#ipivottextfilterinfo) \| [`IPivotConditionFilterInfo`](GC.Spread.Pivot.md#ipivotconditionfilterinfo) |
| `sortInfo?` | [`IPivotViewSortInfo`](GC.Pivot.md#ipivotviewsortinfo) |
| `sourceName` | `string` |
| `subtotal?` | [`SubtotalType`](../enums/GC.Pivot.SubtotalType.md) |
| `valueFilter?` | [`IPivotConditionFilterInfo`](GC.Spread.Pivot.md#ipivotconditionfilterinfo) |

___

### <a id="iserializeinfo" name="iserializeinfo"></a> ISerializeInfo

Ƭ **ISerializeInfo**: `Object`

**`property`** {GC.Spread.Pivot.PivotTableLayoutType} [layoutType]

**`property`** {object} [options] 透视表的选项

**`property`** {string} [theme] 透视表的主题

**`property`** {GC.Pivot.IDataPosition} [valuePosition] 透视表的valuePosition信息

**`property`** {number[]} [pivotTablePosition] 透视表的位置

**`property`** {GC.Spread.Pivot.ISerializeFieldInfo[][]} [fieldsInfo] 透视表的字段信息

**`property`** {GC.Spread.Pivot.IPivotStyle} [styles] 透视表的透视区域样式

**`property`** {object} [collapseItems] 透视表的折叠信息

**`property`** {GC.Spread.Pivot.ISerializeShowDataAsInfo[]} [showDataAsList] 将数据显示为透视表的信息

#### Type declaration

| Name | Type |
| :------ | :------ |
| `collapseItems?` | `object` |
| `fieldsInfo?` | [`ISerializeFieldInfo`](GC.Spread.Pivot.md#iserializefieldinfo)[][] |
| `layoutType?` | [`PivotTableLayoutType`](../enums/GC.Spread.Pivot.PivotTableLayoutType.md) |
| `options?` | `object` |
| `pivotTablePosition?` | `number`[] |
| `showDataAsList?` | [`ISerializeShowDataAsInfo`](GC.Spread.Pivot.md#iserializeshowdataasinfo)[] |
| `showNoDataInfo?` | `object` |
| `styles?` | [`IPivotStyle`](GC.Spread.Pivot.md#ipivotstyle)[] |
| `theme?` | `string` |
| `valuePosition?` | [`IDataPosition`](GC.Pivot.md#idataposition) |

___

### <a id="iserializeshowdataasinfo" name="iserializeshowdataasinfo"></a> ISerializeShowDataAsInfo

Ƭ **ISerializeShowDataAsInfo**: `Object`

**`property`** {string} valueFieldName

**`property`** {GC.Spread.Pivot.IPivotShowDataAsInfo} showDataAsInfo

#### Type declaration

| Name | Type |
| :------ | :------ |
| `showDataAsInfo` | [`IPivotShowDataAsInfo`](GC.Spread.Pivot.md#ipivotshowdataasinfo) |
| `valueFieldName` | `string` |

___

### <a id="isourcefieldinfo" name="isourcefieldinfo"></a> ISourceFieldInfo

Ƭ **ISourceFieldInfo**: `Object`

**`property`** {string} name 源字段的名称

**`property`** {GC.Pivot.PivotSourceFieldType} [fieldType] 数据透视字段类型为calc字段或group字段

#### Type declaration

| Name | Type |
| :------ | :------ |
| `fieldType?` | [`PivotSourceFieldType`](../enums/GC.Pivot.PivotSourceFieldType.md) |
| `name` | `string` |

___

### <a id="itextcollectioncondition" name="itextcollectioncondition"></a> ITextCollectionCondition

Ƭ **ITextCollectionCondition**: `Object`

**`property`** {string[]} list

**`property`** {boolean} isAll

#### Type declaration

| Name | Type |
| :------ | :------ |
| `isAll` | `boolean` |
| `list` | `string`[] |

___

### <a id="itextgroupinfo" name="itextgroupinfo"></a> ITextGroupInfo

Ƭ **ITextGroupInfo**: `Object`

**`property`** {string} originFieldName  源字段名称

**`property`** {object} textGroup  文本组

**`property`** {string} textGroup.fieldName  组字段名

**`property`** {GC.Pivot.IStringGroupItems} textGroup.groupItems  文本组项信息

#### Type declaration

| Name | Type |
| :------ | :------ |
| `originFieldName` | `string` |
| `textGroup` | { `fieldName`: `string` ; `groupItems`: [`IStringGroupItems`](GC.Pivot.md#istringgroupitems)  } |
| `textGroup.fieldName` | `string` |
| `textGroup.groupItems` | [`IStringGroupItems`](GC.Pivot.md#istringgroupitems) |
