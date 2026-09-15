# Class: TimescaleTier

[Sheets](../modules/GC.Spread.Sheets.md).[GanttSheet](../modules/GC.Spread.Sheets.GanttSheet.md).TimescaleTier

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.GanttSheet.TimescaleTier.md#constructor)

### Properties

- [count](GC.Spread.Sheets.GanttSheet.TimescaleTier.md#count)
- [formatter](GC.Spread.Sheets.GanttSheet.TimescaleTier.md#formatter)
- [labelAlign](GC.Spread.Sheets.GanttSheet.TimescaleTier.md#labelalign)
- [showTickLines](GC.Spread.Sheets.GanttSheet.TimescaleTier.md#showticklines)
- [unit](GC.Spread.Sheets.GanttSheet.TimescaleTier.md#unit)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new TimescaleTier**()

创建时间刻度的层级。仅供内部使用。

**`classdesc`** 表示时间刻度的层级。

## Properties

### <a id="count" name="count"></a> count

• **count**: `number`

获取或设置一个数值，表示一个刻度代表多少个时间单位。默认值为1。

**`default`** 1

___

### <a id="formatter" name="formatter"></a> formatter

• **formatter**: `string` \| [`TimescaleLabelFormatter`](../modules/GC.Spread.Sheets.GanttSheet.md#timescalelabelformatter)

获取或设置此层级的格式化器，用于格式化刻度标签。
格式化器可以是类似"yyyy-mm-dd"的Spread数字格式字符串，支持GanttSheet特殊关键字，
也可以是一个在格式化时执行的回调函数。

**`example`**
```javascript
 // 以下关键字可以在格式化字符串中使用。它们可以单独使用，也可以与文字或Spread数字格式化文本组合使用。
 '{!YEAR_FROM_START}' // 替换为从项目开始日期算起的年数。
 '{!YEAR_FROM_END}' // 替换为从项目结束日期算起的年数。
 '{!HALF_YEAR("H1", "H2")}' // 替换为对应半年度的参数文本。
 '{!HALF_YEAR_FROM_START}' // 替换为从项目开始日期算起的半年数。
 '{!HALF_YEAR_FROM_END}' // 替换为从项目结束日期算起的半年数。
 '{!QUARTER("Q1", "Q2", "Q3", "Q4")}' // 替换为对应季度的参数文本。
 '{!QUARTER_FROM_START}' // 替换为从项目开始日期算起的季度数。
 '{!QUARTER_FROM_END}' // 替换为从项目结束日期算起的季度数。
 '{!MONTH_FROM_START}' // 替换为从项目开始日期算起的月数。
 '{!MONTH_FROM_END}' // 替换为从项目结束日期算起的月数。
 '{!THIRDS_OF_MONTH("B", "M", "E")}' // 替换为对应月份三分之一的参数文本。
 '{!WEEK_OF_YEAR}' // 替换为表示一年中第几周的数字。
 '{!DAY_OF_WEEK("SUN", "MON", "TUE", "WED", "THR", "FRI", "STA")}' // 替换为对应星期几的参数文本。
 '{!WEEK_FROM_START}' // 替换为从项目开始日期算起的周数。
 '{!WEEK_FROM_END}' // 替换为从项目结束日期算起的周数。
 '{!DAY_OF_YEAR}' // 替换为表示一年中第几天的数字（1到366）。
 '{!DAY_FROM_START}' // 替换为从项目开始日期算起的天数。
 '{!DAY_FROM_END}' // 替换为从项目结束日期算起的天数。
 '{!HOUR_FROM_START}' // 替换为从项目开始日期算起的小时数。
 '{!HOUR_FROM_END}' // 替换为从项目结束日期算起的小时数。
 '{!MINUTE}' // 替换为分钟值，因为在数字格式化中"mm"会被视为月份。
 '{!MINUTE_FROM_START}' // 替换为从项目开始日期算起的分钟数。
 '{!MINUTE_FROM_END}' // 替换为从项目结束日期算起的分钟数。
```

___

### <a id="labelalign" name="labelalign"></a> labelAlign

• **labelAlign**: ``"Left"`` \| ``"Center"`` \| ``"Right"``

获取或设置一个字符串值，表示刻度标签的对齐方式。默认为"Left"。

**`default`** "Left"

___

### <a id="showticklines" name="showticklines"></a> showTickLines

• **showTickLines**: `boolean`

获取或设置一个布尔值，表示是否显示此层级的刻度线。默认值为true.

**`default`** true

___

### <a id="unit" name="unit"></a> unit

• **unit**: [`TimescaleUnit`](../enums/GC.Spread.Sheets.GanttSheet.TimescaleUnit.md)

获取或设置此层级的单位。
