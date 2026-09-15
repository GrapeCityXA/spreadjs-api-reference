# Class: SlicerStyleInfo

[Sheets](../modules/GC.Spread.Sheets.md).[Slicers](../modules/GC.Spread.Sheets.Slicers.md).SlicerStyleInfo

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md#constructor)

### Methods

- [backColor](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md#backcolor)
- [borderBottom](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md#borderbottom)
- [borderLeft](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md#borderleft)
- [borderRight](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md#borderright)
- [borderTop](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md#bordertop)
- [font](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md#font)
- [foreColor](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md#forecolor)
- [setBorders](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md#setborders)
- [textDecoration](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md#textdecoration)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new SlicerStyleInfo**(`backColor?`, `foreColor?`, `font?`, `borderLeft?`, `borderTop?`, `borderRight?`, `borderBottom?`, `textDecoration?`)

切片器样式信息

#### Parameters

| Name | Type |
| :------ | :------ |
| `backColor?` | `string` |
| `foreColor?` | `string` |
| `font?` | `string` |
| `borderLeft?` | [`SlicerBorder`](GC.Spread.Sheets.Slicers.SlicerBorder.md) |
| `borderTop?` | [`SlicerBorder`](GC.Spread.Sheets.Slicers.SlicerBorder.md) |
| `borderRight?` | [`SlicerBorder`](GC.Spread.Sheets.Slicers.SlicerBorder.md) |
| `borderBottom?` | [`SlicerBorder`](GC.Spread.Sheets.Slicers.SlicerBorder.md) |
| `textDecoration?` | [`TextDecorationType`](../enums/GC.Spread.Sheets.TextDecorationType.md) |

## Methods

### <a id="backcolor" name="backcolor"></a> backColor

▸ **backColor**(`value?`): `any`

获取或设置样式信息的背景色

**`代码示例`**
``` javascript
//本示例设置标题背景色
//创建一个表
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
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
//style
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.backColor("red");
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.headerStyle(hstyle);
//向工作表添加一个切片器并返回切片器实例
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
 //改变切片器的属性
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置任何值，则返回样式信息的背景色；否则，返回切片器样式信息

___

### <a id="borderbottom" name="borderbottom"></a> borderBottom

▸ **borderBottom**(`value?`): `any`

获取或设置样式信息的下边框

**`代码示例`**
``` javascript
//本示例设置边框样式
//创建一个表
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
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
//style
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.backColor("red");
hstyle.borderBottom(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green"));
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredSelectedItemWithDataStyle(hstyle);
//向工作表添加一个切片器并返回切片器实例
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
//改变切片器的属性
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SlicerBorder`](GC.Spread.Sheets.Slicers.SlicerBorder.md) |

#### Returns

`any`

如果未设置任何值，则返回样式信息的下边框；否则，返回切片器样式信息

___

### <a id="borderleft" name="borderleft"></a> borderLeft

▸ **borderLeft**(`value?`): `any`

获取或设置样式信息的左边框

**`代码示例`**
``` javascript
//本示例设置左边框
//创建一个表
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
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
//style
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.backColor("red");
hstyle.borderLeft(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green"));
hstyle.borderRight(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green"));
var hstyle1 = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle1.borderTop(new GC.Spread.Sheets.Slicers.SlicerBorder(2, "dashed", "blue"));
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredSelectedItemWithDataStyle(hstyle);
style1.unSelectedItemWithDataStyle(hstyle1);
//向工作表添加一个切片器并返回切片器实例
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
 //改变切片器的属性
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SlicerBorder`](GC.Spread.Sheets.Slicers.SlicerBorder.md) |

#### Returns

`any`

如果未设置任何值，则返回样式信息的左边框；否则，返回切片器样式信息

___

### <a id="borderright" name="borderright"></a> borderRight

▸ **borderRight**(`value?`): `any`

获取或设置样式信息的右边框

**`代码示例`**
``` javascript
//本示例设置边框
//创建一个表
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
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
//style
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.backColor("red");
hstyle.borderLeft(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green"));
hstyle.borderRight(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green"));
var hstyle1 = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle1.borderTop(new GC.Spread.Sheets.Slicers.SlicerBorder(2, "dashed", "blue"));
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredSelectedItemWithDataStyle(hstyle);
style1.unSelectedItemWithDataStyle(hstyle1);
//向工作表添加一个切片器并返回切片器实例
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
 //改变切片器的属性
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SlicerBorder`](GC.Spread.Sheets.Slicers.SlicerBorder.md) |

#### Returns

`any`

如果未设置任何值，则返回样式信息的右边框；否则，返回切片器样式信息

___

### <a id="bordertop" name="bordertop"></a> borderTop

▸ **borderTop**(`value?`): `any`

获取或设置样式信息的上边框

**`代码示例`**
``` javascript
//本示例设置边框
//创建一个表
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
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
//style
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.backColor("red");
hstyle.borderLeft(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green"));
hstyle.borderRight(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green"));
var hstyle1 = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle1.borderTop(new GC.Spread.Sheets.Slicers.SlicerBorder(2, "dashed", "blue"));
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredSelectedItemWithDataStyle(hstyle);
style1.unSelectedItemWithDataStyle(hstyle1);
//向工作表添加一个切片器并返回切片器实例
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
 //改变切片器的属性
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SlicerBorder`](GC.Spread.Sheets.Slicers.SlicerBorder.md) |

#### Returns

`any`

如果未设置任何值，则返回样式信息的上边框；否则，返回切片器样式信息

___

### <a id="font" name="font"></a> font

▸ **font**(`value?`): `any`

获取或设置样式信息的字体

**`代码示例`**
``` javascript
//本示例设置字体
//创建一个表
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
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
//style
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.backColor("red");
hstyle.borderBottom(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green"));
hstyle.font("8pt Arial");
hstyle.textDecoration(GC.Spread.Sheets.TextDecorationType.underline);
var hstyle1 = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle1.borderTop(new GC.Spread.Sheets.Slicers.SlicerBorder(2, "dashed", "blue"));
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredSelectedItemWithDataStyle(hstyle);
style1.unSelectedItemWithDataStyle(hstyle1);
//向工作表添加一个切片器并返回切片器实例
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
 //改变切片器的属性
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置任何值，则返回样式信息的字体；否则，返回切片器样式信息

___

### <a id="forecolor" name="forecolor"></a> foreColor

▸ **foreColor**(`value?`): `any`

获取或设置样式信息的前景色

**`代码示例`**
``` javascript
//本示例为切片器设置头部样式
//创建一个表
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
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
//style
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.foreColor("white");
hstyle.backColor("black");
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.headerStyle(hstyle);
//向工作表添加一个切片器并返回切片器实例
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
 //改变切片器的属性
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置任何值，则返回样式信息的前景色；否则，返回切片器样式信息

___

### <a id="setborders" name="setborders"></a> setBorders

▸ **setBorders**(`value`): `void`

设置样式信息的每个边框

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | [`SlicerBorder`](GC.Spread.Sheets.Slicers.SlicerBorder.md) | 边框设置 |

#### Returns

`void`

___

### <a id="textdecoration" name="textdecoration"></a> textDecoration

▸ **textDecoration**(`value?`): `any`

获取或设置样式信息的文本修饰

**`代码示例`**
``` javascript
//本示例在文本下划线
//创建一个表
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
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
//style
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.backColor("red");
hstyle.borderBottom(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green"));
hstyle.font("8pt Arial");
hstyle.textDecoration(GC.Spread.Sheets.TextDecorationType.underline);
var hstyle1 = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle1.borderTop(new GC.Spread.Sheets.Slicers.SlicerBorder(2, "dashed", "blue"));
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredSelectedItemWithDataStyle(hstyle);
style1.unSelectedItemWithDataStyle(hstyle1);
//向工作表添加一个切片器并返回切片器实例
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
//改变切片器的属性
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`TextDecorationType`](../enums/GC.Spread.Sheets.TextDecorationType.md) |

#### Returns

`any`

如果未设置任何值，则返回样式信息的文本修饰；否则，返回切片器样式信息
