# Namespace: GanttSheet

[Spread](GC.Spread.md).[Sheets](GC.Spread.Sheets.md).GanttSheet

## Table of contents

### Enumerations

- [DayOfWeek](../enums/GC.Spread.Sheets.GanttSheet.DayOfWeek.md)
- [GanttGridlineType](../enums/GC.Spread.Sheets.GanttSheet.GanttGridlineType.md)
- [TimescaleTierMode](../enums/GC.Spread.Sheets.GanttSheet.TimescaleTierMode.md)
- [TimescaleUnit](../enums/GC.Spread.Sheets.GanttSheet.TimescaleUnit.md)

### Classes

- [Calendar](../classes/GC.Spread.Sheets.GanttSheet.Calendar.md)
- [CalendarSettings](../classes/GC.Spread.Sheets.GanttSheet.CalendarSettings.md)
- [Collection](../classes/GC.Spread.Sheets.GanttSheet.Collection.md)
- [CustomWorkWeek](../classes/GC.Spread.Sheets.GanttSheet.CustomWorkWeek.md)
- [GanttGridlines](../classes/GC.Spread.Sheets.GanttSheet.GanttGridlines.md)
- [GanttMapping](../classes/GC.Spread.Sheets.GanttSheet.GanttMapping.md)
- [GanttSheet](../classes/GC.Spread.Sheets.GanttSheet.GanttSheet.md)
- [NonWorkingTimeStyle](../classes/GC.Spread.Sheets.GanttSheet.NonWorkingTimeStyle.md)
- [Project](../classes/GC.Spread.Sheets.GanttSheet.Project.md)
- [Task](../classes/GC.Spread.Sheets.GanttSheet.Task.md)
- [TaskDependency](../classes/GC.Spread.Sheets.GanttSheet.TaskDependency.md)
- [TaskbarLayout](../classes/GC.Spread.Sheets.GanttSheet.TaskbarLayout.md)
- [TaskbarStyleRule](../classes/GC.Spread.Sheets.GanttSheet.TaskbarStyleRule.md)
- [Timescale](../classes/GC.Spread.Sheets.GanttSheet.Timescale.md)
- [TimescaleTier](../classes/GC.Spread.Sheets.GanttSheet.TimescaleTier.md)
- [WorkWeek](../classes/GC.Spread.Sheets.GanttSheet.WorkWeek.md)

### Type aliases

