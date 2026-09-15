# Class: TouchToolStripItem

[Sheets](../modules/GC.Spread.Sheets.md).[Touch](../modules/GC.Spread.Sheets.Touch.md).TouchToolStripItem

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Touch.TouchToolStripItem.md#constructor)

### Methods

- [font](GC.Spread.Sheets.Touch.TouchToolStripItem.md#font)
- [foreColor](GC.Spread.Sheets.Touch.TouchToolStripItem.md#forecolor)
- [image](GC.Spread.Sheets.Touch.TouchToolStripItem.md#image)
- [name](GC.Spread.Sheets.Touch.TouchToolStripItem.md#name)
- [text](GC.Spread.Sheets.Touch.TouchToolStripItem.md#text)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new TouchToolStripItem**(`name`, `text`, `image`, `command?`, `canExecute?`)

表示工具栏中的项目。

**`example`**
```javascript
//此示例添加一个带有红色文本的删除图像。
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripItem("Cut", "Delete", "cut.png", function(){ }))
spread.touchToolStrip.getItem("Cut").font("15px Arial").foreColor("red");
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripSeparator());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 项目名称。 |
| `text` | `string` | 项目文本。 |
| `image` | `string` | 项目图像源。 |
| `command?` | `any` | 定义用户点击项目时执行的函数。 |
| `canExecute?` | `Function` | 定义何时通过函数显示项目。如果返回 `true`，则显示项目；否则隐藏项目。 |

## Methods

### <a id="font" name="font"></a> font

▸ **font**(`value?`): `any`

获取或设置项目文本的字体。

**`example`**
```javascript
//此示例添加一个带有红色文本的删除图像。
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripItem("Cut", "Delete", "cut.png", function(){ }))
spread.touchToolStrip.getItem("Cut").font("15px Arial").foreColor("red");
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripSeparator());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 工具栏项目文本的字体。 |

#### Returns

`any`

如果未设置值，则返回项目文本的字体；否则返回工具栏项目。

___

### <a id="forecolor" name="forecolor"></a> foreColor

▸ **foreColor**(`value?`): `any`

获取或设置项目文本的颜色。

**`example`**
```javascript
//此示例添加一个带有红色文本的删除图像。
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripItem("Cut", "Delete", "cut.png", function(){ }))
spread.touchToolStrip.getItem("Cut").font("15px Arial").foreColor("red");
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripSeparator());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 工具栏项目文本的颜色。 |

#### Returns

`any`

如果未设置值，则返回项目文本的颜色；否则返回工具栏项目。

___

### <a id="image" name="image"></a> image

▸ **image**(`value?`): `any`

获取或设置项目图像的源。

**`example`**
```javascript
//此示例添加一个带有红色文本的删除图像。
var tts = new GC.Spread.Sheets.Touch.TouchToolStripItem();
tts.image("cut.png");
tts.name("C");
tts.text("Delete");
spread.touchToolStrip.add(tts, function(){ });
spread.touchToolStrip.getItem("C").font("15px Arial").foreColor("red");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 项目图像源的路径和文件名。 |

#### Returns

`any`

如果未设置值，则返回项目图像的源；否则返回工具栏项目。

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置项目的名称。

**`example`**
```javascript
//此示例添加一个带有红色文本的删除图像。
var tts = new GC.Spread.Sheets.Touch.TouchToolStripItem();
tts.image("cut.png");
tts.name("C");
tts.text("Delete");
spread.touchToolStrip.add(tts, function(){ });
spread.touchToolStrip.getItem("C").font("15px Arial").foreColor("red");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 工具栏项目的名称。 |

#### Returns

`any`

如果未设置值，则返回项目的名称；否则返回工具栏项目。

___

### <a id="text" name="text"></a> text

▸ **text**(`value?`): `any`

获取或设置项目的文本。

**`example`**
```javascript
//此示例添加一个带有红色文本的删除图像。
var tts = new GC.Spread.Sheets.Touch.TouchToolStripItem();
tts.image("cut.png");
tts.name("C");
tts.text("Delete");
spread.touchToolStrip.add(tts, function(){ });
spread.touchToolStrip.getItem("C").font("15px Arial").foreColor("red");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 工具栏项目的文本。 |

#### Returns

`any`

如果未设置值，则返回项目的文本；否则返回工具栏项目。
