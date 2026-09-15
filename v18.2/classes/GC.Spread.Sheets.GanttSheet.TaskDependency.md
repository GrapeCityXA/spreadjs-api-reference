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

创建任务依赖关系。

**`classdesc`** 表示任务依赖关系。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `from` | [`Task`](GC.Spread.Sheets.GanttSheet.Task.md) | 表示依赖关系的起始任务。 |
| `to` | [`Task`](GC.Spread.Sheets.GanttSheet.Task.md) | 表示依赖关系的目标任务。 |
| `type?` | [`TaskDependencyType`](../modules/GC.Spread.Sheets.GanttSheet.md#taskdependencytype) | - |

## Properties

### <a id="from" name="from"></a> from

• **from**: [`Task`](GC.Spread.Sheets.GanttSheet.Task.md)

获取此依赖关系的起始任务。

**`readonly`**

___

### <a id="to" name="to"></a> to

• **to**: [`Task`](GC.Spread.Sheets.GanttSheet.Task.md)

获取此依赖关系的目标任务。

**`readonly`**

___

### <a id="type" name="type"></a> type

• **type**: [`TaskDependencyType`](../modules/GC.Spread.Sheets.GanttSheet.md#taskdependencytype)

获取此依赖关系的类型。

**`readonly`**
