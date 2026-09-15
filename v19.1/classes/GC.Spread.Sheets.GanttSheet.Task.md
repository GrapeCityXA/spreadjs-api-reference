# Class: Task

[Sheets](../modules/GC.Spread.Sheets.md).[GanttSheet](../modules/GC.Spread.Sheets.GanttSheet.md).Task

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.GanttSheet.Task.md#constructor)

### Properties

- [children](GC.Spread.Sheets.GanttSheet.Task.md#children)
- [complete](GC.Spread.Sheets.GanttSheet.Task.md#complete)
- [completeThrough](GC.Spread.Sheets.GanttSheet.Task.md#completethrough)
- [duration](GC.Spread.Sheets.GanttSheet.Task.md#duration)
- [finish](GC.Spread.Sheets.GanttSheet.Task.md#finish)
- [finishDisplayed](GC.Spread.Sheets.GanttSheet.Task.md#finishdisplayed)
- [isMilestone](GC.Spread.Sheets.GanttSheet.Task.md#ismilestone)
- [isNormal](GC.Spread.Sheets.GanttSheet.Task.md#isnormal)
- [isSummary](GC.Spread.Sheets.GanttSheet.Task.md#issummary)
- [level](GC.Spread.Sheets.GanttSheet.Task.md#level)
- [mode](GC.Spread.Sheets.GanttSheet.Task.md#mode)
- [name](GC.Spread.Sheets.GanttSheet.Task.md#name)
- [parent](GC.Spread.Sheets.GanttSheet.Task.md#parent)
- [predecessorDependencies](GC.Spread.Sheets.GanttSheet.Task.md#predecessordependencies)
- [predecessors](GC.Spread.Sheets.GanttSheet.Task.md#predecessors)
- [rowIndex](GC.Spread.Sheets.GanttSheet.Task.md#rowindex)
- [start](GC.Spread.Sheets.GanttSheet.Task.md#start)
- [startDisplayed](GC.Spread.Sheets.GanttSheet.Task.md#startdisplayed)
- [style](GC.Spread.Sheets.GanttSheet.Task.md#style)
- [successorDependencies](GC.Spread.Sheets.GanttSheet.Task.md#successordependencies)
- [successors](GC.Spread.Sheets.GanttSheet.Task.md#successors)
- [taskNumber](GC.Spread.Sheets.GanttSheet.Task.md#tasknumber)

### Methods

- [getValue](GC.Spread.Sheets.GanttSheet.Task.md#getvalue)
- [setValue](GC.Spread.Sheets.GanttSheet.Task.md#setvalue)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Task**()

创建任务实例。仅供内部使用。

**`classdesc`** 表示项目中的任务。

## Properties

### <a id="children" name="children"></a> children

• **children**: [`Task`](GC.Spread.Sheets.GanttSheet.Task.md)[]

获取此任务的子任务。
这是内部任务的克隆数组。要修改子任务，请调用 project.insertTasks 和 project.removeTasks。

**`readonly`**

___

### <a id="complete" name="complete"></a> complete

• **complete**: `number`

获取或设置表示此任务完成百分比的浮点数。该值应大于或等于 0。

___

### <a id="completethrough" name="completethrough"></a> completeThrough

• **completeThrough**: `Date`

获取或设置表示任务进度的日期值。它是任务实际报告的时间点。

___

### <a id="duration" name="duration"></a> duration

• **duration**: `string` \| `number` \| [`Duration`](../modules/GC.Spread.Sheets.GanttSheet.md#duration)

获取或设置此任务的持续时间。
允许设置数字或字符串值来表示持续时间，获取结果将始终是有效的 {@link GC.Spread.Sheets.GanttSheet.Duration} 对象。
注意，对于手动调度模式下的仅开始或仅完成任务，持续时间可能为 null。

___

### <a id="finish" name="finish"></a> finish

• **finish**: `Date`

获取或设置此任务的完成日期。
注意，对于手动调度模式下的仅开始或仅持续时间任务，完成日期可能为 null。在这些情况下，使用 finishDisplayed 获取甘特图中的实际值。

___

### <a id="finishdisplayed" name="finishdisplayed"></a> finishDisplayed

• **finishDisplayed**: `Date`

获取此任务在甘特图中显示的完成日期。

**`readonly`**

___

### <a id="ismilestone" name="ismilestone"></a> isMilestone

• **isMilestone**: `boolean`

获取或设置一个布尔值，指示此任务是否为里程碑。
如果未指定，当持续时间时间为 0 时，任务将显示为里程碑。

___

### <a id="isnormal" name="isnormal"></a> isNormal

• **isNormal**: `boolean`

获取一个布尔值，指示此任务是否为普通任务。普通任务既不是摘要任务也不是里程碑。

**`readonly`**

___

### <a id="issummary" name="issummary"></a> isSummary

• **isSummary**: `boolean`

获取一个布尔值，指示此任务是否为摘要任务。摘要任务是其他任务的父任务。

**`readonly`**

___

### <a id="level" name="level"></a> level

• **level**: `number`

获取此任务的级别。对于根任务，值为 0。

**`readonly`**

___

### <a id="mode" name="mode"></a> mode

• **mode**: [`TaskScheduleMode`](../modules/GC.Spread.Sheets.GanttSheet.md#taskschedulemode)

获取或设置此任务的调度模式。

___

### <a id="name" name="name"></a> name

• **name**: `string`

获取或设置此任务的名称。

___

### <a id="parent" name="parent"></a> parent

• **parent**: [`Task`](GC.Spread.Sheets.GanttSheet.Task.md)

获取此任务的父任务。注意根任务没有父任务。

**`readonly`**

___

### <a id="predecessordependencies" name="predecessordependencies"></a> predecessorDependencies

• **predecessorDependencies**: [`TaskDependency`](GC.Spread.Sheets.GanttSheet.TaskDependency.md)[]

获取包含此任务所有前置任务的 {@link GC.Spread.Sheets.GanttSheet.TaskDependency} 数组。
要修改前置任务，请设置任务的 predecessor 字段，或调用项目的 addDependency 或 removeDependency。

**`readonly`**

___

### <a id="predecessors" name="predecessors"></a> predecessors

• **predecessors**: `string`

获取或设置表示此任务前置任务的字符串值。
前置任务字符串包含一个或多个任务编号和依赖类型。

___

### <a id="rowindex" name="rowindex"></a> rowIndex

• **rowIndex**: `number`

获取此任务的行索引。如果任务未排序，行索引与任务 ID 相同。

**`readonly`**

___

### <a id="start" name="start"></a> start

• **start**: `Date`

获取或设置此任务的开始日期。
注意，对于手动调度模式下的仅完成或仅持续时间任务，开始日期可能为 null。在这些情况下，使用 startDisplayed 获取甘特图中的实际值。

___

### <a id="startdisplayed" name="startdisplayed"></a> startDisplayed

• **startDisplayed**: `Date`

获取此任务在甘特图中显示的开始日期。

**`readonly`**

___

### <a id="style" name="style"></a> style

• **style**: `Object`

获取或设置此任务的任务条样式。任务在甘特图中可能有多个任务条，您可以通过指定的规则名称设置每个条的样式。
注意不要修改此值的成员，而是为此字段设置新的对象实例。

#### Index signature

▪ [key: `string`]: [`TaskStyle`](../modules/GC.Spread.Sheets.GanttSheet.md#taskstyle)

___

### <a id="successordependencies" name="successordependencies"></a> successorDependencies

• **successorDependencies**: [`TaskDependency`](GC.Spread.Sheets.GanttSheet.TaskDependency.md)[]

获取包含此任务所有后续任务的 {@link GC.Spread.Sheets.GanttSheet.TaskDependency} 数组。
要修改后续任务，请设置任务的 successors 字段，或调用项目的 addDependency 或 removeDependency。

**`readonly`**

___

### <a id="successors" name="successors"></a> successors

• **successors**: `string`

获取或设置表示此任务后续任务的字符串值。
后续任务字符串包含一个或多个任务编号和依赖类型。

___

### <a id="tasknumber" name="tasknumber"></a> taskNumber

• **taskNumber**: `number`

获取此任务的编号。对于根任务，值为 0。

**`readonly`**

## Methods

### <a id="getvalue" name="getvalue"></a> getValue

▸ **getValue**(`property`): `void`

通过指定的属性获取任务值。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `property` | `string` | 指定的属性。 |

#### Returns

`void`

任务值。

___

### <a id="setvalue" name="setvalue"></a> setValue

▸ **setValue**(`property`, `value`): `void`

通过指定的属性设置任务值。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `property` | `string` | 指定的属性。 |
| `value` | `any` | 指定的值。 |

#### Returns

`void`
