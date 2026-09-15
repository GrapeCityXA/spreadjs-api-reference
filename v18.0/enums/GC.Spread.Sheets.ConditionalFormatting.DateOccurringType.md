# Enumeration: DateOccurringType

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).DateOccurringType

日期发生的类型

**`代码示例`**
``` javascript
//本示例创建一个规则
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
var rule = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule(GC.Spread.Sheets.ConditionalFormatting.RuleType.dateOccurringRule, [new GC.Spread.Sheets.Range(0,0,10,1)], style, null, null, null, null, null, GC.Spread.Sheets.ConditionalFormatting.DateOccurringType.nextWeek);
activeSheet.conditionalFormats.addRule(rule);
var d = new Date();
activeSheet.setValue(0, 0, d);
activeSheet.setValue(1, 0, new Date(d.setDate(d.getDate()+1)));
activeSheet.setValue(2, 0, new Date(d.setDate(d.getDate()+5)));
activeSheet.setValue(3, 0,new Date(d.setDate(d.getDate()+6)));
activeSheet.setValue(4, 0,new Date(d.setDate(d.getDate()+7)));
activeSheet.setValue(5, 0, new Date(d.setDate(d.getDate()+8)));
```

## Table of contents

### Enumeration members

- [last7Days](GC.Spread.Sheets.ConditionalFormatting.DateOccurringType.md#last7days)
- [lastMonth](GC.Spread.Sheets.ConditionalFormatting.DateOccurringType.md#lastmonth)
- [lastQuarter](GC.Spread.Sheets.ConditionalFormatting.DateOccurringType.md#lastquarter)
- [lastWeek](GC.Spread.Sheets.ConditionalFormatting.DateOccurringType.md#lastweek)
- [lastYear](GC.Spread.Sheets.ConditionalFormatting.DateOccurringType.md#lastyear)
- [nextMonth](GC.Spread.Sheets.ConditionalFormatting.DateOccurringType.md#nextmonth)
- [nextQuarter](GC.Spread.Sheets.ConditionalFormatting.DateOccurringType.md#nextquarter)
- [nextWeek](GC.Spread.Sheets.ConditionalFormatting.DateOccurringType.md#nextweek)
- [nextYear](GC.Spread.Sheets.ConditionalFormatting.DateOccurringType.md#nextyear)
- [thisMonth](GC.Spread.Sheets.ConditionalFormatting.DateOccurringType.md#thismonth)
- [thisQuarter](GC.Spread.Sheets.ConditionalFormatting.DateOccurringType.md#thisquarter)
- [thisWeek](GC.Spread.Sheets.ConditionalFormatting.DateOccurringType.md#thisweek)
- [thisYear](GC.Spread.Sheets.ConditionalFormatting.DateOccurringType.md#thisyear)
- [today](GC.Spread.Sheets.ConditionalFormatting.DateOccurringType.md#today)
- [tomorrow](GC.Spread.Sheets.ConditionalFormatting.DateOccurringType.md#tomorrow)
- [yesterday](GC.Spread.Sheets.ConditionalFormatting.DateOccurringType.md#yesterday)

## Enumeration members

### <a id="last7days" name="last7days"></a> last7Days

• **last7Days** = `3`

最近7天

___

### <a id="lastmonth" name="lastmonth"></a> lastMonth

• **lastMonth** = `5`

上个月

___

### <a id="lastquarter" name="lastquarter"></a> lastQuarter

• **lastQuarter** = `12`

上个季度.

___

### <a id="lastweek" name="lastweek"></a> lastWeek

• **lastWeek** = `8`

上周

___

### <a id="lastyear" name="lastyear"></a> lastYear

• **lastYear** = `15`

去年

___

### <a id="nextmonth" name="nextmonth"></a> nextMonth

• **nextMonth** = `6`

下个月

___

### <a id="nextquarter" name="nextquarter"></a> nextQuarter

• **nextQuarter** = `10`

下个季度

___

### <a id="nextweek" name="nextweek"></a> nextWeek

• **nextWeek** = `9`

下周

___

### <a id="nextyear" name="nextyear"></a> nextYear

• **nextYear** = `13`

明年

___

### <a id="thismonth" name="thismonth"></a> thisMonth

• **thisMonth** = `4`

本月

___

### <a id="thisquarter" name="thisquarter"></a> thisQuarter

• **thisQuarter** = `11`

本季度

___

### <a id="thisweek" name="thisweek"></a> thisWeek

• **thisWeek** = `7`

这周

___

### <a id="thisyear" name="thisyear"></a> thisYear

• **thisYear** = `14`

今年

___

### <a id="today" name="today"></a> today

• **today** = `0`

今天

___

### <a id="tomorrow" name="tomorrow"></a> tomorrow

• **tomorrow** = `2`

明天

___

### <a id="yesterday" name="yesterday"></a> yesterday

• **yesterday** = `1`

昨天
