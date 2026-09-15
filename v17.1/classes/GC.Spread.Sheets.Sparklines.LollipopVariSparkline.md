# Class: LollipopVariSparkline

[Sheets](../modules/GC.Spread.Sheets.md).[Sparklines](../modules/GC.Spread.Sheets.Sparklines.md).LollipopVariSparkline

## Hierarchy

- [`SparklineEx`](GC.Spread.Sheets.Sparklines.SparklineEx.md)

  ↳ **`LollipopVariSparkline`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Sparklines.LollipopVariSparkline.md#constructor)

### Properties

- [typeName](GC.Spread.Sheets.Sparklines.LollipopVariSparkline.md#typename)

### Methods

- [createFunction](GC.Spread.Sheets.Sparklines.LollipopVariSparkline.md#createfunction)
- [fromJSON](GC.Spread.Sheets.Sparklines.LollipopVariSparkline.md#fromjson)
- [name](GC.Spread.Sheets.Sparklines.LollipopVariSparkline.md#name)
- [paint](GC.Spread.Sheets.Sparklines.LollipopVariSparkline.md#paint)
- [toJSON](GC.Spread.Sheets.Sparklines.LollipopVariSparkline.md#tojson)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new LollipopVariSparkline**()

棒棒糖迷你图类

#### Overrides

[SparklineEx](GC.Spread.Sheets.Sparklines.SparklineEx.md).[constructor](GC.Spread.Sheets.Sparklines.SparklineEx.md#constructor)

## Properties

### <a id="typename" name="typename"></a> typeName

• **typeName**: `string`

表示用于支撑序列化的类型名称字符串

#### Inherited from

[SparklineEx](GC.Spread.Sheets.Sparklines.SparklineEx.md).[typeName](GC.Spread.Sheets.Sparklines.SparklineEx.md#typename)

## Methods

### <a id="createfunction" name="createfunction"></a> createFunction

▸ **createFunction**(): [`Function`](GC.Spread.CalcEngine.Functions.Function.md)

创建一个自定义功能，用于为SparklineEx提供数据和设置

#### Returns

[`Function`](GC.Spread.CalcEngine.Functions.Function.md)

创建的自定义功能

#### Inherited from

[SparklineEx](GC.Spread.Sheets.Sparklines.SparklineEx.md).[createFunction](GC.Spread.Sheets.Sparklines.SparklineEx.md#createfunction)

___

### <a id="fromjson" name="fromjson"></a> fromJSON

▸ **fromJSON**(`settings`): `void`

从指定的JSON字符串加载对象状态

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `settings` | `Object` | 反序列化后的设置 |

#### Returns

`void`

#### Inherited from

[SparklineEx](GC.Spread.Sheets.Sparklines.SparklineEx.md).[fromJSON](GC.Spread.Sheets.Sparklines.SparklineEx.md#fromjson)

___

### <a id="name" name="name"></a> name

▸ **name**(): `string`

迷你图名称

#### Returns

`string`

迷你图名称

#### Inherited from

[SparklineEx](GC.Spread.Sheets.Sparklines.SparklineEx.md).[name](GC.Spread.Sheets.Sparklines.SparklineEx.md#name)

___

### <a id="paint" name="paint"></a> paint

▸ **paint**(`context`, `value`, `x`, `y`, `width`, `height`): `void`

在画布上绘制迷你图

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context` | `CanvasRenderingContext2D` | 画布上下文 |
| `value` | `any` | 值 |
| `x` | `number` | <i>x</i>-相对于画布的坐标 |
| `y` | `number` | <i>y</i>-相对于画布的坐标 |
| `width` | `number` | 单元格宽度 |
| `height` | `number` | 单元格高度 |

#### Returns

`void`

#### Inherited from

[SparklineEx](GC.Spread.Sheets.Sparklines.SparklineEx.md).[paint](GC.Spread.Sheets.Sparklines.SparklineEx.md#paint)

___

### <a id="tojson" name="tojson"></a> toJSON

▸ **toJSON**(): `Object`

保存为 JSON

#### Returns

`Object`

迷你图数据

#### Inherited from

[SparklineEx](GC.Spread.Sheets.Sparklines.SparklineEx.md).[toJSON](GC.Spread.Sheets.Sparklines.SparklineEx.md#tojson)
