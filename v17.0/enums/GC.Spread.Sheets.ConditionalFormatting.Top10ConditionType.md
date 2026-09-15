# Enumeration: Top10ConditionType

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).Top10ConditionType

前10条件类型

**`代码示例`**
```
//本示例使用Top10ConditionType枚举
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
var ranges=[new GC.Spread.Sheets.Range(0,0,10,1)];
activeSheet.conditionalFormats.addTop10Rule(GC.Spread.Sheets.ConditionalFormatting.Top10ConditionType.top, 2, style, ranges);
activeSheet.setValue(0, 0, 1);
activeSheet.setValue(1, 0, 50);
activeSheet.setValue(2, 0, 11);
activeSheet.setValue(3, 0, 5);
```

## Table of contents

### Enumeration members

- [bottom](GC.Spread.Sheets.ConditionalFormatting.Top10ConditionType.md#bottom)
- [top](GC.Spread.Sheets.ConditionalFormatting.Top10ConditionType.md#top)

## Enumeration members

### <a id="bottom" name="bottom"></a> bottom

• **bottom** = `1`

最低条件

___

### <a id="top" name="top"></a> top

• **top** = `0`

最高条件
