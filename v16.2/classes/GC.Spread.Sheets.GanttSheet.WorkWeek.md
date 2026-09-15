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

在每天指定的工作时间中创建一个新的一周。

**`classdesc`** 代表日历中的一个星期，它定义了每天的工作时间。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workDays` | [`WorkDay`](../modules/GC.Spread.Sheets.GanttSheet.md#workday)[] | 一个工作日阵列，从周日到星期六，有7个项目，指定了一周内每天的工作时间 |

## Methods

### <a id="getworkday" name="getworkday"></a> getWorkDay

▸ **getWorkDay**(`index`): [`WorkDay`](../modules/GC.Spread.Sheets.GanttSheet.md#workday)

获取本周指定一天的工作时间。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 从0到6的数字或 Dayofweek 值表示这一天 |

#### Returns

[`WorkDay`](../modules/GC.Spread.Sheets.GanttSheet.md#workday)

指定一天的工作时间。
