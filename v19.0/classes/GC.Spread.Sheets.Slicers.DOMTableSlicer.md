# Class: DOMTableSlicer

[Sheets](../modules/GC.Spread.Sheets.md).[Slicers](../modules/GC.Spread.Sheets.Slicers.md).DOMTableSlicer

## Hierarchy

- [`FloatingObject`](GC.Spread.Sheets.FloatingObjects.FloatingObject.md)

  ↳ **`DOMTableSlicer`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#constructor)

### Properties

- [typeName](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#typename)

### Methods

- [allowMove](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#allowmove)
- [allowResize](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#allowresize)
- [alt](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#alt)
- [captionName](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#captionname)
- [cloneContent](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#clonecontent)
- [columnCount](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#columncount)
- [content](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#content)
- [disableResizingAndMoving](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#disableresizingandmoving)
- [dynamicMove](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#dynamicmove)
- [dynamicSize](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#dynamicsize)
- [endColumn](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#endcolumn)
- [endColumnOffset](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#endcolumnoffset)
- [endRow](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#endrow)
- [endRowOffset](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#endrowoffset)
- [fixedPosition](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#fixedposition)
- [getHost](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#gethost)
- [height](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#height)
- [isLocked](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#islocked)
- [isSelected](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#isselected)
- [isVisible](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#isvisible)
- [itemHeight](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#itemheight)
- [name](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#name)
- [refreshContent](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#refreshcontent)
- [showHeader](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#showheader)
- [showNoDataItems](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#shownodataitems)
- [showNoDataItemsInLast](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#shownodataitemsinlast)
- [sortState](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#sortstate)
- [startColumn](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#startcolumn)
- [startColumnOffset](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#startcolumnoffset)
- [startRow](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#startrow)
- [startRowOffset](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#startrowoffset)
- [style](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#style)
- [toImageSrc](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#toimagesrc)
- [toImageSrcAsync](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#toimagesrcasync)
- [visuallyNoDataItems](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#visuallynodataitems)
- [width](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#width)
- [x](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#x)
- [y](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#y)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new DOMTableSlicer**(`name`, `table`, `columnName`)

表示一个切片器。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 切片器名称。 |
| `table` | [`Table`](GC.Spread.Sheets.Tables.Table.md) | 与切片器关联的表格。 |
| `columnName` | `string` | 表格列的名称。 |

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
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

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
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

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
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

浮动对象的替代文本。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[alt](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#alt)

___

### <a id="captionname" name="captionname"></a> captionName

▸ **captionName**(`value?`): `any`

获取或设置切片器的标题名称。

**`example`**
```
//此示例使用captionName方法。
//创建表格
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
//切片器样式
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.light4();
var slicer = new GC.Spread.Sheets.Slicers.DOMTableSlicer('slicer1', table, 'Name');
// 将项目切片器添加到 DOM 树中。
// 其中 "slicerHost" 是你要用于承载切片器 DOM 元素的 div 容器。
var slicerHost = document.getElementById("slicerHost");
slicerHost.appendChild(slicer.cloneContent()); // 把切片器添加到 DOM 树中（完成挂载）
//更改切片器属性。
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.captionName("S1");
slicer.style(style1);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置值，返回切片器的标题名称；否则返回切片器。

___

### <a id="clonecontent" name="clonecontent"></a> cloneContent

▸ **cloneContent**(): `HTMLElement`

获取实例当前内容的副本。

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

实例当前内容的副本。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[cloneContent](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#clonecontent)

___

### <a id="columncount" name="columncount"></a> columnCount

▸ **columnCount**(`value?`): `any`

获取或设置切片器的列数。

**`example`**
```
//此示例更改切片器列数
//创建表格
var datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
//向工作表添加切片器并返回切片器实例。
var slicer = new GC.Spread.Sheets.Slicers.DOMTableSlicer('slicer1', table, 'Name');
// 将项目切片器添加到 DOM 树中。
// 其中 "slicerHost" 是你要用于承载切片器 DOM 元素的 div 容器。
var slicerHost = document.getElementById("slicerHost");
slicerHost.appendChild(slicer.cloneContent()); // 把切片器添加到 DOM 树中（完成挂载）
console.log(slicer.columnCount());
slicer.columnCount(3);
console.log(slicer.columnCount());
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置值，返回切片器的列数；否则返回切片器。

___

### <a id="content" name="content"></a> content

▸ **content**(`value?`): `any`

获取或设置自定义浮动对象的内容。

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `HTMLElement` |

#### Returns

`any`

如果未设置值，则返回自定义浮动对象的内容；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[content](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#content)

___

### <a id="disableresizingandmoving" name="disableresizingandmoving"></a> disableResizingAndMoving

▸ **disableResizingAndMoving**(`value?`): `any`

获取或设置是否禁用切片器的调整大小和移动。

**`example`**
```
//此示例阻止移动或调整切片器大小。
//创建表格
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
//切片器样式
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.light4();
var slicer = new GC.Spread.Sheets.Slicers.DOMTableSlicer('slicer1', table, 'Name');
// 将项目切片器添加到 DOM 树中。
// 其中 "slicerHost" 是你要用于承载切片器 DOM 元素的 div 容器。
var slicerHost = document.getElementById("slicerHost");
slicerHost.appendChild(slicer.cloneContent()); // 把切片器添加到 DOM 树中（完成挂载）
//更改切片器属性。
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.disableResizingAndMoving(true);
slicer.style(style1);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置值，返回是否禁用切片器的调整大小和移动；否则返回切片器。

___

### <a id="dynamicmove" name="dynamicmove"></a> dynamicMove

▸ **dynamicMove**(`value?`): `any`

获取或设置当隐藏或显示、调整大小或移动行或列时，对象是否移动。

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

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
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

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
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置值，则返回浮动对象位置的结束列索引；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[endColumn](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#endcolumn)

___

### <a id="endcolumnoffset" name="endcolumnoffset"></a> endColumnOffset

▸ **endColumnOffset**(`value?`): `any`

Gets or sets the offset relative to the end column of the floating object.

**`example`**
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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

If no value is set, returns the offset relative to the end column of the floating object; otherwise, returns the floating object.

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[endColumnOffset](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#endcolumnoffset)

___

### <a id="endrow" name="endrow"></a> endRow

▸ **endRow**(`value?`): `any`

获取或设置浮动对象位置的结束行索引。

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

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
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

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
```
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

### <a id="height" name="height"></a> height

▸ **height**(`value?`): `any`

获取或设置浮动对象的高度。

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

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

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

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
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

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
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置值，则返回此浮动对象是否可见；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[isVisible](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#isvisible)

___

### <a id="itemheight" name="itemheight"></a> itemHeight

▸ **itemHeight**(`value?`): `any`

获取或设置切片器的项目高度。

**`example`**
```
//此示例更改切片器项目高度。
//创建表格
var datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var slicer = new GC.Spread.Sheets.Slicers.DOMTableSlicer('slicer1', table, 'Name');
// 将项目切片器添加到 DOM 树中。
// 其中 "slicerHost" 是你要用于承载切片器 DOM 元素的 div 容器。
var slicerHost = document.getElementById("slicerHost");
slicerHost.appendChild(slicer.cloneContent()); // 把切片器添加到 DOM 树中（完成挂载）
console.log(slicer.itemHeight()); // 21
slicer.itemHeight(35);
console.log(slicer.itemHeight()); // 35
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置值，返回切片器的项目高度；否则返回切片器。

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置切片器的名称。

**`example`**
```javascript
//这个示例使用了name方法。
//创建一个表格
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
var slicer = new GC.Spread.Sheets.Slicers.DOMTableSlicer('slicer1', table, 'Name');
// 将项目切片器添加到 DOM 树中。
// 其中 "slicerHost" 是你要用于承载切片器 DOM 元素的 div 容器。
var slicerHost = document.getElementById("slicerHost");
slicerHost.appendChild(slicer.cloneContent()); // 把切片器添加到 DOM 树中（完成挂载）
console.log(slicer.name());
slicer.name("slicer2");
console.log(slicer.name());
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置值，返回切片器的名称；否则返回切片器。

#### Overrides

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[name](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#name)

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

### <a id="showheader" name="showheader"></a> showHeader

▸ **showHeader**(`value?`): `any`

获取或设置是否显示切片器标题。

**`example`**
```
//此示例隐藏切片器标题。
//创建表格
var datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
//切片器样式
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.light4();
//向工作表添加切片器并返回切片器实例。
var slicer = new GC.Spread.Sheets.Slicers.DOMTableSlicer('slicer1', table, 'Name');
// 将项目切片器添加到 DOM 树中。
// 其中 "slicerHost" 是你要用于承载切片器 DOM 元素的 div 容器。
var slicerHost = document.getElementById("slicerHost");
slicerHost.appendChild(slicer.cloneContent()); // 把切片器添加到 DOM 树中（完成挂载）
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.showHeader(false);
slicer.style(style1);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置值，返回是否显示切片器标题；否则返回切片器。

___

### <a id="shownodataitems" name="shownodataitems"></a> showNoDataItems

▸ **showNoDataItems**(`value?`): `any`

获取或设置是否显示切片器的无数据项目。

**`example`**
```
//创建表格
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
var slicer = new GC.Spread.Sheets.Slicers.DOMTableSlicer('slicer1', table, 'Name');
// 将项目切片器添加到 DOM 树中。
// 其中 "slicerHost" 是你要用于承载切片器 DOM 元素的 div 容器。
var slicerHost = document.getElementById("slicerHost");
slicerHost.appendChild(slicer.cloneContent()); // 把切片器添加到 DOM 树中（完成挂载）
//更改切片器属性。
slicer.showNoDataItems(false);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置值，返回是否显示切片器的无数据项目；否则返回切片器。

___

### <a id="shownodataitemsinlast" name="shownodataitemsinlast"></a> showNoDataItemsInLast

▸ **showNoDataItemsInLast**(`value?`): `any`

获取或设置是否最后显示无数据项目。

**`example`**
```
//创建表格
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
var slicer = new GC.Spread.Sheets.Slicers.DOMTableSlicer('slicer1', table, 'Name');
// 将项目切片器添加到 DOM 树中。
// 其中 "slicerHost" 是你要用于承载切片器 DOM 元素的 div 容器。
var slicerHost = document.getElementById("slicerHost");
slicerHost.appendChild(slicer.cloneContent()); // 把切片器添加到 DOM 树中（完成挂载）
//更改切片器属性。
slicer.showNoDataItemsInLast(false);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置值，返回是否最后显示无数据项目；否则返回切片器。

___

### <a id="sortstate" name="sortstate"></a> sortState

▸ **sortState**(`value?`): `any`

获取或设置切片器的排序状态。

**`example`**
```
//此示例设置切片器中项目的排序顺序。
//创建表格
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
// 切片器样式
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.light4();
var slicer = new GC.Spread.Sheets.Slicers.DOMTableSlicer('slicer1', table, 'Name');
// 将项目切片器添加到 DOM 树中。
// 其中 "slicerHost" 是你要用于承载切片器 DOM 元素的 div 容器。
var slicerHost = document.getElementById("slicerHost");
slicerHost.appendChild(slicer.cloneContent()); // 把切片器添加到 DOM 树中（完成挂载）
//设置切片器属性
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.sortState(GC.Spread.Sheets.SortState.descending);
slicer.style(style1);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SortState`](../enums/GC.Spread.Sheets.SortState.md) |

#### Returns

`any`

如果未设置值，返回切片器的排序状态；否则返回切片器。

___

### <a id="startcolumn" name="startcolumn"></a> startColumn

▸ **startColumn**(`value?`): `any`

获取或设置浮动对象位置的起始列索引。

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

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
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

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
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

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
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置值，则返回浮动对象相对于起始行的偏移量；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[startRowOffset](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#startrowoffset)

___

### <a id="style" name="style"></a> style

▸ **style**(`value?`): `any`

获取或设置切片器的样式。

**`example`**
```
// 此示例使用内置样式。
//创建表格
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
// 切片器样式
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.light4();
var slicer = new GC.Spread.Sheets.Slicers.DOMTableSlicer('slicer1', table, 'Name');
//更改切片器属性
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` \| [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md) | 切片器的样式或样式名称。切片器的style属性指定应用于切片器的视觉外观和格式样式，定义其整体外观和呈现方式。 |

#### Returns

`any`

如果未设置值，返回切片器的样式；否则返回切片器。

___

### <a id="toimagesrc" name="toimagesrc"></a> toImageSrc

▸ **toImageSrc**(): `string`

获取切片器图像的Base64字符串类型的src。

**`example`**
```
let slicerImageSrc = sheet.slicers.all()[0].toImageSrc();
```

#### Returns

`string`

返回切片器图像的Base64 src字符串。

___

### <a id="toimagesrcasync" name="toimagesrcasync"></a> toImageSrcAsync

▸ **toImageSrcAsync**(): `Promise`<`string`\>

获取切片器图像的Base64字符串类型的src。

**`example`**
```
let slicerImageSrc = await sheet.slicers.all()[0].toImageSrcAsync();
```

#### Returns

`Promise`<`string`\>

返回切片器图像的Base64 src字符串。

___

### <a id="visuallynodataitems" name="visuallynodataitems"></a> visuallyNoDataItems

▸ **visuallyNoDataItems**(`value?`): `any`

获取或设置是否在视觉上区分没有数据的项目。

**`example`**
```
//创建表格
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
var slicer = new GC.Spread.Sheets.Slicers.DOMTableSlicer('slicer1', table, 'Name');
// 将项目切片器添加到 DOM 树中。
// 其中 "slicerHost" 是你要用于承载切片器 DOM 元素的 div 容器。
var slicerHost = document.getElementById("slicerHost");
slicerHost.appendChild(slicer.cloneContent()); // 把切片器添加到 DOM 树中（完成挂载）
//更改切片器属性
slicer.visuallyNoDataItems(false);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置值，返回是否在视觉上区分没有数据的项目；否则返回切片器。

___

### <a id="width" name="width"></a> width

▸ **width**(`value?`): `any`

获取或设置浮动对象的宽度。

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

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
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

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
```
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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置值，则返回浮动对象的垂直位置；否则返回浮动对象。

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[y](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#y)
