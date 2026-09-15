# Class: WinlossSparkline

[Sheets](../modules/GC.Spread.Sheets.md).[Sparklines](../modules/GC.Spread.Sheets.Sparklines.md).WinlossSparkline

## Hierarchy

- [`SparklineEx`](GC.Spread.Sheets.Sparklines.SparklineEx.md)

  ↳ **`WinlossSparkline`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Sparklines.WinlossSparkline.md#constructor)

### Properties

- [typeName](GC.Spread.Sheets.Sparklines.WinlossSparkline.md#typename)

### Methods

- [createFunction](GC.Spread.Sheets.Sparklines.WinlossSparkline.md#createfunction)
- [fromJSON](GC.Spread.Sheets.Sparklines.WinlossSparkline.md#fromjson)
- [name](GC.Spread.Sheets.Sparklines.WinlossSparkline.md#name)
- [paint](GC.Spread.Sheets.Sparklines.WinlossSparkline.md#paint)
- [toJSON](GC.Spread.Sheets.Sparklines.WinlossSparkline.md#tojson)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new WinlossSparkline**()

表示盈亏迷你图的类。

#### Overrides

[SparklineEx](GC.Spread.Sheets.Sparklines.SparklineEx.md).[constructor](GC.Spread.Sheets.Sparklines.SparklineEx.md#constructor)

## Properties

### <a id="typename" name="typename"></a> typeName

• **typeName**: `string`

表示用于支持序列化的类型名称字符串。

#### Inherited from

[SparklineEx](GC.Spread.Sheets.Sparklines.SparklineEx.md).[typeName](GC.Spread.Sheets.Sparklines.SparklineEx.md#typename)

## Methods

### <a id="createfunction" name="createfunction"></a> createFunction

▸ **createFunction**(): [`Function`](GC.Spread.CalcEngine.Functions.Function.md)

创建一个自定义函数，用于为SparklineEx提供数据和设置。

#### Returns

[`Function`](GC.Spread.CalcEngine.Functions.Function.md)

创建的自定义函数。

#### Inherited from

[SparklineEx](GC.Spread.Sheets.Sparklines.SparklineEx.md).[createFunction](GC.Spread.Sheets.Sparklines.SparklineEx.md#createfunction)

___

### <a id="fromjson" name="fromjson"></a> fromJSON

▸ **fromJSON**(`settings`): `void`

从指定的JSON字符串加载对象状态。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `settings` | `Object` | 来自反序列化的sparklineEx数据。 |

#### Returns

`void`

#### Inherited from

[SparklineEx](GC.Spread.Sheets.Sparklines.SparklineEx.md).[fromJSON](GC.Spread.Sheets.Sparklines.SparklineEx.md#fromjson)

___

### <a id="name" name="name"></a> name

▸ **name**(): `string`

获取SparklineEx的名称。

#### Returns

`string`

SparklineEx的名称。

#### Inherited from

[SparklineEx](GC.Spread.Sheets.Sparklines.SparklineEx.md).[name](GC.Spread.Sheets.Sparklines.SparklineEx.md#name)

___

### <a id="paint" name="paint"></a> paint

▸ **paint**(`context`, `value`, `x`, `y`, `width`, `height`): `void`

在画布上绘制SparklineEx。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context` | `CanvasRenderingContext2D` | 画布的二维上下文。 |
| `value` | `any` | 由自定义函数计算的值。 |
| `x` | `number` | 相对于画布的<i>x</i>坐标。 |
| `y` | `number` | 相对于画布的<i>y</i>坐标。 |
| `width` | `number` | 单元格的宽度。 |
| `height` | `number` | 单元格的高度。 |

#### Returns

`void`

#### Inherited from

[SparklineEx](GC.Spread.Sheets.Sparklines.SparklineEx.md).[paint](GC.Spread.Sheets.Sparklines.SparklineEx.md#paint)

___

### <a id="tojson" name="tojson"></a> toJSON

▸ **toJSON**(): `Object`

将对象状态保存为JSON字符串。

#### Returns

`Object`

sparklineEx数据。

#### Inherited from

[SparklineEx](GC.Spread.Sheets.Sparklines.SparklineEx.md).[toJSON](GC.Spread.Sheets.Sparklines.SparklineEx.md#tojson)
