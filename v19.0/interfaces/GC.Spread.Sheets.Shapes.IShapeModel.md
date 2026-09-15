# Interface: IShapeModel

[Sheets](../modules/GC.Spread.Sheets.md).[Shapes](../modules/GC.Spread.Sheets.Shapes.md).IShapeModel

## Table of contents

### Properties

- [angle](GC.Spread.Sheets.Shapes.IShapeModel.md#angle)
- [connectionPoints](GC.Spread.Sheets.Shapes.IShapeModel.md#connectionpoints)
- [controls](GC.Spread.Sheets.Shapes.IShapeModel.md#controls)
- [height](GC.Spread.Sheets.Shapes.IShapeModel.md#height)
- [id](GC.Spread.Sheets.Shapes.IShapeModel.md#id)
- [left](GC.Spread.Sheets.Shapes.IShapeModel.md#left)
- [options](GC.Spread.Sheets.Shapes.IShapeModel.md#options)
- [path](GC.Spread.Sheets.Shapes.IShapeModel.md#path)
- [textRect](GC.Spread.Sheets.Shapes.IShapeModel.md#textrect)
- [top](GC.Spread.Sheets.Shapes.IShapeModel.md#top)
- [variables](GC.Spread.Sheets.Shapes.IShapeModel.md#variables)
- [width](GC.Spread.Sheets.Shapes.IShapeModel.md#width)

## Properties

### <a id="angle" name="angle"></a> angle

• `Optional` **angle**: `string` \| `number`

数值或公式字符串（以 = 开头）将获取一个数值

___

### <a id="connectionpoints" name="connectionpoints"></a> connectionPoints

• `Optional` **connectionPoints**: [`IPointInfo`](GC.Spread.Sheets.Shapes.IPointInfo.md)[]

___

### <a id="controls" name="controls"></a> controls

• `Optional` **controls**: [`IControlInfo`](GC.Spread.Sheets.Shapes.IControlInfo.md)[]

___

### <a id="height" name="height"></a> height

• `Optional` **height**: `string` \| `number`

数值或公式字符串（以 = 开头）将获取一个数值

___

### <a id="id" name="id"></a> id

• `Optional` **id**: `string`

___

### <a id="left" name="left"></a> left

• `Optional` **left**: `string` \| `number`

数值或公式字符串（以 = 开头）将获取一个数值

___

### <a id="options" name="options"></a> options

• `Optional` **options**: [`IShapeOptions`](GC.Spread.Sheets.Shapes.IShapeOptions.md)

___

### <a id="path" name="path"></a> path

• **path**: `string`[][]

___

### <a id="textrect" name="textrect"></a> textRect

• `Optional` **textRect**: `Object`

指定形状文本的矩形区域

#### Type declaration

| Name | Type |
| :------ | :------ |
| `bottom` | `number` |
| `left` | `number` |
| `right` | `number` |
| `top` | `number` |

___

### <a id="top" name="top"></a> top

• `Optional` **top**: `string` \| `number`

数值或公式字符串（以 = 开头）将获取一个数值

___

### <a id="variables" name="variables"></a> variables

• `Optional` **variables**: `Object`

键值对对象，值可以是数值或公式字符串（以 = 开头），可以在公式中通过 variables[key] 引用

___

### <a id="width" name="width"></a> width

• `Optional` **width**: `string` \| `number`

数值或公式字符串（以 = 开头）将获取一个数值
