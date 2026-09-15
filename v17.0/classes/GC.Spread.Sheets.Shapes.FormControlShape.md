# Class: FormControlShape

[Sheets](../modules/GC.Spread.Sheets.md).[Shapes](../modules/GC.Spread.Sheets.Shapes.md).FormControlShape

## Hierarchy

- [`Shape`](GC.Spread.Sheets.Shapes.Shape.md)

  ↳ **`FormControlShape`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Shapes.FormControlShape.md#constructor)

### Methods

- [adjustments](GC.Spread.Sheets.Shapes.FormControlShape.md#adjustments)
- [allowMove](GC.Spread.Sheets.Shapes.FormControlShape.md#allowmove)
- [allowResize](GC.Spread.Sheets.Shapes.FormControlShape.md#allowresize)
- [allowRotate](GC.Spread.Sheets.Shapes.FormControlShape.md#allowrotate)
- [alt](GC.Spread.Sheets.Shapes.FormControlShape.md#alt)
- [canPrint](GC.Spread.Sheets.Shapes.FormControlShape.md#canprint)
- [dynamicMove](GC.Spread.Sheets.Shapes.FormControlShape.md#dynamicmove)
- [dynamicSize](GC.Spread.Sheets.Shapes.FormControlShape.md#dynamicsize)
- [enabled](GC.Spread.Sheets.Shapes.FormControlShape.md#enabled)
- [endColumn](GC.Spread.Sheets.Shapes.FormControlShape.md#endcolumn)
- [endColumnOffset](GC.Spread.Sheets.Shapes.FormControlShape.md#endcolumnoffset)
- [endRow](GC.Spread.Sheets.Shapes.FormControlShape.md#endrow)
- [endRowOffset](GC.Spread.Sheets.Shapes.FormControlShape.md#endrowoffset)
- [formControlType](GC.Spread.Sheets.Shapes.FormControlShape.md#formcontroltype)
- [getFormula](GC.Spread.Sheets.Shapes.FormControlShape.md#getformula)
- [height](GC.Spread.Sheets.Shapes.FormControlShape.md#height)
- [hyperlink](GC.Spread.Sheets.Shapes.FormControlShape.md#hyperlink)
- [isLocked](GC.Spread.Sheets.Shapes.FormControlShape.md#islocked)
- [isSelected](GC.Spread.Sheets.Shapes.FormControlShape.md#isselected)
- [isTextBox](GC.Spread.Sheets.Shapes.FormControlShape.md#istextbox)
- [isVisible](GC.Spread.Sheets.Shapes.FormControlShape.md#isvisible)
- [name](GC.Spread.Sheets.Shapes.FormControlShape.md#name)
- [options](GC.Spread.Sheets.Shapes.FormControlShape.md#options)
- [rotate](GC.Spread.Sheets.Shapes.FormControlShape.md#rotate)
- [setFormula](GC.Spread.Sheets.Shapes.FormControlShape.md#setformula)
- [showHandle](GC.Spread.Sheets.Shapes.FormControlShape.md#showhandle)
- [startColumn](GC.Spread.Sheets.Shapes.FormControlShape.md#startcolumn)
- [startColumnOffset](GC.Spread.Sheets.Shapes.FormControlShape.md#startcolumnoffset)
- [startRow](GC.Spread.Sheets.Shapes.FormControlShape.md#startrow)
- [startRowOffset](GC.Spread.Sheets.Shapes.FormControlShape.md#startrowoffset)
- [style](GC.Spread.Sheets.Shapes.FormControlShape.md#style)
- [text](GC.Spread.Sheets.Shapes.FormControlShape.md#text)
- [type](GC.Spread.Sheets.Shapes.FormControlShape.md#type)
- [value](GC.Spread.Sheets.Shapes.FormControlShape.md#value)
- [width](GC.Spread.Sheets.Shapes.FormControlShape.md#width)
- [x](GC.Spread.Sheets.Shapes.FormControlShape.md#x)
- [y](GC.Spread.Sheets.Shapes.FormControlShape.md#y)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new FormControlShape**(`worksheet`, `formControlType`, `left?`, `top?`, `width?`, `height?`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `worksheet` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 形状的宿主表单 |
| `formControlType` | [`FormControlType`](../enums/GC.Spread.Sheets.Shapes.FormControlType.md) | - |
| `left?` | `number` | 形状的<i>x</i>位置 |
| `top?` | `number` | 形状的<i>y</i>位置 |
| `width?` | `number` | 形状的宽度 |
| `height?` | `number` | 形状的高度 |

#### Overrides

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[constructor](GC.Spread.Sheets.Shapes.Shape.md#constructor)

## Methods

### <a id="adjustments" name="adjustments"></a> adjustments

▸ **adjustments**(`arrayValue?`): `void` \| `number`[]

获取或设置形状的调整值

**`代码示例`**
```
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
| `arrayValue?` | `number`[] | 数组中的调整值 |

#### Returns

`void` \| `number`[]

如果未设置任何值，则返回形状的当前调整值

#### Inherited from

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[adjustments](GC.Spread.Sheets.Shapes.Shape.md#adjustments)

___

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

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[allowMove](GC.Spread.Sheets.Shapes.Shape.md#allowmove)

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

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[allowResize](GC.Spread.Sheets.Shapes.Shape.md#allowresize)

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

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[allowRotate](GC.Spread.Sheets.Shapes.Shape.md#allowrotate)

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

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[alt](GC.Spread.Sheets.Shapes.Shape.md#alt)

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

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[canPrint](GC.Spread.Sheets.Shapes.Shape.md#canprint)

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

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[dynamicMove](GC.Spread.Sheets.Shapes.Shape.md#dynamicmove)

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

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[dynamicSize](GC.Spread.Sheets.Shapes.Shape.md#dynamicsize)

___

### <a id="enabled" name="enabled"></a> enabled

▸ **enabled**(`v?`): `boolean`

Gets or Sets the enabled of form control shape.

#### Parameters

| Name | Type |
| :------ | :------ |
| `v?` | `boolean` |

#### Returns

`boolean`

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

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[endColumn](GC.Spread.Sheets.Shapes.Shape.md#endcolumn)

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

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[endColumnOffset](GC.Spread.Sheets.Shapes.Shape.md#endcolumnoffset)

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

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[endRow](GC.Spread.Sheets.Shapes.Shape.md#endrow)

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

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[endRowOffset](GC.Spread.Sheets.Shapes.Shape.md#endrowoffset)

___

### <a id="formcontroltype" name="formcontroltype"></a> formControlType

▸ **formControlType**(): [`FormControlType`](../enums/GC.Spread.Sheets.Shapes.FormControlType.md)

Gets FormControl specific type.

#### Returns

[`FormControlType`](../enums/GC.Spread.Sheets.Shapes.FormControlType.md)

___

### <a id="getformula" name="getformula"></a> getFormula

▸ **getFormula**(`path`): `string`

通过路径从形状中获取公式字符串

**`代码示例`**
```
sheet.name("Sheet1");
sheet.setValue(0, 1, "This is a rectangle.");
var shape1 = sheet.shapes.add("myShape1", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 100, 100, 200, 200);
shape1.setFormula("text", "=Sheet1!B1");
shape1.getFormula("text");//返回 "=Sheet1!B1"
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `path` | `string` | 可以接收公式字符串的路径，可以是 "x", "y", "width", "height", "rotate", "text", "style.fill.color", "style.fill.transparency", "style.fill.src", "style.fill.tilePictureAsTexture", "style.fill.offsetLeft", "style.fill.offsetRight", "style.fill.offsetTop", "style.fill.offsetBottom", "style.fill.offsetX", "style.fill.offsetY", "style.fill.scaleX", "style.fill.scaleY", "style.fill.alignment", "style.fill.mirrorType", "style.fill.type", "style.fill.angle", "style.fill.direction", "style.fill.stops.0.color", "style.fill.stops.0.position", "style.fill.stops.0.transparency", "style.fill.stops.0.brightness", "style.line.color", "style.line.lineStyle", "style.line.width", "style.line.capType", "style.line.joinType", "style.line.compoundType",  "style.line.transparency", "style.textEffect.color", "style.textEffect.transparency", "style.textEffect.font", "style.textFrame.vAlign", "style.textFrame.hAlign". |

#### Returns

`string`

通过路径从形状返回公式字符串

#### Inherited from

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[getFormula](GC.Spread.Sheets.Shapes.Shape.md#getformula)

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

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[height](GC.Spread.Sheets.Shapes.Shape.md#height)

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

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[hyperlink](GC.Spread.Sheets.Shapes.Shape.md#hyperlink)

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

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[isLocked](GC.Spread.Sheets.Shapes.Shape.md#islocked)

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

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[isSelected](GC.Spread.Sheets.Shapes.Shape.md#isselected)

___

### <a id="istextbox" name="istextbox"></a> isTextBox

▸ **isTextBox**(`value?`): `boolean` \| `void`

设置形状为文本框

**`example`**
```
var rectangle = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 100, 60, 200, 160);
rectangle.isTextBox(true);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`boolean` \| `void`

如果未设值，返回形状是否是文本框

#### Inherited from

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[isTextBox](GC.Spread.Sheets.Shapes.Shape.md#istextbox)

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

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[isVisible](GC.Spread.Sheets.Shapes.Shape.md#isvisible)

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

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[name](GC.Spread.Sheets.Shapes.Shape.md#name)

___

### <a id="options" name="options"></a> options

▸ **options**(`v?`): [`IFormControlShapeOptions`](../modules/GC.Spread.Sheets.Shapes.md#iformcontrolshapeoptions)

Gets or Sets the options of form control shape.

#### Parameters

| Name | Type |
| :------ | :------ |
| `v?` | [`IFormControlShapeOptions`](../modules/GC.Spread.Sheets.Shapes.md#iformcontrolshapeoptions) |

#### Returns

[`IFormControlShapeOptions`](../modules/GC.Spread.Sheets.Shapes.md#iformcontrolshapeoptions)

___

### <a id="rotate" name="rotate"></a> rotate

▸ **rotate**(`value?`): `number` \| `void`

获取或设置形状的旋转角度(以度为单位)

**`代码示例`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.rotate();
heart.rotate(n + 30);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` \| `number` | 由数字或公式(以=开头)的形状(以度为单位)的旋转角度可以设置数字值 |

#### Returns

`number` \| `void`

如果未设置任何值，则返回形状的旋转角度(以度为单位)

#### Inherited from

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[rotate](GC.Spread.Sheets.Shapes.Shape.md#rotate)

___

### <a id="setformula" name="setformula"></a> setFormula

▸ **setFormula**(`path`, `formula`): `void`

通过路径将公式字符串设置为形状

**`代码示例`**
```
sheet.name("Sheet1");
sheet.setValue(0, 1, "This is a rectangle.");
var shape1 = sheet.shapes.add("myShape1", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 100, 100, 200, 200);
shape1.setFormula("text", "=Sheet1!B1");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `path` | `string` | 可以接收公式字符串的路径，可以是 "x", "y", "width", "height", "rotate", "text", "style.fill.color", "style.fill.transparency", "style.fill.src", "style.fill.tilePictureAsTexture", "style.fill.offsetLeft", "style.fill.offsetRight", "style.fill.offsetTop", "style.fill.offsetBottom", "style.fill.offsetX", "style.fill.offsetY", "style.fill.scaleX", "style.fill.scaleY", "style.fill.alignment", "style.fill.mirrorType", "style.fill.type", "style.fill.angle", "style.fill.direction", "style.fill.stops.0.color", "style.fill.stops.0.position", "style.fill.stops.0.transparency", "style.fill.stops.0.brightness", "style.line.color", "style.line.lineStyle", "style.line.width", "style.line.capType", "style.line.joinType", "style.line.compoundType", "style.line.transparency", "style.textEffect.color", "style.textEffect.transparency", "style.textEffect.font", "style.textFrame.vAlign", "style.textFrame.hAlign". |
| `formula` | `string` | 公式字符串 |

#### Returns

`void`

#### Inherited from

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[setFormula](GC.Spread.Sheets.Shapes.Shape.md#setformula)

___

### <a id="showhandle" name="showhandle"></a> showHandle

▸ **showHandle**(`value?`): `any`

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

`any`

如果未设置任何值，则返回是否显示形状句柄的设置

#### Inherited from

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[showHandle](GC.Spread.Sheets.Shapes.Shape.md#showhandle)

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

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[startColumn](GC.Spread.Sheets.Shapes.Shape.md#startcolumn)

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

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[startColumnOffset](GC.Spread.Sheets.Shapes.Shape.md#startcolumnoffset)

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

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[startRow](GC.Spread.Sheets.Shapes.Shape.md#startrow)

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

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[startRowOffset](GC.Spread.Sheets.Shapes.Shape.md#startrowoffset)

___

### <a id="style" name="style"></a> style

▸ **style**(`value?`): `any`

获取或设置形状的样式

**`代码示例`**
```
//本示例设置形状的样式
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
| `value?` | [`ShapeStyle`](GC.Spread.Sheets.Shapes.ShapeStyle.md) | 形状样式 |

#### Returns

`any`

如果未设置值，则返回形状的当前样式

#### Inherited from

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[style](GC.Spread.Sheets.Shapes.Shape.md#style)

___

### <a id="text" name="text"></a> text

▸ **text**(`value?`): `any`

获取或设置形状的文本

**`代码示例`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
heart.text("My Shape");
var s = heart.text();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 由字符串或公式(以=开头)的形状的文本可以获取字符串 |

#### Returns

`any`

如果未设置任何值，则返回形状的文本

#### Inherited from

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[text](GC.Spread.Sheets.Shapes.Shape.md#text)

___

### <a id="type" name="type"></a> type

▸ **type**(`value?`): `any`

获取或设置形状的类型

**`代码示例`**
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var n = heart.type();
heart.type(GC.Spread.Sheets.Shapes.AutoShapeType.cloud);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`AutoShapeType`](../enums/GC.Spread.Sheets.Shapes.AutoShapeType.md) | 形状的类型 |

#### Returns

`any`

如果未设置任何值，则返回形状的类型

#### Inherited from

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[type](GC.Spread.Sheets.Shapes.Shape.md#type)

___

### <a id="value" name="value"></a> value

▸ **value**(`v?`): [`IFormControlShapeValue`](../modules/GC.Spread.Sheets.Shapes.md#iformcontrolshapevalue)

Gets or Sets the value of form control shape.

#### Parameters

| Name | Type |
| :------ | :------ |
| `v?` | [`IFormControlShapeValue`](../modules/GC.Spread.Sheets.Shapes.md#iformcontrolshapevalue) |

#### Returns

[`IFormControlShapeValue`](../modules/GC.Spread.Sheets.Shapes.md#iformcontrolshapevalue)

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

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[width](GC.Spread.Sheets.Shapes.Shape.md#width)

___

### <a id="x" name="x"></a> x

▸ **x**(`value?`): `any`

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

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[x](GC.Spread.Sheets.Shapes.Shape.md#x)

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

[Shape](GC.Spread.Sheets.Shapes.Shape.md).[y](GC.Spread.Sheets.Shapes.Shape.md#y)
