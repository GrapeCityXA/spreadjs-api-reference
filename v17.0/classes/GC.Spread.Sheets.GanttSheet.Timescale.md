# Class: Timescale

[Sheets](../modules/GC.Spread.Sheets.md).[GanttSheet](../modules/GC.Spread.Sheets.GanttSheet.md).Timescale

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.GanttSheet.Timescale.md#constructor)

### Properties

- [bottomTier](GC.Spread.Sheets.GanttSheet.Timescale.md#bottomtier)
- [currentDate](GC.Spread.Sheets.GanttSheet.Timescale.md#currentdate)
- [maxDate](GC.Spread.Sheets.GanttSheet.Timescale.md#maxdate)
- [middleTier](GC.Spread.Sheets.GanttSheet.Timescale.md#middletier)
- [minDate](GC.Spread.Sheets.GanttSheet.Timescale.md#mindate)
- [nonWorkingTime](GC.Spread.Sheets.GanttSheet.Timescale.md#nonworkingtime)
- [showScaleSeparator](GC.Spread.Sheets.GanttSheet.Timescale.md#showscaleseparator)
- [tierMode](GC.Spread.Sheets.GanttSheet.Timescale.md#tiermode)
- [timescaleBottomTierTextStyle](GC.Spread.Sheets.GanttSheet.Timescale.md#timescalebottomtiertextstyle)
- [timescaleMiddleTierTextStyle](GC.Spread.Sheets.GanttSheet.Timescale.md#timescalemiddletiertextstyle)
- [timescaleTopTierTextStyle](GC.Spread.Sheets.GanttSheet.Timescale.md#timescaletoptiertextstyle)
- [topTier](GC.Spread.Sheets.GanttSheet.Timescale.md#toptier)
- [zoomFactor](GC.Spread.Sheets.GanttSheet.Timescale.md#zoomfactor)

### Methods

- [scroll](GC.Spread.Sheets.GanttSheet.Timescale.md#scroll)
- [scrollBy](GC.Spread.Sheets.GanttSheet.Timescale.md#scrollby)
- [scrollOneTick](GC.Spread.Sheets.GanttSheet.Timescale.md#scrollonetick)
- [scrollTo](GC.Spread.Sheets.GanttSheet.Timescale.md#scrollto)
- [zoomAuto](GC.Spread.Sheets.GanttSheet.Timescale.md#zoomauto)
- [zoomIn](GC.Spread.Sheets.GanttSheet.Timescale.md#zoomin)
- [zoomOut](GC.Spread.Sheets.GanttSheet.Timescale.md#zoomout)
- [zoomTo](GC.Spread.Sheets.GanttSheet.Timescale.md#zoomto)
- [zoomToRange](GC.Spread.Sheets.GanttSheet.Timescale.md#zoomtorange)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Timescale**()

为项目创建一个时间尺度。内部仅使用

**`classdesc`** 代表Ganttchart的时间尺度

## Properties

### <a id="bottomtier" name="bottomtier"></a> bottomTier

• **bottomTier**: [`TimescaleTier`](GC.Spread.Sheets.GanttSheet.TimescaleTier.md)

获取时间尺度的底层

**`readonly`**

___

### <a id="currentdate" name="currentdate"></a> currentDate

• **currentDate**: `Date`

获取时间尺度的当前日期。要更改它，请调用时间尺度的滚动功能

**`readonly`**

___

### <a id="maxdate" name="maxdate"></a> maxDate

• **maxDate**: `Date`

获取或设置时间尺度可滚动区域的最大日期。默认值为2030-1-1

___

### <a id="middletier" name="middletier"></a> middleTier

• **middleTier**: [`TimescaleTier`](GC.Spread.Sheets.GanttSheet.TimescaleTier.md)

获取时间尺度的中层

**`readonly`**

___

### <a id="mindate" name="mindate"></a> minDate

• **minDate**: `Date`

获取或设置时间尺度可滚动区域的最低日期。默认值为2020-1-1

___

### <a id="nonworkingtime" name="nonworkingtime"></a> nonWorkingTime

• **nonWorkingTime**: [`NonWorkingTimeStyle`](GC.Spread.Sheets.GanttSheet.NonWorkingTimeStyle.md)

获取时间尺度的非工作时间区域

**`readonly`**

___

### <a id="showscaleseparator" name="showscaleseparator"></a> showScaleSeparator

• **showScaleSeparator**: `boolean`

获取或设置一个布尔值，该值指示是否显示顶级和中层之间的比例分离线

___

### <a id="tiermode" name="tiermode"></a> tierMode

• **tierMode**: [`TimescaleTierMode`](../enums/GC.Spread.Sheets.GanttSheet.TimescaleTierMode.md)

获取或设置时间尺度的层模式

___

### <a id="timescalebottomtiertextstyle" name="timescalebottomtiertextstyle"></a> timescaleBottomTierTextStyle

• **timescaleBottomTierTextStyle**: [`TextStyle`](../modules/GC.Spread.Sheets.GanttSheet.md#textstyle)

获取或设置时间尺度底部标签的文本样式

___

### <a id="timescalemiddletiertextstyle" name="timescalemiddletiertextstyle"></a> timescaleMiddleTierTextStyle

• **timescaleMiddleTierTextStyle**: [`TextStyle`](../modules/GC.Spread.Sheets.GanttSheet.md#textstyle)

获取或设置时间尺度中间标签的文本样式

___

### <a id="timescaletoptiertextstyle" name="timescaletoptiertextstyle"></a> timescaleTopTierTextStyle

• **timescaleTopTierTextStyle**: [`TextStyle`](../modules/GC.Spread.Sheets.GanttSheet.md#textstyle)

获取或设置时间尺度顶部标签的文本样式

___

### <a id="toptier" name="toptier"></a> topTier

• **topTier**: [`TimescaleTier`](GC.Spread.Sheets.GanttSheet.TimescaleTier.md)

获得时间尺度的顶层

**`readonly`**

___

### <a id="zoomfactor" name="zoomfactor"></a> zoomFactor

• **zoomFactor**: `number`

获取一个指示时间尺度的缩放因子的数值。要更改它，请调用时间表的缩放功能

**`readonly`**

## Methods

### <a id="scroll" name="scroll"></a> scroll

▸ **scroll**(`pixels`): `void`

滚动以像素为单位。注意时间尺度将滚动到最近的刻度

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pixels` | `number` | 指示滚动的像素。正数表示向前滚动，负数表示向后滚动 |

#### Returns

`void`

___

### <a id="scrollby" name="scrollby"></a> scrollBy

▸ **scrollBy**(`count`, `unit`): `void`

按指定的单位计数滚动时间尺度。注意时间尺度将滚动到最近的刻度

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `count` | `number` | 指示指定单元滚动的时间。正数表示向前滚动，负数表示向后滚动 |
| `unit` | [`TimescaleUnit`](../enums/GC.Spread.Sheets.GanttSheet.TimescaleUnit.md) | 指示计数值的单位 |

#### Returns

`void`

___

### <a id="scrollonetick" name="scrollonetick"></a> scrollOneTick

▸ **scrollOneTick**(`forward`): `void`

滚动时间尺度一个刻度单位

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `forward` | `boolean` | 布尔值表示向前滚动或向后滚动 |

#### Returns

`void`

___

### <a id="scrollto" name="scrollto"></a> scrollTo

▸ **scrollTo**(`date`, `percentOfViewport?`): `void`

将时间时间尺度滚动到指定的日期。注意时间表将滚动到最近的刻度

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `date` | `Date` | 日期值表示滚动目标 |
| `percentOfViewport?` | `number` | - |

#### Returns

`void`

___

### <a id="zoomauto" name="zoomauto"></a> zoomAuto

▸ **zoomAuto**(): `void`

根据每个层上的刻度标签，将时间尺度放大到合适的因子

#### Returns

`void`

___

### <a id="zoomin" name="zoomin"></a> zoomIn

▸ **zoomIn**(`adjustTierUnit?`): `void`

放大时间尺度到一个新的级别

#### Parameters

| Name | Type |
| :------ | :------ |
| `adjustTierUnit?` | `boolean` |

#### Returns

`void`

___

### <a id="zoomout" name="zoomout"></a> zoomOut

▸ **zoomOut**(`adjustTierUnit?`): `void`

将时间表放大到一个新的水平

#### Parameters

| Name | Type |
| :------ | :------ |
| `adjustTierUnit?` | `boolean` |

#### Returns

`void`

___

### <a id="zoomto" name="zoomto"></a> zoomTo

▸ **zoomTo**(`zoomFactor`, `adjustTierUnit?`): `void`

将时间尺度放大到指定因素

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `zoomFactor` | `number` | 一个数值表示目标变焦因子 |
| `adjustTierUnit?` | `boolean` | - |

#### Returns

`void`

___

### <a id="zoomtorange" name="zoomtorange"></a> zoomToRange

▸ **zoomToRange**(`start`, `end`, `adjustTierUnit?`): `void`

缩放时间尺度以显示视口中的目标日期范围。注意时间尺度将调整为最近的壁虱

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `start` | `Date` | 日期值表示要显示的数据范围的开始 |
| `end` | `Date` | 日期值表示要显示的数据范围的结束 |
| `adjustTierUnit?` | `boolean` | - |

#### Returns

`void`
