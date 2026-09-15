# Enumeration: LogicalOperators

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).LogicalOperators

指定关系运算符。

**`example`**
```
//此示例验证数据。
var condition1 = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.dateCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.DateCompareType.afterEqualsTo, expected: new Date(2012, 11, 31)});
var condition2 = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.dateCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.DateCompareType.beforeEqualsTo, expected: new Date(2013, 11, 31)});
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.relationCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.LogicalOperators.and, item1: condition1, item2: condition2});
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, new Date(2012, 11, 25));
```

## Table of contents

### Enumeration members

- [and](GC.Spread.Sheets.ConditionalFormatting.LogicalOperators.md#and)
- [or](GC.Spread.Sheets.ConditionalFormatting.LogicalOperators.md#or)

## Enumeration members

### <a id="and" name="and"></a> and

• **and** = `1`

指定与关系。

___

### <a id="or" name="or"></a> or

• **or** = `0`

指定或关系。
