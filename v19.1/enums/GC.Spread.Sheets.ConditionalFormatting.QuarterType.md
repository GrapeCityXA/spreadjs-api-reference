# Enumeration: QuarterType

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).QuarterType

表示季度类型。

**`example`**
```javascript
var style = new GC.Spread.Sheets.Style();
style.backColor = "lightgreen";
// 创建第一季度的条件
var condition = new GC.Spread.Sheets.ConditionalFormatting.Condition(
    GC.Spread.Sheets.ConditionalFormatting.ConditionType.dateExCondition,
    {
        expected: GC.Spread.Sheets.ConditionalFormatting.QuarterType.quarter1
    }
);
condition.expectTypeId(GC.Spread.Sheets.ConditionalFormatting.DateExConditionExpectType.quarterOccurring);
// 使用该条件创建规则
var rule = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
rule.condition(condition);
rule.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 1)]);
rule.style(style);
activeSheet.conditionalFormats.addRule(rule);
```

## Table of contents

### Enumeration members

- [quarter1](GC.Spread.Sheets.ConditionalFormatting.QuarterType.md#quarter1)
- [quarter2](GC.Spread.Sheets.ConditionalFormatting.QuarterType.md#quarter2)
- [quarter3](GC.Spread.Sheets.ConditionalFormatting.QuarterType.md#quarter3)
- [quarter4](GC.Spread.Sheets.ConditionalFormatting.QuarterType.md#quarter4)

## Enumeration members

### <a id="quarter1" name="quarter1"></a> quarter1

• **quarter1** = `0`

指示一年中的第一季度。

___

### <a id="quarter2" name="quarter2"></a> quarter2

• **quarter2** = `1`

指示一年中的第二季度。

___

### <a id="quarter3" name="quarter3"></a> quarter3

• **quarter3** = `2`

指示一年中的第三季度。

___

### <a id="quarter4" name="quarter4"></a> quarter4

• **quarter4** = `3`

指示一年中的第四季度。
