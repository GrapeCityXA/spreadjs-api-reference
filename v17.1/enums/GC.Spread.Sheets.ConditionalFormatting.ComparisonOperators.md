# Enumeration: ComparisonOperators

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).ComparisonOperators

比较运算符

**`代码示例`**
```
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createDateValidator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.between, new Date(2012, 11, 31), new Date(2013, 11, 31));
dv.showInputMessage(true);
dv.inputMessage("Enter a date between 12/31/2012 and 12/31/2013.");
dv.inputTitle("Tip");
activeSheet.getCell(1, -1).validator(dv);
```

## Table of contents

### Enumeration members

- [between](GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.md#between)
- [equalsTo](GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.md#equalsto)
- [greaterThan](GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.md#greaterthan)
- [greaterThanOrEqualsTo](GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.md#greaterthanorequalsto)
- [lessThan](GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.md#lessthan)
- [lessThanOrEqualsTo](GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.md#lessthanorequalsto)
- [notBetween](GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.md#notbetween)
- [notEqualsTo](GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.md#notequalsto)

## Enumeration members

### <a id="between" name="between"></a> between

• **between** = `6`

单元格值是否在两个参数值之间

___

### <a id="equalsto" name="equalsto"></a> equalsTo

• **equalsTo** = `0`

单元格值是否等于参数值

___

### <a id="greaterthan" name="greaterthan"></a> greaterThan

• **greaterThan** = `2`

单元格值是否大于参数值

___

### <a id="greaterthanorequalsto" name="greaterthanorequalsto"></a> greaterThanOrEqualsTo

• **greaterThanOrEqualsTo** = `3`

单元格值是否大于或等于参数值

___

### <a id="lessthan" name="lessthan"></a> lessThan

• **lessThan** = `4`

单元格值是否小于参数值

___

### <a id="lessthanorequalsto" name="lessthanorequalsto"></a> lessThanOrEqualsTo

• **lessThanOrEqualsTo** = `5`

单元格值是否小于或等于参数值

___

### <a id="notbetween" name="notbetween"></a> notBetween

• **notBetween** = `7`

值是否不在两个参数值之间

___

### <a id="notequalsto" name="notequalsto"></a> notEqualsTo

• **notEqualsTo** = `1`

单元格值是否不等于参数值
