# Class: Shape

[Sheets](../modules/GC.Spread.Sheets.md).[Shapes](../modules/GC.Spread.Sheets.Shapes.md).Shape

## Hierarchy

- [`ShapeBase`](GC.Spread.Sheets.Shapes.ShapeBase.md)

  ↳ **`Shape`**

  ↳↳ [`FormControlShape`](GC.Spread.Sheets.Shapes.FormControlShape.md)

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Shapes.Shape.md#constructor)

### Methods

- [adjustments](GC.Spread.Sheets.Shapes.Shape.md#adjustments)
- [allowMove](GC.Spread.Sheets.Shapes.Shape.md#allowmove)
- [allowResize](GC.Spread.Sheets.Shapes.Shape.md#allowresize)
- [allowRotate](GC.Spread.Sheets.Shapes.Shape.md#allowrotate)
- [alt](GC.Spread.Sheets.Shapes.Shape.md#alt)
- [canPrint](GC.Spread.Sheets.Shapes.Shape.md#canprint)
- [dynamicMove](GC.Spread.Sheets.Shapes.Shape.md#dynamicmove)
- [dynamicSize](GC.Spread.Sheets.Shapes.Shape.md#dynamicsize)
- [endColumn](GC.Spread.Sheets.Shapes.Shape.md#endcolumn)
- [endColumnOffset](GC.Spread.Sheets.Shapes.Shape.md#endcolumnoffset)
- [endRow](GC.Spread.Sheets.Shapes.Shape.md#endrow)
- [endRowOffset](GC.Spread.Sheets.Shapes.Shape.md#endrowoffset)
- [getFormula](GC.Spread.Sheets.Shapes.Shape.md#getformula)
- [height](GC.Spread.Sheets.Shapes.Shape.md#height)
- [hyperlink](GC.Spread.Sheets.Shapes.Shape.md#hyperlink)
- [isLocked](GC.Spread.Sheets.Shapes.Shape.md#islocked)
- [isSelected](GC.Spread.Sheets.Shapes.Shape.md#isselected)
- [isTextBox](GC.Spread.Sheets.Shapes.Shape.md#istextbox)
- [isVisible](GC.Spread.Sheets.Shapes.Shape.md#isvisible)
- [name](GC.Spread.Sheets.Shapes.Shape.md#name)
- [rotate](GC.Spread.Sheets.Shapes.Shape.md#rotate)
- [setFormula](GC.Spread.Sheets.Shapes.Shape.md#setformula)
- [showHandle](GC.Spread.Sheets.Shapes.Shape.md#showhandle)
- [startColumn](GC.Spread.Sheets.Shapes.Shape.md#startcolumn)
- [startColumnOffset](GC.Spread.Sheets.Shapes.Shape.md#startcolumnoffset)
- [startRow](GC.Spread.Sheets.Shapes.Shape.md#startrow)
- [startRowOffset](GC.Spread.Sheets.Shapes.Shape.md#startrowoffset)
- [style](GC.Spread.Sheets.Shapes.Shape.md#style)
- [text](GC.Spread.Sheets.Shapes.Shape.md#text)
- [toImageSrc](GC.Spread.Sheets.Shapes.Shape.md#toimagesrc)
- [toImageSrcAsync](GC.Spread.Sheets.Shapes.Shape.md#toimagesrcasync)
- [type](GC.Spread.Sheets.Shapes.Shape.md#type)
- [width](GC.Spread.Sheets.Shapes.Shape.md#width)
- [x](GC.Spread.Sheets.Shapes.Shape.md#x)
- [y](GC.Spread.Sheets.Shapes.Shape.md#y)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Shape**(`worksheet`, `name`, `autoShapeTypeOrModel`, `left?`, `top?`, `width?`, `height?`)

SpreadJS 中的 Shape 类是工作表上所有可视化形状对象的基类，提供了用于控制形状位置、尺寸、样式和交互行为的通用属性与方法。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `worksheet` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 形状所在的工作表。 |
| `name` | `string` | 形状的名称。如果名称为空字符串，将自动生成一个唯一名称。 |
| `autoShapeTypeOrModel` | [`IShapeModel`](../interfaces/GC.Spread.Sheets.Shapes.IShapeModel.md) \| [`AutoShapeType`](../enums/GC.Spread.Sheets.Shapes.AutoShapeType.md) | 形状的内置自动形状类型（AutoShapeType 枚举值）或自定义形状模型（IShapeModel 对象）。 |
| `left?` | `number` | 可选参数。形状的 <i>x</i> 坐标位置（水平位置）。 |
| `top?` | `number` | 可选参数。形状的 <i>y</i> 坐标位置（垂直位置）。 |
| `width?` | `number` | 可选参数。形状的宽度。 |
| `height?` | `number` | 可选参数。形状的高度。 |

#### Overrides

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[constructor](GC.Spread.Sheets.Shapes.ShapeBase.md#constructor)

## Methods

### <a id="adjustments" name="adjustments"></a> adjustments

▸ **adjustments**(`arrayValue?`): `void` \| `number`[]

获取或设置形状的调整值。

**`example`**
```javascript
var blockArc = sheet.shapes.add("", GC.Spread.Sheets.Shapes.AutoShapeType.blockArc, 100, 60, 200, 160);
var adjustments = blockArc.adjustments();
console.log(adjustments);
adjustments[0] = 150;
adjustments[1] = 15;
adjustments[2] = 0.35;
blockArc.adjustments(adjustments);
blockArc.isSelected(true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `arrayValue?` | `number`[] | 调整值数组。 |

#### Returns

`void` \| `number`[]

如果未设置值，返回形状当前的调整值。

___

### <a id="allowmove" name="allowmove"></a> allowMove

▸ **allowMove**(`value?`): `any`

获取或设置是否禁用移动形状。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var state = heart.allowMove();
heart.allowMove(!state);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否禁用移动形状的设置。 |

#### Returns

`any`

如果未设置值，返回是否禁用移动形状的设置。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[allowMove](GC.Spread.Sheets.Shapes.ShapeBase.md#allowmove)

___

### <a id="allowresize" name="allowresize"></a> allowResize

▸ **allowResize**(`value?`): `any`

获取或设置形状的调整大小模式。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var state = heart.allowResize();
heart.allowResize(GC.Spread.Sheets.Shapes.ResizeMode.aspect);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` \| [`ResizeMode`](../enums/GC.Spread.Sheets.Shapes.ResizeMode.md) | 是否禁用调整形状大小的设置。 |

#### Returns

`any`

如果未设置值，返回是否禁用调整形状大小的设置。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[allowResize](GC.Spread.Sheets.Shapes.ShapeBase.md#allowresize)

___

### <a id="allowrotate" name="allowrotate"></a> allowRotate

▸ **allowRotate**(`value?`): `any`

获取或设置是否禁用旋转形状。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var state = heart.allowRotate();
heart.allowRotate(!state);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否禁用旋转形状的设置。 |

#### Returns

`any`

如果未设置值，返回是否禁用旋转形状的设置。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[allowRotate](GC.Spread.Sheets.Shapes.ShapeBase.md#allowrotate)

___

### <a id="alt" name="alt"></a> alt

▸ **alt**(`value?`): `any`

获取或设置形状的替代文本（用于屏幕阅读器）。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
heart.alt("一个心形");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 形状的替代文本。 |

#### Returns

`any`

形状的替代文本。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[alt](GC.Spread.Sheets.Shapes.ShapeBase.md#alt)

___

### <a id="canprint" name="canprint"></a> canPrint

▸ **canPrint**(`value?`): `any`

获取或设置此形状是否可打印。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var state = heart.canPrint(); // 获取形状是否可打印，默认值为 true.
workbook.print(); // 心形被打印。
heart.canPrint(false);
workbook.print(); // 心形不被打印。
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 指示此形状是否可打印的值。 |

#### Returns

`any`

如果未设置值，返回此形状是否可打印。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[canPrint](GC.Spread.Sheets.Shapes.ShapeBase.md#canprint)

___

### <a id="dynamicmove" name="dynamicmove"></a> dynamicMove

▸ **dynamicMove**(`value?`): `any`

获取或设置形状在隐藏或显示、调整大小或移动行或列时是否移动。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var state = heart.dynamicMove();
heart.dynamicMove(!state);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 指示形状在隐藏或显示、调整大小或移动行或列时是否移动的值。 |

#### Returns

`any`

如果未设置值，返回此形状是否动态移动。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[dynamicMove](GC.Spread.Sheets.Shapes.ShapeBase.md#dynamicmove)

___

### <a id="dynamicsize" name="dynamicsize"></a> dynamicSize

▸ **dynamicSize**(`value?`): `any`

获取或设置形状在隐藏或显示、调整大小或移动行或列时是否改变大小。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var state = heart.dynamicSize();
heart.dynamicSize(!state);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 指示形状在隐藏或显示、调整大小或移动行或列时是否改变大小的值。 |

#### Returns

`any`

如果未设置值，返回此形状是否动态改变大小。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[dynamicSize](GC.Spread.Sheets.Shapes.ShapeBase.md#dynamicsize)

___

### <a id="endcolumn" name="endcolumn"></a> endColumn

▸ **endColumn**(`value?`): `any`

获取或设置形状位置的结束列索引。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.endColumn();
heart.endColumn(n + 1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 形状位置的结束列索引。 |

#### Returns

`any`

如果未设置值，返回形状位置的结束列索引。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[endColumn](GC.Spread.Sheets.Shapes.ShapeBase.md#endcolumn)

___

### <a id="endcolumnoffset" name="endcolumnoffset"></a> endColumnOffset

▸ **endColumnOffset**(`value?`): `any`

获取或设置相对于形状结束列的偏移量。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.endColumnOffset();
heart.endColumnOffset(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 相对于形状结束列的偏移量。 |

#### Returns

`any`

如果未设置值，返回相对于形状结束列的偏移量。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[endColumnOffset](GC.Spread.Sheets.Shapes.ShapeBase.md#endcolumnoffset)

___

### <a id="endrow" name="endrow"></a> endRow

▸ **endRow**(`value?`): `any`

获取或设置形状位置的结束行索引。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.endRow();
heart.endRow(n + 2);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 形状位置的结束行索引。 |

#### Returns

`any`

如果未设置值，返回形状位置的结束行索引。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[endRow](GC.Spread.Sheets.Shapes.ShapeBase.md#endrow)

___

### <a id="endrowoffset" name="endrowoffset"></a> endRowOffset

▸ **endRowOffset**(`value?`): `any`

获取或设置相对于形状结束行的偏移量。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.endRowOffset();
heart.endRowOffset(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 相对于形状结束行的偏移量。 |

#### Returns

`any`

如果未设置值，返回相对于形状结束行的偏移量。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[endRowOffset](GC.Spread.Sheets.Shapes.ShapeBase.md#endrowoffset)

___

### <a id="getformula" name="getformula"></a> getFormula

▸ **getFormula**(`path`): `string`

通过路径获取形状的公式字符串。

**`example`**
```javascript
sheet.name("Sheet1");
sheet.setValue(0, 1, "This is a rectangle.");
var shape1 = sheet.shapes.add("myShape1", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 100, 100, 200, 200);
shape1.setFormula("text", "=Sheet1!B1");
shape1.getFormula("text");//returns "=Sheet1!B1"
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `path` | `string` | 可以接受公式字符串的路径，可以是以下之一："x", "y", "width", "height", "rotate", "text", 填充："style.fill.color", "style.fill.transparency", 填充图片："style.fill.src", "style.fill.tilePictureAsTexture", 填充偏移："style.fill.offsetLeft", "style.fill.offsetRight", "style.fill.offsetTop", "style.fill.offsetBottom", 填充缩放与对齐："style.fill.offsetX", "style.fill.offsetY", "style.fill.scaleX", "style.fill.scaleY", "style.fill.alignment", "style.fill.mirrorType", 填充类型："style.fill.type", "style.fill.angle", "style.fill.direction", 渐变停止点："style.fill.stops.0.color", "style.fill.stops.0.position", "style.fill.stops.0.transparency", "style.fill.stops.0.brightness", 线条："style.line.color", "style.line.lineStyle", "style.line.width", "style.line.capType", "style.line.joinType", "style.line.compoundType", "style.line.transparency", 文本效果："style.textEffect.color", "style.textEffect.transparency", "style.textEffect.font", 文本框："style.textFrame.vAlign", "style.textFrame.hAlign"。 |

#### Returns

`string`

返回通过路径获取的形状公式字符串。

#### Overrides

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[getFormula](GC.Spread.Sheets.Shapes.ShapeBase.md#getformula)

___

### <a id="height" name="height"></a> height

▸ **height**(`value?`): `any`

获取或设置形状的高度。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.height();
heart.height(n + 50);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` \| `number` | 形状的高度，可以是数值或公式（以=开头）。 |

#### Returns

`any`

如果未设置值，返回形状的高度。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[height](GC.Spread.Sheets.Shapes.ShapeBase.md#height)

___

### <a id="hyperlink" name="hyperlink"></a> hyperlink

▸ **hyperlink**(`value?`): `void` \| [`IHyperlink`](../interfaces/GC.Spread.Sheets.IHyperlink.md)

获取或设置形状的超链接。

**`example`**
```javascript
var shape = sheet.shapes.add("myShape", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 62 * 9, 0, 200, 200);
shape.hyperlink({url: "http://www.spreadjs.com", target: 0, tooltip: 'goes to SpreadJS'});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`IHyperlink`](../interfaces/GC.Spread.Sheets.IHyperlink.md) | 超链接设置。 |

#### Returns

`void` \| [`IHyperlink`](../interfaces/GC.Spread.Sheets.IHyperlink.md)

如果未设置值，返回形状当前的超链接设置。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[hyperlink](GC.Spread.Sheets.Shapes.ShapeBase.md#hyperlink)

___

### <a id="islocked" name="islocked"></a> isLocked

▸ **isLocked**(`value?`): `any`

获取或设置此形状是否被锁定。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var state = heart.isLocked();
heart.isLocked(!state);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 指示此形状是否被锁定的值。 |

#### Returns

`any`

如果未设置值，返回此形状是否被锁定。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[isLocked](GC.Spread.Sheets.Shapes.ShapeBase.md#islocked)

___

### <a id="isselected" name="isselected"></a> isSelected

▸ **isSelected**(`value?`): `any`

获取或设置此形状是否被选中。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var state = heart.isSelected();
heart.isSelected(!state);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 指示此形状是否被选中的值。 |

#### Returns

`any`

如果未设置值，返回此形状是否被选中。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[isSelected](GC.Spread.Sheets.Shapes.ShapeBase.md#isselected)

___

### <a id="istextbox" name="istextbox"></a> isTextBox

▸ **isTextBox**(`value?`): `boolean` \| `void`

获取或设置形状是否为文本框。

**`example`**
```javascript
var rectangle = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 100, 60, 200, 160);
rectangle.isTextBox(true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 指示形状是否为文本框的值。 |

#### Returns

`boolean` \| `void`

如果未设置值，返回形状是否为文本框。

___

### <a id="isvisible" name="isvisible"></a> isVisible

▸ **isVisible**(`value?`): `any`

获取或设置此形状是否可见。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var state = heart.isVisible();
heart.isVisible(!state);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 指示此形状是否可见的值。 |

#### Returns

`any`

如果未设置值，返回此形状是否可见。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[isVisible](GC.Spread.Sheets.Shapes.ShapeBase.md#isvisible)

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置形状的名称。

**`example`**
```javascript
var shape1 = sheet.shapes.add("myShape1", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 62 * 9, 0, 200, 200);
var shape2 = sheet.shapes.add("myShape2", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 20, 20, 200, 200);
var shape = sheet.shapes.group([shape1, shape2]);
shape.name("myGroupShape");
var shapeName = shape.name();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 形状的名称。 |

#### Returns

`any`

如果未设置值，返回形状的名称。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[name](GC.Spread.Sheets.Shapes.ShapeBase.md#name)

___

### <a id="rotate" name="rotate"></a> rotate

▸ **rotate**(`value?`): `number` \| `void`

获取或设置形状的旋转角度（单位为度）。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.rotate();
heart.rotate(n + 30);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` \| `number` | 形状的旋转角度（单位为度），可以由数字或公式（以=开头）指定，可以获取数字值。 |

#### Returns

`number` \| `void`

如果未设置值，返回形状的旋转角度（单位为度）。

___

### <a id="setformula" name="setformula"></a> setFormula

▸ **setFormula**(`path`, `formula`): `void`

通过路径设置形状的公式字符串。

**`example`**
```javascript
sheet.name("Sheet1");
sheet.setValue(0, 1, "This is a rectangle.");
var shape1 = sheet.shapes.add("myShape1", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 100, 100, 200, 200);
shape1.setFormula("text", "=Sheet1!B1");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `path` | `string` | 可以接受公式字符串的路径，可以是以下之一："x", "y", "width", "height", "rotate", "text", 填充："style.fill.color", "style.fill.transparency", 填充图片："style.fill.src", "style.fill.tilePictureAsTexture", 填充偏移："style.fill.offsetLeft", "style.fill.offsetRight", "style.fill.offsetTop", "style.fill.offsetBottom", 填充缩放与对齐："style.fill.offsetX", "style.fill.offsetY", "style.fill.scaleX", "style.fill.scaleY", "style.fill.alignment", "style.fill.mirrorType", 填充类型："style.fill.type", "style.fill.angle", "style.fill.direction", 渐变停止点："style.fill.stops.0.color", "style.fill.stops.0.position", "style.fill.stops.0.transparency", "style.fill.stops.0.brightness", 线条："style.line.color", "style.line.lineStyle", "style.line.width", "style.line.capType", "style.line.joinType", "style.line.compoundType", "style.line.transparency", 文本效果："style.textEffect.color", "style.textEffect.transparency", "style.textEffect.font", 文本框："style.textFrame.vAlign", "style.textFrame.hAlign"。 |
| `formula` | `string` | 公式字符串。 |

#### Returns

`void`

#### Overrides

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[setFormula](GC.Spread.Sheets.Shapes.ShapeBase.md#setformula)

___

### <a id="showhandle" name="showhandle"></a> showHandle

▸ **showHandle**(`value?`): `any`

获取或设置是否显示形状的控制柄。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var state = heart.showHandle();
heart.showHandle(!state);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否显示形状控制柄的设置。 |

#### Returns

`any`

如果未设置值，返回是否显示形状控制柄的设置。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[showHandle](GC.Spread.Sheets.Shapes.ShapeBase.md#showhandle)

___

### <a id="startcolumn" name="startcolumn"></a> startColumn

▸ **startColumn**(`value?`): `any`

获取或设置形状位置的起始列索引。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.startColumn();
heart.startColumn(n + 2);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 形状位置的起始列索引。 |

#### Returns

`any`

如果未设置值，返回形状位置的起始列索引。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[startColumn](GC.Spread.Sheets.Shapes.ShapeBase.md#startcolumn)

___

### <a id="startcolumnoffset" name="startcolumnoffset"></a> startColumnOffset

▸ **startColumnOffset**(`value?`): `any`

获取或设置相对于形状起始列的偏移量。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.startColumnOffset();
heart.startColumnOffset(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 相对于形状起始列的偏移量。 |

#### Returns

`any`

如果未设置值，返回相对于形状起始列的偏移量。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[startColumnOffset](GC.Spread.Sheets.Shapes.ShapeBase.md#startcolumnoffset)

___

### <a id="startrow" name="startrow"></a> startRow

▸ **startRow**(`value?`): `any`

获取或设置形状位置的起始行索引。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.startRow();
heart.startRow(n + 2);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 形状位置的起始行索引。 |

#### Returns

`any`

如果未设置值，返回形状位置的起始行索引。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[startRow](GC.Spread.Sheets.Shapes.ShapeBase.md#startrow)

___

### <a id="startrowoffset" name="startrowoffset"></a> startRowOffset

▸ **startRowOffset**(`value?`): `any`

获取或设置相对于形状起始行的偏移量。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.startRowOffset();
heart.startRowOffset(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 相对于形状起始行的偏移量。 |

#### Returns

`any`

如果未设置值，返回相对于形状起始行的偏移量。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[startRowOffset](GC.Spread.Sheets.Shapes.ShapeBase.md#startrowoffset)

___

### <a id="style" name="style"></a> style

▸ **style**(`value?`): `any`

获取或设置形状的样式。

**`example`**
```javascript
//此示例为形状设置样式。
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var oldStyle = heart.style();
oldStyle.fill.color = "red";
oldStyle.fill.transparency = 0.5;
oldStyle.line.color = "green";
oldStyle.line.lineStyle = GC.Spread.Sheets.Shapes.PresetLineDashStyle.dashDot;
oldStyle.line.width = 5;
oldStyle.line.capType = GC.Spread.Sheets.Shapes.LineCapStyle.square;
oldStyle.line.joinType = GC.Spread.Sheets.Shapes.LineJoinStyle.miter;
oldStyle.line.compoundType = GC.Spread.Sheets.Shapes.CompoundType.double;
oldStyle.line.transparency = 0.5;
oldStyle.textEffect.color = "yellow";
oldStyle.textEffect.transparency = 0.5;
oldStyle.textEffect.font = "20px Arial";
oldStyle.textFrame.vAlign = GC.Spread.Sheets.VerticalAlign.center;
oldStyle.textFrame.hAlign = GC.Spread.Sheets.HorizontalAlign.center;
heart.style(oldStyle);
heart.text("Heart");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`ShapeStyle`](GC.Spread.Sheets.Shapes.ShapeStyle.md) | 形状样式。 |

#### Returns

`any`

如果未设置值，返回形状当前的样式。

___

### <a id="text" name="text"></a> text

▸ **text**(`value?`): `any`

获取或设置形状的文本。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
heart.text("My Shape");
var s = heart.text();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 形状的文本，可以由字符串或公式（以=开头）指定，可以获取字符串。 |

#### Returns

`any`

如果未设置值，返回形状的文本。

___

### <a id="toimagesrc" name="toimagesrc"></a> toImageSrc

▸ **toImageSrc**(): `string`

获取形状的Base64字符串类型的图片源。

**`example`**
```javascript
let shapeImageSrc = sheet.shapes.all()[0].toImageSrc();
```

#### Returns

`string`

返回形状的Base64字符串类型的图片源。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[toImageSrc](GC.Spread.Sheets.Shapes.ShapeBase.md#toimagesrc)

___

### <a id="toimagesrcasync" name="toimagesrcasync"></a> toImageSrcAsync

▸ **toImageSrcAsync**(): `Promise`<`string`\>

获取形状的Base64字符串类型的图片源。

**`example`**
```javascript
let shapeImageSrc = await sheet.shapes.all()[0].toImageSrcAsync();
```

#### Returns

`Promise`<`string`\>

返回形状的Base64字符串类型的图片源。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[toImageSrcAsync](GC.Spread.Sheets.Shapes.ShapeBase.md#toimagesrcasync)

___

### <a id="type" name="type"></a> type

▸ **type**(`value?`): `any`

获取或设置形状的类型。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.type();
heart.type(GC.Spread.Sheets.Shapes.AutoShapeType.cloud);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`AutoShapeType`](../enums/GC.Spread.Sheets.Shapes.AutoShapeType.md) | 形状的类型。 |

#### Returns

`any`

如果未设置值，则返回形状的类型。

___

### <a id="width" name="width"></a> width

▸ **width**(`value?`): `any`

获取或设置形状的宽度。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.width();
heart.width(n + 50);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` \| `number` | 形状的宽度，可以是数值或公式（以=开头）。 |

#### Returns

`any`

如果未设置值，返回形状的宽度。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[width](GC.Spread.Sheets.Shapes.ShapeBase.md#width)

___

### <a id="x" name="x"></a> x

▸ **x**(`value?`): `any`

获取或设置形状的水平位置。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.x();
heart.x(n + 50);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` \| `number` | 形状的水平位置，可以是数值或公式（以=开头）。 |

#### Returns

`any`

如果未设置值，返回形状的水平位置。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[x](GC.Spread.Sheets.Shapes.ShapeBase.md#x)

___

### <a id="y" name="y"></a> y

▸ **y**(`value?`): `any`

获取或设置形状的垂直位置。

**`example`**
```javascript
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.y();
heart.y(n + 50);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` \| `number` | 形状的垂直位置，可以是数值或公式（以=开头）。 |

#### Returns

`any`

如果未设置值，返回形状的垂直位置。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[y](GC.Spread.Sheets.Shapes.ShapeBase.md#y)
