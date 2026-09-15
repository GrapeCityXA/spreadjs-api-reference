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

A number value or a formula string (starts with =) will get a number value

___

### <a id="connectionpoints" name="connectionpoints"></a> connectionPoints

• `Optional` **connectionPoints**: [`IPointInfo`](GC.Spread.Sheets.Shapes.IPointInfo.md)[]

___

### <a id="controls" name="controls"></a> controls

• `Optional` **controls**: [`IControlInfo`](GC.Spread.Sheets.Shapes.IControlInfo.md)[]

___

### <a id="height" name="height"></a> height

• `Optional` **height**: `string` \| `number`

A number value or a formula string (starts with =) will get a number value

___

### <a id="id" name="id"></a> id

• `Optional` **id**: `string`

___

### <a id="left" name="left"></a> left

• `Optional` **left**: `string` \| `number`

A number value or a formula string (starts with =) will get a number value

___

### <a id="options" name="options"></a> options

• `Optional` **options**: [`IShapeOptions`](GC.Spread.Sheets.Shapes.IShapeOptions.md)

___

### <a id="path" name="path"></a> path

• **path**: `string`[][]

___

### <a id="textrect" name="textrect"></a> textRect

• `Optional` **textRect**: `Object`

specify the rectangle for shape text

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

A number value or a formula string (starts with =) will get a number value

___

### <a id="variables" name="variables"></a> variables

• `Optional` **variables**: `Object`

a key-value pairs object, value can be a number or formula string (starts with =), can be referred by variables[key] in formula

___

### <a id="width" name="width"></a> width

• `Optional` **width**: `string` \| `number`

A number value or a formula string (starts with =) will get a number value
