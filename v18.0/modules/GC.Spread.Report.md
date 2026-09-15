# Namespace: Report

[GC](GC.md).[Spread](GC.Spread.md).Report

## Table of contents

### Classes

- [ReportSheet](../classes/GC.Spread.Report.ReportSheet.md)
- [TemplateSheet](../classes/GC.Spread.Report.TemplateSheet.md)

### Interfaces

- [IColumnLayoutSetting](../interfaces/GC.Spread.Report.IColumnLayoutSetting.md)
- [IConditionRuleCellType](../interfaces/GC.Spread.Report.IConditionRuleCellType.md)
- [IConditionRuleDataColumnType](../interfaces/GC.Spread.Report.IConditionRuleDataColumnType.md)
- [IConditionRuleFormulaType](../interfaces/GC.Spread.Report.IConditionRuleFormulaType.md)
- [IConditionRuleParameterType](../interfaces/GC.Spread.Report.IConditionRuleParameterType.md)
- [IConditionRuleValueType](../interfaces/GC.Spread.Report.IConditionRuleValueType.md)
- [IDataCell](../interfaces/GC.Spread.Report.IDataCell.md)
- [IDataCellBase](../interfaces/GC.Spread.Report.IDataCellBase.md)
- [IDataColumn](../interfaces/GC.Spread.Report.IDataColumn.md)
- [IEntityFieldInfo](../interfaces/GC.Spread.Report.IEntityFieldInfo.md)
- [IFailedRecord](../interfaces/GC.Spread.Report.IFailedRecord.md)
- [IField](../interfaces/GC.Spread.Report.IField.md)
- [IFilter](../interfaces/GC.Spread.Report.IFilter.md)
- [IFilterConditionAndRelationType](../interfaces/GC.Spread.Report.IFilterConditionAndRelationType.md)
- [IFilterConditionOrRelationType](../interfaces/GC.Spread.Report.IFilterConditionOrRelationType.md)
- [IGroupBin](../interfaces/GC.Spread.Report.IGroupBin.md)
- [IPaginationSetting](../interfaces/GC.Spread.Report.IPaginationSetting.md)
- [IParameterChangedArgs](../interfaces/GC.Spread.Report.IParameterChangedArgs.md)
- [IRecord](../interfaces/GC.Spread.Report.IRecord.md)
- [IReportOptions](../interfaces/GC.Spread.Report.IReportOptions.md)
- [IReportSheetDataChangedEventArgs](../interfaces/GC.Spread.Report.IReportSheetDataChangedEventArgs.md)
- [IReportSheetDataChangingEventArgs](../interfaces/GC.Spread.Report.IReportSheetDataChangingEventArgs.md)
- [IReportSheetRecordsSubmittedEventArgs](../interfaces/GC.Spread.Report.IReportSheetRecordsSubmittedEventArgs.md)
- [IReportSheetRecordsSubmittingEventArgs](../interfaces/GC.Spread.Report.IReportSheetRecordsSubmittingEventArgs.md)
- [IRowLayoutSetting](../interfaces/GC.Spread.Report.IRowLayoutSetting.md)
- [ITemplateCellCommonSetting](../interfaces/GC.Spread.Report.ITemplateCellCommonSetting.md)
- [ITemplateOptions](../interfaces/GC.Spread.Report.ITemplateOptions.md)
- [IWriteBackRule](../interfaces/GC.Spread.Report.IWriteBackRule.md)

### Type aliases

