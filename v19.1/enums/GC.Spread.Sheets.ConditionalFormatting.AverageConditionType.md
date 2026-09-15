# Enumeration: AverageConditionType

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).AverageConditionType

指定平均值条件类型。

**`example`**
```javascript
//此示例创建一个平均值规则。
activeSheet.setValue(0,0, 1,3);
activeSheet.setValue(1,0, 50,3);
activeSheet.setValue(2,0, 100,3);
activeSheet.setValue(3,0, 2,3);
activeSheet.setValue(4,0, 60,3);
activeSheet.setValue(5,0, 90,3);
activeSheet.setValue(6,0, 3,3);
activeSheet.setValue(7,0, 40,3);
activeSheet.setValue(8,0, 70,3);
activeSheet.setValue(9,0, 5,3);
activeSheet.setValue(10,0, 35,3);
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
style.borderLeft =new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderTop = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderRight = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderBottom = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
var rule = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
rule.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.averageRule);
rule.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 3)]);
rule.style(style);
rule.type(GC.Spread.Sheets.ConditionalFormatting.AverageConditionType.above);
activeSheet.conditionalFormats.addRule(rule);
```

## Table of contents

### Enumeration members

- [above](GC.Spread.Sheets.ConditionalFormatting.AverageConditionType.md#above)
- [above1StdDev](GC.Spread.Sheets.ConditionalFormatting.AverageConditionType.md#above1stddev)
- [above2StdDev](GC.Spread.Sheets.ConditionalFormatting.AverageConditionType.md#above2stddev)
- [above3StdDev](GC.Spread.Sheets.ConditionalFormatting.AverageConditionType.md#above3stddev)
- [below](GC.Spread.Sheets.ConditionalFormatting.AverageConditionType.md#below)
- [below1StdDev](GC.Spread.Sheets.ConditionalFormatting.AverageConditionType.md#below1stddev)
- [below2StdDev](GC.Spread.Sheets.ConditionalFormatting.AverageConditionType.md#below2stddev)
- [below3StdDev](GC.Spread.Sheets.ConditionalFormatting.AverageConditionType.md#below3stddev)
- [equalOrAbove](GC.Spread.Sheets.ConditionalFormatting.AverageConditionType.md#equalorabove)
- [equalOrBelow](GC.Spread.Sheets.ConditionalFormatting.AverageConditionType.md#equalorbelow)

## Enumeration members

### <a id="above" name="above"></a> above

• **above** = `0`

指定高于平均值的条件。

___

### <a id="above1stddev" name="above1stddev"></a> above1StdDev

• **above1StdDev** = `4`

指定高于一个标准差的条件。

___

### <a id="above2stddev" name="above2stddev"></a> above2StdDev

• **above2StdDev** = `6`

指定高于两个标准差的条件。

___

### <a id="above3stddev" name="above3stddev"></a> above3StdDev

• **above3StdDev** = `8`

指定高于三个标准差的条件。

___

### <a id="below" name="below"></a> below

• **below** = `1`

指定低于平均值的条件。

___

### <a id="below1stddev" name="below1stddev"></a> below1StdDev

• **below1StdDev** = `5`

指定低于一个标准差的条件。

___

### <a id="below2stddev" name="below2stddev"></a> below2StdDev

• **below2StdDev** = `7`

指定低于两个标准差的条件。

___

### <a id="below3stddev" name="below3stddev"></a> below3StdDev

• **below3StdDev** = `9`

指定低于三个标准差的条件。

___

### <a id="equalorabove" name="equalorabove"></a> equalOrAbove

• **equalOrAbove** = `2`

指定高于或等于平均值的条件。

___

### <a id="equalorbelow" name="equalorbelow"></a> equalOrBelow

• **equalOrBelow** = `3`

指定低于或等于平均值的条件。
