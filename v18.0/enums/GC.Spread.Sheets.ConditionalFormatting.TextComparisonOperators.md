# Enumeration: TextComparisonOperators

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).TextComparisonOperators

文本比较运算符

**`代码示例`**
``` javascript
//本示例创建一个规则
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
var ranges=[new GC.Spread.Sheets.Range(0,0,10,1)];
activeSheet.conditionalFormats.addSpecificTextRule(GC.Spread.Sheets.ConditionalFormatting.TextComparisonOperators.contains, "test", style, ranges);
activeSheet.setValue(0, 0, "testing");
activeSheet.setValue(1, 0, "test");
activeSheet.setValue(2, 0, "a");
activeSheet.setValue(3, 0, "t");
```

## Table of contents

### Enumeration members

- [beginsWith](GC.Spread.Sheets.ConditionalFormatting.TextComparisonOperators.md#beginswith)
- [contains](GC.Spread.Sheets.ConditionalFormatting.TextComparisonOperators.md#contains)
- [doesNotContain](GC.Spread.Sheets.ConditionalFormatting.TextComparisonOperators.md#doesnotcontain)
- [endsWith](GC.Spread.Sheets.ConditionalFormatting.TextComparisonOperators.md#endswith)

## Enumeration members

### <a id="beginswith" name="beginswith"></a> beginsWith

• **beginsWith** = `2`

确定单元格值是否以参数值开头

___

### <a id="contains" name="contains"></a> contains

• **contains** = `0`

确定单元格值是否包含参数值

___

### <a id="doesnotcontain" name="doesnotcontain"></a> doesNotContain

• **doesNotContain** = `1`

确定单元格值是否不包含参数值

___

### <a id="endswith" name="endswith"></a> endsWith

• **endsWith** = `3`

确定单元格值是否以参数值结尾
