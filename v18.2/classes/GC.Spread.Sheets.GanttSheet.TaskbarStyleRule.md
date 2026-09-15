# Class: TaskbarStyleRule

[Sheets](../modules/GC.Spread.Sheets.md).[GanttSheet](../modules/GC.Spread.Sheets.GanttSheet.md).TaskbarStyleRule

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.GanttSheet.TaskbarStyleRule.md#constructor)

### Properties

- [name](GC.Spread.Sheets.GanttSheet.TaskbarStyleRule.md#name)
- [style](GC.Spread.Sheets.GanttSheet.TaskbarStyleRule.md#style)

### Methods

- [getFromDate](GC.Spread.Sheets.GanttSheet.TaskbarStyleRule.md#getfromdate)
- [getToDate](GC.Spread.Sheets.GanttSheet.TaskbarStyleRule.md#gettodate)
- [match](GC.Spread.Sheets.GanttSheet.TaskbarStyleRule.md#match)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new TaskbarStyleRule**()

使用指定名称创建任务条样式规则。

**`classdesc`** 表示项目的任务条样式规则。可以继承此类并实现自定义规则。

**`example`**
```
 class MyProgressRule extends TaskbarStyleRule {
     constructor() {
         super("My Progress");
         this.style = {
             taskbarStyle: {
                 middleColor: "#3B87D4",
                 middleShape: "RectangleMiddle",
                 middlePattern: "solidFill",
             }
         };
     }
     match(task: Task): boolean {
         return task.complete > 0;
     }
     getFromDate(task: Task) {
         return task.startDisplayed;
     }
     getToDate(task: Task) {
         return task.completeThrough;
     }
 }
```

## Properties

### <a id="name" name="name"></a> name

• **name**: `string`

获取此规则的名称。

___

### <a id="style" name="style"></a> style

• **style**: [`TaskStyle`](../modules/GC.Spread.Sheets.GanttSheet.md#taskstyle)

获取或设置此规则匹配的所有任务条的样式。

## Methods

### <a id="getfromdate" name="getfromdate"></a> getFromDate

▸ **getFromDate**(`task`): `Date`

获取指定任务的任务条开始日期。
默认返回 task.startDisplayed。在自定义规则中重写此方法并返回结果。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `task` | [`Task`](GC.Spread.Sheets.GanttSheet.Task.md) | 此规则匹配的任务。 |

#### Returns

`Date`

表示指定任务的任务条开始日期的日期值。

___

### <a id="gettodate" name="gettodate"></a> getToDate

▸ **getToDate**(`task`): `Date`

获取指定任务的任务条结束日期。
默认返回 task.finishDisplayed。在自定义规则中重写此方法并返回结果。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `task` | [`Task`](GC.Spread.Sheets.GanttSheet.Task.md) | 此规则匹配的任务。 |

#### Returns

`Date`

表示指定任务的任务条结束日期的日期值。

___

### <a id="match" name="match"></a> match

▸ **match**(`task`): `boolean`

确定此规则定义的任务条是否匹配指定任务。
在自定义规则中重写此方法并返回结果。

**`abstract`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `task` | [`Task`](GC.Spread.Sheets.GanttSheet.Task.md) | 要检查的任务。 |

#### Returns

`boolean`

如果任务匹配并将显示此规则的任务条，则为 true；否则为 false。
