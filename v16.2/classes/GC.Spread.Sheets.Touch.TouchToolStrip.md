# Class: TouchToolStrip

[Sheets](../modules/GC.Spread.Sheets.md).[Touch](../modules/GC.Spread.Sheets.Touch.md).TouchToolStrip

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Touch.TouchToolStrip.md#constructor)

### Methods

- [add](GC.Spread.Sheets.Touch.TouchToolStrip.md#add)
- [clear](GC.Spread.Sheets.Touch.TouchToolStrip.md#clear)
- [close](GC.Spread.Sheets.Touch.TouchToolStrip.md#close)
- [getItem](GC.Spread.Sheets.Touch.TouchToolStrip.md#getitem)
- [getItems](GC.Spread.Sheets.Touch.TouchToolStrip.md#getitems)
- [imageAreaHeight](GC.Spread.Sheets.Touch.TouchToolStrip.md#imageareaheight)
- [itemHeight](GC.Spread.Sheets.Touch.TouchToolStrip.md#itemheight)
- [itemWidth](GC.Spread.Sheets.Touch.TouchToolStrip.md#itemwidth)
- [open](GC.Spread.Sheets.Touch.TouchToolStrip.md#open)
- [remove](GC.Spread.Sheets.Touch.TouchToolStrip.md#remove)
- [separatorHeight](GC.Spread.Sheets.Touch.TouchToolStrip.md#separatorheight)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new TouchToolStrip**(`workbook`, `host`)

工具栏

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workbook` | [`Workbook`](GC.Spread.Sheets.Workbook.md) | Spread对象 |
| `host` | `HTMLElement` | 宿主DOM元素 |

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`item`): `void`

将项添加到触摸工具栏

**`remarks`** 要添加的项可以是工具栏项或行分隔符

**`代码示例`**
```
//本示例添加一个自定义项
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripItem("C", "Delete", "tsoutline.png", function(){ }))
spread.touchToolStrip.getItem("C").font("15px Arial").foreColor("red");
spread.touchToolStrip.imageAreaHeight(30);
spread.touchToolStrip.itemHeight(80);
spread.touchToolStrip.itemWidth(50);
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripSeparator());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | [`TouchToolStripSeparator`](GC.Spread.Sheets.Touch.TouchToolStripSeparator.md) \| [`TouchToolStripItem`](GC.Spread.Sheets.Touch.TouchToolStripItem.md) | 要添加的项 |

#### Returns

`void`

___

### <a id="clear" name="clear"></a> clear

▸ **clear**(): `void`

清除工具栏中的所有项

**`代码示例`**
```
//本示例使用clear方法
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripItem("C", "Delete", "tsoutline.png", function(){ }))
spread.touchToolStrip.getItem("C").font("15px Arial").foreColor("red");
spread.touchToolStrip.imageAreaHeight(30);
spread.touchToolStrip.itemHeight(80);
spread.touchToolStrip.itemWidth(50);
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripSeparator());
spread.touchToolStrip.clear();
```

#### Returns

`void`

___

### <a id="close" name="close"></a> close

▸ **close**(): `void`

关闭工具栏

#### Returns

`void`

___

### <a id="getitem" name="getitem"></a> getItem

▸ **getItem**(`name`): `any`

获取具有指定名称的项

**`代码示例`**
```
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripItem("Cut", "Delete", "cut.png", function(){ }))
spread.touchToolStrip.getItem("Cut").font("15px Arial").foreColor("red");
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripSeparator());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 项名称 |

#### Returns

`any`

如果该项存在于工具栏中,则返回该项;否则,返回undefined

___

### <a id="getitems" name="getitems"></a> getItems

▸ **getItems**(): `any`

获取属于工具栏的所有项

#### Returns

`any`

包含工具栏中所有项的数组

___

### <a id="imageareaheight" name="imageareaheight"></a> imageAreaHeight

▸ **imageAreaHeight**(`height?`): `any`

获取或设置图像区域的高度

**`代码示例`**
```
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripItem("C", "Delete", "tsoutline.png", function(){ }))
spread.touchToolStrip.getItem("C").font("15px Arial").foreColor("red");
spread.touchToolStrip.imageAreaHeight(30);
spread.touchToolStrip.itemHeight(80);
spread.touchToolStrip.itemWidth(50);
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripSeparator());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `height?` | `number` | 图像区域的高度 |

#### Returns

`any`

如果未设置任何值,则返回图像区域的高度;否则,返回工具栏

___

### <a id="itemheight" name="itemheight"></a> itemHeight

▸ **itemHeight**(`height?`): `any`

获取或设置工具栏项的高度

**`代码示例`**
```
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripItem("C", "Delete", "tsoutline.png", function(){ }))
spread.touchToolStrip.getItem("C").font("15px Arial").foreColor("red");
spread.touchToolStrip.imageAreaHeight(30);
spread.touchToolStrip.itemHeight(80);
spread.touchToolStrip.itemWidth(50);
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripSeparator());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `height?` | `number` | 工具栏项的高度 |

#### Returns

`any`

如果未设置任何值,则返回工具栏项的高度;否则,返回工具栏

___

### <a id="itemwidth" name="itemwidth"></a> itemWidth

▸ **itemWidth**(`width?`): `any`

获取或设置工具栏项的宽度

**`代码示例`**
```
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripItem("C", "Delete", "tsoutline.png", function(){ }))
spread.touchToolStrip.getItem("C").font("15px Arial").foreColor("red");
spread.touchToolStrip.imageAreaHeight(30);
spread.touchToolStrip.itemHeight(80);
spread.touchToolStrip.itemWidth(50);
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripSeparator());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `width?` | `number` | 工具栏项的宽度 |

#### Returns

`any`

如果未设置任何值,则返回工具栏项的宽度;否则,返回工具栏

___

### <a id="open" name="open"></a> open

▸ **open**(`x`, `y`): `void`

在相对于触摸点的特定位置打开工具栏

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | <i>x</i>坐标 |
| `y` | `number` | <i>y</i>坐标 |

#### Returns

`void`

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`name`): [`TouchToolStripItem`](GC.Spread.Sheets.Touch.TouchToolStripItem.md)

删除具有指定名称的工具栏项

**`代码示例`**
```
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripItem("Cut", "Delete", "cut.png", function(){ }))
spread.touchToolStrip.getItem("Cut").font("15px Arial").foreColor("red");
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripSeparator());
spread.touchToolStrip.remove("Cut");
activeSheet.resumePaint();
activeSheet.repaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 被删除项的名称 |

#### Returns

[`TouchToolStripItem`](GC.Spread.Sheets.Touch.TouchToolStripItem.md)

删除项

___

### <a id="separatorheight" name="separatorheight"></a> separatorHeight

▸ **separatorHeight**(`height?`): `any`

获取或设置工具栏分隔符的高度

**`代码示例`**
```
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripItem("Cut", "Delete", "cut.png", function(){ }))
spread.touchToolStrip.getItem("Cut").font("15px Arial").foreColor("red");
spread.touchToolStrip.separatorHeight(33);
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripSeparator());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `height?` | `number` | 工具栏分隔符的高度 |

#### Returns

`any`

如果未设置任何值,则返回工具栏分隔符的高度;否则,返回工具栏