- [Binding](GC.Spread.Report.md#binding)
- [CellAddress](GC.Spread.Report.md#celladdress)
- [Change](GC.Spread.Report.md#change)
- [ChartCell](GC.Spread.Report.md#chartcell)
- [ConditionRule](GC.Spread.Report.md#conditionrule)
- [ConditionRuleOperator](GC.Spread.Report.md#conditionruleoperator)
- [DataEntrySetting](GC.Spread.Report.md#dataentrysetting)
- [DataType](GC.Spread.Report.md#datatype)
- [FieldState](GC.Spread.Report.md#fieldstate)
- [FilterCondition](GC.Spread.Report.md#filtercondition)
- [FilterConditionFormulaRule](GC.Spread.Report.md#filterconditionformularule)
- [Formula](GC.Spread.Report.md#formula)
- [GroupCell](GC.Spread.Report.md#groupcell)
- [InitParametersUIFunctionType](GC.Spread.Report.md#initparametersuifunctiontype)
- [LayoutSetting](GC.Spread.Report.md#layoutsetting)
- [ListCell](GC.Spread.Report.md#listcell)
- [OnChangeFunctionType](GC.Spread.Report.md#onchangefunctiontype)
- [PaginationOrder](GC.Spread.Report.md#paginationorder)
- [RenderMode](GC.Spread.Report.md#rendermode)
- [SheetNameGenerator](GC.Spread.Report.md#sheetnamegenerator)
- [SortOption](GC.Spread.Report.md#sortoption)
- [SpillDirection](GC.Spread.Report.md#spilldirection)
- [StaticCell](GC.Spread.Report.md#staticcell)
- [SummaryAggregate](GC.Spread.Report.md#summaryaggregate)
- [SummaryCell](GC.Spread.Report.md#summarycell)
- [TemplateCell](GC.Spread.Report.md#templatecell)

## Type aliases

### <a id="binding" name="binding"></a> Binding

Ƭ **Binding**: `string`

___

### <a id="celladdress" name="celladdress"></a> CellAddress

Ƭ **CellAddress**: `string`

___

### <a id="change" name="change"></a> Change

Ƭ **Change**: `Object`

**`property`** {GC.Spread.Report.IRecord[]} records - 更新和插入的记录。

**`property`** {GC.Spread.Report.IRecord[]} deleteRecords - 已删除的记录。

**`property`** {GC.Spread.Report.IWriteBackRule} rule - 报表表dataEntry回写规则。

#### Type declaration

| Name | Type | Description |
| :------ | :------ | :------ |
| `deleteRecords` | [`IRecord`](../interfaces/GC.Spread.Report.IRecord.md)[] | 已删除的记录。 |
| `records` | [`IRecord`](../interfaces/GC.Spread.Report.IRecord.md)[] | 更新和插入的记录。 |
| `rule` | [`IWriteBackRule`](../interfaces/GC.Spread.Report.IWriteBackRule.md) | 报表表dataEntry回写规则。 |

___

### <a id="chartcell" name="chartcell"></a> ChartCell

Ƭ **ChartCell**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `chartPreviewVisible?` | `boolean` |
| `dataChartName` | `string` |
| `type` | ``"Chart"`` |

___

### <a id="conditionrule" name="conditionrule"></a> ConditionRule

Ƭ **ConditionRule**: { `column`: `string` ; `operator`: [`ConditionRuleOperator`](GC.Spread.Report.md#conditionruleoperator)  } & [`IConditionRuleValueType`](../interfaces/GC.Spread.Report.IConditionRuleValueType.md) \| [`IConditionRuleCellType`](../interfaces/GC.Spread.Report.IConditionRuleCellType.md) \| [`IConditionRuleDataColumnType`](../interfaces/GC.Spread.Report.IConditionRuleDataColumnType.md) \| [`IConditionRuleParameterType`](../interfaces/GC.Spread.Report.IConditionRuleParameterType.md) \| [`IConditionRuleFormulaType`](../interfaces/GC.Spread.Report.IConditionRuleFormulaType.md)

___

### <a id="conditionruleoperator" name="conditionruleoperator"></a> ConditionRuleOperator

Ƭ **ConditionRuleOperator**: ``"Equal"`` \| ``"NotEqual"`` \| ``"GreaterThanOrEqual"`` \| ``"GreaterThan"`` \| ``"LessThanOrEqual"`` \| ``"LessThan"`` \| ``"StartWith"`` \| ``"NotStartWith"`` \| ``"EndWith"`` \| ``"NotEndWith"`` \| ``"Contains"`` \| ``"NotContains"`` \| ``"In"`` \| ``"NotIn"``

___

### <a id="dataentrysetting" name="dataentrysetting"></a> DataEntrySetting

Ƭ **DataEntrySetting**: [`IWriteBackRule`](../interfaces/GC.Spread.Report.IWriteBackRule.md)[]

___

### <a id="datatype" name="datatype"></a> DataType

Ƭ **DataType**: `number` \| `string` \| `Date` \| `boolean`

___

### <a id="fieldstate" name="fieldstate"></a> FieldState

Ƭ **FieldState**: ``"normal"`` \| ``"new"`` \| ``"updated"`` \| ``"deleted"``

___

### <a id="filtercondition" name="filtercondition"></a> FilterCondition

Ƭ **FilterCondition**: [`ConditionRule`](GC.Spread.Report.md#conditionrule) \| [`FilterConditionFormulaRule`](GC.Spread.Report.md#filterconditionformularule) \| [`IFilterConditionAndRelationType`](../interfaces/GC.Spread.Report.IFilterConditionAndRelationType.md) \| [`IFilterConditionOrRelationType`](../interfaces/GC.Spread.Report.IFilterConditionOrRelationType.md)

___

### <a id="filterconditionformularule" name="filterconditionformularule"></a> FilterConditionFormulaRule

Ƭ **FilterConditionFormulaRule**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `formula` | `string` |

___

### <a id="formula" name="formula"></a> Formula

Ƭ **Formula**: `string`

___

### <a id="groupcell" name="groupcell"></a> GroupCell

Ƭ **GroupCell**: [`IDataCellBase`](../interfaces/GC.Spread.Report.IDataCellBase.md) & { `bins?`: [`IGroupBin`](../interfaces/GC.Spread.Report.IGroupBin.md)[] ; `formula?`: [`Formula`](GC.Spread.Report.md#formula) ; `type`: ``"Group"``  }

___

### <a id="initparametersuifunctiontype" name="initparametersuifunctiontype"></a> InitParametersUIFunctionType

Ƭ **InitParametersUIFunctionType**: (`sheet`: [`Worksheet`](../classes/GC.Spread.Sheets.Worksheet.md)) => `void`

#### Type declaration

▸ (`sheet`): `void`

**`description`** 渲染parameterUIsheet时的回调。

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheet` | [`Worksheet`](../classes/GC.Spread.Sheets.Worksheet.md) | 初始化parameterUI表，用户可以在这里更新parameterUI表。 |

##### Returns

`void`

___

### <a id="layoutsetting" name="layoutsetting"></a> LayoutSetting

Ƭ **LayoutSetting**: [`IRowLayoutSetting`](../interfaces/GC.Spread.Report.IRowLayoutSetting.md) \| [`IColumnLayoutSetting`](../interfaces/GC.Spread.Report.IColumnLayoutSetting.md)

___

### <a id="listcell" name="listcell"></a> ListCell

Ƭ **ListCell**: [`IDataCellBase`](../interfaces/GC.Spread.Report.IDataCellBase.md) & { `spillMode?`: ``"Insert"`` \| ``"Overwrite"`` ; `type`: ``"List"``  }

___

### <a id="onchangefunctiontype" name="onchangefunctiontype"></a> OnChangeFunctionType

Ƭ **OnChangeFunctionType**: (`sheet`: [`ReportSheet`](../classes/GC.Spread.Report.ReportSheet.md), `changedArgs`: [`IParameterChangedArgs`](../interfaces/GC.Spread.Report.IParameterChangedArgs.md)) => `void`

#### Type declaration

▸ (`sheet`, `changedArgs`): `void`

**`description`** 参数UI值改变时的回调。

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheet` | [`ReportSheet`](../classes/GC.Spread.Report.ReportSheet.md) | 参数UI绑定reportSheet。 |
| `changedArgs` | [`IParameterChangedArgs`](../interfaces/GC.Spread.Report.IParameterChangedArgs.md) | 更改后的参数值。 |

##### Returns

`void`

___

### <a id="paginationorder" name="paginationorder"></a> PaginationOrder

Ƭ **PaginationOrder**: ``"DownThenOver"`` \| ``"OverThenDown"``

___

### <a id="rendermode" name="rendermode"></a> RenderMode

Ƭ **RenderMode**: ``"Design"`` \| ``"PaginatedPreview"`` \| ``"Preview"``

___

### <a id="sheetnamegenerator" name="sheetnamegenerator"></a> SheetNameGenerator

Ƭ **SheetNameGenerator**: (`pageIndex`: `number`) => `string`

#### Type declaration

▸ (`pageIndex`): `string`

##### Parameters

| Name | Type |
| :------ | :------ |
| `pageIndex` | `number` |

##### Returns

`string`

___

### <a id="sortoption" name="sortoption"></a> SortOption

Ƭ **SortOption**: { `asc`: `string`  } \| { `desc`: `string`  } & { `list?`: `string`[]  }

___

### <a id="spilldirection" name="spilldirection"></a> SpillDirection

Ƭ **SpillDirection**: ``"Horizontal"`` \| ``"Vertical"`` \| ``"None"``

___

### <a id="staticcell" name="staticcell"></a> StaticCell

Ƭ **StaticCell**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `autoExpand?` | ``"Both"`` \| ``"Horizontal"`` \| ``"Vertical"`` \| ``"None"`` |
| `initialExpansionState?` | ``"Expanded"`` \| ``"Collapsed"`` |
| `pin?` | ``"None"`` \| ``"Row"`` \| ``"Column"`` \| ``"Both"`` |
| `showCollapseButton?` | `boolean` |
| `type` | ``"Static"`` |

___

### <a id="summaryaggregate" name="summaryaggregate"></a> SummaryAggregate

Ƭ **SummaryAggregate**: ``"Sum"`` \| ``"Avg"`` \| ``"Max"`` \| ``"Min"`` \| ``"Count"``

___

### <a id="summarycell" name="summarycell"></a> SummaryCell

Ƭ **SummaryCell**: [`IDataCellBase`](../interfaces/GC.Spread.Report.IDataCellBase.md) & { `aggregate`: [`SummaryAggregate`](GC.Spread.Report.md#summaryaggregate) ; `type`: ``"Summary"``  }

___

### <a id="templatecell" name="templatecell"></a> TemplateCell

Ƭ **TemplateCell**: [`ListCell`](GC.Spread.Report.md#listcell) \| [`GroupCell`](GC.Spread.Report.md#groupcell) \| [`SummaryCell`](GC.Spread.Report.md#summarycell) \| [`StaticCell`](GC.Spread.Report.md#staticcell) \| [`ChartCell`](GC.Spread.Report.md#chartcell) & [`ITemplateCellCommonSetting`](../interfaces/GC.Spread.Report.ITemplateCellCommonSetting.md)
