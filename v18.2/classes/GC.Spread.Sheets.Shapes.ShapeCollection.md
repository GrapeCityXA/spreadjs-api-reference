# Class: ShapeCollection

[Sheets](../modules/GC.Spread.Sheets.md).[Shapes](../modules/GC.Spread.Sheets.Shapes.md).ShapeCollection

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Shapes.ShapeCollection.md#constructor)

### Methods

- [add](GC.Spread.Sheets.Shapes.ShapeCollection.md#add)
- [addCameraShape](GC.Spread.Sheets.Shapes.ShapeCollection.md#addcamerashape)
- [addConnector](GC.Spread.Sheets.Shapes.ShapeCollection.md#addconnector)
- [addFormControl](GC.Spread.Sheets.Shapes.ShapeCollection.md#addformcontrol)
- [addPictureShape](GC.Spread.Sheets.Shapes.ShapeCollection.md#addpictureshape)
- [all](GC.Spread.Sheets.Shapes.ShapeCollection.md#all)
- [clear](GC.Spread.Sheets.Shapes.ShapeCollection.md#clear)
- [get](GC.Spread.Sheets.Shapes.ShapeCollection.md#get)
- [group](GC.Spread.Sheets.Shapes.ShapeCollection.md#group)
- [remove](GC.Spread.Sheets.Shapes.ShapeCollection.md#remove)
- [snapMode](GC.Spread.Sheets.Shapes.ShapeCollection.md#snapmode)
- [ungroup](GC.Spread.Sheets.Shapes.ShapeCollection.md#ungroup)
- [zIndex](GC.Spread.Sheets.Shapes.ShapeCollection.md#zindex)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new ShapeCollection**(`sheet`)

表示一个管理工作表中所有形状的形状管理器。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheet` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 工作表。 |

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`name`, `autoShapeTypeOrModel`, `left?`, `top?`, `width?`, `height?`): [`Shape`](GC.Spread.Sheets.Shapes.Shape.md)

向形状集合中添加新形状

**`example`**
```
// 此示例展示如何添加新形状
var shape = activeSheet.shapes.add("shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 50, 100, 150);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 形状的名称。如果名称为空字符串，将生成一个唯一名称。 |
| `autoShapeTypeOrModel` | [`IShapeModel`](../interfaces/GC.Spread.Sheets.Shapes.IShapeModel.md) \| [`AutoShapeType`](../enums/GC.Spread.Sheets.Shapes.AutoShapeType.md) | 形状的类型（用于内置类型之一）或自定义形状的模型。 |
| `left?` | `number` | - |
| `top?` | `number` | - |
| `width?` | `number` | - |
| `height?` | `number` | - |

#### Returns

[`Shape`](GC.Spread.Sheets.Shapes.Shape.md)

已添加到工作表中的形状。

___

### <a id="addcamerashape" name="addcamerashape"></a> addCameraShape

▸ **addCameraShape**(`name`, `range`, `left?`, `top?`, `width?`, `height?`): [`CameraShape`](GC.Spread.Sheets.Shapes.CameraShape.md)

向形状集合中添加新的相机形状

**`example`**
```
// 此示例展示如何添加新的相机形状
var shape = activeSheet.shapes.addCameraShape("camera shape 1", 'Sheet1!A1:A8', 100, 50, 100, 150);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 相机形状的名称。如果名称为空字符串，将生成一个唯一名称。 |
| `range` | `string` | 生成形状的范围，应该是一个范围公式，如Sheet1!A1:A8。 |
| `left?` | `number` | - |
| `top?` | `number` | - |
| `width?` | `number` | - |
| `height?` | `number` | - |

#### Returns

[`CameraShape`](GC.Spread.Sheets.Shapes.CameraShape.md)

已添加到工作表中的形状。

___

### <a id="addconnector" name="addconnector"></a> addConnector

▸ **addConnector**(`name`, `connectorType`, `beginX?`, `beginY?`, `endX?`, `endY?`): [`ConnectorShape`](GC.Spread.Sheets.Shapes.ConnectorShape.md)

向形状集合中添加连接器形状

**`example`**
```
// 此示例展示如何添加连接器形状
var shape1 = activeSheet.shapes.addConnector("shape1", GC.Spread.Sheets.Shapes.ConnectorType.elbow, 200, 50, 300, 200);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 形状的名称。如果名称为空字符串，将生成一个唯一名称。 |
| `connectorType` | [`ConnectorType`](../enums/GC.Spread.Sheets.Shapes.ConnectorType.md) | 连接器的类型。 |
| `beginX?` | `number` | - |
| `beginY?` | `number` | - |
| `endX?` | `number` | - |
| `endY?` | `number` | - |

#### Returns

[`ConnectorShape`](GC.Spread.Sheets.Shapes.ConnectorShape.md)

已添加到工作表中的连接器形状。

___

### <a id="addformcontrol" name="addformcontrol"></a> addFormControl

▸ **addFormControl**(`name`, `formControlType`, `left?`, `top?`, `width?`, `height?`): [`FormControlShape`](GC.Spread.Sheets.Shapes.FormControlShape.md)

向形状集合中添加新的表单控件形状

**`example`**
```
// 此示例展示如何添加新的表单控件形状
var shape = activeSheet.shapes.addFormControl("spinButton", GC.Spread.Sheets.Shapes.FormControlType.spinButton, 100, 50, 100, 50);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 形状的名称。如果名称为空字符串，将生成一个唯一名称。 |
| `formControlType` | [`FormControlType`](../enums/GC.Spread.Sheets.Shapes.FormControlType.md) | 表单控件形状的类型 |
| `left?` | `number` | - |
| `top?` | `number` | - |
| `width?` | `number` | - |
| `height?` | `number` | - |

#### Returns

[`FormControlShape`](GC.Spread.Sheets.Shapes.FormControlShape.md)

已添加到工作表中的表单控件形状。

___

### <a id="addpictureshape" name="addpictureshape"></a> addPictureShape

▸ **addPictureShape**(`name`, `src`, `left?`, `top?`, `width?`, `height?`): [`PictureShape`](GC.Spread.Sheets.Shapes.PictureShape.md)

向形状集合中添加新的图片形状

**`example`**
```
// 此示例展示如何添加新的图片形状
var shape = activeSheet.shapes.addPictureShape("Picture 1", "data:image/svg+xml;base64.....", 100, 50, 100, 100);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 形状的名称。如果名称为空字符串，将生成一个唯一名称。 |
| `src` | `string` | 图片的源地址。 |
| `left?` | `number` | - |
| `top?` | `number` | - |
| `width?` | `number` | - |
| `height?` | `number` | - |

#### Returns

[`PictureShape`](GC.Spread.Sheets.Shapes.PictureShape.md)

已添加到工作表中的图片形状。

___

### <a id="all" name="all"></a> all

▸ **all**(): [`Shape`](GC.Spread.Sheets.Shapes.Shape.md)[]

获取所有形状

**`example`**
```
// 此示例展示如何获取形状集合中的所有形状
activeSheet.shapes.add("shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 50, 100, 150);
activeSheet.shapes.addConnector("shape2", GC.Spread.Sheets.Shapes.ConnectorType.elbow, 200, 50, 300, 200);
var shapes = activeSheet.shapes.all();
```

#### Returns

[`Shape`](GC.Spread.Sheets.Shapes.Shape.md)[]

所有形状

___

### <a id="clear" name="clear"></a> clear

▸ **clear**(): `void`

清除所有形状

**`example`**
```
// 此示例展示如何清除形状集合中的所有形状
activeSheet.shapes.add("shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 50, 100, 150);
activeSheet.shapes.addConnector("shape2", GC.Spread.Sheets.Shapes.ConnectorType.elbow, 200, 50, 300, 200);
activeSheet.shapes.clear();
```

#### Returns

`void`

___

### <a id="get" name="get"></a> get

▸ **get**(`name`): [`Shape`](GC.Spread.Sheets.Shapes.Shape.md)

通过名称获取形状

**`example`**
```
// 此示例展示如何通过名称获取形状
activeSheet.shapes.add("shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 50, 100, 150);
activeSheet.shapes.get("shape1");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 形状的名称。 |

#### Returns

[`Shape`](GC.Spread.Sheets.Shapes.Shape.md)

形状对象

___

### <a id="group" name="group"></a> group

▸ **group**(`shapes`): [`GroupShape`](GC.Spread.Sheets.Shapes.GroupShape.md)

将形状组合成组

**`example`**
```
// 此示例展示如何将形状组合成组
var shape1 = activeSheet.shapes.add("shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 50, 100, 150);
var shape2 = activeSheet.shapes.addConnector("shape2", GC.Spread.Sheets.Shapes.ConnectorType.elbow, 200, 50, 300, 200);
var shapes = [shape1, shape2];
var groupShape = activeSheet.shapes.group(shapes)
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `shapes` | [`Shape`](GC.Spread.Sheets.Shapes.Shape.md)[] | 要组合的形状数组。 |

#### Returns

[`GroupShape`](GC.Spread.Sheets.Shapes.GroupShape.md)

形状组

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`name`): `void`

移除形状

**`example`**
```
// 此示例展示如何移除形状
activeSheet.shapes.add("shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 50, 100, 150);
activeSheet.shapes.remove("shape1");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 形状的名称。 |

#### Returns

`void`

___

### <a id="snapmode" name="snapmode"></a> snapMode

▸ **snapMode**(`value?`): `void` \| [`SnapMode`](../enums/GC.Spread.Sheets.Shapes.SnapMode.md)

获取或设置是否将形状对齐到网格线或其他形状

**`example`**
```
sheet1.shapes.SnapMode(GC.Spread.Sheets.Shapes.SnapMode.grid);
var snapMode = sheet1.shapes.snapMode();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SnapMode`](../enums/GC.Spread.Sheets.Shapes.SnapMode.md) | 是否将形状对齐到网格线或其他形状。 |

#### Returns

`void` \| [`SnapMode`](../enums/GC.Spread.Sheets.Shapes.SnapMode.md)

如果未设置值，返回当前使用的对齐模式。

___

### <a id="ungroup" name="ungroup"></a> ungroup

▸ **ungroup**(`groupShape`): `void`

将形状组拆分为多个形状

**`example`**
```
// 此示例展示如何将形状组拆分为多个形状
var shape1 = activeSheet.shapes.add("shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 50, 100, 150);
var shape2 = activeSheet.shapes.addConnector("shape2", GC.Spread.Sheets.Shapes.ConnectorType.elbow, 200, 50, 300, 200);
var shapes = [shape1, shape2];
var groupShape = activeSheet.shapes.group(shapes);
activeSheet.shapes.ungroup(groupShape);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `groupShape` | [`GroupShape`](GC.Spread.Sheets.Shapes.GroupShape.md) | 要拆分的形状组。 |

#### Returns

`void`

___

### <a id="zindex" name="zindex"></a> zIndex

▸ **zIndex**(`shapeName`, `zIndex`): `number`

获取或设置形状的z-index值

**`example`**
```
// 此示例展示如何使用zIndex
var shape1 = activeSheet.shapes.add("shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 50, 100, 150);
var style = shape1.style();
style.fill.color = "red";
shape1.style(style);
var shape2 = activeSheet.shapes.addConnector("shape2", GC.Spread.Sheets.Shapes.ConnectorType.elbow, 100, 50, 200, 200);
activeSheet.shapes.zIndex("shape2"); // 1
activeSheet.shapes.zIndex("shape2", 0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `shapeName` | `string` | 形状的名称 |
| `zIndex` | `number` | 形状的z-index值。zIndex应该在0到所有形状数量之间（不包含）。zIndex值较大的形状始终显示在zIndex值较小的形状前面。 |

#### Returns

`number`
