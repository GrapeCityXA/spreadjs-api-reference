# Enumeration: RuleType

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).RuleType

指定规则类型。

**`example`**
```
// 此示例展示如何为NormalConditionRule设置规则类型。
activeSheet.setArray(0, 0, [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]);
activeSheet.setArray(0, 2, [1, 2, 3, 4, 5, 6, 5, 8, 1, 10]);
var greatThan = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
greatThan.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.cellValueRule);
greatThan.operator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.greaterThan);
greatThan.value1(4);
greatThan.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 1)]);
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
greatThan.style(style);
activeSheet.conditionalFormats.addRule(greatThan);
var unique = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
unique.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.uniqueRule);
unique.operator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.greaterThan);
unique.value1(5);
unique.ranges([new GC.Spread.Sheets.Range(0, 2, 10, 1)]);
var style = new GC.Spread.Sheets.Style();
style.backColor = "gold";
unique.style(style);
activeSheet.conditionalFormats.addRule(unique);
```

## Table of contents

### Enumeration members

- [averageRule](GC.Spread.Sheets.ConditionalFormatting.RuleType.md#averagerule)
- [cellValueRule](GC.Spread.Sheets.ConditionalFormatting.RuleType.md#cellvaluerule)
- [columnStateRule](GC.Spread.Sheets.ConditionalFormatting.RuleType.md#columnstaterule)
- [conditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.RuleType.md#conditionrulebase)
- [dataBarRule](GC.Spread.Sheets.ConditionalFormatting.RuleType.md#databarrule)
- [dateOccurringRule](GC.Spread.Sheets.ConditionalFormatting.RuleType.md#dateoccurringrule)
- [duplicateRule](GC.Spread.Sheets.ConditionalFormatting.RuleType.md#duplicaterule)
- [formulaRule](GC.Spread.Sheets.ConditionalFormatting.RuleType.md#formularule)
- [iconSetRule](GC.Spread.Sheets.ConditionalFormatting.RuleType.md#iconsetrule)
- [rowStateRule](GC.Spread.Sheets.ConditionalFormatting.RuleType.md#rowstaterule)
- [specificTextRule](GC.Spread.Sheets.ConditionalFormatting.RuleType.md#specifictextrule)
- [threeScaleRule](GC.Spread.Sheets.ConditionalFormatting.RuleType.md#threescalerule)
- [top10Rule](GC.Spread.Sheets.ConditionalFormatting.RuleType.md#top10rule)
- [twoScaleRule](GC.Spread.Sheets.ConditionalFormatting.RuleType.md#twoscalerule)
- [uniqueRule](GC.Spread.Sheets.ConditionalFormatting.RuleType.md#uniquerule)

## Enumeration members

### <a id="averagerule" name="averagerule"></a> averageRule

• **averageRule** = `8`

指定平均值规则。

___

### <a id="cellvaluerule" name="cellvaluerule"></a> cellValueRule

• **cellValueRule** = `1`

指定单元格值规则。

___

### <a id="columnstaterule" name="columnstaterule"></a> columnStateRule

• **columnStateRule** = `15`

指定列状态规则。

___

### <a id="conditionrulebase" name="conditionrulebase"></a> conditionRuleBase

• **conditionRuleBase** = `0`

指定条件的基础规则。

___

### <a id="databarrule" name="databarrule"></a> dataBarRule

• **dataBarRule** = `12`

指定数据条规则。

___

### <a id="dateoccurringrule" name="dateoccurringrule"></a> dateOccurringRule

• **dateOccurringRule** = `4`

指定日期出现规则。

___

### <a id="duplicaterule" name="duplicaterule"></a> duplicateRule

• **duplicateRule** = `7`

指定重复规则。

___

### <a id="formularule" name="formularule"></a> formulaRule

• **formulaRule** = `3`

指定公式规则。

___

### <a id="iconsetrule" name="iconsetrule"></a> iconSetRule

• **iconSetRule** = `13`

指定图标集规则。

___

### <a id="rowstaterule" name="rowstaterule"></a> rowStateRule

• **rowStateRule** = `14`

指定行状态规则。

___

### <a id="specifictextrule" name="specifictextrule"></a> specificTextRule

• **specificTextRule** = `2`

指定特定文本规则。

___

### <a id="threescalerule" name="threescalerule"></a> threeScaleRule

• **threeScaleRule** = `11`

指定三刻度规则。

___

### <a id="top10rule" name="top10rule"></a> top10Rule

• **top10Rule** = `5`

指定前10规则。

___

### <a id="twoscalerule" name="twoscalerule"></a> twoScaleRule

• **twoScaleRule** = `10`

指定双刻度规则。

___

### <a id="uniquerule" name="uniquerule"></a> uniqueRule

• **uniqueRule** = `6`

指定唯一规则。
