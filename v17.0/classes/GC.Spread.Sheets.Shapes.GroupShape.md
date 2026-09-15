# Class: GroupShape

[Sheets](../modules/GC.Spread.Sheets.md).[Shapes](../modules/GC.Spread.Sheets.Shapes.md).GroupShape

## Hierarchy

- [`ShapeBase`](GC.Spread.Sheets.Shapes.ShapeBase.md)

  ↳ **`GroupShape`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Shapes.GroupShape.md#constructor)

### Methods

- [add](GC.Spread.Sheets.Shapes.GroupShape.md#add)
- [all](GC.Spread.Sheets.Shapes.GroupShape.md#all)
- [allowMove](GC.Spread.Sheets.Shapes.GroupShape.md#allowmove)
- [allowResize](GC.Spread.Sheets.Shapes.GroupShape.md#allowresize)
- [allowRotate](GC.Spread.Sheets.Shapes.GroupShape.md#allowrotate)
- [alt](GC.Spread.Sheets.Shapes.GroupShape.md#alt)
- [canPrint](GC.Spread.Sheets.Shapes.GroupShape.md#canprint)
- [dynamicMove](GC.Spread.Sheets.Shapes.GroupShape.md#dynamicmove)
- [dynamicSize](GC.Spread.Sheets.Shapes.GroupShape.md#dynamicsize)
- [endColumn](GC.Spread.Sheets.Shapes.GroupShape.md#endcolumn)
- [endColumnOffset](GC.Spread.Sheets.Shapes.GroupShape.md#endcolumnoffset)
- [endRow](GC.Spread.Sheets.Shapes.GroupShape.md#endrow)
- [endRowOffset](GC.Spread.Sheets.Shapes.GroupShape.md#endrowoffset)
- [find](GC.Spread.Sheets.Shapes.GroupShape.md#find)
- [getFormula](GC.Spread.Sheets.Shapes.GroupShape.md#getformula)
- [height](GC.Spread.Sheets.Shapes.GroupShape.md#height)
- [hyperlink](GC.Spread.Sheets.Shapes.GroupShape.md#hyperlink)
- [isLocked](GC.Spread.Sheets.Shapes.GroupShape.md#islocked)
- [isSelected](GC.Spread.Sheets.Shapes.GroupShape.md#isselected)
- [isVisible](GC.Spread.Sheets.Shapes.GroupShape.md#isvisible)
- [name](GC.Spread.Sheets.Shapes.GroupShape.md#name)
- [remove](GC.Spread.Sheets.Shapes.GroupShape.md#remove)
- [rotate](GC.Spread.Sheets.Shapes.GroupShape.md#rotate)
- [setFormula](GC.Spread.Sheets.Shapes.GroupShape.md#setformula)
- [showHandle](GC.Spread.Sheets.Shapes.GroupShape.md#showhandle)
- [startColumn](GC.Spread.Sheets.Shapes.GroupShape.md#startcolumn)
- [startColumnOffset](GC.Spread.Sheets.Shapes.GroupShape.md#startcolumnoffset)
- [startRow](GC.Spread.Sheets.Shapes.GroupShape.md#startrow)
- [startRowOffset](GC.Spread.Sheets.Shapes.GroupShape.md#startrowoffset)
- [width](GC.Spread.Sheets.Shapes.GroupShape.md#width)
- [x](GC.Spread.Sheets.Shapes.GroupShape.md#x)
- [y](GC.Spread.Sheets.Shapes.GroupShape.md#y)
- [zIndex](GC.Spread.Sheets.Shapes.GroupShape.md#zindex)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new GroupShape**(`worksheet`, `name?`)

组合形状

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `worksheet` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 组合形状的宿主表 |
| `name?` | `string` | - |

#### Overrides

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[constructor](GC.Spread.Sheets.Shapes.ShapeBase.md#constructor)

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`shape`): `void`

向组合形状添加形状

**`example`**
```
var shape1 = activeSheet.shapes.add("shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 50, 100, 150);
var shape2 = activeSheet.shapes.add("shape2", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 260, 50, 100, 150);
var groupShape = activeSheet.shapes.group([shape1, shape2]);
var shape3 = activeSheet.shapes.add("shape3", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 260, 100, 150);
// add shape3 to groupShape.
groupShape.add(shape3);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `shape` | [`Shape`](GC.Spread.Sheets.Shapes.Shape.md) | 添加到组形状的形状 |

#### Returns

`void`

___

### <a id="all" name="all"></a> all

▸ **all**(): [`Shape`](GC.Spread.Sheets.Shapes.Shape.md)[]

得到组合形状的所有形状

**`代码示例`**
```
// 本示例演示如何将所有形状组合为组合形状
var shape1 = sheet.shapes.add("myShape1", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 62 * 9, 0, 200, 200);
var shape2 = sheet.shapes.add("myShape2", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 20, 20, 200, 200);
var groupShape = sheet.shapes.group([shape1, shape2]);
var shapes = groupShape.all();
```

#### Returns

[`Shape`](GC.Spread.Sheets.Shapes.Shape.md)[]

所有形状

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

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

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

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置任何值，则返回此形状是否可打印

#### Inherited from

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[canPrint](GC.Spread.Sheets.Shapes.ShapeBase.md#canprint)

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

### <a id="find" name="find"></a> find

▸ **find**(`name`): [`Shape`](GC.Spread.Sheets.Shapes.Shape.md)

通过名称获取组合形状中的形状

**`example`**
```
var shape1 = activeSheet.shapes.add("heart1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 50, 100, 150);
var shape2 = activeSheet.shapes.add("heart2", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 260, 50, 100, 150);
var groupShape = activeSheet.shapes.group([shape1, shape2]);
var heart1 = groupShape.find("heart1"); // heart1 is equal to shape1.
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name?` | `string` | 组合形状中形状的名称 |

#### Returns

[`Shape`](GC.Spread.Sheets.Shapes.Shape.md)

如果名称属于组合形状的形状则返回一个Shape实例,;否则为`null`

___

### <a id="getformula" name="getformula"></a> getFormula

▸ **getFormula**(`path`): `string`

通过路径从形状中获取公式字符串

**`代码示例`**
```
sheet.name("Sheet1");
sheet.setValue(0, 1, 30);
var shape1 = sheet.shapes.add("myShape1", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 62 * 9, 0, 200, 200);
var shape2 = sheet.shapes.add("myShape2", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 20, 20, 200, 200);
var shape = sheet.shapes.group([shape1, shape2]);
shape.setFormula("rotate", "=Sheet1!B1");
shape.getFormula("rotate");//returns "=Sheet1!B1"
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `path` | `string` | 可以接收公式字符串的路径，可以是"x","y","width","height","rotate"之一 |

#### Returns

`string`

通过路径从形状返回公式字符串

#### Overrides

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

### <a id="remove" name="remove"></a> remove

▸ **remove**(`shape`): `void`

从组合形状中删除形状

**`example`**
```
var shape1 = activeSheet.shapes.add("shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 50, 100, 150);
var shape2 = activeSheet.shapes.add("shape2", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 260, 50, 100, 150);
var shape3 = activeSheet.shapes.add("shape3", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 260, 100, 150);
var groupShape = activeSheet.shapes.group([shape1, shape2, shape3]);
// remove shape3 from groupShape.
groupShape.remove(shape3);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `shape` | [`Shape`](GC.Spread.Sheets.Shapes.Shape.md) | 要从组形状中删除的形状 |

#### Returns

`void`

___

### <a id="rotate" name="rotate"></a> rotate

▸ **rotate**(`value?`): `number` \| `void`

获取或设置组合形状的旋转角度

**`代码示例`**
```
var shape1 = sheet.shapes.add("myShape1", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 62 * 9, 0, 200, 200);
var shape2 = sheet.shapes.add("myShape2", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 20, 20, 200, 200);
var shape = sheet.shapes.group([shape1, shape2]);
shape.rotate(60);
var angle = shape.rotate();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` \| `number` | 组合形状的旋转角度 |

#### Returns

`number` \| `void`

如果参数'value'为null或undefined,它将返回组合形状的旋转角度

___

### <a id="setformula" name="setformula"></a> setFormula

▸ **setFormula**(`path`, `formula`): `void`

通过路径将公式字符串设置为形状

**`代码示例`**
```
sheet.name("Sheet1");
sheet.setValue(0, 1, 30);
var shape1 = sheet.shapes.add("myShape1", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 62 * 9, 0, 200, 200);
var shape2 = sheet.shapes.add("myShape2", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 20, 20, 200, 200);
var shape = sheet.shapes.group([shape1, shape2]);
shape.setFormula("rotate", "=Sheet1!B1");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `path` | `string` | 可以接收公式字符串的路径，可以是"x","y","width","height","rotate"之一 |
| `formula` | `string` | 公式字符串 |

#### Returns

`void`

#### Overrides

[ShapeBase](GC.Spread.Sheets.Shapes.ShapeBase.md).[setFormula](GC.Spread.Sheets.Shapes.ShapeBase.md#setformula)

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

___

### <a id="zindex" name="zindex"></a> zIndex

▸ **zIndex**(`shapeName`, `zIndex?`): `any`

 获取或设置组合形状中形状的z-index

**`代码示例`**
```
//本示例显示了如何在组合形状中使用z-Index
var shape1 = activeSheet.shapes.add("shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 50, 100, 150);
var shape2 = activeSheet.shapes.add("shape2", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 150, 50, 100, 150);
var style = shape1.style();
style.fill.color = "red";
shape1.style(style);
var myGroup = activeSheet.shapes.group([shape1, shape2]);
myGroup.zIndex("shape2"); // 1
myGroup.zIndex("shape2", 0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `shapeName` | `string` | 形状的名称 |
| `zIndex?` | `number` | 形状的Z-indexz-Index应该在0到所有形状长度(不包含)之间 z-Index较大的形状始终在z-Index较低的形状之前 |

#### Returns

`any`
