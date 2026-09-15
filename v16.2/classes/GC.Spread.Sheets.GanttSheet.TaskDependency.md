# Class: TaskDependency

[Sheets](../modules/GC.Spread.Sheets.md).[GanttSheet](../modules/GC.Spread.Sheets.GanttSheet.md).TaskDependency

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.GanttSheet.TaskDependency.md#constructor)

### Properties

- [from](GC.Spread.Sheets.GanttSheet.TaskDependency.md#from)
- [to](GC.Spread.Sheets.GanttSheet.TaskDependency.md#to)
- [type](GC.Spread.Sheets.GanttSheet.TaskDependency.md#type)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new TaskDependency**(`from`, `to`, `type?`)

创建一个任务依赖。

**`classdesc`** 代表任务依赖。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `from` | [`Task`](GC.Spread.Sheets.GanttSheet.Task.md) | 指示依赖的任务 - From |
| `to` | [`Task`](GC.Spread.Sheets.GanttSheet.Task.md) | 指示依赖的任务 - To |
| `type?` | [`TaskDependencyType`](../modules/GC.Spread.Sheets.GanttSheet.md#taskdependencytype) | - |

## Properties

### <a id="from" name="from"></a> from

• **from**: [`Task`](GC.Spread.Sheets.GanttSheet.Task.md)

获取依赖此关系的任务 - From。

**`readonly`**

___

### <a id="to" name="to"></a> to

• **to**: [`Task`](GC.Spread.Sheets.GanttSheet.Task.md)

获取依赖此关系的任务 - To。

**`readonly`**

___

### <a id="type" name="type"></a> type

• **type**: [`TaskDependencyType`](../modules/GC.Spread.Sheets.GanttSheet.md#taskdependencytype)

获取依赖的类型。

**`readonly`**
