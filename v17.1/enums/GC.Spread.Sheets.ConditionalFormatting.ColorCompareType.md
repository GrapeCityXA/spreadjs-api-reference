# Enumeration: ColorCompareType

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).ColorCompareType

颜色比较类型

**`代码示例`**
```
//本示例筛选使用颜色
activeSheet.suspendPaint();
var rowFilter = new GC.Spread.Sheets.Filter.HideRowFilter(new GC.Spread.Sheets.Range(-1, 0, -1, 1));
activeSheet.rowFilter(rowFilter);
activeSheet.getCell(0, 0).value("A1").backColor("blue");
activeSheet.getCell(1, 0).value("A2").backColor("yellow");
activeSheet.getCell(2, 0).value("A3").backColor("red");
activeSheet.getCell(3, 0).value("A4").backColor("green");
activeSheet.getCell(4, 0).value("A5").backColor("yellow");
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.colorCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.ColorCompareType.backgroundColor, expected: "yellow"});
var filter = activeSheet.rowFilter();
filter.addFilterItem(0, nCondition);
filter.filter(0);
activeSheet.resumePaint();
```

## Table of contents

### Enumeration members

- [backgroundColor](GC.Spread.Sheets.ConditionalFormatting.ColorCompareType.md#backgroundcolor)
- [foregroundColor](GC.Spread.Sheets.ConditionalFormatting.ColorCompareType.md#foregroundcolor)

## Enumeration members

### <a id="backgroundcolor" name="backgroundcolor"></a> backgroundColor

• **backgroundColor** = `0`

单元格背景色是否等于指定的颜色

___

### <a id="foregroundcolor" name="foregroundcolor"></a> foregroundColor

• **foregroundColor** = `1`

单元格前景色是否等于指定的颜色
