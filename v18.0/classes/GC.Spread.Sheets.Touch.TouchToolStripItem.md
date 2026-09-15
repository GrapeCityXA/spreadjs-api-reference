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

工具栏中的一个项

**`代码示例`**
``` javascript
//本示例添加带有红色文本的删除图像
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripItem("Cut", "Delete", "cut.png", function(){ }))
spread.touchToolStrip.getItem("Cut").font("15px Arial").foreColor("red");
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripSeparator());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 项名称 |
| `text` | `string` | 项文本 |
| `image` | `string` | 项图像源 |
| `command?` | `any` | 定义当用户点击项时执行的执行功能 |
| `canExecute?` | `Function` | 定义当通过函数显示项时，如果该项显示，则返回true;否则为false |

## Methods

### <a id="font" name="font"></a> font

▸ **font**(`value?`): `any`

获取或设置项文本的字体

**`代码示例`**
``` javascript
//本示例添加带有红色文本的删除图像
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripItem("Cut", "Delete", "cut.png", function(){ }))
spread.touchToolStrip.getItem("Cut").font("15px Arial").foreColor("red");
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripSeparator());
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置任何值，则返回项文本的字体；否则，返回工具栏项

___

### <a id="forecolor" name="forecolor"></a> foreColor

▸ **foreColor**(`value?`): `any`

获取或设置项文本的颜色

**`代码示例`**
``` javascript
//本示例添加带有红色文本的删除图像
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripItem("Cut", "Delete", "cut.png", function(){ }))
spread.touchToolStrip.getItem("Cut").font("15px Arial").foreColor("red");
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripSeparator());
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置任何值，则返回项文本的颜色；否则，返回工具栏项

___

### <a id="image" name="image"></a> image

▸ **image**(`value?`): `any`

获取或设置项图像的来源

**`代码示例`**
``` javascript
//本示例添加带有红色文本的删除图像
var tts = new GC.Spread.Sheets.Touch.TouchToolStripItem();
tts.image("cut.png");
tts.name("C");
tts.text("Delete");
spread.touchToolStrip.add(tts, function(){ });
spread.touchToolStrip.getItem("C").font("15px Arial").foreColor("red");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置任何值，则返回项图像的来源；否则，返回工具栏项

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置项的名称

**`代码示例`**
``` javascript
//本示例添加带有红色文本的删除图像
var tts = new GC.Spread.Sheets.Touch.TouchToolStripItem();
tts.image("cut.png");
tts.name("C");
tts.text("Delete");
spread.touchToolStrip.add(tts, function(){ });
spread.touchToolStrip.getItem("C").font("15px Arial").foreColor("red");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置任何值，则返回项的名称；否则，返回工具栏项

___

### <a id="text" name="text"></a> text

▸ **text**(`value?`): `any`

获取或设置项的文本

**`代码示例`**
``` javascript
//本示例添加带有红色文本的删除图像
var tts = new GC.Spread.Sheets.Touch.TouchToolStripItem();
tts.image("cut.png");
tts.name("C");
tts.text("Delete");
spread.touchToolStrip.add(tts, function(){ });
spread.touchToolStrip.getItem("C").font("15px Arial").foreColor("red");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置任何值，则返回项的文本；否则，返回工具栏项
