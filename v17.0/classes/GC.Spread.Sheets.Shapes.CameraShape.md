# Class: CameraShape

[Sheets](../modules/GC.Spread.Sheets.md).[Shapes](../modules/GC.Spread.Sheets.Shapes.md).CameraShape

## Hierarchy

- [`ShapeBase`](GC.Spread.Sheets.Shapes.ShapeBase.md)

  ↳ **`CameraShape`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Shapes.CameraShape.md#constructor)

### Methods

- [allowMove](GC.Spread.Sheets.Shapes.CameraShape.md#allowmove)
- [allowResize](GC.Spread.Sheets.Shapes.CameraShape.md#allowresize)
- [allowRotate](GC.Spread.Sheets.Shapes.CameraShape.md#allowrotate)
- [alt](GC.Spread.Sheets.Shapes.CameraShape.md#alt)
- [canPrint](GC.Spread.Sheets.Shapes.CameraShape.md#canprint)
- [doubleClickCommand](GC.Spread.Sheets.Shapes.CameraShape.md#doubleclickcommand)
- [dynamicMove](GC.Spread.Sheets.Shapes.CameraShape.md#dynamicmove)
- [dynamicSize](GC.Spread.Sheets.Shapes.CameraShape.md#dynamicsize)
- [endColumn](GC.Spread.Sheets.Shapes.CameraShape.md#endcolumn)
- [endColumnOffset](GC.Spread.Sheets.Shapes.CameraShape.md#endcolumnoffset)
- [endRow](GC.Spread.Sheets.Shapes.CameraShape.md#endrow)
- [endRowOffset](GC.Spread.Sheets.Shapes.CameraShape.md#endrowoffset)
- [getFormula](GC.Spread.Sheets.Shapes.CameraShape.md#getformula)
- [height](GC.Spread.Sheets.Shapes.CameraShape.md#height)
- [hyperlink](GC.Spread.Sheets.Shapes.CameraShape.md#hyperlink)
- [isLocked](GC.Spread.Sheets.Shapes.CameraShape.md#islocked)
- [isSelected](GC.Spread.Sheets.Shapes.CameraShape.md#isselected)
- [isVisible](GC.Spread.Sheets.Shapes.CameraShape.md#isvisible)
- [name](GC.Spread.Sheets.Shapes.CameraShape.md#name)
- [range](GC.Spread.Sheets.Shapes.CameraShape.md#range)
- [rotate](GC.Spread.Sheets.Shapes.CameraShape.md#rotate)
- [setFormula](GC.Spread.Sheets.Shapes.CameraShape.md#setformula)
- [showHandle](GC.Spread.Sheets.Shapes.CameraShape.md#showhandle)
- [startColumn](GC.Spread.Sheets.Shapes.CameraShape.md#startcolumn)
- [startColumnOffset](GC.Spread.Sheets.Shapes.CameraShape.md#startcolumnoffset)
- [startRow](GC.Spread.Sheets.Shapes.CameraShape.md#startrow)
- [startRowOffset](GC.Spread.Sheets.Shapes.CameraShape.md#startrowoffset)
- [style](GC.Spread.Sheets.Shapes.CameraShape.md#style)
- [width](GC.Spread.Sheets.Shapes.CameraShape.md#width)
- [x](GC.Spread.Sheets.Shapes.CameraShape.md#x)
- [y](GC.Spread.Sheets.Shapes.CameraShape.md#y)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new CameraShape**(`worksheet`, `name`, `range`, `left?`, `top?`, `width?`, `height?`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `worksheet` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 形状的宿主表单 |
| `name` | `string` | 摄影机形状的名称.如果为空，将生成唯一名称 |
| `range` | `string` | 生成形状的区域，是一个区域公式，如Sheet1!A1:A8 |
| `left?` | `number` | 形状的<i>x</i>位置 |
| `top?` | `number` | 形状的<i>y</i>位置 |
| `width?` | `number` | 快照形状的宽度，如果留空，则默认值应与原始范围宽度相同 |
| `height?` | `number` | 快照形状的高度，如果留空，默认值应与原始范围高度相同 |

#### Overrides

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[constructor](GC.Spread.Sheets.Shapes.ShapeBase.md#constructor)

## Methods

### <a id="allowmove" name="allowmove"></a> allowMove

▸ **allowMove**(`value?`): `any`

获取或设置是否禁用移动形状

**`代码示例`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var state = heart.allowMove();
heart.allowMove(!state);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否禁用移动形状的设置 |

#### Returns

`any`

如果未设置任何值，则返回是否禁用移动形状的设置

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[allowMove](GC.Spread.Sheets.Shapes.ShapeBase.md#allowmove)

___

### <a id="allowresize" name="allowresize"></a> allowResize

▸ **allowResize**(`value?`): `any`

Gets or sets the resize mode of the shape.

**`代码示例`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var state = heart.allowResize();
heart.allowResize(GC.Spread.Sheets.Shapes.ResizeMode.aspect);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` \| [`ResizeMode`](../enums/GC.Spread.Sheets.Shapes.ResizeMode.md) | 是否禁用调整形状大小的设置 |

#### Returns

`any`

如果未设置任何值，则返回是否禁用调整形状大小的设置

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[allowResize](GC.Spread.Sheets.Shapes.ShapeBase.md#allowresize)

___

### <a id="allowrotate" name="allowrotate"></a> allowRotate

▸ **allowRotate**(`value?`): `any`

获取或设置是否禁用旋转形状

**`代码示例`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var state = heart.allowRotate();
heart.allowRotate(!state);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否禁用旋转形状的设置 |

#### Returns

`any`

如果未设置任何值，则返回是否禁用旋转形状的设置

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[allowRotate](GC.Spread.Sheets.Shapes.ShapeBase.md#allowrotate)

___

### <a id="alt" name="alt"></a> alt

▸ **alt**(`value?`): `any`

获取或设置形状的可选文本

**`example`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
heart.alt("A heart shape");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 形状的可选文本 |

#### Returns

`any`

形状的可选文本

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[alt](GC.Spread.Sheets.Shapes.ShapeBase.md#alt)

___

### <a id="canprint" name="canprint"></a> canPrint

▸ **canPrint**(`value?`): `any`

获取或设置此形状是否可打印

**`代码示例`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var state = heart.canPrint(); // Get whether the shape is printable, defaulat value is true.
workbook.print(); // The heart shape is printed.
heart.canPrint(false);
workbook.print(); // The heart shape is not printed.
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 此形状是否可打印的值 |

#### Returns

`any`

如果未设置任何值，则返回此形状是否可打印

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[canPrint](GC.Spread.Sheets.Shapes.ShapeBase.md#canprint)

___

### <a id="doubleclickcommand" name="doubleclickcommand"></a> doubleClickCommand

▸ **doubleClickCommand**(`value?`): `string` \| `void` \| `Function`

获取或设置形状的双击命令

**`代码示例`**
```
var shape = sheet.shapes.addCameraShape("shape1", 'Sheet1!A1:A8', 100, 50, 100, 150);
shape.doubleClickCommand(null);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` \| `Function` |

#### Returns

`string` \| `void` \| `Function`

如果未设置值，则返回形状的当前双击命令设置

___

### <a id="dynamicmove" name="dynamicmove"></a> dynamicMove

▸ **dynamicMove**(`value?`): `any`

获取或设置在隐藏或显示、调整大小或移动行或列时形状是否移动

**`代码示例`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var state = heart.dynamicMove();
heart.dynamicMove(!state);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 该值指示在隐藏或显示、调整大小或移动行或列时形状是否移动 |

#### Returns

`any`

如果未设置任何值，则返回此形状是否动态移动

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[dynamicMove](GC.Spread.Sheets.Shapes.ShapeBase.md#dynamicmove)

___

### <a id="dynamicsize" name="dynamicsize"></a> dynamicSize

▸ **dynamicSize**(`value?`): `any`

获取或设置在隐藏或显示、调整大小或移动行或列时形状的大小是否改变

**`代码示例`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var state = heart.dynamicSize();
heart.dynamicSize(!state);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 该值指示在隐藏或显示、调整大小或移动行或列时形状的大小是否改变 |

#### Returns

`any`

如果未设置任何值，则返回此形状是否动态更改大小

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[dynamicSize](GC.Spread.Sheets.Shapes.ShapeBase.md#dynamicsize)

___

### <a id="endcolumn" name="endcolumn"></a> endColumn

▸ **endColumn**(`value?`): `any`

获取或设置形状位置的结束列索引

**`代码示例`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.endColumn();
heart.endColumn(n + 1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 形状位置的结束列索引 |

#### Returns

`any`

如果未设置任何值，则返回形状位置的结束列索引

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[endColumn](GC.Spread.Sheets.Shapes.ShapeBase.md#endcolumn)

___

### <a id="endcolumnoffset" name="endcolumnoffset"></a> endColumnOffset

▸ **endColumnOffset**(`value?`): `any`

获取或设置相对于形状末端的偏移量

**`代码示例`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.endColumnOffset();
heart.endColumnOffset(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 相对于形状末端的偏移量 |

#### Returns

`any`

如果未设置任何值，则返回相对于形状末端的偏移量

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[endColumnOffset](GC.Spread.Sheets.Shapes.ShapeBase.md#endcolumnoffset)

___

### <a id="endrow" name="endrow"></a> endRow

▸ **endRow**(`value?`): `any`

获取或设置形状位置的末端行索引

**`代码示例`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.endRow();
heart.endRow(n + 2);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 形状位置的末端行索引 |

#### Returns

`any`

如果未设置任何值，则返回形状位置的末端行索引

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[endRow](GC.Spread.Sheets.Shapes.ShapeBase.md#endrow)

___

### <a id="endrowoffset" name="endrowoffset"></a> endRowOffset

▸ **endRowOffset**(`value?`): `any`

获取或设置相对于形状末端的偏移量

**`代码示例`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.endRowOffset();
heart.endRowOffset(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 相对于形状末端的偏移量 |

#### Returns

`any`

如果未设置任何值，则返回相对于形状末端的偏移量

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[endRowOffset](GC.Spread.Sheets.Shapes.ShapeBase.md#endrowoffset)

___

### <a id="getformula" name="getformula"></a> getFormula

▸ **getFormula**(`path`): `string`

通过路径从形状中获取公式字符串

**`代码示例`**
```
sheet.name("Sheet1");
sheet.setValue(0, 1, 150);
var shape1 = sheet.shapes.add("myShape1", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 100, 100, 200, 200);
shape1.setFormula("x", "=Sheet1!B1");
shape1.getFormula("x");//返回 "=Sheet1!B1"
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `path` | `string` | 可以接收公式字符串的路径，可以是"x","y","width","height"之一 |

#### Returns

`string`

通过路径从形状返回公式字符串

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[getFormula](GC.Spread.Sheets.Shapes.ShapeBase.md#getformula)

___

### <a id="height" name="height"></a> height

▸ **height**(`value?`): `any`

获取或设置形状的高度

**`代码示例`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.height();
heart.height(n + 50);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` \| `number` | 由数字或公式的形状高度(以=开头)可以获取数字值 |

#### Returns

`any`

如果未设置任何值，则返回形状的高度

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[height](GC.Spread.Sheets.Shapes.ShapeBase.md#height)

___

### <a id="hyperlink" name="hyperlink"></a> hyperlink

▸ **hyperlink**(`value?`): `void` \| [`IHyperlink`](../interfaces/GC.Spread.Sheets.IHyperlink.md)

获取或设置形状的超链接

**`代码示例`**
```
var shape = sheet.shapes.add("myShape", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 62 * 9, 0, 200, 200);
shape.hyperlink({url: "http://www.grapecity.com", target: 0, tooltip: 'goes to grapecity'});
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`IHyperlink`](../interfaces/GC.Spread.Sheets.IHyperlink.md) |

#### Returns

`void` \| [`IHyperlink`](../interfaces/GC.Spread.Sheets.IHyperlink.md)

如果未设置值，则返回形状的当前超链接设置

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[hyperlink](GC.Spread.Sheets.Shapes.ShapeBase.md#hyperlink)

___

### <a id="islocked" name="islocked"></a> isLocked

▸ **isLocked**(`value?`): `any`

获取或设置此形状是否被锁定

**`代码示例`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var state = heart.isLocked();
heart.isLocked(!state);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 此形状是否被锁定的值 |

#### Returns

`any`

如果未设置任何值，则返回此形状是否被锁定

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[isLocked](GC.Spread.Sheets.Shapes.ShapeBase.md#islocked)

___

### <a id="isselected" name="isselected"></a> isSelected

▸ **isSelected**(`value?`): `any`

获取或设置是否选择此形状

**`代码示例`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var state = heart.isSelected();
heart.isSelected(!state);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否选择此形状的值 |

#### Returns

`any`

如果未设置任何值，则返回是否选择此形状

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[isSelected](GC.Spread.Sheets.Shapes.ShapeBase.md#isselected)

___

### <a id="isvisible" name="isvisible"></a> isVisible

▸ **isVisible**(`value?`): `any`

获取或设置此形状是否可见

**`代码示例`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var state = heart.isVisible();
heart.isVisible(!state);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 此形状是否可见的值 |

#### Returns

`any`

如果未设置任何值，则返回此形状是否可见

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[isVisible](GC.Spread.Sheets.Shapes.ShapeBase.md#isvisible)

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置形状的名称

**`代码示例`**
```
var shape1 = sheet.shapes.add("myShape1", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 62 * 9, 0, 200, 200);
var shape2 = sheet.shapes.add("myShape2", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 20, 20, 200, 200);
var shape = sheet.shapes.group([shape1, shape2]);
shape.name("myGroupShape");
var shapeName = shape.name();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 形状的名称 |

#### Returns

`any`

如果未设置任何值，则返回形状的名称

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[name](GC.Spread.Sheets.Shapes.ShapeBase.md#name)

___

### <a id="range" name="range"></a> range

▸ **range**(`value?`): `string` \| `void`

获取或设置快照形状的单元格区域

**`代码示例`**
```
var shape = sheet.shapes.addCameraShape("shape1", 'Sheet1!A1:A8', 100, 50, 100, 150);
shape.range('Sheet2!A2:B8');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 快照形状的单元格区域(如Sheet1!A1:A8) |

#### Returns

`string` \| `void`

如果未设置值，则返回快照形状的单元格区域

___

### <a id="rotate" name="rotate"></a> rotate

▸ **rotate**(`value?`): `number` \| `void`

获取或设置摄影机形状的旋转角度(单位为度)

**`代码示例`**
```
var shape = sheet.shapes.addCameraShape("shape1", 'Sheet1!A1:A8', 100, 50, 100, 150);
var n = shape.rotate();
shape.rotate(n + 30);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` \| `number` | 由数字或公式(以=)的快照形状的旋转角度(以度为单位)可以获得数值 |

#### Returns

`number` \| `void`

如果未设置值，则返回快照形状的旋转角度(单位为度)

___

### <a id="setformula" name="setformula"></a> setFormula

▸ **setFormula**(`path`, `formula`): `void`

通过路径将公式字符串设置为形状

**`代码示例`**
```
sheet.name("Sheet1");
sheet.setValue(0, 1, 150);
var shape1 = sheet.shapes.add("myShape1", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 100, 100, 200, 200);
shape1.setFormula("x", "=Sheet1!B1");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `path` | `string` | 可以接收公式字符串的路径，可以是"x","y","width","height"之一 |
| `formula` | `string` | 公式字符串 |

#### Returns

`void`

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[setFormula](GC.Spread.Sheets.Shapes.ShapeBase.md#setformula)

___

### <a id="showhandle" name="showhandle"></a> showHandle

▸ **showHandle**(`value?`): `boolean` \| `void`

获取或设置是否显示形状句柄

**`代码示例`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var state = heart.showHandle();
heart.showHandle(!state);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否显示形状句柄的设置 |

#### Returns

`boolean` \| `void`

如果未设置任何值，则返回是否显示形状句柄的设置

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[showHandle](GC.Spread.Sheets.Shapes.ShapeBase.md#showhandle)

___

### <a id="startcolumn" name="startcolumn"></a> startColumn

▸ **startColumn**(`value?`): `any`

获取或设置形状位置的起始列索引

**`代码示例`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.startColumn();
heart.startColumn(n + 2);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 形状位置的起始列索引 |

#### Returns

`any`

如果未设置任何值，则返回形状位置的起始列索引

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[startColumn](GC.Spread.Sheets.Shapes.ShapeBase.md#startcolumn)

___

### <a id="startcolumnoffset" name="startcolumnoffset"></a> startColumnOffset

▸ **startColumnOffset**(`value?`): `any`

获取或设置相对于图形开始列的偏移量

**`代码示例`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.startColumnOffset();
heart.startColumnOffset(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 相对于形状的起始列的偏移量 |

#### Returns

`any`

如果未设置任何值，则返回相对于图形起始列的偏移量

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[startColumnOffset](GC.Spread.Sheets.Shapes.ShapeBase.md#startcolumnoffset)

___

### <a id="startrow" name="startrow"></a> startRow

▸ **startRow**(`value?`): `any`

获取或设置形状位置的起始行索引

**`代码示例`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.startRow();
heart.startRow(n + 2);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 形状位置的起始行索引 |

#### Returns

`any`

如果未设置任何值，则返回形状的起始行索引

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[startRow](GC.Spread.Sheets.Shapes.ShapeBase.md#startrow)

___

### <a id="startrowoffset" name="startrowoffset"></a> startRowOffset

▸ **startRowOffset**(`value?`): `any`

获取或设置相对于图形起始行的偏移量

**`代码示例`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.startRowOffset();
heart.startRowOffset(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 相对于图形起始行的偏移量 |

#### Returns

`any`

如果未设置任何值，则返回相对于图形起始行的偏移量

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[startRowOffset](GC.Spread.Sheets.Shapes.ShapeBase.md#startrowoffset)

___

### <a id="style" name="style"></a> style

▸ **style**(`value?`): `any`

获取或设置快照形状的样式

**`代码示例`**
```
//本示例设置形状的样式
var shape = sheet.shapes.addCameraShape("shape1", 'Sheet1!A1:A8', 100, 50, 100, 150);
var oldStyle = shape.style();
oldStyle.fill.color = "red";
oldStyle.fill.transparency = 0.5;
oldStyle.line.color = "green";
oldStyle.line.lineStyle = GC.Spread.Sheets.Shapes.PresetLineDashStyle.dashDot;
oldStyle.line.width = 5;
oldStyle.line.capType = GC.Spread.Sheets.Shapes.LineCapStyle.square;
oldStyle.line.joinType = GC.Spread.Sheets.Shapes.LineJoinStyle.miter;
oldStyle.line.transparency = 0.5;
shape.style(oldStyle);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`ShapeStyle`](GC.Spread.Sheets.Shapes.ShapeStyle.md) | 形状样式 |

#### Returns

`any`

如果未设置值，则返回形状的当前样式

___

### <a id="width" name="width"></a> width

▸ **width**(`value?`): `any`

获取或设置形状的宽度

**`代码示例`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.width();
heart.width(n + 50);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` \| `number` | 由数字或公式的形状的宽度(以=开头)可以获取数字值 |

#### Returns

`any`

如果未设置任何值，则返回形状的宽度

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[width](GC.Spread.Sheets.Shapes.ShapeBase.md#width)

___

### <a id="x" name="x"></a> x

▸ **x**(`value?`): `number` \| `void`

获取或设置形状的水平位置

**`代码示例`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.x();
heart.x(n + 50);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` \| `number` | 由数字或公式的形状的水平位置(以=开头)可以获取数字值 |

#### Returns

`any`

如果未设置任何值，则返回形状的水平位置

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[x](GC.Spread.Sheets.Shapes.ShapeBase.md#x)

___

### <a id="y" name="y"></a> y

▸ **y**(`value?`): `any`

获取或设置形状的垂直位置

**`代码示例`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.y();
heart.y(n + 50);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` \| `number` | 由数字或公式的形状的垂直位置(以=开头)可以获取数字值 |

#### Returns

`any`

如果未设置任何值，则返回形状的垂直位置

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[y](GC.Spread.Sheets.Shapes.ShapeBase.md#y)