- [Duration](GC.Spread.Sheets.GanttSheet.md#duration)
- [DurationUnit](GC.Spread.Sheets.GanttSheet.md#durationunit)
- [GanttGridline](GC.Spread.Sheets.GanttSheet.md#ganttgridline)
- [GanttGridlineInterval](GC.Spread.Sheets.GanttSheet.md#ganttgridlineinterval)
- [GridStyle](GC.Spread.Sheets.GanttSheet.md#gridstyle)
- [IGanttSheetOptions](GC.Spread.Sheets.GanttSheet.md#iganttsheetoptions)
- [ITaskData](GC.Spread.Sheets.GanttSheet.md#itaskdata)
- [ITaskDependency](GC.Spread.Sheets.GanttSheet.md#itaskdependency)
- [NonWorkingTimeDrawMode](GC.Spread.Sheets.GanttSheet.md#nonworkingtimedrawmode)
- [TaskDependencyType](GC.Spread.Sheets.GanttSheet.md#taskdependencytype)
- [TaskScheduleMode](GC.Spread.Sheets.GanttSheet.md#taskschedulemode)
- [TaskStyle](GC.Spread.Sheets.GanttSheet.md#taskstyle)
- [TaskbarEndShape](GC.Spread.Sheets.GanttSheet.md#taskbarendshape)
- [TaskbarEndType](GC.Spread.Sheets.GanttSheet.md#taskbarendtype)
- [TaskbarFillPattern](GC.Spread.Sheets.GanttSheet.md#taskbarfillpattern)
- [TaskbarLinkMode](GC.Spread.Sheets.GanttSheet.md#taskbarlinkmode)
- [TaskbarMiddleShape](GC.Spread.Sheets.GanttSheet.md#taskbarmiddleshape)
- [TaskbarStyle](GC.Spread.Sheets.GanttSheet.md#taskbarstyle)
- [TaskbarStyleRuleName](GC.Spread.Sheets.GanttSheet.md#taskbarstylerulename)
- [TextStyle](GC.Spread.Sheets.GanttSheet.md#textstyle)
- [Time](GC.Spread.Sheets.GanttSheet.md#time)
- [TimescaleLabelFormatter](GC.Spread.Sheets.GanttSheet.md#timescalelabelformatter)
- [WorkDay](GC.Spread.Sheets.GanttSheet.md#workday)
- [WorkTime](GC.Spread.Sheets.GanttSheet.md#worktime)

## Type aliases

### <a id="duration" name="duration"></a> Duration

Ƭ **Duration**: `Object`

表示一个时间段的持续时间。要创建一个有效的持续时间，请调用 project.parseDuration 方法。

**`property`** {number} [value] 表示持续时间的单位值。

**`property`** {GC.Spread.Sheets.GanttSheet.DurationUnit} [unit] 表示值的单位。如果未指定，则将使用默认单位，即 [GC.Spread.Sheets.GanttSheet.CalendarSettings](../classes/GC.Spread.Sheets.GanttSheet.CalendarSettings.md) 中设置的单位。

**`property`** {number} [time] 表示以毫秒为单位的实际持续时间。

#### Type declaration

| Name | Type |
| :------ | :------ |
| `time?` | `number` |
| `unit?` | [`DurationUnit`](GC.Spread.Sheets.GanttSheet.md#durationunit) |
| `value?` | `number` |

___

### <a id="durationunit" name="durationunit"></a> DurationUnit

Ƭ **DurationUnit**: ``"Month"`` \| ``"Week"`` \| ``"Day"`` \| ``"Hour"`` \| ``"Minute"``

**`description`** 表示持续时间的单位。

___

### <a id="ganttgridline" name="ganttgridline"></a> GanttGridline

Ƭ **GanttGridline**: `Object`

表示如何在甘特图上绘制网格线。

**`property`** {GC.Spread.Sheets.GanttSheet.GanttGridlineType} lineType 线条的类型。

**`property`** {GC.Data.ColorString} lineColor 线条的颜色。

#### Type declaration

| Name | Type |
| :------ | :------ |
| `lineColor` | [`ColorString`](GC.Data.md#colorstring) |
| `lineType` | [`GanttGridlineType`](../enums/GC.Spread.Sheets.GanttSheet.GanttGridlineType.md) |

___

### <a id="ganttgridlineinterval" name="ganttgridlineinterval"></a> GanttGridlineInterval

Ƭ **GanttGridlineInterval**: `Object`

表示如何在甘特图上绘制具有间隔的网格线。

**`property`** {GC.Spread.Sheets.GanttSheet.GanttGridlineType} lineType 普通网格线的类型。

**`property`** {GC.Data.ColorString} lineColor 普通网格线的颜色。

**`property`** {number} [interval] 间隔计数。位于间隔值的倍数处的线条将使用 intervalType 和 intervalColor。

**`property`** {GC.Spread.Sheets.GanttSheet.GanttGridlineType} [intervalLineType] 间隔线的类型。

**`property`** {GC.Data.ColorString} [intervalLineColor] 间隔线的颜色。

#### Type declaration

| Name | Type |
| :------ | :------ |
| `interval?` | `number` |
| `intervalLineColor?` | [`ColorString`](GC.Data.md#colorstring) |
| `intervalLineType?` | [`GanttGridlineType`](../enums/GC.Spread.Sheets.GanttSheet.GanttGridlineType.md) |
| `lineColor` | [`ColorString`](GC.Data.md#colorstring) |
| `lineType` | [`GanttGridlineType`](../enums/GC.Spread.Sheets.GanttSheet.GanttGridlineType.md) |

___

### <a id="gridstyle" name="gridstyle"></a> GridStyle

Ƭ **GridStyle**: `Object`

表示任务网格的样式。

**`property`** {string} [font] 文本的字体。

**`property`** {GC.Data.ColorString} [color] 文本的颜色。

**`property`** {GC.Data.ColorString} [backColor] 文本的背景颜色。

**`property`** {GC.Spread.Sheets.TextDecorationType} [textDecoration] 文本的装饰风格。

#### Type declaration

| Name | Type |
| :------ | :------ |
| `backColor?` | `string` |
| `color?` | `string` |
| `font?` | `string` |
| `textDecoration?` | [`TextDecorationType`](../enums/GC.Spread.Sheets.TextDecorationType.md) |

___

### <a id="iganttsheetoptions" name="iganttsheetoptions"></a> IGanttSheetOptions

Ƭ **IGanttSheetOptions**: `Object`

表示甘特图表选项。

**`property`** {boolean} [enableGanttColumn] 是否显示甘特列。默认为 true。

**`property`** {boolean} [allowAddNew] 是否允许添加新的空行。

**`property`** {boolean} [sheetTabColor] 用于表示工作表标签颜色的颜色字符串，例如 "red"、"#FFFF00"、"rgb(255,0,0)"、"Accent 5" 等。

#### Type declaration

| Name | Type | Description |
| :------ | :------ | :------ |
| `allowAddNew?` | `boolean` | 是否允许添加新的空行 |
| `enableGanttColumn?` | `boolean` | 是否显示甘特列。默认为 true |
| `sheetTabColor?` | `string` | 用于表示工作表标签颜色的颜色字符串，例如 "red"、"#FFFF00"、"rgb(255,0,0)"、"Accent 5" 等 |

___

### <a id="itaskdata" name="itaskdata"></a> ITaskData

Ƭ **ITaskData**: `Object`

表示用于创建任务的数据。它在项目的add、insert和renew任务方法中使用。

 **`property`** {string} [name] 任务的名称。

 **`property`** {Date} [start] 任务的开始日期。

 **`property`** {Date} [finish] 任务的结束日期。

 **`property`** {GC.Spread.Sheets.GanttSheet.Duration} [duration] 任务的持续时间。

 **`property`** {GC.Spread.Sheets.GanttSheet.TaskScheduleMode} [mode] 任务的调度模式。

 **`property`** {Object.<string, GC.Spread.Sheets.GanttSheet.TaskbarStyle>} [barStyles] 任务的条形图样式。

#### Type declaration

| Name | Type |
| :------ | :------ |
| `barStyles?` | { `[key: string]`: [`TaskbarStyle`](GC.Spread.Sheets.GanttSheet.md#taskbarstyle);  } |
| `duration?` | [`Duration`](GC.Spread.Sheets.GanttSheet.md#duration) |
| `finish?` | `Date` |
| `mode?` | [`TaskScheduleMode`](GC.Spread.Sheets.GanttSheet.md#taskschedulemode) |
| `name?` | `string` |
| `start?` | `Date` |

___

### <a id="itaskdependency" name="itaskdependency"></a> ITaskDependency

Ƭ **ITaskDependency**: `Object`

表示添加任务依赖关系的一对参数。

 **`property`** {number} fromTaskNumber 表示依赖关系所属的任务编号。

 **`property`** {number} toTaskNumber 表示依赖关系指向的任务编号。

 **`property`** {GC.Spread.Sheets.GanttSheet.TaskDependencyType} [type] 可选。表示依赖关系的类型。默认为 'FS' (Finish to Start)。

#### Type declaration

| Name | Type |
| :------ | :------ |
| `fromTaskNumber` | `number` |
| `toTaskNumber` | `number` |
| `type?` | [`TaskDependencyType`](GC.Spread.Sheets.GanttSheet.md#taskdependencytype) |

___

### <a id="nonworkingtimedrawmode" name="nonworkingtimedrawmode"></a> NonWorkingTimeDrawMode

Ƭ **NonWorkingTimeDrawMode**: ``"Behind"`` \| ``"None"``

**`description`** 表示如何在甘特图中绘制非工作时间区域。

___

### <a id="taskdependencytype" name="taskdependencytype"></a> TaskDependencyType

Ƭ **TaskDependencyType**: ``"FS"`` \| ``"SS"`` \| ``"FF"`` \| ``"SF"``

**`description`** 表示任务依赖关系的类型。

___

### <a id="taskschedulemode" name="taskschedulemode"></a> TaskScheduleMode

Ƭ **TaskScheduleMode**: ``"Auto"`` \| ``"Manual"``

**`description`** 表示任务的调度模式。

___

### <a id="taskstyle" name="taskstyle"></a> TaskStyle

Ƭ **TaskStyle**: `Object`

任务样式表示任务在甘特图中的外观样式。

 **`property`** {string} [name] 任务样式的名称。

 **`property`** {GC.Spread.Sheets.GanttSheet.TaskbarStyle} [taskbarStyle] 任务条形图部分的样式。

 **`property`** {GC.Spread.Sheets.GanttSheet.GridStyle} [gridStyle] 任务网格部分的样式。

#### Type declaration

| Name | Type |
| :------ | :------ |
| `gridStyle?` | [`GridStyle`](GC.Spread.Sheets.GanttSheet.md#gridstyle) |
| `name?` | `string` |
| `taskbarStyle?` | [`TaskbarStyle`](GC.Spread.Sheets.GanttSheet.md#taskbarstyle) |

___

### <a id="taskbarendshape" name="taskbarendshape"></a> TaskbarEndShape

Ƭ **TaskbarEndShape**: ``"arrowDown"`` \| ``"arrowUp"`` \| ``"caretDownTop"`` \| ``"caretUpBottom"`` \| ``"circle"`` \| ``"circleArrowDown"`` \| ``"circleArrowUp"`` \| ``"circleDiamond"`` \| ``"circleTriangleDown"`` \| ``"circleTriangleUp"`` \| ``"diamond"`` \| ``"houseDown"`` \| ``"houseUp"`` \| ``"leftBracket"`` \| ``"leftFade"`` \| ``"lineShape"`` \| ``"rightBracket"`` \| ``"rightFade"`` \| ``"square"`` \| ``"star"`` \| ``"triangleDown"`` \| ``"triangleLeft"`` \| ``"triangleRight"`` \| ``"triangleUp"``

**`description`** 表示任务条形图开始部分和结束部分的形状。

___

### <a id="taskbarendtype" name="taskbarendtype"></a> TaskbarEndType

Ƭ **TaskbarEndType**: ``"solid"`` \| ``"dashed"`` \| ``"framed"``

**`description`** 任务条形图结束部分形状的绘制类型。

___

### <a id="taskbarfillpattern" name="taskbarfillpattern"></a> TaskbarFillPattern

Ƭ **TaskbarFillPattern**: ``"hollow"`` \| ``"solidFill"`` \| ``"lightFill"`` \| ``"mediumFill"`` \| ``"darkFill"`` \| ``"diagonalRight"`` \| ``"diagonalLeft"`` \| ``"diagonalCross"`` \| ``"lineVertical"`` \| ``"lineHorizontal"`` \| ``"lineCross"`` \| ``"dashedBorder"``

**`description`** 表示甘特图中任务条形图中间部分或非工作时间区域的填充模式。

___

### <a id="taskbarlinkmode" name="taskbarlinkmode"></a> TaskbarLinkMode

Ƭ **TaskbarLinkMode**: ``"noLinks"`` \| ``"toEnd"`` \| ``"toTop"``

**`description`** 表示如何在任务栏之间绘制链路线。

___

### <a id="taskbarmiddleshape" name="taskbarmiddleshape"></a> TaskbarMiddleShape

Ƭ **TaskbarMiddleShape**: ``"rectangleBar"`` \| ``"lineTop"`` \| ``"lineMiddle"`` \| ``"lineBottom"`` \| ``"rectangleTop"`` \| ``"rectangleMiddle"`` \| ``"rectangleBottom"``

**`description`** 代表任务栏中间部分的形状。

___

### <a id="taskbarstyle" name="taskbarstyle"></a> TaskbarStyle

Ƭ **TaskbarStyle**: `Object`

表示任务条的样式。

 **`property`** {GC.Spread.Sheets.GanttSheet.TaskbarEndShape} [startShape] 指示开始部分的形状。

 **`property`** {GC.Spread.Sheets.GanttSheet.TaskbarEndType} [startType] 指示开始部分的类型。

 **`property`** {GC.Data.ColorString} [startColor] 指示开始部分的颜色。

 **`property`** {GC.Spread.Sheets.GanttSheet.TaskbarEndShape} [endShape] 指示结束部分的形状。

 **`property`** {GC.Spread.Sheets.GanttSheet.TaskbarEndType} [endType] 指示结束部分的类型。

 **`property`** {GC.Data.ColorString} [endColor] 指示结束部分的颜色。

 **`property`** {GC.Spread.Sheets.GanttSheet.TaskbarMiddleShape} [middleShape] 指示中间部分的形状。

 **`property`** {GC.Spread.Sheets.GanttSheet.TaskbarFillPattern} [middlePattern] 指示中间部分的填充模式。

 **`property`** {GC.Data.ColorString} [middleColor] 指示中间部分的颜色。

 **`property`** {string} [leftText] 指示任务字段或公式的名称，在条形图的左侧显示文本。

 **`property`** {GC.Spread.Sheets.GanttSheet.TextStyle} [leftTextStyle] 指示任务条左侧任务字段的样式。

 **`property`** {string} [rightText] 指示任务字段或公式的名称，在条形图的右侧显示文本。

 **`property`** {GC.Spread.Sheets.GanttSheet.TextStyle} [rightTextStyle] 指示任务条右侧任务字段的样式。

 **`property`** {string} [topText] 指示任务字段或公式的名称，在条形图的上方显示文本。

 **`property`** {GC.Spread.Sheets.GanttSheet.TextStyle} [topTextStyle] 指示任务条上方任务字段的样式。

 **`property`** {string} [bottomText] 指示任务字段或公式的名称，在条形图的下方显示文本。

 **`property`** {GC.Spread.Sheets.GanttSheet.TextStyle} [bottomTextStyle] 指示任务条下方任务字段的样式。

 **`property`** {string} [insideText] 指示任务字段或公式的名称，在条形图内部显示文本。

 **`property`** {GC.Spread.Sheets.GanttSheet.TextStyle} [insideTextStyle] 指示任务条内部任务字段的样式。

通过设置这些属性，可以定义任务条的样式，包括开始部分的形状、类型和颜色，结束部分的形状、类型和颜色，中间部分的形状、填充模式和颜色，以及任务条上方、下方、左侧、右侧和内部的文本及其样式。这些样式设置能够使任务条更加个性化和可视化，提供更好的展示效果。

#### Type declaration

| Name | Type |
| :------ | :------ |
| `bottomText?` | `string` |
| `bottomTextStyle?` | [`TextStyle`](GC.Spread.Sheets.GanttSheet.md#textstyle) |
| `endColor?` | [`ColorString`](GC.Data.md#colorstring) |
| `endShape?` | [`TaskbarEndShape`](GC.Spread.Sheets.GanttSheet.md#taskbarendshape) |
| `endType?` | [`TaskbarEndType`](GC.Spread.Sheets.GanttSheet.md#taskbarendtype) |
| `insideText?` | `string` |
| `insideTextStyle?` | [`TextStyle`](GC.Spread.Sheets.GanttSheet.md#textstyle) |
| `leftText?` | `string` |
| `leftTextStyle?` | [`TextStyle`](GC.Spread.Sheets.GanttSheet.md#textstyle) |
| `middleColor?` | [`ColorString`](GC.Data.md#colorstring) |
| `middlePattern?` | [`TaskbarFillPattern`](GC.Spread.Sheets.GanttSheet.md#taskbarfillpattern) |
| `middleShape?` | [`TaskbarMiddleShape`](GC.Spread.Sheets.GanttSheet.md#taskbarmiddleshape) |
| `rightText?` | `string` |
| `rightTextStyle?` | [`TextStyle`](GC.Spread.Sheets.GanttSheet.md#textstyle) |
| `startColor?` | [`ColorString`](GC.Data.md#colorstring) |
| `startShape?` | [`TaskbarEndShape`](GC.Spread.Sheets.GanttSheet.md#taskbarendshape) |
| `startType?` | [`TaskbarEndType`](GC.Spread.Sheets.GanttSheet.md#taskbarendtype) |
| `topText?` | `string` |
| `topTextStyle?` | [`TextStyle`](GC.Spread.Sheets.GanttSheet.md#textstyle) |

___

### <a id="taskbarstylerulename" name="taskbarstylerulename"></a> TaskbarStyleRuleName

Ƭ **TaskbarStyleRuleName**: ``"projectSummary"`` \| ``"summary"`` \| ``"manualSummary"`` \| ``"task"`` \| ``"manualTask"`` \| ``"milestone"`` \| ``"manualMilestone"`` \| ``"progress"`` \| ``"manualProgress"`` \| ``"startOnly"`` \| ``"finishOnly"`` \| ``"durationOnly"`` \| ``"startOnlyMilestone"`` \| ``"finishOnlyMilestone"`` \| ``"durationOnlyMilestone"``

**`description`** 表示内置任务条样式规则的名称。用于 project.taskStyleRules.getRule 方法。

___

### <a id="textstyle" name="textstyle"></a> TextStyle

Ƭ **TextStyle**: `Object`

表示甘特图上的时间刻度和任务条的文本样式。

 **`property`** {string} [font] 指示文本的字体。

 **`property`** {GC.Data.ColorString} [color] 指示文本的颜色。

 **`property`** {GC.Spread.Sheets.TextDecorationType} [textDecoration] 指示文本的装饰效果。

通过设置这些属性，可以定义甘特图上时间刻度和任务条的文本样式。可以指定文本的字体、颜色和装饰效果，以满足个性化的显示需求。

#### Type declaration

| Name | Type |
| :------ | :------ |
| `color?` | [`ColorString`](GC.Data.md#colorstring) |
| `font?` | `string` |
| `textDecoration?` | [`TextDecorationType`](../enums/GC.Spread.Sheets.TextDecorationType.md) |

___

### <a id="time" name="time"></a> Time

Ƭ **Time**: `Object`

表示一个包含小时和分钟的时间值。

 **`property`** {number} hour 指示该时间的小时数。可以是0到24之间的值。

 **`property`** {number} minute 指示该时间的分钟数。可以是0到59之间的值。

这个数据结构用于表示具体的时间值，包括小时和分钟。通过hour属性可以设置或获取时间的小时数，范围为0到24。通过minute属性可以设置或获取时间的分钟数，范围为0到59。使用这个数据结构可以方便地处理时间相关的逻辑和计算。

#### Type declaration

| Name | Type |
| :------ | :------ |
| `hour` | `number` |
| `minute` | `number` |

___

### <a id="timescalelabelformatter" name="timescalelabelformatter"></a> TimescaleLabelFormatter

Ƭ **TimescaleLabelFormatter**: (`date`: `Date`, `project`: [`Project`](../classes/GC.Spread.Sheets.GanttSheet.Project.md)) => `string`

#### Type declaration

▸ (`date`, `project`): `string`

这个回调函数用于格式化时间刻度标签。

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `date` | `Date` | 指定需要格式化的日期。 |
| `project` | [`Project`](../classes/GC.Spread.Sheets.GanttSheet.Project.md) | 此时间刻度所属的项目。可以使用开始日期、日历设置或其他数据进行格式化。 |

这个回调函数通常用于自定义时间刻度标签的格式。它接收两个参数：`date` 和 `project`。`date` 参数表示需要格式化的日期，以 `Date` 对象的形式传入。`project` 参数是一个 `Project` 对象，该对象包含了与时间刻度相关的信息，比如项目的开始日期、日历设置等。在回调函数中可以根据这些参数来动态生成或修改时间刻度标签的显示内容和样式。

##### Returns

`string`

___

### <a id="workday" name="workday"></a> WorkDay

Ƭ **WorkDay**: [`WorkTime`](GC.Spread.Sheets.GanttSheet.md#worktime)[]

Represents the work periods in one day.

___

### <a id="worktime" name="worktime"></a> WorkTime

Ƭ **WorkTime**: `Object`

表示一天中的工作时间段，由开始时间和结束时间定义。

 **`property`** {GC.Spread.Sheets.GanttSheet.Time} start 指示开始时间。可以是0:00到23:59之间的值。

 **`property`** {GC.Spread.Sheets.GanttSheet.Time} end 指示结束时间。可以是0:01到24:00之间的值。

这个数据结构用于表示一天中的工作时间段，包括开始时间和结束时间。通过start属性可以设置或获取工作时间段的开始时间，范围为0:00到23:59。通过end属性可以设置或获取工作时间段的结束时间，范围为0:01到24:00。使用这个数据结构可以方便地处理工作时间段相关的逻辑和计算。

#### Type declaration

| Name | Type |
| :------ | :------ |
| `end` | [`Time`](GC.Spread.Sheets.GanttSheet.md#time) |
| `start` | [`Time`](GC.Spread.Sheets.GanttSheet.md#time) |
