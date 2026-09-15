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

使用指定名称创建任务栏样式规则

**`classdesc`** 代表项目的任务栏样式规则。可以从此类扩展并实施自定义规则

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

获取此规则的名称

___

### <a id="style" name="style"></a> style

• **style**: [`TaskStyle`](../modules/GC.Spread.Sheets.GanttSheet.md#taskstyle)

获取或设置所有任务栏的样式，此规则匹配

## Methods

### <a id="getfromdate" name="getfromdate"></a> getFromDate

▸ **getFromDate**(`task`): `Date`

获取指示指定任务的任务栏开始的日期
默认情况下，它返回 task.startDisplayed
在您的自定义规则中覆盖此方法并返回结果

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `task` | [`Task`](GC.Spread.Sheets.GanttSheet.Task.md) | 匹配该规则的任务 |

#### Returns

`Date`

日期值表示指定任务的任务栏的开始

___

### <a id="gettodate" name="gettodate"></a> getToDate

▸ **getToDate**(`task`): `Date`

获取指示指定任务的任务栏结束的日期
默认情况下，它返回任务。在您的自定义规则中覆盖此方法并返回结果

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `task` | [`Task`](GC.Spread.Sheets.GanttSheet.Task.md) | 匹配该规则的任务 |

#### Returns

`Date`

日期值表示指定任务的任务栏的结束

___

### <a id="match" name="match"></a> match

▸ **match**(`task`): `boolean`

确定该规则定义的任务栏是否匹配指定的任务
在您的自定义规则中覆盖此方法并返回结果

**`abstract`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `task` | [`Task`](GC.Spread.Sheets.GanttSheet.Task.md) | 检查的任务 |

#### Returns

`boolean`

如果任务匹配并将显示此规则的任务栏，则是 True ；否则为 False
