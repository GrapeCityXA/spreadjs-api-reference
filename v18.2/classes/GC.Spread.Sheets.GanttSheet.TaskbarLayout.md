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

创建任务条布局实例。仅供内部使用。

**`classdesc`** 表示甘特图上任务条的布局。

## Properties

### <a id="barheight" name="barheight"></a> barHeight

• **barHeight**: `number`

获取或设置任务条的高度（以像素为单位）。默认值为12。

**`default`** 12

___

### <a id="bartextdateformat" name="bartextdateformat"></a> barTextDateFormat

• **barTextDateFormat**: `string`

获取或设置甘特图上任务条显示的日期值格式字符串。默认值为"yyyy/mm/dd hh:mm"。

**`default`** "yyyy/mm/dd hh:mm"

___

### <a id="linklinemode" name="linklinemode"></a> linkLineMode

• **linkLineMode**: [`TaskbarLinkMode`](../modules/GC.Spread.Sheets.GanttSheet.md#taskbarlinkmode)

获取或设置链接线模式。默认值为'toTop'。

**`default`** "toTop"

___

### <a id="roundbarstowholedays" name="roundbarstowholedays"></a> roundBarsToWholeDays

• **roundBarsToWholeDays**: `boolean`

获取或设置一个布尔值，指示任务条是否应四舍五入到整天。
如果为true，project.calendarSettings.defaultStartTime之前的时间将显示为一天的开始，
project.calendarSettings.defaultFinishTime之后的时间将显示为一天的结束。
默认值为true。

**`default`** true

___

### <a id="tipdateformat" name="tipdateformat"></a> tipDateFormat

• **tipDateFormat**: `string`

获取或设置甘特图上任务条提示或链接线提示中显示的日期值格式字符串。默认值为"yyyy/mm/dd hh:mm"。

**`default`** "yyyy/mm/dd hh:mm"
