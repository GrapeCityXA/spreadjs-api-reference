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

创建甘特表的映射

**`classdesc`** 表示甘特表的映射，用于转换和转换回任务值。

## Methods

### <a id="formatboolean" name="formatboolean"></a> formatBoolean

▸ **formatBoolean**(`value`): `string`

一个辅助函数，用于将布尔值格式化为字符串。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `boolean` | 要格式化的布尔值。 |

#### Returns

`string`

___

### <a id="formatdate" name="formatdate"></a> formatDate

▸ **formatDate**(`value`, `format?`, `culture?`): `string`

一个辅助函数，用于将日期值格式化为字符串。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `Date` | 要格式化的日期值。 |
| `format?` | `string` | 可选。一个字符串值，表示日期值的格式字符串。 |
| `culture?` | `string` | 可选。一个字符串值，表示用于格式化日期的区域设置。 |

#### Returns

`string`

___

### <a id="formatduration" name="formatduration"></a> formatDuration

▸ **formatDuration**(`value`): `string`

一个辅助函数，用于将 {@link GC.Spread.Sheets.GanttSheet.Duration} 值格式化为字符串。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | [`Duration`](../modules/GC.Spread.Sheets.GanttSheet.md#duration) | 要格式化的持续时间值。 |

#### Returns

`string`

___

### <a id="formatint" name="formatint"></a> formatInt

▸ **formatInt**(`value`): `string`

一个辅助函数，用于将数字值格式化为字符串。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `number` | 要格式化的数字值。 |

#### Returns

`string`

___

### <a id="formatmode" name="formatmode"></a> formatMode

▸ **formatMode**(`value`): `string`

一个辅助函数，用于将 {@link GC.Spread.Sheets.GanttSheet.TaskScheduleMode} 值格式化为字符串。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | [`TaskScheduleMode`](../modules/GC.Spread.Sheets.GanttSheet.md#taskschedulemode) | 要格式化的值。 |

#### Returns

`string`

___

### <a id="parseboolean" name="parseboolean"></a> parseBoolean

▸ **parseBoolean**(`value`): `boolean`

一个辅助函数，用于将字符串或其他类型的原始值解析为布尔值。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 要解析的原始值。 |

#### Returns

`boolean`

___

### <a id="parsedate" name="parsedate"></a> parseDate

▸ **parseDate**(`value`, `format?`, `culture?`): `Date`

一个辅助函数，用于将字符串或其他类型的原始值解析为日期值。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 要解析的原始值。 |
| `format?` | `string` | 可选。一个字符串值，表示日期值的格式字符串。 |
| `culture?` | `string` | 可选。一个字符串值，表示用于解析日期的区域设置。 |

#### Returns

`Date`

___

### <a id="parseduration" name="parseduration"></a> parseDuration

▸ **parseDuration**(`value`): [`Duration`](../modules/GC.Spread.Sheets.GanttSheet.md#duration)

一个辅助函数，用于将字符串或其他类型的原始值解析为 {@link GC.Spread.Sheets.GanttSheet.Duration} 值。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 要解析的原始值。 |

#### Returns

[`Duration`](../modules/GC.Spread.Sheets.GanttSheet.md#duration)

___

### <a id="parseint" name="parseint"></a> parseInt

▸ **parseInt**(`value`): `number`

一个辅助函数，用于将字符串或其他类型的原始值解析为整数值。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 要解析的原始值。 |

#### Returns

`number`

___

### <a id="parsemode" name="parsemode"></a> parseMode

▸ **parseMode**(`value`): [`TaskScheduleMode`](../modules/GC.Spread.Sheets.GanttSheet.md#taskschedulemode)

一个辅助函数，用于将字符串或其他类型的原始值解析为 {@link GC.Spread.Sheets.GanttSheet.TaskScheduleMode} 值。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 要解析的原始值。 |

#### Returns

[`TaskScheduleMode`](../modules/GC.Spread.Sheets.GanttSheet.md#taskschedulemode)
