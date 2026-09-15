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

代表一个计划的项目

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 指示此项目的名称。该名称也将适用于根部任务 |

## Properties

### <a id="calendar" name="calendar"></a> calendar

• **calendar**: [`Calendar`](GC.Spread.Sheets.GanttSheet.Calendar.md)

获取或设置此项目的日历。它是该项目中所有任务的默认日历
注意不要修改日历的成员，而是请替换为修改的日历实例

___

### <a id="calendarsettings" name="calendarsettings"></a> calendarSettings

• **calendarSettings**: [`CalendarSettings`](GC.Spread.Sheets.GanttSheet.CalendarSettings.md)

获取此项目的日历设置，并配置用于计算日期和持续时间的参数

**`readonly`**

___

### <a id="count" name="count"></a> count

• **count**: `number`

在此项目中获取任务和空白行的计数

**`readonly`**

___

### <a id="currentdate" name="currentdate"></a> currentDate

• **currentDate**: `Date`

获取或设置此项目的当前日期。甘特图将显示一个网格线以指示当前日期

___

### <a id="dependencies" name="dependencies"></a> dependencies

• **dependencies**: [`TaskDependency`](GC.Spread.Sheets.GanttSheet.TaskDependency.md)[]

获取该项目中的任务依赖项
这是内部任务依赖项的克隆数组。调用add依赖性或删除依赖性以修改它

**`readonly`**

___

### <a id="finishdate" name="finishdate"></a> finishDate

• **finishDate**: `Date`

获取该项目的完成日期。默认情况下，完成日期是按开始日期安排的

___

### <a id="layout" name="layout"></a> layout

• **layout**: [`TaskbarLayout`](GC.Spread.Sheets.GanttSheet.TaskbarLayout.md)

获取甘特图的布局，并配置任务栏和链接的布局外观

**`readonly`**

___

### <a id="root" name="root"></a> root

• **root**: [`Task`](GC.Spread.Sheets.GanttSheet.Task.md)

获取该项目的根本任务

**`readonly`**

___

### <a id="sorted" name="sorted"></a> sorted

• **sorted**: `boolean`

指示任务已排序

**`readonly`**

___

### <a id="startdate" name="startdate"></a> startDate

• **startDate**: `Date`

获取或设置此项目的开始日期。调度将从此日期开始

___

### <a id="taskstylerules" name="taskstylerules"></a> taskStyleRules

• **taskStyleRules**: [`Collection`](GC.Spread.Sheets.GanttSheet.Collection.md)<[`TaskbarStyleRule`](GC.Spread.Sheets.GanttSheet.TaskbarStyleRule.md)\>

获取甘特图的任务样式规则列表，并使用指定规则配置任务的外观

**`readonly`**

___

### <a id="tasks" name="tasks"></a> tasks

• **tasks**: [`Task`](GC.Spread.Sheets.GanttSheet.Task.md)[]

在此项目中获取任务
这是内部任务的克隆阵列。如果要使用指定的任务编号，请使用 GetTask

**`readonly`**

___

### <a id="taskssorted" name="taskssorted"></a> tasksSorted

• **tasksSorted**: [`Task`](GC.Spread.Sheets.GanttSheet.Task.md)[]

按顺序获取该项目中的任务
特别是，null表示数组中的空白行
这是内部任务的克隆阵列。如果您想在排序之后使用指定的行索引获得一个任务，请使用 GetTaskByRow

**`readonly`**

___

### <a id="timescale" name="timescale"></a> timescale

• **timescale**: [`Timescale`](GC.Spread.Sheets.GanttSheet.Timescale.md)

获取甘特图的时间尺度，并配置时间尺度的外观和位置

**`readonly`**

## Methods

### <a id="adddependency" name="adddependency"></a> addDependency

▸ **addDependency**(`dependencies`): `void`

