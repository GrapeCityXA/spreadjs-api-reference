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

为自定义日期范围创建具有指定每天工作时间的周。

**`classdesc`** 表示日历中的一周，定义了每天的工作时间。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workDays` | [`WorkDay`](../modules/GC.Spread.Sheets.GanttSheet.md#workday)[] | 从周日到周六包含7个工作日的工作日数组，指定一周中每天的工作时间。 |
| `start` | `Date` | 指定在日历中应用此周定义的日期范围的开始日期。 |
| `finish` | `Date` | 指定在日历中应用此周定义的日期范围的结束日期。 |

#### Overrides

[WorkWeek](GC.Spread.Sheets.GanttSheet.WorkWeek.md).[constructor](GC.Spread.Sheets.GanttSheet.WorkWeek.md#constructor)

## Properties

### <a id="finish" name="finish"></a> finish

• **finish**: `Date`

获取或设置此自定义工作周的结束日期。

___

### <a id="start" name="start"></a> start

• **start**: `Date`

获取或设置此自定义工作周的开始日期。

## Methods

### <a id="getworkday" name="getworkday"></a> getWorkDay

▸ **getWorkDay**(`index`): [`WorkDay`](../modules/GC.Spread.Sheets.GanttSheet.md#workday)

获取一周中指定日期的工作时间。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 0 到 6 之间的数字或 DayOfWeek 值表示该日期。 |

#### Returns

[`WorkDay`](../modules/GC.Spread.Sheets.GanttSheet.md#workday)

指定日期的工作时间。

#### Inherited from

[WorkWeek](GC.Spread.Sheets.GanttSheet.WorkWeek.md).[getWorkDay](GC.Spread.Sheets.GanttSheet.WorkWeek.md#getworkday)
