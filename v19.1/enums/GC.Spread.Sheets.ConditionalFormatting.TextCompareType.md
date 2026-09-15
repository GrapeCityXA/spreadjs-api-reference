# Enumeration: TextCompareType

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).TextCompareType

指定文本比较类型。

**`example`**
```javascript
//此示例使用TextCompareType枚举。
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.textCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.TextCompareType.contains, expected: "test"});
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, "testing");
//在0,0处输入不包含"test"的文本以查看无效符号
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

指示字符串是否以指定字符串开头。

___

### <a id="contains" name="contains"></a> contains

• **contains** = `6`

指示字符串是否包含指定字符串。

___

### <a id="doesnotbeginwith" name="doesnotbeginwith"></a> doesNotBeginWith

• **doesNotBeginWith** = `3`

指示字符串是否不以指定字符串开头。

___

### <a id="doesnotcontain" name="doesnotcontain"></a> doesNotContain

• **doesNotContain** = `7`

指示字符串是否不包含指定字符串。

___

### <a id="doesnotendwith" name="doesnotendwith"></a> doesNotEndWith

• **doesNotEndWith** = `5`

指示字符串是否不以指定字符串结尾。

___

### <a id="endswith" name="endswith"></a> endsWith

• **endsWith** = `4`

指示字符串是否以指定字符串结尾。

___

### <a id="equalsto" name="equalsto"></a> equalsTo

• **equalsTo** = `0`

指示字符串是否等于指定字符串。

___

### <a id="notequalsto" name="notequalsto"></a> notEqualsTo

• **notEqualsTo** = `1`

指示字符串是否不等于指定字符串。
