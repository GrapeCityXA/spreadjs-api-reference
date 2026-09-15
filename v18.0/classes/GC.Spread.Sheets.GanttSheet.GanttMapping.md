# Class: GanttMapping

[Sheets](../modules/GC.Spread.Sheets.md).[GanttSheet](../modules/GC.Spread.Sheets.GanttSheet.md).GanttMapping

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.GanttSheet.GanttMapping.md#constructor)

### Methods

- [formatBoolean](GC.Spread.Sheets.GanttSheet.GanttMapping.md#formatboolean)
- [formatDate](GC.Spread.Sheets.GanttSheet.GanttMapping.md#formatdate)
- [formatDuration](GC.Spread.Sheets.GanttSheet.GanttMapping.md#formatduration)
- [formatInt](GC.Spread.Sheets.GanttSheet.GanttMapping.md#formatint)
- [formatMode](GC.Spread.Sheets.GanttSheet.GanttMapping.md#formatmode)
- [parseBoolean](GC.Spread.Sheets.GanttSheet.GanttMapping.md#parseboolean)
- [parseDate](GC.Spread.Sheets.GanttSheet.GanttMapping.md#parsedate)
- [parseDuration](GC.Spread.Sheets.GanttSheet.GanttMapping.md#parseduration)
- [parseInt](GC.Spread.Sheets.GanttSheet.GanttMapping.md#parseint)
- [parseMode](GC.Spread.Sheets.GanttSheet.GanttMapping.md#parsemode)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new GanttMapping**()

为ganttsheet创建映射

**`classdesc`** 表示ganttsheet的映射以转换并转换任务值

## Methods

### <a id="formatboolean" name="formatboolean"></a> formatBoolean

▸ **formatBoolean**(`value`): `string`

辅助函数，将布尔值格式为字符串

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `boolean` | 格式化的布尔值 |

#### Returns

`string`

___

### <a id="formatdate" name="formatdate"></a> formatDate

▸ **formatDate**(`value`, `format?`, `culture?`): `string`

辅助函数，将格式为字符串的日期值

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `Date` | 格式化的日期值 |
| `format?` | `string` | - |
| `culture?` | `string` | - |

#### Returns

`string`

___

### <a id="formatduration" name="formatduration"></a> formatDuration

▸ **formatDuration**(`value`): `string`

辅助功能将格式化 [GC.Spread.Sheets.GanttSheet.Duration](../modules/GC.Spread.Sheets.GanttSheet.md#duration) 值为字符串.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | [`Duration`](../modules/GC.Spread.Sheets.GanttSheet.md#duration) | 格式的持续时间值 |

#### Returns

`string`

___

### <a id="formatint" name="formatint"></a> formatInt

▸ **formatInt**(`value`): `string`

辅助函数，将格式为字符串的数值值

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `number` | 格式化的数字值 |

#### Returns

`string`

___

### <a id="formatmode" name="formatmode"></a> formatMode

▸ **formatMode**(`value`): `string`

辅助功能将格式化 [GC.Spread.Sheets.GanttSheet.TaskScheduleMode](../modules/GC.Spread.Sheets.GanttSheet.md#taskschedulemode) 值为字符串

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | [`TaskScheduleMode`](../modules/GC.Spread.Sheets.GanttSheet.md#taskschedulemode) | 格式的值 |

#### Returns

`string`

___

### <a id="parseboolean" name="parseboolean"></a> parseBoolean

▸ **parseBoolean**(`value`): `boolean`

辅助功能，将字符串或其他类型的原始值解析为布尔值

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 解析的原始值 |

#### Returns

`boolean`

___

### <a id="parsedate" name="parsedate"></a> parseDate

▸ **parseDate**(`value`, `format?`, `culture?`): `Date`

辅助功能，将字符串或其他类型的原始值分析为日期值

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 解析的原始值 |
| `format?` | `string` | - |
| `culture?` | `string` | - |

#### Returns

`Date`

___

### <a id="parseduration" name="parseduration"></a> parseDuration

▸ **parseDuration**(`value`): [`Duration`](../modules/GC.Spread.Sheets.GanttSheet.md#duration)

辅助功能，将字符串或其他类型的原始值分析为 [GC.Spread.Sheets.GanttSheet.Duration](../modules/GC.Spread.Sheets.GanttSheet.md#duration) 值

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 解析的原始值 |

#### Returns

[`Duration`](../modules/GC.Spread.Sheets.GanttSheet.md#duration)

___

### <a id="parseint" name="parseint"></a> parseInt

▸ **parseInt**(`value`): `number`

辅助功能，将字符串或其他类型的原始值解析为整数值

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 原始值 |

#### Returns

`number`

___

### <a id="parsemode" name="parsemode"></a> parseMode

▸ **parseMode**(`value`): [`TaskScheduleMode`](../modules/GC.Spread.Sheets.GanttSheet.md#taskschedulemode)

辅助功能，将字符串或其他类型的原始值分析为 [GC.Spread.Sheets.GanttSheet.TaskScheduleMode](../modules/GC.Spread.Sheets.GanttSheet.md#taskschedulemode) 值

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 解析的原始值 |

#### Returns

[`TaskScheduleMode`](../modules/GC.Spread.Sheets.GanttSheet.md#taskschedulemode)
