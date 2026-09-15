# Enumeration: CriteriaType

[Sheets](../modules/GC.Spread.Sheets.md).[DataValidation](../modules/GC.Spread.Sheets.DataValidation.md).CriteriaType

数据验证条件类型

**`代码示例`**
``` javascript
//本示例使用CriteriaType枚举
var textLengthCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.textLengthCondition);
textLengthCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.greaterThan);
textLengthCondition.formula("$C$1"); // 公式用于计算数字
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(textLengthCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, "abcf");
//将值3设置为$C$1,此代码之后，单元格(0,0)中的值有效
activeSheet.setValue(0, 2, 3);
//将值5设置为$C$1,此代码之后，单元格(0,0)中的值无效
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

数据验证允许任何类型的值，并且不检查值的类型或区域

___

### <a id="custom" name="custom"></a> custom

• **custom** = `7`

数据验证使用自定义公式来检查单元格值

___

### <a id="date" name="date"></a> date

• **date** = `4`

数据验证检查并允许满足给定条件的日期值

___

### <a id="decimalvalues" name="decimalvalues"></a> decimalValues

• **decimalValues** = `2`

数据验证检查并允许满足给定条件的十进制值

___

### <a id="list" name="list"></a> list

• **list** = `3`

数据验证检查并允许与值列表中的一个值匹配的值

___

### <a id="textlength" name="textlength"></a> textLength

• **textLength** = `6`

数据验证检查并允许其长度满足给定条件的文本值

___

### <a id="time" name="time"></a> time

• **time** = `5`

数据验证检查并允许时间值满足给定条件

___

### <a id="wholenumber" name="wholenumber"></a> wholeNumber

• **wholeNumber** = `1`

数据验证检查并允许满足给定条件的整数值
