# Class: Comment

[Sheets](../modules/GC.Spread.Sheets.md).[Comments](../modules/GC.Spread.Sheets.Comments.md).Comment

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Comments.Comment.md#constructor)

### Methods

- [autoSize](GC.Spread.Sheets.Comments.Comment.md#autosize)
- [backColor](GC.Spread.Sheets.Comments.Comment.md#backcolor)
- [borderColor](GC.Spread.Sheets.Comments.Comment.md#bordercolor)
- [borderStyle](GC.Spread.Sheets.Comments.Comment.md#borderstyle)
- [borderWidth](GC.Spread.Sheets.Comments.Comment.md#borderwidth)
- [commentState](GC.Spread.Sheets.Comments.Comment.md#commentstate)
- [displayMode](GC.Spread.Sheets.Comments.Comment.md#displaymode)
- [dynamicMove](GC.Spread.Sheets.Comments.Comment.md#dynamicmove)
- [dynamicSize](GC.Spread.Sheets.Comments.Comment.md#dynamicsize)
- [fontFamily](GC.Spread.Sheets.Comments.Comment.md#fontfamily)
- [fontSize](GC.Spread.Sheets.Comments.Comment.md#fontsize)
- [fontStyle](GC.Spread.Sheets.Comments.Comment.md#fontstyle)
- [fontWeight](GC.Spread.Sheets.Comments.Comment.md#fontweight)
- [foreColor](GC.Spread.Sheets.Comments.Comment.md#forecolor)
- [height](GC.Spread.Sheets.Comments.Comment.md#height)
- [horizontalAlign](GC.Spread.Sheets.Comments.Comment.md#horizontalalign)
- [indicatorColor](GC.Spread.Sheets.Comments.Comment.md#indicatorcolor)
- [indicatorSize](GC.Spread.Sheets.Comments.Comment.md#indicatorsize)
- [location](GC.Spread.Sheets.Comments.Comment.md#location)
- [lockText](GC.Spread.Sheets.Comments.Comment.md#locktext)
- [locked](GC.Spread.Sheets.Comments.Comment.md#locked)
- [opacity](GC.Spread.Sheets.Comments.Comment.md#opacity)
- [padding](GC.Spread.Sheets.Comments.Comment.md#padding)
- [showShadow](GC.Spread.Sheets.Comments.Comment.md#showshadow)
- [text](GC.Spread.Sheets.Comments.Comment.md#text)
- [textDecoration](GC.Spread.Sheets.Comments.Comment.md#textdecoration)
- [width](GC.Spread.Sheets.Comments.Comment.md#width)
- [zIndex](GC.Spread.Sheets.Comments.Comment.md#zindex)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Comment**(`text?`)

表示一个批注。

**`example`**
```javascript
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
comment.autoSize(true);
activeSheet.getCell(5,5).comment(comment);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `text?` | `string` | 批注的文本内容。 |

## Methods

### <a id="autosize" name="autosize"></a> autoSize

▸ **autoSize**(`value?`): `any`

获取或设置批注是否根据其内容自动调整大小。

**`example`**
```javascript
//此示例使用autoSize方法。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
comment.autoSize(true);
activeSheet.getCell(5,5).comment(comment);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 批注是否自动调整大小。 |

#### Returns

`any`

如果未设置值，则返回批注是否自动调整大小；否则返回批注对象。

___

### <a id="backcolor" name="backcolor"></a> backColor

▸ **backColor**(`value?`): `any`

获取或设置批注的背景颜色。

**`example`**
```javascript
//此示例设置backColor方法。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
activeSheet.getCell(5,5).comment(comment);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 批注的背景颜色。 |

#### Returns

`any`

如果未设置值，则返回批注的背景颜色；否则返回批注对象。

___

### <a id="bordercolor" name="bordercolor"></a> borderColor

▸ **borderColor**(`value?`): `any`

获取或设置批注的边框颜色。

**`example`**
```javascript
//此示例设置borderColor方法。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
comment.borderWidth(2);
comment.borderStyle("dotted");
comment.borderColor("red");
activeSheet.getCell(5,5).comment(comment);
activeSheet.suspendPaint();
activeSheet.resumePaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 批注的边框颜色。 |

#### Returns

`any`

如果未设置值，则返回批注的边框颜色；否则返回批注对象。

___

### <a id="borderstyle" name="borderstyle"></a> borderStyle

▸ **borderStyle**(`value?`): `any`

获取或设置批注的边框样式。

**`example`**
```javascript
//此示例设置borderStyle方法。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
comment.borderWidth(2);
comment.borderStyle("dotted");
comment.borderColor("red");
activeSheet.getCell(5,5).comment(comment);
activeSheet.suspendPaint();
activeSheet.resumePaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 批注的边框样式。 |

#### Returns

`any`

如果未设置值，则返回批注的边框样式；否则返回批注对象。

___

### <a id="borderwidth" name="borderwidth"></a> borderWidth

▸ **borderWidth**(`value?`): `any`

获取或设置批注的边框宽度。

**`example`**
```javascript
//此示例设置borderWidth方法。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
comment.borderWidth(2);
comment.borderStyle("dotted");
comment.borderColor("red");
activeSheet.getCell(5,5).comment(comment);
activeSheet.suspendPaint();
activeSheet.resumePaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 批注的边框宽度。 |

#### Returns

`any`

如果未设置值，则返回批注的边框宽度；否则返回批注对象。

___

### <a id="commentstate" name="commentstate"></a> commentState

▸ **commentState**(`value?`): `any`

获取或设置批注的状态。

**`example`**
```javascript
//此示例获取批注状态。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
activeSheet.getCell(5,5).comment(comment);
alert(comment.commentState());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`CommentState`](../enums/GC.Spread.Sheets.Comments.CommentState.md) | 批注的状态。 |

#### Returns

`any`

如果未设置值，则返回批注的状态；否则返回批注对象。

___

### <a id="displaymode" name="displaymode"></a> displayMode

▸ **displayMode**(`value?`): `any`

获取或设置批注的显示模式。

**`example`**
```javascript
//此示例设置displayMode方法。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
activeSheet.getCell(5,5).comment(comment);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`DisplayMode`](../enums/GC.Spread.Sheets.Comments.DisplayMode.md) | 批注的显示模式。 |

#### Returns

`any`

如果未设置值，则返回批注的显示模式；否则返回批注对象。

___

### <a id="dynamicmove" name="dynamicmove"></a> dynamicMove

▸ **dynamicMove**(`value?`): `any`

获取或设置批注是否动态移动。

**`example`**
```javascript
//此示例使用dynamicMove方法。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
comment.dynamicMove(true);
comment.dynamicSize(true);
activeSheet.getCell(5,5).comment(comment);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 批注是否动态移动。 |

#### Returns

`any`

如果未设置值，则返回批注是否动态移动；否则返回批注对象。

___

### <a id="dynamicsize" name="dynamicsize"></a> dynamicSize

▸ **dynamicSize**(`value?`): `any`

获取或设置批注是否动态调整大小。

**`example`**
```javascript
//此示例使用dynamicSize方法。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
comment.dynamicMove(true);
comment.dynamicSize(true);
activeSheet.getCell(5,5).comment(comment);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 批注是否动态调整大小。 |

#### Returns

`any`

如果未设置值，则返回批注是否动态调整大小；否则返回批注对象。

___

### <a id="fontfamily" name="fontfamily"></a> fontFamily

▸ **fontFamily**(`value?`): `any`

获取或设置批注的字体。

**`example`**
```javascript
//此示例使用fontFamily方法。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
comment.fontFamily("Comic Sans MS");
comment.fontSize("10pt");
activeSheet.getCell(5,5).comment(comment);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 批注的字体。 |

#### Returns

`any`

如果未设置值，则返回批注的字体；否则返回批注对象。

___

### <a id="fontsize" name="fontsize"></a> fontSize

▸ **fontSize**(`value?`): `any`

获取或设置批注的字体大小。有效值是数字后跟"pt"（必需），例如"12pt"。

**`example`**
```javascript
//此示例使用fontSize方法。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
comment.fontFamily("Comic Sans MS");
comment.fontSize("10pt");
activeSheet.getCell(5,5).comment(comment);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 批注的字体大小。 |

#### Returns

`any`

如果未设置值，则返回批注的字体大小；否则返回批注对象。

___

### <a id="fontstyle" name="fontstyle"></a> fontStyle

▸ **fontStyle**(`value?`): `any`

获取或设置批注的字体样式。

**`example`**
```javascript
//此示例使用fontStyle方法。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
comment.fontFamily("Comic Sans MS");
comment.fontStyle("normal");
comment.fontWeight("normal");
activeSheet.getCell(5,5).comment(comment);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 批注的字体样式。 |

#### Returns

`any`

如果未设置值，则返回批注的字体样式；否则返回批注对象。

___

### <a id="fontweight" name="fontweight"></a> fontWeight

▸ **fontWeight**(`value?`): `any`

获取或设置批注的字体粗细。

**`example`**
```javascript
//此示例使用fontWeight方法。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
comment.fontFamily("Comic Sans MS");
comment.fontStyle("normal");
comment.fontWeight("normal");
activeSheet.getCell(5,5).comment(comment);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 批注的字体粗细。 |

#### Returns

`any`

如果未设置值，则返回批注的字体粗细；否则返回批注对象。

___

### <a id="forecolor" name="forecolor"></a> foreColor

▸ **foreColor**(`value?`): `any`

获取或设置批注的文本颜色。

**`example`**
```javascript
//此示例使用foreColor方法。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
activeSheet.getCell(5,5).comment(comment);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 批注的文本颜色。 |

#### Returns

`any`

如果未设置值，则返回批注的文本颜色；否则返回批注对象。

___

### <a id="height" name="height"></a> height

▸ **height**(`value?`): `any`

获取或设置批注的高度。

**`example`**
```javascript
//此示例使用height方法。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
comment.height(50);
comment.width(90);
activeSheet.getCell(5,5).comment(comment);
activeSheet.suspendPaint();
activeSheet.resumePaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 批注的高度。 |

#### Returns

`any`

如果未设置值，则返回批注的高度；否则返回批注对象。

___

### <a id="horizontalalign" name="horizontalalign"></a> horizontalAlign

▸ **horizontalAlign**(`value?`): `any`

获取或设置批注的水平对齐方式。

**`example`**
```javascript
//此示例使用horizontalAlign方法。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
comment.horizontalAlign(GC.Spread.Sheets.HorizontalAlign.center);
activeSheet.getCell(5,5).comment(comment);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`HorizontalAlign`](../enums/GC.Spread.Sheets.HorizontalAlign.md) | 批注的水平对齐方式。 |

#### Returns

`any`

如果未设置值，则返回批注的水平对齐方式；否则返回批注对象。

___

### <a id="indicatorcolor" name="indicatorcolor"></a> indicatorColor

▸ **indicatorColor**(`value?`): `any`

获取或设置批注的指示器颜色。

**`example`**
```javascript
//此示例使用indicatorColor方法。
var comment = new GC.Spread.Sheets.Comments.Comment();
var color1 = "red";
var color2 = "#FFFFFF";
var color2 = "rgba(255, 255, 255, 0.01)";
comment.indicatorColor(color1);
activeSheet.comments.add(5, 5, comment);
activeSheet.getCell(5,5).comment(comment);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 批注的指示器颜色。 |

#### Returns

`any`

如果未设置值，则返回批注指示器的颜色；否则返回批注对象。

___

### <a id="indicatorsize" name="indicatorsize"></a> indicatorSize

▸ **indicatorSize**(`value?`): `any`

获取或设置批注的指示器大小。

**`example`**
```javascript
//此示例使用indicatorSize方法。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.indicatorSize(6);
activeSheet.comments.add(5, 5, comment);
activeSheet.getCell(5,5).comment(comment);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 批注的指示器大小。 |

#### Returns

`any`

如果未设置值，则返回批注指示器的大小；否则返回批注对象。

___

### <a id="location" name="location"></a> location

▸ **location**(`value?`): `any`

获取或设置批注的位置。

**`example`**
```javascript
//此示例使用location方法。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
comment.location(new GC.Spread.Sheets.Point(10, 10));
activeSheet.getCell(5,5).comment(comment);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`Point`](GC.Spread.Sheets.Point.md) | 批注的位置。 |

#### Returns

`any`

如果未设置值，则返回批注的位置；否则返回批注对象。

___

### <a id="locktext" name="locktext"></a> lockText

▸ **lockText**(`value?`): `any`

获取或设置批注的文本锁定状态。

**`example`**
```javascript
//此示例使用lockText方法。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.lockText(false);
comment.locked(false);
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
activeSheet.options.isProtected = true;
activeSheet.getCell(5,5).comment(comment);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 批注的文本锁定状态。 |

#### Returns

`any`

如果未设置值，则返回批注的文本锁定状态；否则返回批注对象。

___

### <a id="locked" name="locked"></a> locked

▸ **locked**(`value?`): `any`

获取或设置批注的锁定状态。

**`example`**
```javascript
//此示例使用locked方法。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.lockText(false);
comment.locked(false);
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
activeSheet.options.isProtected = true;
activeSheet.getCell(5,5).comment(comment);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 批注的锁定状态。 |

#### Returns

`any`

如果未设置值，则返回批注的锁定状态；否则返回批注对象。

___

### <a id="opacity" name="opacity"></a> opacity

▸ **opacity**(`value?`): `any`

获取或设置批注的不透明度。

**`example`**
```javascript
//此示例设置不透明度。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
comment.opacity(10);
activeSheet.getCell(5,5).comment(comment);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 批注的不透明度。 |

#### Returns

`any`

如果未设置值，则返回批注的不透明度；否则返回批注对象。

___

### <a id="padding" name="padding"></a> padding

▸ **padding**(`value?`): `any`

获取或设置批注的内边距。

**`example`**
```javascript
//此示例使用padding方法。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
comment.padding(new GC.Spread.Sheets.Comments.Padding(2, 2, 2, 2));
activeSheet.getCell(5,5).comment(comment);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`Padding`](GC.Spread.Sheets.Comments.Padding.md) | 批注的内边距。 |

#### Returns

`any`

如果未设置值，则返回批注的内边距；否则返回批注对象。

___

### <a id="showshadow" name="showshadow"></a> showShadow

▸ **showShadow**(`value?`): `any`

获取或设置批注是否显示阴影。

**`example`**
```javascript
//此示例使用showShadow方法。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
comment.borderWidth(2);
comment.borderStyle("dotted");
comment.borderColor("red");
comment.showShadow(true);
activeSheet.getCell(5,5).comment(comment);
activeSheet.suspendPaint();
activeSheet.resumePaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 批注是否显示阴影。 |

#### Returns

`any`

如果未设置值，则返回批注是否显示阴影；否则返回批注对象。

___

### <a id="text" name="text"></a> text

▸ **text**(`value?`): `any`

获取或设置批注的文本。

**`example`**
```javascript
//此示例设置text方法。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
activeSheet.getCell(5,5).comment(comment);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 批注的文本。 |

#### Returns

`any`

如果未设置值，则返回批注的文本；否则返回批注对象。

___

### <a id="textdecoration" name="textdecoration"></a> textDecoration

▸ **textDecoration**(`value?`): `any`

获取或设置批注的文本装饰。

**`example`**
```javascript
//此示例使用textDecoration方法。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
comment.textDecoration(GC.Spread.Sheets.TextDecorationType.underline);
activeSheet.getCell(5,5).comment(comment);
activeSheet.suspendPaint();
activeSheet.resumePaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`TextDecorationType`](../enums/GC.Spread.Sheets.TextDecorationType.md) | 批注的文本装饰。 |

#### Returns

`any`

如果未设置值，则返回批注的文本装饰；否则返回批注对象。

___

### <a id="width" name="width"></a> width

▸ **width**(`value?`): `any`

获取或设置批注的宽度。

**`example`**
```javascript
//此示例设置width方法。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
comment.height(50);
comment.width(90);
activeSheet.getCell(5,5).comment(comment);
activeSheet.suspendPaint();
activeSheet.resumePaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 批注的宽度。 |

#### Returns

`any`

如果未设置值，则返回批注的宽度；否则返回批注对象。

___

### <a id="zindex" name="zindex"></a> zIndex

▸ **zIndex**(`value?`): `any`

获取或设置批注的z-index。

**`example`**
```javascript
//此示例获取z-index。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
activeSheet.getCell(5,5).comment(comment);
alert(comment.zIndex());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 批注的z-index。 |

#### Returns

`any`

如果未设置值，则返回批注的z-index；否则返回批注对象。
