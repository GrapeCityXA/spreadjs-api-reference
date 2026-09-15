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

Creates a new week with the specified work times of each day.

**`classdesc`** Represents the a week in calender, which defines the work times of each day.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workDays` | [`WorkDay`](../modules/GC.Spread.Sheets.GanttSheet.md#workday)[] | A workday array with 7 items from Sunday to Saturday, specifies the work times of each day in a week. |

## Methods

### <a id="getworkday" name="getworkday"></a> getWorkDay

▸ **getWorkDay**(`index`): [`WorkDay`](../modules/GC.Spread.Sheets.GanttSheet.md#workday)

Gets the work times for the specified day in the week.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | A number from 0 to 6, or a DayOfWeek value indicates the day. |

#### Returns

[`WorkDay`](../modules/GC.Spread.Sheets.GanttSheet.md#workday)

The work times for the specified day.
