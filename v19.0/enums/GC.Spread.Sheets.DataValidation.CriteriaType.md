# Enumeration: CriteriaType

[Sheets](../modules/GC.Spread.Sheets.md).[DataValidation](../modules/GC.Spread.Sheets.DataValidation.md).CriteriaType

表示数据验证器的条件类型。

**`example`**
```
//此示例使用 CriteriaType 枚举。
var textLengthCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.textLengthCondition);
textLengthCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.greaterThan);
textLengthCondition.formula("$C$1"); // 用于计算数字的公式。
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(textLengthCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, "abcf");
//将值 3 设置到 $C$1，执行此代码后，Cell(0,0) 中的值有效。
activeSheet.setValue(0, 2, 3);
//将值 5 设置到 $C$1，执行此代码后，Cell(0,0) 中的值无效。
// activeSheet.setValue(0, 2, 5);
```

## Table of contents

### Enumeration members

- [anyValue](GC.Spread.Sheets.DataValidation.CriteriaType.md#anyvalue)
- [custom](GC.Spread.Sheets.DataValidation.CriteriaType.md#custom)
- [date](GC.Spread.Sheets.DataValidation.CriteriaType.md#date)
- [decimalValues](GC.Spread.Sheets.DataValidation.CriteriaType.md#decimalvalues)
- [list](GC.Spread.Sheets.DataValidation.CriteriaType.md#list)
- [textLength](GC.Spread.Sheets.DataValidation.CriteriaType.md#textlength)
- [time](GC.Spread.Sheets.DataValidation.CriteriaType.md#time)
- [wholeNumber](GC.Spread.Sheets.DataValidation.CriteriaType.md#wholenumber)

## Enumeration members

### <a id="anyvalue" name="anyvalue"></a> anyValue

• **anyValue** = `0`

指定数据验证允许任何类型的值，不检查值的类型或范围。

___

### <a id="custom" name="custom"></a> custom

• **custom** = `7`

指定数据验证使用自定义公式检查单元格值。

___

### <a id="date" name="date"></a> date

• **date** = `4`

指定数据验证检查并允许满足给定条件的日期值。

___

### <a id="decimalvalues" name="decimalvalues"></a> decimalValues

• **decimalValues** = `2`

指定数据验证检查并允许满足给定条件的小数值。

___

### <a id="list" name="list"></a> list

• **list** = `3`

指定数据验证检查并允许匹配值列表中的某个值。

___

### <a id="textlength" name="textlength"></a> textLength

• **textLength** = `6`

指定数据验证检查并允许长度满足给定条件的文本值。

___

### <a id="time" name="time"></a> time

• **time** = `5`

指定数据验证检查并允许满足给定条件的时间值。

___

### <a id="wholenumber" name="wholenumber"></a> wholeNumber

• **wholeNumber** = `1`

指定数据验证检查并允许满足给定条件的整数值。
