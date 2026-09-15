# Enumeration: CustomValueType

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).CustomValueType

自定义值类型

**`代码示例`**
``` javascript
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.formulaCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.CustomValueType.nonEmpty});
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
validator.ignoreBlank(false);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
```

## Table of contents

### Enumeration members

- [empty](GC.Spread.Sheets.ConditionalFormatting.CustomValueType.md#empty)
- [error](GC.Spread.Sheets.ConditionalFormatting.CustomValueType.md#error)
- [formula](GC.Spread.Sheets.ConditionalFormatting.CustomValueType.md#formula)
- [nonEmpty](GC.Spread.Sheets.ConditionalFormatting.CustomValueType.md#nonempty)
- [nonError](GC.Spread.Sheets.ConditionalFormatting.CustomValueType.md#nonerror)

## Enumeration members

### <a id="empty" name="empty"></a> empty

• **empty** = `0`

单元格值是否为empty还是null

___

### <a id="error" name="error"></a> error

• **error** = `2`

单元格值是否包含计算错误

___

### <a id="formula" name="formula"></a> formula

• **formula** = `4`

单元格值是否为公式

___

### <a id="nonempty" name="nonempty"></a> nonEmpty

• **nonEmpty** = `1`

单元格值是否不为empty或null

___

### <a id="nonerror" name="nonerror"></a> nonError

• **nonError** = `3`

单元格值是否不包含计算错误
