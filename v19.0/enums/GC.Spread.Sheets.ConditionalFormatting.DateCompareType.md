# Enumeration: DateCompareType

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).DateCompareType

指定日期比较类型。

**`example`**
```
//此示例验证单元格数据。
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.dateCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.DateCompareType.before, expected: new Date(2012, 11, 31)});
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, new Date(2012, 12, 12));
```

## Table of contents

### Enumeration members

- [after](GC.Spread.Sheets.ConditionalFormatting.DateCompareType.md#after)
- [afterEqualsTo](GC.Spread.Sheets.ConditionalFormatting.DateCompareType.md#afterequalsto)
- [before](GC.Spread.Sheets.ConditionalFormatting.DateCompareType.md#before)
- [beforeEqualsTo](GC.Spread.Sheets.ConditionalFormatting.DateCompareType.md#beforeequalsto)
- [equalsTo](GC.Spread.Sheets.ConditionalFormatting.DateCompareType.md#equalsto)
- [notEqualsTo](GC.Spread.Sheets.ConditionalFormatting.DateCompareType.md#notequalsto)

## Enumeration members

### <a id="after" name="after"></a> after

• **after** = `4`

指示日期时间是否在某个时间之后。

___

### <a id="afterequalsto" name="afterequalsto"></a> afterEqualsTo

• **afterEqualsTo** = `5`

指示日期时间是否在某个时间之后或等于该时间。

___

### <a id="before" name="before"></a> before

• **before** = `2`

指示日期时间是否在某个时间之前。

___

### <a id="beforeequalsto" name="beforeequalsto"></a> beforeEqualsTo

• **beforeEqualsTo** = `3`

指示日期时间是否在某个时间之前或等于该时间。

___

### <a id="equalsto" name="equalsto"></a> equalsTo

• **equalsTo** = `0`

指示日期时间是否等于某个时间。

___

### <a id="notequalsto" name="notequalsto"></a> notEqualsTo

• **notEqualsTo** = `1`

指示日期时间是否不等于某个时间。
