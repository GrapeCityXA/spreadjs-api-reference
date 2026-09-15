# Class: CustomWorkWeek

[Sheets](../modules/GC.Spread.Sheets.md).[GanttSheet](../modules/GC.Spread.Sheets.GanttSheet.md).CustomWorkWeek

## Hierarchy

- [`WorkWeek`](GC.Spread.Sheets.GanttSheet.WorkWeek.md)

  ↳ **`CustomWorkWeek`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.GanttSheet.CustomWorkWeek.md#constructor)

### Properties

- [finish](GC.Spread.Sheets.GanttSheet.CustomWorkWeek.md#finish)
- [start](GC.Spread.Sheets.GanttSheet.CustomWorkWeek.md#start)

### Methods

- [getWorkDay](GC.Spread.Sheets.GanttSheet.CustomWorkWeek.md#getworkday)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new CustomWorkWeek**(`workDays`, `start`, `finish`)

在自定义日期范围内每天的指定工作时间创建新的一周

**`classdesc`** 代表日历中的一个星期，它定义了每天的工作时间

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workDays` | [`WorkDay`](../modules/GC.Spread.Sheets.GanttSheet.md#workday)[] | 一个工作日阵列，从周日到星期六，有7个项目，指定一周内每天的工作时间 |
| `start` | `Date` | 日期指定在日历中应用本周定义的日期范围的开始 |
| `finish` | `Date` | 日期指定在日历中应用本周定义的日期范围的完成 |

#### Overrides

[WorkWeek](GC.Spread.Sheets.GanttSheet.WorkWeek.md).[constructor](GC.Spread.Sheets.GanttSheet.WorkWeek.md#constructor)

## Properties

### <a id="finish" name="finish"></a> finish

• **finish**: `Date`

获取或设置本自定义工作周的完成日期
___

### <a id="start" name="start"></a> start

• **start**: `Date`

获取或设置本自定义工作周的开始日期

## Methods

### <a id="getworkday" name="getworkday"></a> getWorkDay

▸ **getWorkDay**(`index`): [`WorkDay`](../modules/GC.Spread.Sheets.GanttSheet.md#workday)

获取本周指定一天的工作时间

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 从0到6的数字或 DayOfWeek 值表示这一天 |

#### Returns

[`WorkDay`](../modules/GC.Spread.Sheets.GanttSheet.md#workday)

指定一天的工作时间

#### Inherited from

[WorkWeek](GC.Spread.Sheets.GanttSheet.WorkWeek.md).[getWorkDay](GC.Spread.Sheets.GanttSheet.WorkWeek.md#getworkday)
