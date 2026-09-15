# Class: Project

[Sheets](../modules/GC.Spread.Sheets.md).[GanttSheet](../modules/GC.Spread.Sheets.GanttSheet.md).Project

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.GanttSheet.Project.md#constructor)

### Properties

- [calendar](GC.Spread.Sheets.GanttSheet.Project.md#calendar)
- [calendarSettings](GC.Spread.Sheets.GanttSheet.Project.md#calendarsettings)
- [count](GC.Spread.Sheets.GanttSheet.Project.md#count)
- [currentDate](GC.Spread.Sheets.GanttSheet.Project.md#currentdate)
- [dependencies](GC.Spread.Sheets.GanttSheet.Project.md#dependencies)
- [finishDate](GC.Spread.Sheets.GanttSheet.Project.md#finishdate)
- [layout](GC.Spread.Sheets.GanttSheet.Project.md#layout)
- [root](GC.Spread.Sheets.GanttSheet.Project.md#root)
- [sorted](GC.Spread.Sheets.GanttSheet.Project.md#sorted)
- [startDate](GC.Spread.Sheets.GanttSheet.Project.md#startdate)
- [taskStyleRules](GC.Spread.Sheets.GanttSheet.Project.md#taskstylerules)
- [tasks](GC.Spread.Sheets.GanttSheet.Project.md#tasks)
- [tasksSorted](GC.Spread.Sheets.GanttSheet.Project.md#taskssorted)
- [timescale](GC.Spread.Sheets.GanttSheet.Project.md#timescale)

### Methods

- [addDependency](GC.Spread.Sheets.GanttSheet.Project.md#adddependency)
- [addTasks](GC.Spread.Sheets.GanttSheet.Project.md#addtasks)
- [getTask](GC.Spread.Sheets.GanttSheet.Project.md#gettask)
- [indentTasks](GC.Spread.Sheets.GanttSheet.Project.md#indenttasks)
- [indentTasksByRange](GC.Spread.Sheets.GanttSheet.Project.md#indenttasksbyrange)
- [insertTasks](GC.Spread.Sheets.GanttSheet.Project.md#inserttasks)
- [outdentTasks](GC.Spread.Sheets.GanttSheet.Project.md#outdenttasks)
- [outdentTasksByRange](GC.Spread.Sheets.GanttSheet.Project.md#outdenttasksbyrange)
- [removeDependency](GC.Spread.Sheets.GanttSheet.Project.md#removedependency)
- [removeTasks](GC.Spread.Sheets.GanttSheet.Project.md#removetasks)
- [removeTasksByRange](GC.Spread.Sheets.GanttSheet.Project.md#removetasksbyrange)
- [resumeSchedule](GC.Spread.Sheets.GanttSheet.Project.md#resumeschedule)
- [sort](GC.Spread.Sheets.GanttSheet.Project.md#sort)
- [suspendSchedule](GC.Spread.Sheets.GanttSheet.Project.md#suspendschedule)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Project**(`name`)

表示用于排程的项目。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 表示此项目的名称。该名称也将应用于根任务。 |

## Properties

### <a id="calendar" name="calendar"></a> calendar

• **calendar**: [`Calendar`](GC.Spread.Sheets.GanttSheet.Calendar.md)

获取或设置此项目的日历。它是此项目中所有任务的默认日历。
注意不要修改日历的成员，而是请替换日历实例进行修改。

___

### <a id="calendarsettings" name="calendarsettings"></a> calendarSettings

• **calendarSettings**: [`CalendarSettings`](GC.Spread.Sheets.GanttSheet.CalendarSettings.md)

获取此项目的日历设置，并配置用于计算日期和持续时间的参数。

**`readonly`**

___

### <a id="count" name="count"></a> count

• **count**: `number`

获取此项目中的任务和空行数量。

**`readonly`**

___

### <a id="currentdate" name="currentdate"></a> currentDate

• **currentDate**: `Date`

获取或设置此项目的当前日期。甘特图将显示一条网格线来指示当前日期。

___

### <a id="dependencies" name="dependencies"></a> dependencies

• **dependencies**: [`TaskDependency`](GC.Spread.Sheets.GanttSheet.TaskDependency.md)[]

获取此项目中的任务依赖关系。
这是内部任务依赖关系的克隆数组。调用 addDependency 或 removeDependency 来修改它。

**`readonly`**

___

### <a id="finishdate" name="finishdate"></a> finishDate

• **finishDate**: `Date`

获取此项目的完成日期。默认情况下，完成日期由开始日期安排。

___

### <a id="layout" name="layout"></a> layout

• **layout**: [`TaskbarLayout`](GC.Spread.Sheets.GanttSheet.TaskbarLayout.md)

获取甘特图的布局，并配置任务条和链接的布局外观。

**`readonly`**

___

### <a id="root" name="root"></a> root

• **root**: [`Task`](GC.Spread.Sheets.GanttSheet.Task.md)

获取此项目的根任务。

**`readonly`**

___

### <a id="sorted" name="sorted"></a> sorted

• **sorted**: `boolean`

指示任务是否已排序。

**`readonly`**

___

### <a id="startdate" name="startdate"></a> startDate

• **startDate**: `Date`

获取或设置此项目的开始日期。排程将从该日期开始。

___

### <a id="taskstylerules" name="taskstylerules"></a> taskStyleRules

• **taskStyleRules**: [`Collection`](GC.Spread.Sheets.GanttSheet.Collection.md)<[`TaskbarStyleRule`](GC.Spread.Sheets.GanttSheet.TaskbarStyleRule.md)\>

获取甘特图的任务样式规则列表，并配置具有指定规则的任务的外观。

**`readonly`**

___

### <a id="tasks" name="tasks"></a> tasks

• **tasks**: [`Task`](GC.Spread.Sheets.GanttSheet.Task.md)[]

获取此项目中的任务。
这是内部任务的克隆数组。如果要获取具有指定任务编号的任务，请使用 getTask。

**`readonly`**

___

### <a id="taskssorted" name="taskssorted"></a> tasksSorted

• **tasksSorted**: [`Task`](GC.Spread.Sheets.GanttSheet.Task.md)[]

获取此项目中按排序顺序排列的任务。
特别地，null 表示数组中的空行。
这是内部任务的克隆数组。如果要获取排序后具有指定行索引的任务，请使用 getTaskByRow。

**`readonly`**

___

### <a id="timescale" name="timescale"></a> timescale

• **timescale**: [`Timescale`](GC.Spread.Sheets.GanttSheet.Timescale.md)

获取甘特图的时间刻度，并配置时间刻度的外观和位置。

**`readonly`**

## Methods

### <a id="adddependency" name="adddependency"></a> addDependency

▸ **addDependency**(`dependencies`): `void`

为项目添加一个或多个任务依赖关系。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `dependencies` | [`ITaskDependency`](../modules/GC.Spread.Sheets.GanttSheet.md#itaskdependency) \| [`TaskDependency`](GC.Spread.Sheets.GanttSheet.TaskDependency.md) \| [`TaskDependency`](GC.Spread.Sheets.GanttSheet.TaskDependency.md)[] \| [`ITaskDependency`](../modules/GC.Spread.Sheets.GanttSheet.md#itaskdependency)[] | 表示要添加的任务依赖关系。 |

#### Returns

`void`

___

### <a id="addtasks" name="addtasks"></a> addTasks

▸ **addTasks**(`data?`, `level?`): [`Task`](GC.Spread.Sheets.GanttSheet.Task.md)[]

使用指定的数量或数据为此项目添加任务。

#### Parameters

| Name | Type |
| :------ | :------ |
| `data?` | `number` \| [`ITaskData`](../modules/GC.Spread.Sheets.GanttSheet.md#itaskdata) \| [`ITaskData`](../modules/GC.Spread.Sheets.GanttSheet.md#itaskdata)[] |
| `level?` | `number` |

#### Returns

[`Task`](GC.Spread.Sheets.GanttSheet.Task.md)[]

添加的任务数组。

___

### <a id="gettask" name="gettask"></a> getTask

▸ **getTask**(`taskNumber`): [`Task`](GC.Spread.Sheets.GanttSheet.Task.md)

获取具有指定任务编号的任务。
通常，任务编号是任务在项目中的索引。
如果任务已排序，请使用 getTaskByRow 获取具有指定行索引的任务。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskNumber` | `number` | 指定目标任务的任务编号。 |

#### Returns

[`Task`](GC.Spread.Sheets.GanttSheet.Task.md)

具有指定任务编号的任务。

___

### <a id="indenttasks" name="indenttasks"></a> indentTasks

▸ **indentTasks**(`taskNumbers`): `void`

增加此项目中指定任务的级别。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskNumbers` | `number` \| `number`[] | 一个数字或数字数组，表示要增加级别的任务编号。 |

#### Returns

`void`

___

### <a id="indenttasksbyrange" name="indenttasksbyrange"></a> indentTasksByRange

▸ **indentTasksByRange**(`taskNumber`, `count?`): `void`

增加此项目中具有连续编号的任务范围的级别。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskNumber` | `number` | 一个数字，表示要增加级别的第一个任务编号。 |
| `count?` | `number` | - |

#### Returns

`void`

___

### <a id="inserttasks" name="inserttasks"></a> insertTasks

▸ **insertTasks**(`taskNumber`, `data?`, `level?`): [`Task`](GC.Spread.Sheets.GanttSheet.Task.md)[]

在指定位置插入具有提供数据的任务。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskNumber` | `number` | 指定要插入的目标任务编号。 |
| `data?` | `number` \| [`ITaskData`](../modules/GC.Spread.Sheets.GanttSheet.md#itaskdata) \| [`ITaskData`](../modules/GC.Spread.Sheets.GanttSheet.md#itaskdata)[] | - |
| `level?` | `number` | - |

#### Returns

[`Task`](GC.Spread.Sheets.GanttSheet.Task.md)[]

插入的任务数组。

___

### <a id="outdenttasks" name="outdenttasks"></a> outdentTasks

▸ **outdentTasks**(`taskNumbers`): `void`

减少此项目中指定任务的级别。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskNumbers` | `number` \| `number`[] | 一个数字或数字数组，表示要减少级别的任务编号。 |

#### Returns

`void`

___

### <a id="outdenttasksbyrange" name="outdenttasksbyrange"></a> outdentTasksByRange

▸ **outdentTasksByRange**(`taskNumber`, `count?`): `void`

减少此项目中具有连续编号的任务范围的级别。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskNumber` | `number` | 一个数字，表示要减少级别的第一个任务编号。 |
| `count?` | `number` | - |

#### Returns

`void`

___

### <a id="removedependency" name="removedependency"></a> removeDependency

▸ **removeDependency**(`dependencies`): `void`

移除项目的一个或多个任务依赖关系。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `dependencies` | [`TaskDependency`](GC.Spread.Sheets.GanttSheet.TaskDependency.md) \| [`TaskDependency`](GC.Spread.Sheets.GanttSheet.TaskDependency.md)[] | 表示要移除的任务依赖关系。注意依赖关系实例应该是 project.dependencies 的成员。 |

#### Returns

`void`

___

### <a id="removetasks" name="removetasks"></a> removeTasks

▸ **removeTasks**(`taskNumbers`): `void`

移除此项目中具有指定任务编号的任务。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskNumbers` | `number` \| `number`[] | 一个数字或数字数组，表示要移除的任务编号。 |

#### Returns

`void`

___

### <a id="removetasksbyrange" name="removetasksbyrange"></a> removeTasksByRange

▸ **removeTasksByRange**(`taskNumber`, `count?`): `void`

移除此项目中具有连续任务编号的任务范围。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskNumber` | `number` | 一个数字，表示要移除的第一个任务编号。 |
| `count?` | `number` | - |

#### Returns

`void`

___

### <a id="resumeschedule" name="resumeschedule"></a> resumeSchedule

▸ **resumeSchedule**(): `void`

在对多个任务或依赖关系进行修改后恢复调度过程。

#### Returns

`void`

___

### <a id="sort" name="sort"></a> sort

▸ **sort**(`fields`, `ascendingStates?`, `keepStructure?`, `renumber?`): `void`

使用指定的任务字段对任务进行排序。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fields` | `string`[] | 指定要排序的字段。 |
| `ascendingStates?` | `boolean`[] | - |
| `keepStructure?` | `boolean` | - |
| `renumber?` | `boolean` | - |

#### Returns

`void`

___

### <a id="suspendschedule" name="suspendschedule"></a> suspendSchedule

▸ **suspendSchedule**(): `void`

在对多个任务或依赖关系进行修改之前暂停调度过程。

#### Returns

`void`
