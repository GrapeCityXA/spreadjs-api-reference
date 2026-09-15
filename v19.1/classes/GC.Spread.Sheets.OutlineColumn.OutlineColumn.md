# Class: OutlineColumn

[Sheets](../modules/GC.Spread.Sheets.md).[OutlineColumn](../modules/GC.Spread.Sheets.OutlineColumn.md).OutlineColumn

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.OutlineColumn.OutlineColumn.md#constructor)

### Methods

- [getCheckStatus](GC.Spread.Sheets.OutlineColumn.OutlineColumn.md#getcheckstatus)
- [getCollapsed](GC.Spread.Sheets.OutlineColumn.OutlineColumn.md#getcollapsed)
- [options](GC.Spread.Sheets.OutlineColumn.OutlineColumn.md#options)
- [refresh](GC.Spread.Sheets.OutlineColumn.OutlineColumn.md#refresh)
- [setCheckStatus](GC.Spread.Sheets.OutlineColumn.OutlineColumn.md#setcheckstatus)
- [setCollapsed](GC.Spread.Sheets.OutlineColumn.OutlineColumn.md#setcollapsed)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new OutlineColumn**(`sheet`)

表示一个缩进列。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheet` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | outlineColumn的工作表。 |

## Methods

### <a id="getcheckstatus" name="getcheckstatus"></a> getCheckStatus

▸ **getCheckStatus**(`row?`): `any`

获取行或所有行的选中状态。

**`example`**
```javascript
spread.suspendPaint();
var activeSheet = spread.getActiveSheet();
activeSheet.setValue(0, 0, "Name", GC.Spread.Sheets.SheetArea.colHeader);
activeSheet.setValue(0, 1, "Chapter", GC.Spread.Sheets.SheetArea.colHeader);
activeSheet.setValue(0, 2, "Page", GC.Spread.Sheets.SheetArea.colHeader);
activeSheet.setColumnWidth(0, 200);
activeSheet.setRowCount(13);
var commands = [
    {name: 'Preface', chapter: '1', page: 1, indent: 0},
    {name: 'Java SE5 and SE6', chapter: '1.1', page: 2, indent: 1},
    {name: 'Java SE6', chapter: '1.1.1', page: 2, indent: 2},
    {name: 'The 4th edition', chapter: '1.2', page: 2, indent: 1},
    {name: 'Changes', chapter: '1.2.1', page: 3, indent: 2},
    {name: 'Note on the cover design', chapter: '1.3', page: 4, indent: 1},
    {name: 'Acknowledgements', chapter: '1.4', page: 4, indent: 1},
    {name: 'Introduction', chapter: '2', page: 9, indent: 0},
    {name: 'Prerequisites', chapter: '2.1', page: 9, indent: 1},
    {name: 'Learning Java', chapter: '2.2', page: 10, indent: 1},
    {name: 'Goals', chapter: '2.3', page: 10, indent: 1},
    {name: 'Teaching from this book', chapter: '2.4', page: 11, indent: 1},
    {name: 'JDK HTML documentation', chapter: '2.5', page: 11, indent: 1},
];
for (var r = 0; r < commands.length; r++) {
    activeSheet.setValue(r, 0, commands[r]['name']);
    activeSheet.setValue(r, 1, commands[r]['chapter']);
    activeSheet.setValue(r, 2, commands[r]['page']);
    activeSheet.getRange(r, 0, 1, 1).textIndent(commands[r].indent);
}
activeSheet.outlineColumn.options({
     columnIndex: 0,
     showImage: true,
     showCheckBox: true,
     images: ['star2.png', 'box4.png', 'rating4.png'],
     maxLevel: 2
});
activeSheet.showRowOutline(true);
spread.invalidateLayout();
spread.resumePaint();

console.log(activeSheet.outlineColumn.getCheckStatus(1)); // false
activeSheet.outlineColumn.setCheckStatus(1, true);
console.log(activeSheet.outlineColumn.getCheckStatus(1)); // true
console.log(activeSheet.outlineColumn.getCheckStatus(2)); // true -> sub node of row 1
console.log(activeSheet.outlineColumn.getCheckStatus()); // [false, true, true, false, false, false, false, false, false, false, false, false, false]
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row?` | `number` | 行的索引。 |

#### Returns

`any`

如果row未定义，返回所有行的选中状态；否则返回指定行的选中状态。

___

### <a id="getcollapsed" name="getcollapsed"></a> getCollapsed

▸ **getCollapsed**(`row?`): `any`

获取行或所有行的折叠设置。

**`example`**
```javascript
spread.suspendPaint();
var activeSheet = spread.getActiveSheet();
activeSheet.setValue(0, 0, "Name", GC.Spread.Sheets.SheetArea.colHeader);
activeSheet.setValue(0, 1, "Chapter", GC.Spread.Sheets.SheetArea.colHeader);
activeSheet.setValue(0, 2, "Page", GC.Spread.Sheets.SheetArea.colHeader);
activeSheet.setColumnWidth(0, 200);
activeSheet.setRowCount(13);
var commands = [
    {name: 'Preface', chapter: '1', page: 1, indent: 0},
    {name: 'Java SE5 and SE6', chapter: '1.1', page: 2, indent: 1},
    {name: 'Java SE6', chapter: '1.1.1', page: 2, indent: 2},
    {name: 'The 4th edition', chapter: '1.2', page: 2, indent: 1},
    {name: 'Changes', chapter: '1.2.1', page: 3, indent: 2},
    {name: 'Note on the cover design', chapter: '1.3', page: 4, indent: 1},
    {name: 'Acknowledgements', chapter: '1.4', page: 4, indent: 1},
    {name: 'Introduction', chapter: '2', page: 9, indent: 0},
    {name: 'Prerequisites', chapter: '2.1', page: 9, indent: 1},
    {name: 'Learning Java', chapter: '2.2', page: 10, indent: 1},
    {name: 'Goals', chapter: '2.3', page: 10, indent: 1},
    {name: 'Teaching from this book', chapter: '2.4', page: 11, indent: 1},
    {name: 'JDK HTML documentation', chapter: '2.5', page: 11, indent: 1},
];
for (var r = 0; r < commands.length; r++) {
    activeSheet.setValue(r, 0, commands[r]['name']);
    activeSheet.setValue(r, 1, commands[r]['chapter']);
    activeSheet.setValue(r, 2, commands[r]['page']);
    activeSheet.getRange(r, 0, 1, 1).textIndent(commands[r].indent);
}
activeSheet.outlineColumn.options({
     columnIndex: 0,
     showImage: true,
     showCheckBox: true,
     images: ['star2.png', 'box4.png', 'rating4.png'],
     maxLevel: 2
});
activeSheet.showRowOutline(true);
spread.invalidateLayout();
spread.resumePaint();

console.log(activeSheet.outlineColumn.getCollapsed(1)); // false
activeSheet.outlineColumn.setCollapsed(1, true);
console.log(activeSheet.outlineColumn.getCollapsed(1)); // true
console.log(activeSheet.outlineColumn.getCollapsed(2)); // false -> sub node of row 1
console.log(activeSheet.outlineColumn.getCollapsed()); // [false, true, false, false, false, false, false, false, false, false, false, false, false]
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row?` | `number` | 折叠行的索引。 |

#### Returns

`any`

如果row未定义，返回所有行的折叠状态；否则返回指定行的折叠设置。

___

### <a id="options" name="options"></a> options

▸ **options**(`outlineColumnOptions?`): `any`

获取或设置大纲列的选项。

**`example`**
```javascript
var rowCount = 38;
var colCount = 10;
activeSheet.setColumnCount(colCount);
activeSheet.setRowCount(rowCount);
activeSheet.setColumnWidth(0, 310);
activeSheet.setColumnWidth(1, 150);
activeSheet.setColumnWidth(2, 150);
activeSheet.frozenColumnCount(1);
activeSheet.setValue(0, 0, "Name", GC.Spread.Sheets.SheetArea.colHeader);
activeSheet.setValue(0, 1, "Chapter", GC.Spread.Sheets.SheetArea.colHeader);
activeSheet.setValue(0, 2, "Page", GC.Spread.Sheets.SheetArea.colHeader);
var commands = [
    {name: 'Preface', chapter: '1', page: 1, indent: 0},
    {name: 'Java SE5 and SE6', chapter: '1.1', page: 2, indent: 1},
    {name: 'Java SE6', chapter: '1.1.1', page: 2, indent: 2},
    {name: 'The 4th edition', chapter: '1.2', page: 2, indent: 1},
    {name: 'Changes', chapter: '1.2.1', page: 3, indent: 2},
    {name: 'Note on the cover design', chapter: '1.3', page: 4, indent: 1},
    {name: 'Acknowledgements', chapter: '1.4', page: 4, indent: 1},
    {name: 'Introduction', chapter: '2', page: 9, indent: 0},
    {name: 'Prerequisites', chapter: '2.1', page: 9, indent: 1},
    {name: 'Learning Java', chapter: '2.2', page: 10, indent: 1},
    {name: 'Goals', chapter: '2.3', page: 10, indent: 1},
    {name: 'Teaching from this book', chapter: '2.4', page: 11, indent: 1},
    {name: 'JDK HTML documentation', chapter: '2.5', page: 11, indent: 1},
    {name: 'Exercises', chapter: '2.6', page: 12, indent: 1},
    {name: 'Foundations for Java', chapter: '2.7', page: 12, indent: 1},
    {name: 'Source code', chapter: '2.8', page: 12, indent: 1},
    {name: 'Coding standards', chapter: '2.8.1', page: 14, indent: 2},
    {name: 'Errors', chapter: '2.9', page: 14, indent: 1},
    {name: 'Introduction to Objects', chapter: '3', page: 15, indent: 0},
    {name: 'The progress of abstraction', chapter: '3.1', page: 15, indent: 1},
    {name: 'An object has an interface', chapter: '3.2', page: 17, indent: 1},
    {name: 'An object provides services', chapter: '3.3', page: 18, indent: 1},
    {name: 'The hidden implementation', chapter: '3.4', page: 19, indent: 1},
    {name: 'Reusing the implementation', chapter: '3.5', page: 20, indent: 1},
    {name: 'Inheritance', chapter: '3.6', page: 21, indent: 1},
    {name: 'Is-a vs. is-like-a relationships', chapter: '3.6.1', page: 24, indent: 2},
    {name: 'Interchangeable objects with polymorphism', chapter: '3.7', page: 25, indent: 1},
    {name: 'The singly rooted hierarchy', chapter: '3.8', page: 28, indent: 1},
    {name: 'Containers', chapter: '3.9', page: 28, indent: 1},
    {name: 'Parameterized types (Generics)', chapter: '3.10', page: 29, indent: 1},
    {name: 'Object creation & lifetime', chapter: '3.11', page: 30, indent: 1},
    {name: 'Exception handling: dealing with errors', chapter: '3.12', page: 31, indent: 1},
    {name: 'Concurrent programming', chapter: '3.13', page: 32, indent: 1},
    {name: 'Java and the Internet', chapter: '3.14', page: 33, indent: 1},
    {name: 'What is the Web?', chapter: '3.14.1', page: 33, indent: 2},
    {name: 'Client-side programming', chapter: '3.14.2', page: 34, indent: 2},
    {name: 'Server-side programming', chapter: '3.14.3', page: 38, indent: 2},
    {name: 'Summary', chapter: '3.15', page: 38, indent: 1},
];
for (var r = 0; r < commands.length; r++) {
    activeSheet.setValue(r, 0, commands[r]['name']);
    activeSheet.setValue(r, 1, commands[r]['chapter']);
    activeSheet.setValue(r, 2, commands[r]['page']);
    activeSheet.getRange(r, 0, 1, 1).textIndent(commands[r].indent);
}
activeSheet.outlineColumn.options({
     columnIndex: 0,
     showImage: true,
     showCheckBox: true,
     images: ['star2.png', 'box4.png', 'rating4.png'],
     maxLevel: 2
});
activeSheet.showRowOutline(true);
spread.invalidateLayout();
spread.repaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `outlineColumnOptions?` | [`IOutlineColumnOptions`](../interfaces/GC.Spread.Sheets.OutlineColumn.IOutlineColumnOptions.md) | 大纲列的选项。 |

#### Returns

`any`

outlineColumnOptions|outlineColumn
如果未设置outlineColumnOptions项，则返回outlineColumnOptions；否则返回outlineColumn实例。

___

### <a id="refresh" name="refresh"></a> refresh

▸ **refresh**(): `void`

刷新缩进列。

#### Returns

`void`

___

### <a id="setcheckstatus" name="setcheckstatus"></a> setCheckStatus

▸ **setCheckStatus**(`row`, `checkStatus`): `void`

设置行的选中状态。

**`example`**
```javascript
spread.suspendPaint();
var activeSheet = spread.getActiveSheet();
activeSheet.setValue(0, 0, "Name", GC.Spread.Sheets.SheetArea.colHeader);
activeSheet.setValue(0, 1, "Chapter", GC.Spread.Sheets.SheetArea.colHeader);
activeSheet.setValue(0, 2, "Page", GC.Spread.Sheets.SheetArea.colHeader);
activeSheet.setColumnWidth(0, 200);
activeSheet.setRowCount(13);
var commands = [
    {name: 'Preface', chapter: '1', page: 1, indent: 0},
    {name: 'Java SE5 and SE6', chapter: '1.1', page: 2, indent: 1},
    {name: 'Java SE6', chapter: '1.1.1', page: 2, indent: 2},
    {name: 'The 4th edition', chapter: '1.2', page: 2, indent: 1},
    {name: 'Changes', chapter: '1.2.1', page: 3, indent: 2},
    {name: 'Note on the cover design', chapter: '1.3', page: 4, indent: 1},
    {name: 'Acknowledgements', chapter: '1.4', page: 4, indent: 1},
    {name: 'Introduction', chapter: '2', page: 9, indent: 0},
    {name: 'Prerequisites', chapter: '2.1', page: 9, indent: 1},
    {name: 'Learning Java', chapter: '2.2', page: 10, indent: 1},
    {name: 'Goals', chapter: '2.3', page: 10, indent: 1},
    {name: 'Teaching from this book', chapter: '2.4', page: 11, indent: 1},
    {name: 'JDK HTML documentation', chapter: '2.5', page: 11, indent: 1},
];
for (var r = 0; r < commands.length; r++) {
    activeSheet.setValue(r, 0, commands[r]['name']);
    activeSheet.setValue(r, 1, commands[r]['chapter']);
    activeSheet.setValue(r, 2, commands[r]['page']);
    activeSheet.getRange(r, 0, 1, 1).textIndent(commands[r].indent);
}
activeSheet.outlineColumn.options({
     columnIndex: 0,
     showImage: true,
     showCheckBox: true,
     images: ['star2.png', 'box4.png', 'rating4.png'],
     maxLevel: 2
});
activeSheet.showRowOutline(true);
spread.invalidateLayout();
spread.resumePaint();

console.log(activeSheet.outlineColumn.getCheckStatus(1)); // false
activeSheet.outlineColumn.setCheckStatus(1, true);
console.log(activeSheet.outlineColumn.getCheckStatus(1)); // true
console.log(activeSheet.outlineColumn.getCheckStatus(2)); // true -> sub node of row 1
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行的索引。 |
| `checkStatus` | `boolean` | 行的选中状态。 |

#### Returns

`void`

___

### <a id="setcollapsed" name="setcollapsed"></a> setCollapsed

▸ **setCollapsed**(`row`, `collapsed`): `void`

设置行是否折叠。

**`example`**
```javascript
spread.suspendPaint();
var activeSheet = spread.getActiveSheet();
activeSheet.setValue(0, 0, "Name", GC.Spread.Sheets.SheetArea.colHeader);
activeSheet.setValue(0, 1, "Chapter", GC.Spread.Sheets.SheetArea.colHeader);
activeSheet.setValue(0, 2, "Page", GC.Spread.Sheets.SheetArea.colHeader);
activeSheet.setColumnWidth(0, 200);
activeSheet.setRowCount(13);
var commands = [
    {name: 'Preface', chapter: '1', page: 1, indent: 0},
    {name: 'Java SE5 and SE6', chapter: '1.1', page: 2, indent: 1},
    {name: 'Java SE6', chapter: '1.1.1', page: 2, indent: 2},
    {name: 'The 4th edition', chapter: '1.2', page: 2, indent: 1},
    {name: 'Changes', chapter: '1.2.1', page: 3, indent: 2},
    {name: 'Note on the cover design', chapter: '1.3', page: 4, indent: 1},
    {name: 'Acknowledgements', chapter: '1.4', page: 4, indent: 1},
    {name: 'Introduction', chapter: '2', page: 9, indent: 0},
    {name: 'Prerequisites', chapter: '2.1', page: 9, indent: 1},
    {name: 'Learning Java', chapter: '2.2', page: 10, indent: 1},
    {name: 'Goals', chapter: '2.3', page: 10, indent: 1},
    {name: 'Teaching from this book', chapter: '2.4', page: 11, indent: 1},
    {name: 'JDK HTML documentation', chapter: '2.5', page: 11, indent: 1},
];
for (var r = 0; r < commands.length; r++) {
    activeSheet.setValue(r, 0, commands[r]['name']);
    activeSheet.setValue(r, 1, commands[r]['chapter']);
    activeSheet.setValue(r, 2, commands[r]['page']);
    activeSheet.getRange(r, 0, 1, 1).textIndent(commands[r].indent);
}
activeSheet.outlineColumn.options({
     columnIndex: 0,
     showImage: true,
     showCheckBox: true,
     images: ['star2.png', 'box4.png', 'rating4.png'],
     maxLevel: 2
});
activeSheet.showRowOutline(true);
spread.invalidateLayout();
spread.resumePaint();

console.log(activeSheet.outlineColumn.getCollapsed(1)); // false
activeSheet.outlineColumn.setCollapsed(1, true);
console.log(activeSheet.outlineColumn.getCollapsed(1)); // true
console.log(activeSheet.outlineColumn.getCollapsed(2)); // false -> sub node of row 1
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行的索引。 |
| `collapsed` | `boolean` | 行的折叠设置。 |

#### Returns

`void`
