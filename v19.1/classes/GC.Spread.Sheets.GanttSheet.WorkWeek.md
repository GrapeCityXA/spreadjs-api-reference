# Class: WorkWeek

[Sheets](../modules/GC.Spread.Sheets.md).[GanttSheet](../modules/GC.Spread.Sheets.GanttSheet.md).WorkWeek

## Hierarchy

- **`WorkWeek`**

  ↳ [`CustomWorkWeek`](GC.Spread.Sheets.GanttSheet.CustomWorkWeek.md)

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.GanttSheet.WorkWeek.md#constructor)

### Methods

- [getWorkDay](GC.Spread.Sheets.GanttSheet.WorkWeek.md#getworkday)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new WorkWeek**(`workDays`)

使用每天指定的工作时间创建新的工作周。

**`classdesc`** Represents the a week in calender, which defines the work times of each day.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workDays` | [`WorkDay`](../modules/GC.Spread.Sheets.GanttSheet.md#workday)[] | 包含 7 个项目（从星期日到星期六）的工作日数组，用于指定一周中每天的工作时间。 |

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
