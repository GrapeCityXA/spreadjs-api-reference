# Enumeration: GeneralComparisonOperators

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).GeneralComparisonOperators

通用运算符

**`代码示例`**
```
//本示例验证单元格值
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.cellValueCondition);
nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.equalsTo);
nCondition.expected(0);
//当选项为false时，验证失败并显示红色警报
//当选项为true时，将把空白单元格视为零，验证成功
nCondition.treatNullValueAsZero(false);
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
validator.ignoreBlank(false);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, null);
alert(validator.value2());
```

## Table of contents

### Enumeration members

- [equalsTo](GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.md#equalsto)
- [greaterThan](GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.md#greaterthan)
- [greaterThanOrEqualsTo](GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.md#greaterthanorequalsto)
- [lessThan](GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.md#lessthan)
- [lessThanOrEqualsTo](GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.md#lessthanorequalsto)
- [notEqualsTo](GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.md#notequalsto)

## Enumeration members

### <a id="equalsto" name="equalsto"></a> equalsTo

• **equalsTo** = `0`

该数值是否等于指定数值

___

### <a id="greaterthan" name="greaterthan"></a> greaterThan

• **greaterThan** = `2`

该数值是否大于指定数值

___

### <a id="greaterthanorequalsto" name="greaterthanorequalsto"></a> greaterThanOrEqualsTo

• **greaterThanOrEqualsTo** = `3`

该数值是否大于或等于指定数值

___

### <a id="lessthan" name="lessthan"></a> lessThan

• **lessThan** = `4`

该数值是否小于指定数值

___

### <a id="lessthanorequalsto" name="lessthanorequalsto"></a> lessThanOrEqualsTo

• **lessThanOrEqualsTo** = `5`

该数值是否小于或等于指定数值

___

### <a id="notequalsto" name="notequalsto"></a> notEqualsTo

• **notEqualsTo** = `1`

该数值是否不等于指定数值