为项目添加一个或多个任务依赖性

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `dependencies` | [`ITaskDependency`](../modules/GC.Spread.Sheets.GanttSheet.md#itaskdependency) \| [`TaskDependency`](GC.Spread.Sheets.GanttSheet.TaskDependency.md) \| [`TaskDependency`](GC.Spread.Sheets.GanttSheet.TaskDependency.md)[] \| [`ITaskDependency`](../modules/GC.Spread.Sheets.GanttSheet.md#itaskdependency)[] | 要添加的任务依赖项 |

#### Returns

`void`

___

### <a id="addtasks" name="addtasks"></a> addTasks

▸ **addTasks**(`data?`, `level?`): [`Task`](GC.Spread.Sheets.GanttSheet.Task.md)[]

使用此项目的指定计数或数据添加任务

#### Parameters

| Name | Type |
| :------ | :------ |
| `data?` | `number` \| [`ITaskData`](../modules/GC.Spread.Sheets.GanttSheet.md#itaskdata) \| [`ITaskData`](../modules/GC.Spread.Sheets.GanttSheet.md#itaskdata)[] |
| `level?` | `number` |

#### Returns

[`Task`](GC.Spread.Sheets.GanttSheet.Task.md)[]

Array of the added tasks.

___

### <a id="gettask" name="gettask"></a> getTask

▸ **getTask**(`taskNumber`): [`Task`](GC.Spread.Sheets.GanttSheet.Task.md)

通过指定的任务编号获取任务
通常，任务编号是项目中任务的索引
如果已经对任务进行了分类，请使用getTaskByrow来获得指定的行索引的任务

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskNumber` | `number` | 指定目标任务的任务编号 |

#### Returns

[`Task`](GC.Spread.Sheets.GanttSheet.Task.md)

指定任务编号的任务

___

### <a id="indenttasks" name="indenttasks"></a> indentTasks

▸ **indentTasks**(`taskNumbers`): `void`

增加了该项目的指定任务级别

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskNumbers` | `number` \| `number`[] | 数字或数量数组表示要增加级别的任务数 |

#### Returns

`void`

___

### <a id="indenttasksbyrange" name="indenttasksbyrange"></a> indentTasksByRange

▸ **indentTasksByRange**(`taskNumber`, `count?`): `void`

随着该项目的持续数字，增加了一系列任务的级别

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskNumber` | `number` | 一个数字指示提高级别的任务的第一个数字 |
| `count?` | `number` | - |

#### Returns

`void`

___

### <a id="inserttasks" name="inserttasks"></a> insertTasks

▸ **insertTasks**(`taskNumber`, `data?`, `level?`): [`Task`](GC.Spread.Sheets.GanttSheet.Task.md)[]

用提供的数据在指定位置插入任务

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskNumber` | `number` | 指定要插入的目标任务编号 |
| `data?` | `number` \| [`ITaskData`](../modules/GC.Spread.Sheets.GanttSheet.md#itaskdata) \| [`ITaskData`](../modules/GC.Spread.Sheets.GanttSheet.md#itaskdata)[] | - |
| `level?` | `number` | - |

#### Returns

[`Task`](GC.Spread.Sheets.GanttSheet.Task.md)[]

插入任务的数组

___

### <a id="outdenttasks" name="outdenttasks"></a> outdentTasks

▸ **outdentTasks**(`taskNumbers`): `void`

降低该项目的指定任务级别

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskNumbers` | `number` \| `number`[] | 数字或数数组表示要降低级别的任务数 |

#### Returns

`void`

___

### <a id="outdenttasksbyrange" name="outdenttasksbyrange"></a> outdentTasksByRange

▸ **outdentTasksByRange**(`taskNumber`, `count?`): `void`

随着该项目的持续数字，降低了一系列任务的级别

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskNumber` | `number` | 一个数字指示任务的第一个数字以降低级别 |
| `count?` | `number` | - |

#### Returns

`void`

___

### <a id="removedependency" name="removedependency"></a> removeDependency

▸ **removeDependency**(`dependencies`): `void`

删除项目的一个或多个任务依赖性

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `dependencies` | [`TaskDependency`](GC.Spread.Sheets.GanttSheet.TaskDependency.md) \| [`TaskDependency`](GC.Spread.Sheets.GanttSheet.TaskDependency.md)[] | 指示要删除的任务依赖项。注意依赖项实例应为 project.TaskDependency 的成员 |

#### Returns

`void`

___

### <a id="removetasks" name="removetasks"></a> removeTasks

▸ **removeTasks**(`taskNumbers`): `void`

使用此项目的指定任务编号删除任务

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskNumbers` | `number` \| `number`[] | 数字或数阵列指示要删除的任务数 |

#### Returns

`void`

___

### <a id="removetasksbyrange" name="removetasksbyrange"></a> removeTasksByRange

▸ **removeTasksByRange**(`taskNumber`, `count?`): `void`

删除了该项目的一系列任务

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `taskNumber` | `number` | 一个数字表示要删除的任务的第一个数字 |
| `count?` | `number` | - |

#### Returns

`void`

___

### <a id="resumeschedule" name="resumeschedule"></a> resumeSchedule

▸ **resumeSchedule**(): `void`

修改多个任务或依赖项后，恢复调度过程

#### Returns

`void`

___

### <a id="sort" name="sort"></a> sort

▸ **sort**(`fields`, `ascendingStates?`, `keepStructure?`, `renumber?`): `void`

用指定的任务字段对任务进行分类

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fields` | `string`[] | 指定要排序的字段 |
| `ascendingStates?` | `boolean`[] | - |
| `keepStructure?` | `boolean` | - |
| `renumber?` | `boolean` | - |

#### Returns

`void`

___

### <a id="suspendschedule" name="suspendschedule"></a> suspendSchedule

▸ **suspendSchedule**(): `void`

在对多个任务或依赖项进行修改之前，请暂停调度过程

#### Returns

`void`
