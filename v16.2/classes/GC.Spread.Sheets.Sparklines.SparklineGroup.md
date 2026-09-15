# Class: SparklineGroup

[Sheets](../modules/GC.Spread.Sheets.md).[Sparklines](../modules/GC.Spread.Sheets.Sparklines.md).SparklineGroup

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Sparklines.SparklineGroup.md#constructor)

### Properties

- [setting](GC.Spread.Sheets.Sparklines.SparklineGroup.md#setting)
- [sparklineType](GC.Spread.Sheets.Sparklines.SparklineGroup.md#sparklinetype)

### Methods

- [add](GC.Spread.Sheets.Sparklines.SparklineGroup.md#add)
- [clone](GC.Spread.Sheets.Sparklines.SparklineGroup.md#clone)
- [contains](GC.Spread.Sheets.Sparklines.SparklineGroup.md#contains)
- [count](GC.Spread.Sheets.Sparklines.SparklineGroup.md#count)
- [dateAxisData](GC.Spread.Sheets.Sparklines.SparklineGroup.md#dateaxisdata)
- [dateAxisOrientation](GC.Spread.Sheets.Sparklines.SparklineGroup.md#dateaxisorientation)
- [remove](GC.Spread.Sheets.Sparklines.SparklineGroup.md#remove)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new SparklineGroup**(`type`, `setting`)

迷你图组

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | [`SparklineType`](../enums/GC.Spread.Sheets.Sparklines.SparklineType.md) | 迷你图的类型 |
| `setting` | [`SparklineSetting`](GC.Spread.Sheets.Sparklines.SparklineSetting.md) | 迷你图组的设置 |

## Properties

### <a id="setting" name="setting"></a> setting

• **setting**: [`SparklineSetting`](GC.Spread.Sheets.Sparklines.SparklineSetting.md)

迷你图设置

___

### <a id="sparklinetype" name="sparklinetype"></a> sparklineType

• **sparklineType**: [`SparklineType`](../enums/GC.Spread.Sheets.Sparklines.SparklineType.md)

迷你图类型

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`item`): `void`

将迷你图添加到组中

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | [`Sparkline`](GC.Spread.Sheets.Sparklines.Sparkline.md) | 迷你图项 |

#### Returns

`void`

___

### <a id="clone" name="clone"></a> clone

▸ **clone**(): [`SparklineGroup`](GC.Spread.Sheets.Sparklines.SparklineGroup.md)

克隆当前的迷你图组

#### Returns

[`SparklineGroup`](GC.Spread.Sheets.Sparklines.SparklineGroup.md)

克隆的迷你图组

___

### <a id="contains" name="contains"></a> contains

▸ **contains**(`item`): `boolean`

确定该组是否包含特定值

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | [`Sparkline`](GC.Spread.Sheets.Sparklines.Sparkline.md) | 要在组中定位的对象 |

#### Returns

`boolean`

如果在组中找到该项,返回true;否则为false

___

### <a id="count" name="count"></a> count

▸ **count**(): `number`

迷你图组内部列表的计数

#### Returns

`number`

组中的迷你图数量

___

### <a id="dateaxisdata" name="dateaxisdata"></a> dateAxisData

▸ **dateAxisData**(`value?`): `any`

日期轴数据

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`Range`](GC.Spread.Sheets.Range.md) | 日期轴数据 |

#### Returns

`any`

如果未设置任何值,则返回日期轴数据 否则,返回undefined

___

### <a id="dateaxisorientation" name="dateaxisorientation"></a> dateAxisOrientation

▸ **dateAxisOrientation**(`value`): `any`

日期轴方向

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | [`DataOrientation`](../enums/GC.Spread.Sheets.Sparklines.DataOrientation.md) | 日期轴方向 |

#### Returns

`any`

如果未设置任何值,则返回日期轴方向;否则,返回未定义

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`item`): [`Sparkline`](GC.Spread.Sheets.Sparklines.Sparkline.md)[]

从组中删除第一次出现的特定对象

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | [`Sparkline`](GC.Spread.Sheets.Sparklines.Sparkline.md) | 迷你图项 |

#### Returns

[`Sparkline`](GC.Spread.Sheets.Sparklines.Sparkline.md)[]

The GC.Spread.Sheets.Sparklines.Sparkline 数组
