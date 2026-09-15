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
- [visuallyNoDataItems](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#visuallynodataitems)
- [width](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#width)
- [x](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#x)
- [y](GC.Spread.Sheets.Slicers.DOMTableSlicer.md#y)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new DOMTableSlicer**(`name`, `table`, `columnName`)

切片器

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 切片器名称 |
| `table` | [`Table`](GC.Spread.Sheets.Tables.Table.md) | 与切片器有关的表 |
| `columnName` | `string` | 表的列的名称 |

#### Overrides

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[constructor](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#constructor)

## Properties

### <a id="typename" name="typename"></a> typeName

• **typeName**: `string`

支持序列化的类型名称字符串

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[typeName](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#typename)

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

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[allowMove](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#allowmove)

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

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[allowResize](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#allowresize)

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

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[alt](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#alt)

___

### <a id="captionname" name="captionname"></a> captionName

▸ **captionName**(`value?`): `any`

获取或设置切片器的标题名称

**`代码示例`**
```
//本示例使用了captionName方法
//create a table
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
//切片器样式
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.light4();
var slicer = new GC.Spread.Sheets.Slicers.DOMTableSlicer('slicer1', table, 'Name');
 //改变切片器的属性
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

如果没有设置值，返回切片器的标题名称；否则，返回切片器

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

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[cloneContent](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#clonecontent)

___

### <a id="columncount" name="columncount"></a> columnCount

▸ **columnCount**(`value?`): `any`

获取或设置切片器的列数

**`example`**
```
//This example changes the slicer column count
//create a table
datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
//add a slicer to the sheet and return the slicer instance.
var slicer = new GC.Spread.Sheets.Slicers.DOMTableSlicer('slicer1', table, 'Name');
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

如果没有设置值，返回切片器的列数；否则，返回切片器

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

| Name | Type |
| :------ | :------ |
| `value?` | `HTMLElement` |

#### Returns

`any`

如果未设置任何值，则返回自定义浮动对象元素的内容；否则，返回浮动对象元素

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[content](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#content)

___

### <a id="disableresizingandmoving" name="disableresizingandmoving"></a> disableResizingAndMoving

▸ **disableResizingAndMoving**(`value?`): `any`

获取或设置是否禁止调整切片器的大小和移动

**`代码示例`**
```
//本示例禁止移动或调整切片器的大小
//创建一个表
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
//切片器样式
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.light4();
var slicer = new GC.Spread.Sheets.Slicers.DOMTableSlicer('slicer1', table, 'Name');
//change the slicer properties.
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

如果没有设置值，则返回是否禁用调整大小和移动切片器；否则，返回切片器

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

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[dynamicMove](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#dynamicmove)

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

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[dynamicSize](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#dynamicsize)

___

### <a id="endcolumn" name="endcolumn"></a> endColumn

▸ **endColumn**(`value?`): `any`

获取或设置浮动对象元素位置的结束列索引

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
| `value?` | `number` | 浮动对象元素位置的结束列索引 |

#### Returns

`any`

如果未设置任何值，则返回浮动对象元素位置的结束列索引；否则，返回浮动对象元素

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[endColumn](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#endcolumn)

___

### <a id="endcolumnoffset" name="endcolumnoffset"></a> endColumnOffset

▸ **endColumnOffset**(`value?`): `any`

获取或设置相对于浮动对象元素的结束列的偏移量

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
| `value?` | `number` | 相对于浮动对象元素的结束列的偏移量 |

#### Returns

`any`

如果未设置任何值，则返回相对于浮动对象元素的结束列的偏移量；否则，返回浮动对象元素

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[endColumnOffset](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#endcolumnoffset)

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

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[endRow](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#endrow)

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

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[endRowOffset](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#endrowoffset)

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

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[fixedPosition](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#fixedposition)

___

### <a id="gethost" name="gethost"></a> getHost

▸ **getHost**(): `HTMLElement`[]

获取自定义内容的dom宿主

#### Returns

`HTMLElement`[]

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[getHost](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#gethost)

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

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[height](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#height)

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

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[isLocked](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#islocked)

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

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[isSelected](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#isselected)

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

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[isVisible](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#isvisible)

___

### <a id="itemheight" name="itemheight"></a> itemHeight

▸ **itemHeight**(`value?`): `any`

获取或设置切片器的项高度

**`example`**
```
//This example changes the slicer item height.
//create a table
datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);

var slicer = new GC.Spread.Sheets.Slicers.DOMTableSlicer('slicer1', table, 'Name');
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

如果没有设置值，返回切片器的项高度；否则，返回切片器

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置切片器的name

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果没有设置值，返回切片器的名称；否则，返回切片器

#### Overrides

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[name](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#name)

___

### <a id="refreshcontent" name="refreshcontent"></a> refreshContent

▸ **refreshContent**(): `void`

刷新floatObject中的内容用户应重写此方法，以使其内容与floatObject同步

#### Returns

`void`

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[refreshContent](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#refreshcontent)

___

### <a id="showheader" name="showheader"></a> showHeader

▸ **showHeader**(`value?`): `any`

获取或设置是否显示切片器的标题

**`代码示例`**
```
//This example hides the slicer header.
//create a table
datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
//slicer style
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.light4();
//add a slicer to the sheet and return the slicer instance.
var slicer = new GC.Spread.Sheets.Slicers.DOMTableSlicer('slicer1', table, 'Name');
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

如果未设置值，则返回是否显示切片器头；否则，返回切片器

___

### <a id="shownodataitems" name="shownodataitems"></a> showNoDataItems

▸ **showNoDataItems**(`value?`): `any`

获取或设置是显示切片器的无数据项

**`example`**
```
//create a table
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
var slicer = new GC.Spread.Sheets.Slicers.DOMTableSlicer('slicer1', table, 'Name');
//change the slicer properties.
slicer.showNoDataItems(false);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值，返回是否显示切片器标题；否则，返回切片器

___

### <a id="shownodataitemsinlast" name="shownodataitemsinlast"></a> showNoDataItemsInLast

▸ **showNoDataItemsInLast**(`value?`): `any`

获取或设置是否最后显示无数据项

**`example`**
```
//本示例设置切片器中项的排序顺序
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
var slicer = new GC.Spread.Sheets.Slicers.DOMTableSlicer('slicer1', table, 'Name');
//change the slicer properties.
slicer.showNoDataItemsInLast(false);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值，返回是否显示切片器的排序状态；否则，返回切片器

___

### <a id="sortstate" name="sortstate"></a> sortState

▸ **sortState**(`value?`): `any`

获取或设置相对于浮动对象元素的起始行的偏移量

**`example`**
```
//This example sets the sort order of the items in the slicer.
//create a table
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
// slicer style
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.light4();
var slicer = new GC.Spread.Sheets.Slicers.DOMTableSlicer('slicer1', table, 'Name');
//set slicer properties
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

如果未设置值，请返回切片器的排序状态；否则，返回切片器

___

### <a id="startcolumn" name="startcolumn"></a> startColumn

▸ **startColumn**(`value?`): `any`

Gets or sets the starting column index of the floating object position.

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
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置值，请返回浮动对象位置的起始列索引；否则，返回浮动对象

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[startColumn](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#startcolumn)

___

### <a id="startcolumnoffset" name="startcolumnoffset"></a> startColumnOffset

▸ **startColumnOffset**(`value?`): `any`

获取或设置相对于浮动对象的开始列的偏移

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
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置值，请返回相对于浮动对象的开始列的偏移；否则，返回浮动对象

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[startColumnOffset](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#startcolumnoffset)

___

### <a id="startrow" name="startrow"></a> startRow

▸ **startRow**(`value?`): `any`

Gets or sets the starting row index of the floating object position.

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
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置值，请返回浮动对象位置的开始行索引；否则，返回浮动对象

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[startRow](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#startrow)

___

### <a id="startrowoffset" name="startrowoffset"></a> startRowOffset

▸ **startRowOffset**(`value?`): `any`

获取或设置相对于浮动对象的开始行的偏移

**`example`**
```
//This example creates a floating object.
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
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置值，请返回相对于浮动对象的开始行返回偏移；否则，返回浮动对象

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[startRowOffset](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#startrowoffset)

___

### <a id="style" name="style"></a> style

▸ **style**(`value?`): `any`

Gets or sets the style of the slicer.

**`example`**
```
//This example uses a built-in style.
//create a table
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
// slicer style
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.light4();
var slicer = new GC.Spread.Sheets.Slicers.DOMTableSlicer('slicer1', table, 'Name');
//change the slicer properties.
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md) | 切片器样式 |

#### Returns

`any`

如果没有设置值，返回是否显示切片器样式；否则，返回切片器

___

### <a id="visuallynodataitems" name="visuallynodataitems"></a> visuallyNoDataItems

▸ **visuallyNoDataItems**(`value?`): `any`

获取或设置是否在视觉上区分没有数据的项

**`example`**
```
//create a table
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
var slicer = new GC.Spread.Sheets.Slicers.DOMTableSlicer('slicer1', table, 'Name');
//change the slicer properties.
slicer.visuallyNoDataItems(false);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值，返回是否在视觉区分没有数据的项；否则，返回切片器

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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置任何值，则返回一个浮动对象元素的宽度；否则，返回浮动对象元素

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[width](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#width)

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

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置任何值，则返回浮动对象元素的水平位置；否则，返回浮动对象元素

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[x](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#x)

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

#### Inherited from

[FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md).[y](GC.Spread.Sheets.FloatingObjects.FloatingObject.md#y)
