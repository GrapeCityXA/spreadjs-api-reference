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

形状管理器，用于管理表单中的所有形状

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheet` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 表单 |

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`name`, `autoShapeTypeOrModel`, `left?`, `top?`, `width?`, `height?`): [`Shape`](GC.Spread.Sheets.Shapes.Shape.md)

向形状集合添加新形状

**`代码示例`**
```
// 本示例说明如何添加新形状
var shape = activeSheet.shapes.add("shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 50, 100, 150);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 形状的名称 如果保留空白，将生成一个唯一的名称 |
| `autoShapeTypeOrModel` | [`IShapeModel`](../interfaces/GC.Spread.Sheets.Shapes.IShapeModel.md) \| [`AutoShapeType`](../enums/GC.Spread.Sheets.Shapes.AutoShapeType.md) | 形状的类型(对于一种建筑物类型)或自定义形状的模型 |
| `left?` | `number` | 形状的<i>x</i>位置 |
| `top?` | `number` | 形状的<i>y</i>位置 |
| `width?` | `number` | 形状的宽度 |
| `height?` | `number` | 形状的高度 |

#### Returns

[`Shape`](GC.Spread.Sheets.Shapes.Shape.md)

已添加到表的形状

___

### <a id="addcamerashape" name="addcamerashape"></a> addCameraShape

▸ **addCameraShape**(`name`, `range`, `left?`, `top?`, `width?`, `height?`): [`CameraShape`](GC.Spread.Sheets.Shapes.CameraShape.md)

将新快照形状添加到形状集合

**`代码示例`**
```
// 本示例演示如何添加新的快照形状
var shape = activeSheet.shapes.addCameraShape("camera shape 1", 'Sheet1!A1:A8', 100, 50, 100, 150);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 摄影机形状的名称.如果为空，将生成唯一名称 |
| `range` | `string` | 生成形状的区域，是一个区域公式，如Sheet1!A1:A8 |
| `left?` | `number` | - |
| `top?` | `number` | - |
| `width?` | `number` | - |
| `height?` | `number` | - |

#### Returns

[`CameraShape`](GC.Spread.Sheets.Shapes.CameraShape.md)

已添加到表的形状

___

### <a id="addconnector" name="addconnector"></a> addConnector

▸ **addConnector**(`name`, `connectorType`, `beginX?`, `beginY?`, `endX?`, `endY?`): [`ConnectorShape`](GC.Spread.Sheets.Shapes.ConnectorShape.md)

将连接器形状添加到形状集合

**`代码示例`**
```
//本示例说明如何添加连接器形状
var shape1 = activeSheet.shapes.addConnector("shape1", GC.Spread.Sheets.Shapes.ConnectorType.elbow, 200, 50, 300, 200);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 形状的名称 如果保留空白，将生成一个唯一的名称 |
| `connectorType` | [`ConnectorType`](../enums/GC.Spread.Sheets.Shapes.ConnectorType.md) | 连接器的类型 |
| `beginX?` | `number` | 连接器形状起点的x位置 |
| `beginY?` | `number` | 连接器形状起点的y位置 |
| `endX?` | `number` | 连接器形状终点的x位置 |
| `endY?` | `number` | 连接器形状终点的y位置 |

#### Returns

[`ConnectorShape`](GC.Spread.Sheets.Shapes.ConnectorShape.md)

已添加到表的连接器形状

___

### <a id="addformcontrol" name="addformcontrol"></a> addFormControl

▸ **addFormControl**(`name`, `formControlType`, `left?`, `top?`, `width?`, `height?`): [`FormControlShape`](GC.Spread.Sheets.Shapes.FormControlShape.md)

Add a new form control shape to shape collection

**`代码示例`**
```
// This example shows how to add a new form control shape
var shape = activeSheet.shapes.addFormControl("spinButton", GC.Spread.Sheets.Shapes.FormControlType.spinButton, 100, 50, 100, 50);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 形状的名称 如果保留空白，将生成一个唯一的名称 |
| `formControlType` | [`FormControlType`](../enums/GC.Spread.Sheets.Shapes.FormControlType.md) | The type of the form control shape |
| `left?` | `number` | The <i>x</i> location of the form control shape. |
| `top?` | `number` | The <i>y</i> location of the form control shape. |
| `width?` | `number` | The width of the form control shape. |
| `height?` | `number` | The height of the form control shape. |

#### Returns

[`FormControlShape`](GC.Spread.Sheets.Shapes.FormControlShape.md)

The from control shape that has been added to the sheet.

___

### <a id="addpictureshape" name="addpictureshape"></a> addPictureShape

▸ **addPictureShape**(`name`, `src`, `left?`, `top?`, `width?`, `height?`): [`PictureShape`](GC.Spread.Sheets.Shapes.PictureShape.md)

Add a new picture shape to shape collection

**`代码示例`**
```
// This example shows how to add a new picture shape
var shape = activeSheet.shapes.addPictureShape("Picture 1", "data:image/svg+xml;base64.....", 100, 50, 100, 100);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 形状的名称。 如果名称为空字符串，则会生成唯一的名称 |
| `src` | `string` | 图片的src |
| `left?` | `number` | - |
| `top?` | `number` | - |
| `width?` | `number` | - |
| `height?` | `number` | - |

#### Returns

[`PictureShape`](GC.Spread.Sheets.Shapes.PictureShape.md)

The picture shape that has been added to the sheet.

___

### <a id="all" name="all"></a> all

▸ **all**(): [`Shape`](GC.Spread.Sheets.Shapes.Shape.md)[]

获取所有形状

**`代码示例`**
```
// 本示例显示如何在形状集合中获取所有形状
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

**`代码示例`**
```
//本示例说明如何清除形状集合中的所有形状
activeSheet.shapes.add("shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 50, 100, 150);
activeSheet.shapes.addConnector("shape2", GC.Spread.Sheets.Shapes.ConnectorType.elbow, 200, 50, 300, 200);
activeSheet.shapes.clear();
```

#### Returns

`void`

___

### <a id="get" name="get"></a> get

▸ **get**(`name`): [`Shape`](GC.Spread.Sheets.Shapes.Shape.md)

通过名称设置形状

**`代码示例`**
```
//本示例说明如何获取具有名称的形状
activeSheet.shapes.add("shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 50, 100, 150);
activeSheet.shapes.get("shape1");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 形状的名称 |

#### Returns

[`Shape`](GC.Spread.Sheets.Shapes.Shape.md)

形状

___

### <a id="group" name="group"></a> group

▸ **group**(`shapes`): [`GroupShape`](GC.Spread.Sheets.Shapes.GroupShape.md)

对形状进行分组

**`代码示例`**
```
//本示例显示如何对一些形状进行分组
var shape1 = activeSheet.shapes.add("shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 50, 100, 150);
var shape2 = activeSheet.shapes.addConnector("shape2", GC.Spread.Sheets.Shapes.ConnectorType.elbow, 200, 50, 300, 200);
var shapes = [shape1, shape2];
var groupShape = activeSheet.shapes.group(shapes)
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `shapes` | [`Shape`](GC.Spread.Sheets.Shapes.Shape.md)[] | 要分组的形状 |

#### Returns

[`GroupShape`](GC.Spread.Sheets.Shapes.GroupShape.md)

形状组

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`name`): `void`

去除形状

**`代码示例`**
```
//本示例显示如何删除形状
activeSheet.shapes.add("shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 50, 100, 150);
activeSheet.shapes.remove("shape1");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 形状的名称 |

#### Returns

`void`

___

### <a id="snapmode" name="snapmode"></a> snapMode

▸ **snapMode**(`value?`): `void` \| [`SnapMode`](../enums/GC.Spread.Sheets.Shapes.SnapMode.md)

获取或设置是否将形状与网格线或其他形状对齐

**`代码示例`**
```
sheet1.shapes.SnapMode(GC.Spread.Sheets.Shapes.SnapMode.grid);
var snapMode = sheet1.shapes.snapMode();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SnapMode`](../enums/GC.Spread.Sheets.Shapes.SnapMode.md) | 是将吸附形状贴合到轴网线还是其他形状 |

#### Returns

`void` \| [`SnapMode`](../enums/GC.Spread.Sheets.Shapes.SnapMode.md)

如果未设置值，则返回snapMode

___

### <a id="ungroup" name="ungroup"></a> ungroup

▸ **ungroup**(`groupShape`): `void`

将形状组分离为某些形状

**`代码示例`**
```
//本示例显示如何将groupShape分离为某些形状
var shape1 = activeSheet.shapes.add("shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 50, 100, 150);
var shape2 = activeSheet.shapes.addConnector("shape2", GC.Spread.Sheets.Shapes.ConnectorType.elbow, 200, 50, 300, 200);
var shapes = [shape1, shape2];
var groupShape = activeSheet.shapes.group(shapes);
activeSheet.shapes.ungroup(groupShape);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `groupShape` | [`GroupShape`](GC.Spread.Sheets.Shapes.GroupShape.md) | 要分离的形状组 |

#### Returns

`void`

___

### <a id="zindex" name="zindex"></a> zIndex

▸ **zIndex**(`shapeName`, `zIndex`): `number`

 获取或设置形状的Z-index

**`代码示例`**
```
//本示例显示了如何使用Z-index
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
| `shapeName` | `string` | 形状名称 |
| `zIndex` | `number` | 形状的Z-indexz-Index应该在0到所有形状长度(不包含)之间 z-Index较大的形状始终在z-Index较低的形状之前 |

#### Returns

`number`
