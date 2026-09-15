# Class: Picture

[Sheets](../modules/GC.Spread.Sheets.md).[FloatingObjects](../modules/GC.Spread.Sheets.FloatingObjects.md).Picture

## Hierarchy

- [`FloatingObject`](GC.Spread.Sheets.FloatingObjects.FloatingObject.md)

  ↳ **`Picture`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.FloatingObjects.Picture.md#constructor)

### Properties

- [typeName](GC.Spread.Sheets.FloatingObjects.Picture.md#typename)

### Methods

- [allowMove](GC.Spread.Sheets.FloatingObjects.Picture.md#allowmove)
- [allowResize](GC.Spread.Sheets.FloatingObjects.Picture.md#allowresize)
- [alt](GC.Spread.Sheets.FloatingObjects.Picture.md#alt)
- [backColor](GC.Spread.Sheets.FloatingObjects.Picture.md#backcolor)
- [borderColor](GC.Spread.Sheets.FloatingObjects.Picture.md#bordercolor)
- [borderRadius](GC.Spread.Sheets.FloatingObjects.Picture.md#borderradius)
- [borderStyle](GC.Spread.Sheets.FloatingObjects.Picture.md#borderstyle)
- [borderWidth](GC.Spread.Sheets.FloatingObjects.Picture.md#borderwidth)
- [cloneContent](GC.Spread.Sheets.FloatingObjects.Picture.md#clonecontent)
- [content](GC.Spread.Sheets.FloatingObjects.Picture.md#content)
- [dynamicMove](GC.Spread.Sheets.FloatingObjects.Picture.md#dynamicmove)
- [dynamicSize](GC.Spread.Sheets.FloatingObjects.Picture.md#dynamicsize)
- [endColumn](GC.Spread.Sheets.FloatingObjects.Picture.md#endcolumn)
- [endColumnOffset](GC.Spread.Sheets.FloatingObjects.Picture.md#endcolumnoffset)
- [endRow](GC.Spread.Sheets.FloatingObjects.Picture.md#endrow)
- [endRowOffset](GC.Spread.Sheets.FloatingObjects.Picture.md#endrowoffset)
- [fixedPosition](GC.Spread.Sheets.FloatingObjects.Picture.md#fixedposition)
- [getHost](GC.Spread.Sheets.FloatingObjects.Picture.md#gethost)
- [getOriginalHeight](GC.Spread.Sheets.FloatingObjects.Picture.md#getoriginalheight)
- [getOriginalWidth](GC.Spread.Sheets.FloatingObjects.Picture.md#getoriginalwidth)
- [height](GC.Spread.Sheets.FloatingObjects.Picture.md#height)
- [isLocked](GC.Spread.Sheets.FloatingObjects.Picture.md#islocked)
- [isSelected](GC.Spread.Sheets.FloatingObjects.Picture.md#isselected)
- [isVisible](GC.Spread.Sheets.FloatingObjects.Picture.md#isvisible)
- [name](GC.Spread.Sheets.FloatingObjects.Picture.md#name)
- [pictureStretch](GC.Spread.Sheets.FloatingObjects.Picture.md#picturestretch)
- [refreshContent](GC.Spread.Sheets.FloatingObjects.Picture.md#refreshcontent)
- [src](GC.Spread.Sheets.FloatingObjects.Picture.md#src)
- [startColumn](GC.Spread.Sheets.FloatingObjects.Picture.md#startcolumn)
- [startColumnOffset](GC.Spread.Sheets.FloatingObjects.Picture.md#startcolumnoffset)
- [startRow](GC.Spread.Sheets.FloatingObjects.Picture.md#startrow)
- [startRowOffset](GC.Spread.Sheets.FloatingObjects.Picture.md#startrowoffset)
- [width](GC.Spread.Sheets.FloatingObjects.Picture.md#width)
- [x](GC.Spread.Sheets.FloatingObjects.Picture.md#x)
- [y](GC.Spread.Sheets.FloatingObjects.Picture.md#y)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Picture**(`name`, `src`, `x`, `y`, `width`, `height`)

表示一个图片。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 图片的名称。 |
| `src` | `string` | 图片的图像源。 |
| `x` | `number` | 图片的 <i>x</i> 坐标位置。 |
| `y` | `number` | 图片的 <i>y</i> 坐标位置。 |
| `width` | `number` | 图片的宽度。 |
| `height` | `number` | 图片的高度。 |

#### Overrides

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[constructor](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#constructor)

## Properties

### <a id="typename" name="typename"></a> typeName

• **typeName**: `string`

表示用于支持序列化的类型名称字符串。

**`example`**
```javascript
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject('floatingObject', 10, 10, 64, 30);
console.log(customFloatingObject.typeName); // "0"
```

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[typeName](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#typename)

## Methods

### <a id="allowmove" name="allowmove"></a> allowMove

▸ **allowMove**(`value?`): `any`

获取或设置是否禁用移动浮动对象。

**`example`**
```javascript
//此示例禁止移动或调整浮动对象大小。
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.allowResize(false);
customFloatingObject.allowMove(false);
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否禁用移动浮动对象的设置。 |

#### Returns

`any`

如果未设置值，则返回是否禁用移动浮动对象的设置；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[allowMove](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#allowmove)

___

### <a id="allowresize" name="allowresize"></a> allowResize

▸ **allowResize**(`value?`): `any`

获取或设置是否禁用调整浮动对象大小。

**`example`**
```javascript
//此示例禁止移动或调整浮动对象大小。
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.allowResize(false);
customFloatingObject.allowMove(false);
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否禁用调整浮动对象大小的设置。 |

#### Returns

`any`

如果未设置值，则返回是否禁用调整浮动对象大小的设置；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[allowResize](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#allowresize)

___

### <a id="alt" name="alt"></a> alt

▸ **alt**(`value?`): `any`

获取或设置浮动对象的替代文本（用于屏幕阅读器）。

**`example`**
```javascript
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject('f1', 10, 10, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
customFloatingObject.alt("一个按钮");
activeSheet.floatingObjects.add(customFloatingObject);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 浮动对象的替代文本。 |

#### Returns

`any`

浮动对象的替代文本。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[alt](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#alt)

___

### <a id="backcolor" name="backcolor"></a> backColor

▸ **backColor**(`value?`): `any`

获取或设置图片的背景颜色。

**`example`**
```javascript
//此示例设置图片的背景颜色。
var picture = activeSheet.pictures.add("f2","Event.png",50,50,100,100);
picture.borderStyle("solid");
picture.borderWidth(2);
picture.borderColor("red");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 图片的背景颜色。 |

#### Returns

`any`

如果未设置值，则返回图片的背景颜色；否则返回图片。

___

### <a id="bordercolor" name="bordercolor"></a> borderColor

▸ **borderColor**(`value?`): `any`

获取或设置图片的边框颜色。

**`example`**
```javascript
//此示例设置图片的边框颜色。
var picture = activeSheet.pictures.add("f2","Event.png",50,50,100,100);
picture.borderStyle("solid");
picture.borderWidth(2);
picture.borderColor("red");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 图片的边框颜色。 |

#### Returns

`any`

如果未设置值，则返回图片的边框颜色；否则返回图片。

___

### <a id="borderradius" name="borderradius"></a> borderRadius

▸ **borderRadius**(`value?`): `any`

获取或设置图片的边框圆角。

**`example`**
```javascript
//此示例使用borderRadius方法。
var picture = activeSheet.pictures.add("f2","Event.png",50,50,100,100);
picture.backColor("blue");
picture.borderWidth(2);
picture.borderColor("red");
picture.borderStyle("dotted");
picture.borderRadius(5);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 图片的边框圆角。 |

#### Returns

`any`

如果未设置值，则返回图片的边框圆角；否则返回图片。

___

### <a id="borderstyle" name="borderstyle"></a> borderStyle

▸ **borderStyle**(`value?`): `any`

获取或设置图片的边框样式。

**`example`**
```javascript
//此示例使用 borderStyle 方法。
var picture = activeSheet.pictures.add("f2","Event.png",50,50,100,100);
picture.borderStyle("dotted");
picture.borderWidth(2);
picture.borderColor("red");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 图片的 CSS 边框样式，例如 dotted、dashed、solid 等。 |

#### Returns

`any`

如果未设置值，则返回图片的边框样式；否则返回图片。

___

### <a id="borderwidth" name="borderwidth"></a> borderWidth

▸ **borderWidth**(`value?`): `any`

获取或设置图片的边框宽度。

**`example`**
```javascript
//此示例使用 borderWidth 方法。
var picture = activeSheet.pictures.add("f2","Event.png",50,50,100,100);
picture.borderStyle("solid");
picture.borderWidth(2);
picture.borderColor("red");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 图片的边框宽度。 |

#### Returns

`any`

如果未设置值，则返回图片的边框宽度；否则返回图片。

___

### <a id="clonecontent" name="clonecontent"></a> cloneContent

▸ **cloneContent**(): `HTMLElement`

获取实例当前内容的副本。

**`example`**
```javascript
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject('f1', 10, 10, 64, 30);
customFloatingObject.content(createButton('button 1', '64px', '30px'));
activeSheet.floatingObjects.add(customFloatingObject);

var btn = customFloatingObject.cloneContent();
btn.innerText = 'button 2';
customFloatingObject.content(btn);

function createButton (text, width, height) {
    var btn = document.createElement('button');
    btn.style.width = width;
    btn.style.height = height;
    btn.innerText = text;
    return btn;
}
```

#### Returns

`HTMLElement`

实例当前内容的副本。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[cloneContent](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#clonecontent)

___

### <a id="content" name="content"></a> content

▸ **content**(`value?`): `any`

获取或设置自定义浮动对象的内容。

**`example`**
```javascript
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject('f1', 10, 10, 64, 30);
customFloatingObject.content(createButton('button 1', '64px', '30px'));
activeSheet.floatingObjects.add(customFloatingObject);

console.log(customFloatingObject.content()); // 获取当前内容，结果是文本为"button 1"的按钮元素。
customFloatingObject.content(createButton('button 2', '64px', '30px')); // 设置新内容。

function createButton (text, width, height) {
    var btn = document.createElement('button');
    btn.style.width = width;
    btn.style.height = height;
    btn.innerText = text;
    return btn;
}
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `HTMLElement` | 自定义浮动对象的内容。 |

#### Returns

`any`

如果未设置值，则返回自定义浮动对象的内容；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[content](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#content)

___

### <a id="dynamicmove" name="dynamicmove"></a> dynamicMove

▸ **dynamicMove**(`value?`): `any`

获取或设置当隐藏或显示、调整大小或移动行或列时，对象是否移动。

**`example`**
```javascript
//此示例创建一个浮动对象。
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
customFloatingObject.isVisible(true);
customFloatingObject.dynamicSize(true);
customFloatingObject.dynamicMove(true);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 指示当隐藏或显示、调整大小或移动行或列时，对象是否移动的值。 |

#### Returns

`any`

如果未设置值，则返回此浮动对象是否动态移动；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[dynamicMove](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#dynamicmove)

___

### <a id="dynamicsize" name="dynamicsize"></a> dynamicSize

▸ **dynamicSize**(`value?`): `any`

获取或设置当隐藏或显示、调整大小或移动行或列时，对象的大小是否改变。

**`example`**
```javascript
//此示例创建一个浮动对象。
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
customFloatingObject.isVisible(true);
customFloatingObject.dynamicSize(true);
customFloatingObject.dynamicMove(true);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 指示当隐藏或显示、调整大小或移动行或列时，对象的大小是否改变的值。 |

#### Returns

`any`

如果未设置值，则返回此浮动对象是否动态改变大小；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[dynamicSize](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#dynamicsize)

___

### <a id="endcolumn" name="endcolumn"></a> endColumn

▸ **endColumn**(`value?`): `any`

获取或设置浮动对象位置的结束列索引。

**`example`**
```javascript
//创建一个浮动对象。
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
//通过单元格锚点定位浮动对象的左上角。
customFloatingObject.startRow(2);
customFloatingObject.startColumn(2);
customFloatingObject.startRowOffset(10);
customFloatingObject.startColumnOffset(10);
//通过单元格锚点定位浮动对象的右下角。
customFloatingObject.endRow(7);
customFloatingObject.endColumn(5);
customFloatingObject.endRowOffset(10);
customFloatingObject.endColumnOffset(10);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 浮动对象位置的结束列索引。 |

#### Returns

`any`

如果未设置值，则返回浮动对象位置的结束列索引；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[endColumn](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#endcolumn)

___

### <a id="endcolumnoffset" name="endcolumnoffset"></a> endColumnOffset

▸ **endColumnOffset**(`value?`): `any`

获取或设置浮动对象相对于结束列的偏移量。

**`example`**
```javascript
//创建一个浮动对象。
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
//通过单元格锚点定位浮动对象的左上角。
customFloatingObject.startRow(2);
customFloatingObject.startColumn(2);
customFloatingObject.startRowOffset(10);
customFloatingObject.startColumnOffset(10);
//通过单元格锚点定位浮动对象的右下角。
customFloatingObject.endRow(7);
customFloatingObject.endColumn(5);
customFloatingObject.endRowOffset(10);
customFloatingObject.endColumnOffset(10);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 浮动对象相对于结束列的偏移量。 |

#### Returns

`any`

如果未设置值，则返回浮动对象相对于结束列的偏移量；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[endColumnOffset](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#endcolumnoffset)

___

### <a id="endrow" name="endrow"></a> endRow

▸ **endRow**(`value?`): `any`

获取或设置浮动对象位置的结束行索引。

**`example`**
```javascript
//创建一个浮动对象。
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
//通过单元格锚点定位浮动对象的左上角。
customFloatingObject.startRow(2);
customFloatingObject.startColumn(2);
customFloatingObject.startRowOffset(10);
customFloatingObject.startColumnOffset(10);
//通过单元格锚点定位浮动对象的右下角。
customFloatingObject.endRow(7);
customFloatingObject.endColumn(5);
customFloatingObject.endRowOffset(10);
customFloatingObject.endColumnOffset(10);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 浮动对象位置的结束行索引。 |

#### Returns

`any`

如果未设置值，则返回浮动对象位置的结束行索引；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[endRow](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#endrow)

___

### <a id="endrowoffset" name="endrowoffset"></a> endRowOffset

▸ **endRowOffset**(`value?`): `any`

获取或设置相对于浮动对象结束行的偏移量。

**`example`**
```javascript
//创建一个浮动对象。
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
//通过单元格锚点定位浮动对象的左上角。
customFloatingObject.startRow(2);
customFloatingObject.startColumn(2);
customFloatingObject.startRowOffset(10);
customFloatingObject.startColumnOffset(10);
//通过单元格锚点定位浮动对象的右下角。
customFloatingObject.endRow(7);
customFloatingObject.endColumn(5);
customFloatingObject.endRowOffset(10);
customFloatingObject.endColumnOffset(10);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 相对于浮动对象结束行的偏移量。 |

#### Returns

`any`

如果未设置值，则返回相对于浮动对象结束行的偏移量；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[endRowOffset](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#endrowoffset)

___

### <a id="fixedposition" name="fixedposition"></a> fixedPosition

▸ **fixedPosition**(`value`): `any`

获取或设置浮动对象的位置是否固定。当 fixedPosition 为 true 时，dynamicMove 和 dynamicSize 将被禁用。

**`example`**
```javascript
//此示例将对象的位置设置为固定。
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
customFloatingObject.fixedPosition(true);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | `boolean` |

#### Returns

`any`

如果未设置值，则返回浮动对象的位置是否固定；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[fixedPosition](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#fixedposition)

___

### <a id="gethost" name="gethost"></a> getHost

▸ **getHost**(): `HTMLElement`[]

获取自定义内容的DOM宿主。

#### Returns

`HTMLElement`[]

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[getHost](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#gethost)

___

### <a id="getoriginalheight" name="getoriginalheight"></a> getOriginalHeight

▸ **getOriginalHeight**(): `number`

获取图片的原始高度。

**`example`**
```javascript
activeSheet.pictures.add("f2","Event.png",2,2,6,6);
activeSheet.pictures.add("f1","tsoutline.png",3,0,6,6);
var picture = activeSheet.pictures.get("f2");
picture.pictureStretch(GC.Spread.Sheets.ImageLayout.center);
//button
$("#button1").click(function () {
  alert(picture.getOriginalHeight());
});
```

#### Returns

`number`

图片的原始高度。

___

### <a id="getoriginalwidth" name="getoriginalwidth"></a> getOriginalWidth

▸ **getOriginalWidth**(): `number`

获取图片的原始宽度。

**`example`**
```javascript
activeSheet.pictures.add("f2","Event.png",2,2,6,6);
activeSheet.pictures.add("f1","tsoutline.png",3,0,6,6);
var picture = activeSheet.pictures.get("f2");
picture.pictureStretch(GC.Spread.Sheets.ImageLayout.center);
//button
$("#button1").click(function () {
     alert(picture.getOriginalWidth());
});
```

#### Returns

`number`

图片的原始宽度。

___

### <a id="height" name="height"></a> height

▸ **height**(`value?`): `any`

获取或设置浮动对象的高度。

**`example`**
```javascript
//此示例创建一个浮动对象。
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1");
customFloatingObject.x(10);
customFloatingObject.y(10);
customFloatingObject.width(60);
customFloatingObject.height(64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 浮动对象的高度。 |

#### Returns

`any`

如果未设置值，则返回浮动对象的高度；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[height](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#height)

___

### <a id="islocked" name="islocked"></a> isLocked

▸ **isLocked**(`value?`): `any`

获取或设置此浮动对象是否被锁定。

**`example`**
```javascript
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1");
customFloatingObject.x(10);
customFloatingObject.y(10);
customFloatingObject.width(60);
customFloatingObject.height(64);
customFloatingObject.isLocked(true);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
activeSheet.options.isProtected = true;
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 指示此浮动对象是否被锁定的值。 |

#### Returns

`any`

如果未设置值，则返回此浮动对象是否被锁定；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[isLocked](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#islocked)

___

### <a id="isselected" name="isselected"></a> isSelected

▸ **isSelected**(`value?`): `any`

获取或设置此浮动对象是否被选中。

**`example`**
```javascript
//此示例创建一个浮动对象。
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
customFloatingObject.isSelected(true);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 指示此浮动对象是否被选中的值。 |

#### Returns

`any`

如果未设置值，则返回此浮动对象是否被选中；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[isSelected](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#isselected)

___

### <a id="isvisible" name="isvisible"></a> isVisible

▸ **isVisible**(`value?`): `any`

获取或设置此浮动对象是否可见。

**`example`**
```javascript
//此示例创建一个浮动对象。
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
customFloatingObject.isVisible(true);
customFloatingObject.dynamicSize(true);
customFloatingObject.dynamicMove(true);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 指示此浮动对象是否可见的值。 |

#### Returns

`any`

如果未设置值，则返回此浮动对象是否可见；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[isVisible](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#isvisible)

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取浮动对象的名称。

**`example`**
```javascript
//此示例使用name方法。
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject();
customFloatingObject.name("f1");
customFloatingObject.x(10);
customFloatingObject.y(10);
customFloatingObject.width(60);
customFloatingObject.height(64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 浮动对象的名称。 |

#### Returns

`any`

如果未设置值，则返回浮动对象的名称；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[name](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#name)

___

### <a id="picturestretch" name="picturestretch"></a> pictureStretch

▸ **pictureStretch**(`value?`): `any`

获取或设置图片的拉伸方式。

**`example`**
```javascript
//此示例使用pictureStretch方法。
var picture = activeSheet.pictures.add("f2","Event.png",50,50,100,100);
picture.pictureStretch(GC.Spread.Sheets.ImageLayout.stretch);
picture.backColor("blue");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`ImageLayout`](../enums/GC.Spread.Sheets.ImageLayout.md) | 图片的拉伸方式。 |

#### Returns

`any`

如果未设置值，则返回图片的拉伸方式；否则返回图片。

___

### <a id="refreshcontent" name="refreshcontent"></a> refreshContent

▸ **refreshContent**(): `void`

刷新浮动对象中的内容。用户应该重写此方法以使其内容与浮动对象保持同步。

**`example`**
```javascript
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject('floatingObject', 10, 10, 64, 30);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
// 隐藏浮动对象
customFloatingObject.isVisible(false);
activeSheet.floatingObjects.add(customFloatingObject);

// 显示浮动对象
customFloatingObject.isVisible(true);
customFloatingObject.refreshContent(customFloatingObject.content());
```

#### Returns

`void`

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[refreshContent](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#refreshcontent)

___

### <a id="src" name="src"></a> src

▸ **src**(`value?`): `any`

获取或设置图片的源地址。

**`example`**
```javascript
var pic = sheet.pictures.add("Picture 1", "Event.png", 100, 50, 200, 200);
var src = pic.src(); // 获取当前图片源，结果为"Event.png"。
pic.src("tsoutline.png"); // 设置新的图片源。
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 图片的源地址。 |

#### Returns

`any`

如果未设置值，则返回图片的源地址；否则返回图片。

___

### <a id="startcolumn" name="startcolumn"></a> startColumn

▸ **startColumn**(`value?`): `any`

获取或设置浮动对象位置的起始列索引。

**`example`**
```javascript
//创建一个浮动对象。
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
//通过单元格锚点定位浮动对象的左上角。
customFloatingObject.startRow(2);
customFloatingObject.startColumn(2);
customFloatingObject.startRowOffset(10);
customFloatingObject.startColumnOffset(10);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 浮动对象位置的起始列索引。 |

#### Returns

`any`

如果未设置值，则返回浮动对象位置的起始列索引；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[startColumn](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#startcolumn)

___

### <a id="startcolumnoffset" name="startcolumnoffset"></a> startColumnOffset

▸ **startColumnOffset**(`value?`): `any`

获取或设置浮动对象相对于起始列的偏移量。

**`example`**
```javascript
//创建一个浮动对象。
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
//通过单元格锚点定位浮动对象的左上角。
customFloatingObject.startRow(2);
customFloatingObject.startColumn(2);
customFloatingObject.startRowOffset(10);
customFloatingObject.startColumnOffset(10);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 浮动对象相对于起始列的偏移量。 |

#### Returns

`any`

如果未设置值，则返回浮动对象相对于起始列的偏移量；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[startColumnOffset](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#startcolumnoffset)

___

### <a id="startrow" name="startrow"></a> startRow

▸ **startRow**(`value?`): `any`

获取或设置浮动对象位置的起始行索引。

**`example`**
```javascript
//创建一个浮动对象。
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
//通过单元格锚点定位浮动对象的左上角。
customFloatingObject.startRow(2);
customFloatingObject.startColumn(2);
customFloatingObject.startRowOffset(10);
customFloatingObject.startColumnOffset(10);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 浮动对象位置的起始行索引。 |

#### Returns

`any`

如果未设置值，则返回浮动对象位置的起始行索引；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[startRow](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#startrow)

___

### <a id="startrowoffset" name="startrowoffset"></a> startRowOffset

▸ **startRowOffset**(`value?`): `any`

获取或设置浮动对象相对于起始行的偏移量。

**`example`**
```javascript
//此示例创建一个浮动对象。
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
//通过单元格锚点定位浮动对象的左上角。
customFloatingObject.startRow(2);
customFloatingObject.startColumn(2);
customFloatingObject.startRowOffset(10);
customFloatingObject.startColumnOffset(10);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 浮动对象相对于起始行的偏移量。 |

#### Returns

`any`

如果未设置值，则返回浮动对象相对于起始行的偏移量；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[startRowOffset](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#startrowoffset)

___

### <a id="width" name="width"></a> width

▸ **width**(`value?`): `any`

获取或设置浮动对象的宽度。

**`example`**
```javascript
//此示例创建一个浮动对象。
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1");
customFloatingObject.x(10);
customFloatingObject.y(10);
customFloatingObject.width(60);
customFloatingObject.height(64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 浮动对象的宽度。 |

#### Returns

`any`

如果未设置值，则返回浮动对象的宽度；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[width](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#width)

___

### <a id="x" name="x"></a> x

▸ **x**(`value?`): `any`

获取或设置浮动对象的水平位置。

**`example`**
```javascript
//此示例创建一个浮动对象。
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1");
customFloatingObject.x(10);
customFloatingObject.y(10);
customFloatingObject.width(60);
customFloatingObject.height(64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 浮动对象的水平位置。 |

#### Returns

`any`

如果未设置值，则返回浮动对象的水平位置；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[x](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#x)

___

### <a id="y" name="y"></a> y

▸ **y**(`value?`): `any`

获取或设置浮动对象的垂直位置。

**`example`**
```javascript
//此示例创建一个浮动对象。
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1");
customFloatingObject.x(10);
customFloatingObject.y(10);
customFloatingObject.width(60);
customFloatingObject.height(64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 浮动对象的垂直位置。 |

#### Returns

`any`

如果未设置值，则返回浮动对象的垂直位置；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[y](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#y)
