# Class: TaskbarStyleRule

[Sheets](../modules/GC.Spread.Sheets.md).[GanttSheet](../modules/GC.Spread.Sheets.GanttSheet.md).TaskbarStyleRule

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.GanttSheet.TaskbarStyleRule.md#constructor)

### Properties

- [name](GC.Spread.Sheets.GanttSheet.TaskbarStyleRule.md#name)
- [style](GC.Spread.Sheets.GanttSheet.TaskbarStyleRule.md#style)
- [typeName](GC.Spread.Sheets.GanttSheet.TaskbarStyleRule.md#typename)

### Methods

- [fromJSON](GC.Spread.Sheets.GanttSheet.TaskbarStyleRule.md#fromjson)
- [getFromDate](GC.Spread.Sheets.GanttSheet.TaskbarStyleRule.md#getfromdate)
- [getToDate](GC.Spread.Sheets.GanttSheet.TaskbarStyleRule.md#gettodate)
- [match](GC.Spread.Sheets.GanttSheet.TaskbarStyleRule.md#match)
- [toJSON](GC.Spread.Sheets.GanttSheet.TaskbarStyleRule.md#tojson)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new TaskbarStyleRule**(`name`)

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

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 表示规则的名称。该名称应该是唯一值。 |

## Properties

### <a id="name" name="name"></a> name

• **name**: `string`

获取此规则的名称。

___

### <a id="style" name="style"></a> style

• **style**: [`TaskStyle`](../modules/GC.Spread.Sheets.GanttSheet.md#taskstyle)

获取或设置此规则匹配的所有任务条的样式。

___

### <a id="typename" name="typename"></a> typeName

• **typeName**: `string`

表示用于支持序列化功能的类型名称字符串。
对于自定义规则，此属性应设置为完全限定类型名称（例如："MyNameScape.MyProgressRule"）。

## Methods

### <a id="fromjson" name="fromjson"></a> fromJSON

▸ **fromJSON**(`styleSetting`): `void`

使用 JSON 对象初始化一个 TaskbarStyleRule 实例。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `styleSetting` | `any` | 用于初始化的 JSON 配置对象。 |

#### Returns

`void`

___

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

如果任务匹配并将显示此规则的任务条，则为 true；否则为 false.

___

### <a id="tojson" name="tojson"></a> toJSON

▸ **toJSON**(): `any`

返回一个表示当前 TaskbarStyleRule 实例的 JSON 对象。

#### Returns

`any`

对应 TaskbarStyleRule 实例的 JSON 配置对象。
