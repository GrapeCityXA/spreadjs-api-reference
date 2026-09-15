# Class: TaskbarLayout

[Sheets](../modules/GC.Spread.Sheets.md).[GanttSheet](../modules/GC.Spread.Sheets.GanttSheet.md).TaskbarLayout

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.GanttSheet.TaskbarLayout.md#constructor)

### Properties

- [barHeight](GC.Spread.Sheets.GanttSheet.TaskbarLayout.md#barheight)
- [barTextDateFormat](GC.Spread.Sheets.GanttSheet.TaskbarLayout.md#bartextdateformat)
- [linkLineMode](GC.Spread.Sheets.GanttSheet.TaskbarLayout.md#linklinemode)
- [roundBarsToWholeDays](GC.Spread.Sheets.GanttSheet.TaskbarLayout.md#roundbarstowholedays)
- [tipDateFormat](GC.Spread.Sheets.GanttSheet.TaskbarLayout.md#tipdateformat)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new TaskbarLayout**()

创建一个任务栏布局实例。仅供内部使用。

**`classdesc`** 代表甘特图任务栏的布局。

## Properties

### <a id="barheight" name="barheight"></a> barHeight

• **barHeight**: `number`

获取或设置任务栏高度的像素值。默认值为12。

**`default`** 12

___

### <a id="bartextdateformat" name="bartextdateformat"></a> barTextDateFormat

• **barTextDateFormat**: `string`

获取或设置格式字符串的日期值，以显示甘特图上任务栏的日期值。默认值为“ yyyy/mm/dd HH：mm”。

**`default`** "yyyy/mm/dd hh:mm"

___

### <a id="linklinemode" name="linklinemode"></a> linkLineMode

• **linkLineMode**: [`TaskbarLinkMode`](../modules/GC.Spread.Sheets.GanttSheet.md#taskbarlinkmode)

获取或设置链接线模式。默认值是“ toTop”。

**`default`** "toTop"

___

### <a id="roundbarstowholedays" name="roundbarstowholedays"></a> roundBarsToWholeDays

• **roundBarsToWholeDays**: `boolean`

获取或设置一个布尔值，指示任务栏应舍入到整个天数。
如果为true，则在项目之前的时间。
在项目之后的一段时间。
默认值是true。
**`default`** true

___

### <a id="tipdateformat" name="tipdateformat"></a> tipDateFormat

• **tipDateFormat**: `string`

获取或设置格式字符串的日期值，该字符串在甘特图上显示在任务栏提示或链接行提示中。默认值为“ yyyy/mm/dd HH：mm”。

**`default`** "yyyy/mm/dd hh:mm"
