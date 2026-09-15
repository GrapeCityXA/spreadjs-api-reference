# Enumeration: TextCompareType

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).TextCompareType

文本比较类型

**`代码示例`**
``` javascript
//本示例使用TextCompareType枚举
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.textCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.TextCompareType.contains, expected: "test"});
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, "testing");
//Type text in 0,0 that does not contain "test" to see invalid symbol
```

## Table of contents

### Enumeration members

- [beginsWith](GC.Spread.Sheets.ConditionalFormatting.TextCompareType.md#beginswith)
- [contains](GC.Spread.Sheets.ConditionalFormatting.TextCompareType.md#contains)
- [doesNotBeginWith](GC.Spread.Sheets.ConditionalFormatting.TextCompareType.md#doesnotbeginwith)
- [doesNotContain](GC.Spread.Sheets.ConditionalFormatting.TextCompareType.md#doesnotcontain)
- [doesNotEndWith](GC.Spread.Sheets.ConditionalFormatting.TextCompareType.md#doesnotendwith)
- [endsWith](GC.Spread.Sheets.ConditionalFormatting.TextCompareType.md#endswith)
- [equalsTo](GC.Spread.Sheets.ConditionalFormatting.TextCompareType.md#equalsto)
- [notEqualsTo](GC.Spread.Sheets.ConditionalFormatting.TextCompareType.md#notequalsto)

## Enumeration members

### <a id="beginswith" name="beginswith"></a> beginsWith

• **beginsWith** = `2`

字符串是否以指定的字符串开始

___

### <a id="contains" name="contains"></a> contains

• **contains** = `6`

字符串是否包含指定的字符串

___

### <a id="doesnotbeginwith" name="doesnotbeginwith"></a> doesNotBeginWith

• **doesNotBeginWith** = `3`

字符串是否以指定的字符串开始

___

### <a id="doesnotcontain" name="doesnotcontain"></a> doesNotContain

• **doesNotContain** = `7`

字符串是否不包含指定的字符串

___

### <a id="doesnotendwith" name="doesnotendwith"></a> doesNotEndWith

• **doesNotEndWith** = `5`

字符串是否不以指定的字符串结束

___

### <a id="endswith" name="endswith"></a> endsWith

• **endsWith** = `4`

字符串是否以指定的字符串结束

___

### <a id="equalsto" name="equalsto"></a> equalsTo

• **equalsTo** = `0`

字符串是否等于指定的字符串

___

### <a id="notequalsto" name="notequalsto"></a> notEqualsTo

• **notEqualsTo** = `1`

字符串是否不等于指定的字符串
