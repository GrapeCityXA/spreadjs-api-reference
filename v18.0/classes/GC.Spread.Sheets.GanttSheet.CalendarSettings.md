# Class: CalendarSettings

[Sheets](../modules/GC.Spread.Sheets.md).[GanttSheet](../modules/GC.Spread.Sheets.GanttSheet.md).CalendarSettings

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.GanttSheet.CalendarSettings.md#constructor)

### Properties

- [daysPerMonth](GC.Spread.Sheets.GanttSheet.CalendarSettings.md#dayspermonth)
- [defaultDurationDecimalDigits](GC.Spread.Sheets.GanttSheet.CalendarSettings.md#defaultdurationdecimaldigits)
- [defaultDurationUnit](GC.Spread.Sheets.GanttSheet.CalendarSettings.md#defaultdurationunit)
- [defaultFinishTime](GC.Spread.Sheets.GanttSheet.CalendarSettings.md#defaultfinishtime)
- [defaultStartTime](GC.Spread.Sheets.GanttSheet.CalendarSettings.md#defaultstarttime)
- [hoursPerDay](GC.Spread.Sheets.GanttSheet.CalendarSettings.md#hoursperday)
- [hoursPerWeek](GC.Spread.Sheets.GanttSheet.CalendarSettings.md#hoursperweek)
- [unitLabels](GC.Spread.Sheets.GanttSheet.CalendarSettings.md#unitlabels)
- [unitLabelsPlurals](GC.Spread.Sheets.GanttSheet.CalendarSettings.md#unitlabelsplurals)
- [weekStartOn](GC.Spread.Sheets.GanttSheet.CalendarSettings.md#weekstarton)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new CalendarSettings**()

创建一个日历设置对象。内部仅使用

**`classdesc`** 代表一个日历设置对象，以配置日历和持续时间使用的参数

## Properties

### <a id="dayspermonth" name="dayspermonth"></a> daysPerMonth

• **daysPerMonth**: `number`

获取或设置一个指示一个月内有多少工作日的值。它用于持续时间转换和计算。默认值为20；

**`default`** 20

___

### <a id="defaultdurationdecimaldigits" name="defaultdurationdecimaldigits"></a> defaultDurationDecimalDigits

• **defaultDurationDecimalDigits**: `number`

获取或设置十进制数字以格式化持续时间值。该持续时间值将四舍五入到最近的小数位。默认值为3

**`default`** 3

___

### <a id="defaultdurationunit" name="defaultdurationunit"></a> defaultDurationUnit

• **defaultDurationUnit**: [`DurationUnit`](../modules/GC.Spread.Sheets.GanttSheet.md#durationunit)

获取或设置持续时间的默认单元。它用于解析或编辑持续时间。默认值是“天”

**`default`** "Day"

___

### <a id="defaultfinishtime" name="defaultfinishtime"></a> defaultFinishTime

• **defaultFinishTime**: [`Time`](../modules/GC.Spread.Sheets.GanttSheet.md#time)

获取或设置任务完成的默认时间。如果任务完成日期没有指定时间，则将使用此时间。默认值为17:00

___

### <a id="defaultstarttime" name="defaultstarttime"></a> defaultStartTime

• **defaultStartTime**: [`Time`](../modules/GC.Spread.Sheets.GanttSheet.md#time)

获取或设置任务启动的默认时间。如果任务开始日期没有指定时间，则将使用此时间。默认值为8:00

___

### <a id="hoursperday" name="hoursperday"></a> hoursPerDay

• **hoursPerDay**: `number`

获取或设置一个指示工作日有多少小时的值。它用于持续时间转换和计算。默认值为8;

**`default`** 8

___

### <a id="hoursperweek" name="hoursperweek"></a> hoursPerWeek

• **hoursPerWeek**: `number`

获取或设置一个值，该值指示工作一周中有多少小时。它用于持续时间转换和计算。默认值为40；

**`default`** 40

___

### <a id="unitlabels" name="unitlabels"></a> unitLabels

• **unitLabels**: `string`[]

获取或设置标签持续时间解析和格式。该值应按照分钟，小时，白天，周，月和年的顺序有6个字符串

___

### <a id="unitlabelsplurals" name="unitlabelsplurals"></a> unitLabelsPlurals

• **unitLabelsPlurals**: `string`[]

获取或设置持续时间解析和格式化的复数标签。该值应按照分钟，小时，白天，周，月和年的顺序有6个字符串

___

### <a id="weekstarton" name="weekstarton"></a> weekStartOn

• **weekStartOn**: [`DayOfWeek`](../enums/GC.Spread.Sheets.GanttSheet.DayOfWeek.md)

获取或设置一个指示一周第一天的值。它将影响如何显示和计算几周。默认值是星期日

**`default`** GC.Spread.Sheets.GanttSheet.DayOfWeek.Sunday
