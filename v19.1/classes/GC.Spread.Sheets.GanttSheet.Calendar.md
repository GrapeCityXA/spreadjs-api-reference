# Class: Calendar

[Sheets](../modules/GC.Spread.Sheets.md).[GanttSheet](../modules/GC.Spread.Sheets.GanttSheet.md).Calendar

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.GanttSheet.Calendar.md#constructor)

### Properties

- [customWorkWeeks](GC.Spread.Sheets.GanttSheet.Calendar.md#customworkweeks)
- [defaultWorkWeek](GC.Spread.Sheets.GanttSheet.Calendar.md#defaultworkweek)
- [name](GC.Spread.Sheets.GanttSheet.Calendar.md#name)
- [hours24](GC.Spread.Sheets.GanttSheet.Calendar.md#hours24)
- [nightShift](GC.Spread.Sheets.GanttSheet.Calendar.md#nightshift)
- [standard](GC.Spread.Sheets.GanttSheet.Calendar.md#standard)

### Methods

- [copyTo](GC.Spread.Sheets.GanttSheet.Calendar.md#copyto)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Calendar**(`name`, `defaultWorkWeek?`, `customWorkWeeks?`)

使用提供的工作周创建日历。

**`classdesc`** 表示用于调度的日历，它定义了每天的工作时间。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 指定此日历名称的字符串值。 |
| `defaultWorkWeek?` | [`WorkWeek`](GC.Spread.Sheets.GanttSheet.WorkWeek.md) | 指定每周各天的默认工作时间。如果未指定，工作时间将与标准日历相同。 |
| `customWorkWeeks?` | [`CustomWorkWeek`](GC.Spread.Sheets.GanttSheet.CustomWorkWeek.md)[] | 为指定日期范围指定每周各天的自定义工作时间。 |

## Properties

### <a id="customworkweeks" name="customworkweeks"></a> customWorkWeeks

• **customWorkWeeks**: [`CustomWorkWeek`](GC.Spread.Sheets.GanttSheet.CustomWorkWeek.md)[]

获取或设置此日历的自定义工作周。
注意不要修改正在使用的日历。相反，您可以复制一个日历并进行更改，然后替换原始日历。

___

### <a id="defaultworkweek" name="defaultworkweek"></a> defaultWorkWeek

• **defaultWorkWeek**: [`WorkWeek`](GC.Spread.Sheets.GanttSheet.WorkWeek.md)

获取或设置此日历的默认工作周。
注意不要修改正在使用的日历。相反，您可以复制一个日历并进行更改，然后替换原始日历。

___

### <a id="name" name="name"></a> name

• **name**: `string`

获取或设置日历名称。

___

### <a id="hours24" name="hours24"></a> hours24

▪ `Static` **hours24**: [`Calendar`](GC.Spread.Sheets.GanttSheet.Calendar.md)

24小时日历，将工作时间定义为每周7天24小时。

**`readonly`**

___

### <a id="nightshift" name="nightshift"></a> nightShift

▪ `Static` **nightShift**: [`Calendar`](GC.Spread.Sheets.GanttSheet.Calendar.md)

夜班日历，将工作时间定义为周一晚上到周六早上23:00至3:00和4:00至8:00。

**`readonly`**

___

### <a id="standard" name="standard"></a> standard

▪ `Static` **standard**: [`Calendar`](GC.Spread.Sheets.GanttSheet.Calendar.md)

标准日历，将工作时间定义为周一至周五8:00至12:00和13:00至17:00。

**`readonly`**

## Methods

### <a id="copyto" name="copyto"></a> copyTo

▸ **copyTo**(`newName`): [`Calendar`](GC.Spread.Sheets.GanttSheet.Calendar.md)

将此日历的工作周复制到新日历。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newName` | `string` | 表示新日历名称的字符串。 |

#### Returns

[`Calendar`](GC.Spread.Sheets.GanttSheet.Calendar.md)

复制结果。
