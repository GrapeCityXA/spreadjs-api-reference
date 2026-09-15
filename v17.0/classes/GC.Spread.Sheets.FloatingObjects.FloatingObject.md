# Class: FloatingObject

[Sheets](../modules/GC.Spread.Sheets.md).[FloatingObjects](../modules/GC.Spread.Sheets.FloatingObjects.md).FloatingObject

## Hierarchy

- **`FloatingObject`**

  ↳ [`Chart`](GC.Spread.Sheets.Charts.Chart.md)

  ↳ [`Picture`](GC.Spread.Sheets.FloatingObjects.Picture.md)

  ↳ [`DOMTableSlicer`](GC.Spread.Sheets.Slicers.DOMTableSlicer.md)

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#constructor)

### Properties

- [typeName](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#typename)

### Methods

- [allowMove](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#allowmove)
- [allowResize](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#allowresize)
- [alt](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#alt)
- [cloneContent](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#clonecontent)
- [content](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#content)
- [dynamicMove](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#dynamicmove)
- [dynamicSize](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#dynamicsize)
- [endColumn](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#endcolumn)
- [endColumnOffset](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#endcolumnoffset)
- [endRow](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#endrow)
- [endRowOffset](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#endrowoffset)
- [fixedPosition](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#fixedposition)
- [getHost](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#gethost)
- [height](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#height)
- [isLocked](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#islocked)
- [isSelected](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#isselected)
- [isVisible](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#isvisible)
- [name](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#name)
- [refreshContent](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#refreshcontent)
- [startColumn](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#startcolumn)
- [startColumnOffset](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#startcolumnoffset)
- [startRow](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#startrow)
- [startRowOffset](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#startrowoffset)
- [width](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#width)
- [x](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#x)
- [y](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#y)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new FloatingObject**(`name`, `x`, `y`, `width`, `height`)

一个浮动对象元素

**`remarks`**
这是供内部使用的基类

**`代码示例`**
```
//本示例创建了一个浮动对象
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
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
| `name` | `string` | 浮动对象元素的名称 |
| `x` | `number` | 浮动对象元素的x位置 |
| `y` | `number` | 浮动对象元素的y位置 |
| `width` | `number` | 浮动对象元素的宽度 |
| `height` | `number` | 浮动对象元素的高度 |

## Properties

### <a id="typename" name="typename"></a> typeName

• **typeName**: `string`

支持序列化的类型名称字符串

## Methods

### <a id="allowmove" name="allowmove"></a> allowMove

▸ **allowMove**(`value?`): `any`

获取或设置是否禁用移动浮动对象元素

**`代码示例`**
```
//本示例阻止您移动或调整浮动对象元素的大小
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
| `value?` | `boolean` | 是否禁用移动浮动对象元素的设置 |

#### Returns

`any`

如果未设置任何值，则返回是否禁用移动浮动对象元素的设置；否则，返回浮动对象元素

___

### <a id="allowresize" name="allowresize"></a> allowResize

▸ **allowResize**(`value?`): `any`

获取或设置是否禁用调整浮动对象的大小

**`代码示例`**
```
//本示例阻止您移动或调整浮动对象元素的大小
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
| `value?` | `boolean` | 是否禁用调整浮动对象大小的设置 |

#### Returns

`any`

如果未设置任何值，则返回是否禁用调整浮动对象大小的设置；否则，返回浮动对象

___

### <a id="alt" name="alt"></a> alt

▸ **alt**(`value?`): `any`

获取或设置浮动对象的可选文本

**`example`**
```
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject('f1', 10, 10, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
customFloatingObject.alt("A button");
activeSheet.floatingObjects.add(customFloatingObject);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 浮动对象的可选文本 |

#### Returns

`any`

浮动对象的可选文本

___

### <a id="clonecontent" name="clonecontent"></a> cloneContent

▸ **cloneContent**(): `HTMLElement`

获取当前实例的内容副本

**`example`**
```
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

当前实例内容的副本

___

### <a id="content" name="content"></a> content

▸ **content**(`value?`): `any`

获取或设置自定义浮动对象元素的内容

**`example`**
```
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject('f1', 10, 10, 64, 30);
customFloatingObject.content(createButton('button 1', '64px', '30px'));
activeSheet.floatingObjects.add(customFloatingObject);

console.log(customFloatingObject.content()); // get current content, the result is button element with the text "button 1".
customFloatingObject.content(createButton('button 2', '64px', '30px')); // set new content.

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
| `value?` | `HTMLElement` | 自定义浮动对象元素的内容 |

#### Returns

`any`

如果未设置任何值，则返回自定义浮动对象元素的内容；否则，返回浮动对象元素

___

### <a id="dynamicmove" name="dynamicmove"></a> dynamicMove

▸ **dynamicMove**(`value?`): `any`

获取或设置对象在隐藏或显示，调整大小或移动行或列时是否移动

**`代码示例`**
```
//本示例创建了一个浮动对象
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
| `value?` | `boolean` | 该值指示对象在隐藏或显示，调整大小或移动行或列时是否移动 |

#### Returns

`any`

如果未设置任何值，则返回此浮动对象元素是否动态移动；否则，返回浮动对象元素

___

### <a id="dynamicsize" name="dynamicsize"></a> dynamicSize

▸ **dynamicSize**(`value?`): `any`

获取或设置在隐藏或显示，调整大小或移动行或列时对象的大小是否改变

**`代码示例`**
```
//本示例创建了一个浮动对象
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
| `value?` | `boolean` | 该值指示在隐藏或显示，调整大小或移动行或列时对象的大小是否改变 |

#### Returns

`any`

如果未设置任何值，则返回此浮动对象元素是否动态更改大小；否则，返回浮动对象元素

___

### <a id="endcolumn" name="endcolumn"></a> endColumn

▸ **endColumn**(`value?`): `any`

获取或设置浮动对象元素位置的结束列索引

**`代码示例`**
```
//Creates a floating object.
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
//Position the upper left corner of the floating object by cell anchors.
customFloatingObject.startRow(2);
customFloatingObject.startColumn(2);
customFloatingObject.startRowOffset(10);
customFloatingObject.startColumnOffset(10);
//Position the lower right corner of the floating object by cell anchors.
customFloatingObject.endRow(7);
customFloatingObject.endColumn(5);
customFloatingObject.endRowOffset(10);
customFloatingObject.endColumnOffset(10);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 浮动对象元素位置的结束列索引 |

#### Returns

`any`

如果未设置任何值，则返回浮动对象元素位置的结束列索引；否则，返回浮动对象元素

___

### <a id="endcolumnoffset" name="endcolumnoffset"></a> endColumnOffset

▸ **endColumnOffset**(`value?`): `any`

获取或设置相对于浮动对象元素的结束列的偏移量

**`代码示例`**
```
//Creates a floating object.
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
//Position the upper left corner of the floating object by cell anchors.
customFloatingObject.startRow(2);
customFloatingObject.startColumn(2);
customFloatingObject.startRowOffset(10);
customFloatingObject.startColumnOffset(10);
//Position the lower right corner of the floating object by cell anchors.
customFloatingObject.endRow(7);
customFloatingObject.endColumn(5);
customFloatingObject.endRowOffset(10);
customFloatingObject.endColumnOffset(10);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 相对于浮动对象元素的结束列的偏移量 |

#### Returns

`any`

如果未设置任何值，则返回相对于浮动对象元素的结束列的偏移量；否则，返回浮动对象元素

___

### <a id="endrow" name="endrow"></a> endRow

▸ **endRow**(`value?`): `any`

获取或设置浮动对象元素位置的末行索引

**`代码示例`**
```
//本示例创建了一个浮动对象
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
//Position the upper left corner of the floating object by cell anchors.
customFloatingObject.startRow(2);
customFloatingObject.startColumn(2);
customFloatingObject.startRowOffset(10);
customFloatingObject.startColumnOffset(10);
//Position the lower right corner of the floating object by cell anchors.
customFloatingObject.endRow(7);
customFloatingObject.endColumn(5);
customFloatingObject.endRowOffset(10);
customFloatingObject.endColumnOffset(10);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 浮动对象元素位置的末行索引 |

#### Returns

`any`

如果未设置任何值，则返回浮动对象元素位置的末端行索引；否则，返回浮动对象元素

___

### <a id="endrowoffset" name="endrowoffset"></a> endRowOffset

▸ **endRowOffset**(`value?`): `any`

获取或设置相对于浮动对象元素的最后一行的偏移量

**`代码示例`**
```
//本示例创建了一个浮动对象
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
//Position the upper left corner of the floating object by cell anchors.
customFloatingObject.startRow(2);
customFloatingObject.startColumn(2);
customFloatingObject.startRowOffset(10);
customFloatingObject.startColumnOffset(10);
//Position the lower right corner of the floating object by cell anchors.
customFloatingObject.endRow(7);
customFloatingObject.endColumn(5);
customFloatingObject.endRowOffset(10);
customFloatingObject.endColumnOffset(10);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 相对于浮动对象元素的最后一行的偏移量 |

#### Returns

`any`

如果未设置任何值，则返回相对于浮动对象元素的最后一行的偏移量；否则，返回浮动对象元素

___

### <a id="fixedposition" name="fixedposition"></a> fixedPosition

▸ **fixedPosition**(`value`): `any`

获取或设置浮动对象元素的位置是否固定 当fixedPosition为true时,dynamicMove和dynamicSize被禁用

**`代码示例`**
```
//本示例将对象的位置设置为固定
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

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `boolean` | 该值指示浮动对象元素的位置是否固定 |

#### Returns

`any`

如果未设置任何值，则返回浮动对象元素的位置是否固定 否则，返回浮动对象元素

___

### <a id="gethost" name="gethost"></a> getHost

▸ **getHost**(): `HTMLElement`[]

获取自定义内容的dom宿主

#### Returns

`HTMLElement`[]

___

### <a id="height" name="height"></a> height

▸ **height**(`value?`): `any`

获取或设置浮动对象元素的高度

**`代码示例`**
```
//本示例创建了一个浮动对象
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
| `value?` | `number` | 浮动对象元素的高度 |

#### Returns

`any`

如果未设置任何值，则返回一个浮动对象元素的高度；否则，返回浮动对象元素

___

### <a id="islocked" name="islocked"></a> isLocked

▸ **isLocked**(`value?`): `any`

获取或设置此浮动对象元素是否被锁定

**`代码示例`**
```
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
| `value?` | `boolean` | 该值指示此浮动对象元素是否被锁定 |

#### Returns

`any`

如果未设置任何值，则返回此浮动对象元素是否被锁定；否则，返回浮动对象元素

___

### <a id="isselected" name="isselected"></a> isSelected

▸ **isSelected**(`value?`): `any`

获取或设置是否选择此浮动对象元素

**`代码示例`**
```
//本示例创建了一个浮动对象
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
| `value?` | `boolean` | 该值指示此浮动对象元素是否被选择 |

#### Returns

`any`

如果未设置任何值，则返回是否选择此浮动对象元素；否则，返回浮动对象元素

___

### <a id="isvisible" name="isvisible"></a> isVisible

▸ **isVisible**(`value?`): `any`

获取或设置此浮动对象元素是否可见

**`代码示例`**
```
//本示例创建了一个浮动对象
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
| `value?` | `boolean` | 该值指示此浮动对象元素是否可见 |

#### Returns

`any`

如果未设置任何值，则返回此浮动对象元素是否可见；否则，返回浮动对象元素

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取浮动对象元素的名称

**`代码示例`**
```
//本示例使用name方法
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
| `value?` | `string` | 浮动对象元素的名称 |

#### Returns

`any`

如果未设置任何值，则返回浮动对象元素的名称；否则，返回浮动对象元素

___

### <a id="refreshcontent" name="refreshcontent"></a> refreshContent

▸ **refreshContent**(): `void`

刷新floatObject中的内容用户应重写此方法，以使其内容与floatObject同步

#### Returns

`void`

___

### <a id="startcolumn" name="startcolumn"></a> startColumn

▸ **startColumn**(`value?`): `any`

获取或设置浮动对象元素位置的起始列索引

**`代码示例`**
```
//本示例创建了一个浮动对象
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
//加入表中时生效
customFloatingObject.startRow(2);
customFloatingObject.startColumn(2);
customFloatingObject.startRowOffset(10);
customFloatingObject.startColumnOffset(10);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 浮动对象元素位置的起始列索引 |

#### Returns

`any`

如果未设置任何值，则返回浮动对象元素位置的起始列索引；否则，返回浮动对象元素

___

### <a id="startcolumnoffset" name="startcolumnoffset"></a> startColumnOffset

▸ **startColumnOffset**(`value?`): `any`

获取或设置相对于浮动对象元素的起始列的偏移量

**`代码示例`**
```
//本示例创建了一个浮动对象
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
//加入表中时生效
customFloatingObject.startRow(2);
customFloatingObject.startColumn(2);
customFloatingObject.startRowOffset(10);
customFloatingObject.startColumnOffset(10);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 相对于浮动对象元素的起始列的偏移量 |

#### Returns

`any`

如果未设置任何值，则返回相对于浮动对象元素的起始列的偏移量；否则，返回浮动对象元素

___

### <a id="startrow" name="startrow"></a> startRow

▸ **startRow**(`value?`): `any`

获取或设置浮动对象元素位置的起始行索引

**`代码示例`**
```
//本示例创建了一个浮动对象
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
//加入表中时生效
customFloatingObject.startRow(2);
customFloatingObject.startColumn(2);
customFloatingObject.startRowOffset(10);
customFloatingObject.startColumnOffset(10);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 动对象元素位置的起始行索引 |

#### Returns

`any`

如果未设置任何值，则返回浮动对象元素位置的起始行索引；否则，返回浮动对象

___

### <a id="startrowoffset" name="startrowoffset"></a> startRowOffset

▸ **startRowOffset**(`value?`): `any`

获取或设置相对于浮动对象元素的起始行的偏移量

**`代码示例`**
```
//本示例创建了一个浮动对象
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
//加入表中时生效
customFloatingObject.startRow(2);
customFloatingObject.startColumn(2);
customFloatingObject.startRowOffset(10);
customFloatingObject.startColumnOffset(10);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 相对于浮动对象元素的起始行的偏移量 |

#### Returns

`any`

如果未设置任何值，则返回相对于浮动对象元素起始行的偏移量；否则，返回浮动对象元素

___

### <a id="width" name="width"></a> width

▸ **width**(`value?`): `any`

获取或设置浮动对象元素的宽度

**`代码示例`**
```
//本示例创建了一个浮动对象
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
| `value?` | `number` | 浮动对象元素的宽度 |

#### Returns

`any`

如果未设置任何值，则返回一个浮动对象元素的宽度；否则，返回浮动对象元素

___

### <a id="x" name="x"></a> x

▸ **x**(`value?`): `any`

获取或设置浮动对象元素的水平位置

**`代码示例`**
```
//本示例创建了一个浮动对象
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
| `value?` | `number` | 浮动对象元素的水平位置 |

#### Returns

`any`

如果未设置任何值，则返回浮动对象元素的水平位置；否则，返回浮动对象元素

___

### <a id="y" name="y"></a> y

▸ **y**(`value?`): `any`

获取或设置浮动对象元素的垂直位置

**`代码示例`**
```
//本示例创建了一个浮动对象
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
| `value?` | `number` | 获取或设置浮动对象元素的垂直位置 |

#### Returns

`any`

如果未设置任何值，则返回浮动对象对象的垂直位置；否则，返回浮动对象元素
