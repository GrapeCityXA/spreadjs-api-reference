# Class: Rect

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).Rect

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Rect.md#constructor)

### Properties

- [height](GC.Spread.Sheets.Rect.md#height)
- [width](GC.Spread.Sheets.Rect.md#width)
- [x](GC.Spread.Sheets.Rect.md#x)
- [y](GC.Spread.Sheets.Rect.md#y)

### Methods

- [contains](GC.Spread.Sheets.Rect.md#contains)
- [getIntersectRect](GC.Spread.Sheets.Rect.md#getintersectrect)
- [intersect](GC.Spread.Sheets.Rect.md#intersect)
- [intersectRect](GC.Spread.Sheets.Rect.md#intersectrect)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Rect**(`x`, `y`, `w`, `h`)

具有特殊位置的矩形及其在二维空间中的宽度和高度

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | 矩形左上角的坐标<i>x</i> |
| `y` | `number` | 矩形左上角的坐标<i>y</i> |
| `w` | `number` | 矩形的宽度 |
| `h` | `number` | 矩形的高度 |

## Properties

### <a id="height" name="height"></a> height

• **height**: `number`

矩形的宽度

___

### <a id="width" name="width"></a> width

• **width**: `number`

矩形的高度

___

### <a id="x" name="x"></a> x

• **x**: `number`

矩形左上角的坐标<i>x</i>

___

### <a id="y" name="y"></a> y

• **y**: `number`

矩形左上角的坐标<i>y</i>

## Methods

### <a id="contains" name="contains"></a> contains

▸ **contains**(`x`, `y`): `boolean`

矩形是否包含指定的<i>x</i>坐标和<i>y</i>坐标

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | 要检查点的坐标<i>x</i> |
| `y` | `number` | 要检查点的坐标<i>y</i> |

#### Returns

`boolean`

若为`true`,则(x, y)包含在矩形中;若为`false`则不包含

___

### <a id="getintersectrect" name="getintersectrect"></a> getIntersectRect

▸ **getIntersectRect**(`x`, `y`, `width`, `height`): [`Rect`](GC.Spread.Sheets.Rect.md)

获取与当前矩形相交的矩形

#### Parameters

| Name | Type |
| :------ | :------ |
| `x` | `number` |
| `y` | `number` |
| `width` | `number` |
| `height` | `number` |

#### Returns

[`Rect`](GC.Spread.Sheets.Rect.md)

相交的矩形如果两个矩形不相交,则返回null

___

### <a id="intersect" name="intersect"></a> intersect

▸ **intersect**(`x`, `y`, `width`, `height`): `boolean`

指定的矩形是否与当前矩形相交

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | 矩形左上角的坐标<i>x</i> |
| `y` | `number` | 矩形左上角的坐标<i>y</i> |
| `width` | `number` | - |
| `height` | `number` | - |

#### Returns

`boolean`

若为`true`,指定的矩形与当前矩形相交;若为`false`则不相交

___

### <a id="intersectrect" name="intersectrect"></a> intersectRect

▸ **intersectRect**(`rect`): `boolean`

指定的矩形是否与当前矩形相交

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rect` | [`Rect`](GC.Spread.Sheets.Rect.md) | 指定的矩形 |

#### Returns

`boolean`

若为`true`,指定的矩形与当前矩形相交;若为`false`则不相交
