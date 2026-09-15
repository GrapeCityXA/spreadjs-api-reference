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

为时间尺度创建一个层。内部仅使用。

**`classdesc`** 代表时间尺度的一级。

## Properties

### <a id="count" name="count"></a> count

• **count**: `number`

获取或设置一个指示一个刻度代表多少个单位的时间。默认值为1。

**`default`** 1

___

### <a id="formatter" name="formatter"></a> formatter

• **formatter**: `string` \| [`TimescaleLabelFormatter`](../modules/GC.Spread.Sheets.GanttSheet.md#timescalelabelformatter)

获取或设置该层的格式化器，用于格式化刻度标签。
格式化器可以是一个差异格式字符串，用于日期值，例如“ yyyy-mm-dd”，并带有甘特表特殊关键字支持，
也可以是将以格式执行的回调函数。

**`example`**
```
 // 以下关键字可以在格式字符串中使用。它们可以独立使用，也可以与文字或 SpreadJS 数字格式的文本结合使用。
'{!YEAR_FROM_START}' // 替换为距离项目开始日期的年数。
'{!YEAR_FROM_END}' // 替换为距离项目结束日期的年数。
'{!HALF_YEAR("H1", "H2")}' // 替换为对应半年的参数文本，
'{!HALF_YEAR_FROM_START}' // 替换为距离项目开始日期的半年数。
'{!HALF_YEAR_FROM_END}' // 替换为距离项目结束日期的半年数。
'{!QUARTER("Q1", "Q2", "Q3", "Q4")}' // 替换为对应季度的参数文本。
'{!QUARTER_FROM_START}' // 替换为距离项目开始日期的季度数。
'{!QUARTER_FROM_END}' // 替换为距离项目结束日期的季度数。
'{!MONTH_FROM_START}' // 替换为距离项目开始日期的月数。
'{!MONTH_FROM_END}' // 替换为距离项目结束日期的月数。
'{!THIRDS_OF_MONTH("B", "M", "E")}' // 替换为对应月份三等分的参数文本。
'{!WEEK_OF_YEAR}' // 替换为表示一年中的周索引的数字。
'{!DAY_OF_WEEK("SUN", "MON", "TUE", "WED", "THR", "FRI", "STA")}' // 替换为对应星期几的参数文本。
'{!WEEK_FROM_START}' // 替换为距离项目开始日期的周数。
'{!WEEK_FROM_END}' // 替换为距离项目结束日期的周数。
'{!DAY_OF_YEAR}' // 替换为表示一年中的日期索引的数字（1到366）。
'{!DAY_FROM_START}' // 替换为距离项目开始日期的天数。
'{!DAY_FROM_END}' // 替换为距离项目结束日期的天数。
'{!HOUR_FROM_START}' // 替换为距离项目开始日期的小时数。
'{!HOUR_FROM_END}' // 替换为距离项目结束日期的小时数。
'{!MINUTE}' // 替换为分钟值，因为 "mm" 在数字格式中会被视为月份。
'{!MINUTE_FROM_START}' // 替换为距离项目开始日期的分钟数。
'{!MINUTE_FROM_END}' // 替换为距离项目结束日期的分钟数。
```

___

### <a id="labelalign" name="labelalign"></a> labelAlign

• **labelAlign**: ``"Left"`` \| ``"Center"`` \| ``"Right"``

获取或设置一个指示刻度标签对齐的字符串值。默认值为“左”。

**`default`** "Left"

___

### <a id="showticklines" name="showticklines"></a> showTickLines

• **showTickLines**: `boolean`

获取或设置一个布尔值，该值指示是否显示该层的刻度线。默认值是true。

**`default`** true

___

### <a id="unit" name="unit"></a> unit

• **unit**: [`TimescaleUnit`](../enums/GC.Spread.Sheets.GanttSheet.TimescaleUnit.md)

获取或设置此层的单位。
