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
- [toImageSrc](GC.Spread.Sheets.Shapes.CameraShape.md#toimagesrc)
- [toImageSrcAsync](GC.Spread.Sheets.Shapes.CameraShape.md#toimagesrcasync)
- [width](GC.Spread.Sheets.Shapes.CameraShape.md#width)
- [x](GC.Spread.Sheets.Shapes.CameraShape.md#x)
- [y](GC.Spread.Sheets.Shapes.CameraShape.md#y)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new CameraShape**(`worksheet`, `name`, `range`, `left?`, `top?`, `width?`, `height?`)

用于将工作表中指定单元格区域的内容投影为图像快照，并以独立形状对象的形式进行展示。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `worksheet` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 形状所在的宿主工作表。 |
| `name` | `string` | 照相机形状的名称。如果名称为空字符串，将自动生成唯一名称。 |
| `range` | `string` | 用于生成形状的单元格区域，需传入区域公式（例如 Sheet1!A1:A8）。 |
| `left?` | `number` | - |
| `top?` | `number` | - |
| `width?` | `number` | - |
| `height?` | `number` | - |

#### Overrides

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[constructor](GC.Spread.Sheets.Shapes.ShapeBase.md#constructor)

## Methods

### <a id="allowmove" name="allowmove"></a> allowMove

▸ **allowMove**(`value?`): `any`

获取或设置是否禁用移动形状。

**`example`**
```
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
```
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
```
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
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
heart.alt("一个心形");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

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
```
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var state = heart.canPrint(); // 获取形状是否可打印，默认值为 true.
workbook.print(); // 心形被打印。
heart.canPrint(false);
workbook.print(); // 心形不被打印。
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置值，返回此形状是否可打印。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[canPrint](GC.Spread.Sheets.Shapes.ShapeBase.md#canprint)

___

### <a id="doubleclickcommand" name="doubleclickcommand"></a> doubleClickCommand

▸ **doubleClickCommand**(`value?`): `string` \| `void` \| `Function`

获取或设置形状的双击命令。

**`example`**
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

未设置值时，返回形状当前的双击命令设置。

___

### <a id="dynamicmove" name="dynamicmove"></a> dynamicMove

▸ **dynamicMove**(`value?`): `any`

获取或设置形状在隐藏或显示、调整大小或移动行或列时是否移动。

**`example`**
```
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
```
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
```
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
```
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
```
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
```
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
```
sheet.name("Sheet1");
sheet.setValue(0, 1, 150);
var shape1 = sheet.shapes.add("myShape1", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 100, 100, 200, 200);
shape1.setFormula("x", "=Sheet1!B1");
shape1.getFormula("x");//returns "=Sheet1!B1"
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `path` | `string` | 可以接受公式字符串的路径，可以是以下之一："x", "y", "width", "height"。 |

#### Returns

`string`

返回通过路径获取的形状公式字符串。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[getFormula](GC.Spread.Sheets.Shapes.ShapeBase.md#getformula)

___

### <a id="height" name="height"></a> height

▸ **height**(`value?`): `any`

获取或设置形状的高度。

**`example`**
```
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
```
var shape = sheet.shapes.add("myShape", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 62 * 9, 0, 200, 200);
shape.hyperlink({url: "http://www.spreadjs.com", target: 0, tooltip: 'goes to SpreadJS'});
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`IHyperlink`](../interfaces/GC.Spread.Sheets.IHyperlink.md) |

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
```
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
```
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

### <a id="isvisible" name="isvisible"></a> isVisible

▸ **isVisible**(`value?`): `any`

获取或设置此形状是否可见。

**`example`**
```
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
| `value?` | `string` | 形状的名称。 |

#### Returns

`any`

如果未设置值，返回形状的名称。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[name](GC.Spread.Sheets.Shapes.ShapeBase.md#name)

___

### <a id="range" name="range"></a> range

▸ **range**(`value?`): `string` \| `void`

获取或设置照相机形状的单元格区域。

**`example`**
```
var shape = sheet.shapes.addCameraShape("shape1", 'Sheet1!A1:A8', 100, 50, 100, 150);
shape.range('Sheet2!A2:B8');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 由单元格区域公式指定的照相机形状区域（如Sheet1!A1:A8）。 |

#### Returns

`string` \| `void`

未设置值时，返回照相机形状的单元格区域。

___

### <a id="rotate" name="rotate"></a> rotate

▸ **rotate**(`value?`): `number` \| `void`

获取或设置照相机形状的旋转角度（单位：度）。

**`example`**
```
var shape = sheet.shapes.addCameraShape("shape1", 'Sheet1!A1:A8', 100, 50, 100, 150);
var n = shape.rotate();
shape.rotate(n + 30);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` \| `number` | 旋转角度（单位：度），可通过数值或公式（以=开头，返回数值）指定。 |

#### Returns

`number` \| `void`

未设置值时，返回照相机形状的旋转角度（单位：度）。

___

### <a id="setformula" name="setformula"></a> setFormula

▸ **setFormula**(`path`, `formula`): `void`

通过路径设置形状的公式字符串。

**`example`**
```
sheet.name("Sheet1");
sheet.setValue(0, 1, 150);
var shape1 = sheet.shapes.add("myShape1", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 100, 100, 200, 200);
shape1.setFormula("x", "=Sheet1!B1");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `path` | `string` | 可以接受公式字符串的路径，可以是以下之一："x", "y", "width", "height"。 |
| `formula` | `string` | 公式字符串。 |

#### Returns

`void`

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[setFormula](GC.Spread.Sheets.Shapes.ShapeBase.md#setformula)

___

### <a id="showhandle" name="showhandle"></a> showHandle

▸ **showHandle**(`value?`): `any`

获取或设置是否显示形状的控制柄。

**`example`**
```
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
```
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
```
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
```
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
```
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

获取或设置照相机形状的样式。

**`example`**
```
// 此示例为形状设置样式。
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
| `value?` | [`ShapeStyle`](GC.Spread.Sheets.Shapes.ShapeStyle.md) | 形状样式。 |

#### Returns

`any`

未设置值时，返回形状的当前样式。

___

### <a id="toimagesrc" name="toimagesrc"></a> toImageSrc

▸ **toImageSrc**(): `string`

获取形状的Base64字符串类型的图片源。

**`example`**
```
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
```
let shapeImageSrc = await sheet.shapes.all()[0].toImageSrcAsync();
```

#### Returns

`Promise`<`string`\>

返回形状的Base64字符串类型的图片源。

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[toImageSrcAsync](GC.Spread.Sheets.Shapes.ShapeBase.md#toimagesrcasync)

___

### <a id="width" name="width"></a> width

▸ **width**(`value?`): `any`

获取或设置形状的宽度。

**`example`**
```
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
```
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
```
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
