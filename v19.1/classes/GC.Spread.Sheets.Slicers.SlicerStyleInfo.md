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
- [fontFamily](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md#fontfamily)
- [fontSize](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md#fontsize)
- [fontStyle](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md#fontstyle)
- [fontWeight](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md#fontweight)
- [foreColor](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md#forecolor)
- [setBorders](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md#setborders)
- [textDecoration](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md#textdecoration)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new SlicerStyleInfo**(`backColor?`, `foreColor?`, `font?`, `borderLeft?`, `borderTop?`, `borderRight?`, `borderBottom?`, `textDecoration?`, `fontStyle?`, `fontWeight?`, `fontSize?`, `fontFamily?`)

表示切片器样式信息。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `backColor?` | `string` | 样式信息背景颜色。 |
| `foreColor?` | `string` | 样式信息前景颜色。 |
| `font?` | `string` | 样式信息字体。 |
| `borderLeft?` | [`SlicerBorder`](GC.Spread.Sheets.Slicers.SlicerBorder.md) | 样式信息左边框。 |
| `borderTop?` | [`SlicerBorder`](GC.Spread.Sheets.Slicers.SlicerBorder.md) | 样式信息上边框。 |
| `borderRight?` | [`SlicerBorder`](GC.Spread.Sheets.Slicers.SlicerBorder.md) | 样式信息右边框。 |
| `borderBottom?` | [`SlicerBorder`](GC.Spread.Sheets.Slicers.SlicerBorder.md) | 样式信息下边框。 |
| `textDecoration?` | [`TextDecorationType`](../enums/GC.Spread.Sheets.TextDecorationType.md) | 样式信息文本装饰。 |
| `fontStyle?` | `string` | 样式信息字体样式。 |
| `fontWeight?` | `string` | 样式信息字体粗细。 |
| `fontSize?` | `string` | 样式信息字体大小。 |
| `fontFamily?` | `string` | 样式信息字体家族。 |

## Methods

### <a id="backcolor" name="backcolor"></a> backColor

▸ **backColor**(`value?`): `any`

获取或设置样式信息背景颜色。

**`example`**
```javascript
// 这个例子设置表头背景颜色。
// 创建一个表
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
// 样式
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.backColor("red");
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.headerStyle(hstyle);
// 添加一个切片器到工作表并返回切片器实例。
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
// 更改切片器属性。
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 样式信息背景颜色。 |

#### Returns

`any`

如果未设置值，返回样式信息背景颜色；否则返回切片器样式信息。

___

### <a id="borderbottom" name="borderbottom"></a> borderBottom

▸ **borderBottom**(`value?`): `any`

获取或设置样式信息下边框。

**`example`**
```javascript
// 这个例子设置一个边框样式。
// 创建一个表
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
// 样式
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.backColor("red");
hstyle.borderBottom(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green"));
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredSelectedItemWithDataStyle(hstyle);
// 添加一个切片器到工作表并返回切片器实例。
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
// 更改切片器属性。
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SlicerBorder`](GC.Spread.Sheets.Slicers.SlicerBorder.md) | 样式信息下边框。 |

#### Returns

`any`

如果未设置值，返回样式信息下边框；否则返回切片器样式信息。

___

### <a id="borderleft" name="borderleft"></a> borderLeft

▸ **borderLeft**(`value?`): `any`

获取或设置样式信息左边框。

**`example`**
```javascript
// 这个例子设置左边框。
// 创建一个表
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
// 样式
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.backColor("red");
hstyle.borderLeft(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green"));
hstyle.borderRight(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green"));
var hstyle1 = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle1.borderTop(new GC.Spread.Sheets.Slicers.SlicerBorder(2, "dashed", "blue"));
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredSelectedItemWithDataStyle(hstyle);
style1.unSelectedItemWithDataStyle(hstyle1);
// 添加一个切片器到工作表并返回切片器实例。
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
// 更改切片器属性。
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SlicerBorder`](GC.Spread.Sheets.Slicers.SlicerBorder.md) | 样式信息左边框。 |

#### Returns

`any`

如果未设置值，返回样式信息左边框；否则返回切片器样式信息。

___

### <a id="borderright" name="borderright"></a> borderRight

▸ **borderRight**(`value?`): `any`

获取或设置样式信息右边框。

**`example`**
```javascript
// 这个例子设置右边框。
// 创建一个表
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
// 样式
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.backColor("red");
hstyle.borderLeft(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green"));
hstyle.borderRight(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green"));
var hstyle1 = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle1.borderTop(new GC.Spread.Sheets.Slicers.SlicerBorder(2, "dashed", "blue"));
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredSelectedItemWithDataStyle(hstyle);
style1.unSelectedItemWithDataStyle(hstyle1);
// 添加一个切片器到工作表并返回切片器实例。
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
// 更改切片器属性。
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SlicerBorder`](GC.Spread.Sheets.Slicers.SlicerBorder.md) | 样式信息右边框。 |

#### Returns

`any`

如果未设置值，返回样式信息右边框；否则返回切片器样式信息。

___

### <a id="bordertop" name="bordertop"></a> borderTop

▸ **borderTop**(`value?`): `any`

获取或设置样式信息上边框。

**`example`**
```javascript
// 这个例子设置边框。
// 创建一个表
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
// 样式
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.backColor("red");
hstyle.borderLeft(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green"));
hstyle.borderRight(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green"));
var hstyle1 = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle1.borderTop(new GC.Spread.Sheets.Slicers.SlicerBorder(2, "dashed", "blue"));
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredSelectedItemWithDataStyle(hstyle);
style1.unSelectedItemWithDataStyle(hstyle1);
// 添加一个切片器到工作表并返回切片器实例。
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
// 更改切片器属性。
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SlicerBorder`](GC.Spread.Sheets.Slicers.SlicerBorder.md) | 样式信息上边框。 |

#### Returns

`any`

如果未设置值，返回样式信息上边框；否则返回切片器样式信息。

___

### <a id="font" name="font"></a> font

▸ **font**(`value?`): `any`

获取或设置样式信息字体。

**`example`**
```javascript
// 这个例子设置字体。
// 创建一个表
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
// 样式
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
// 添加一个切片器到工作表并返回切片器实例。
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
// 更改切片器属性。
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 样式信息字体。 |

#### Returns

`any`

如果未设置值，返回样式信息字体；否则返回切片器样式信息。

___

### <a id="fontfamily" name="fontfamily"></a> fontFamily

▸ **fontFamily**(`value?`): `any`

获取或设置样式信息字体家族。

**`example`**
```javascript
// 这个例子设置字体。
// 创建一个表
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
// 样式
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.fontFamily("Arial Black");
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredSelectedItemWithDataStyle(hstyle);
// 添加一个切片器到工作表并返回切片器实例。
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
// 更改切片器属性。
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 样式信息字体家族。 |

#### Returns

`any`

如果未设置值，返回样式信息字体家族；否则返回切片器样式信息。

___

### <a id="fontsize" name="fontsize"></a> fontSize

▸ **fontSize**(`value?`): `any`

获取或设置字体大小。

**`example`**
```javascript
//这个例子设置字体大小。
// 创建一个表
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
// 样式
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.fontSize("18pt");
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredSelectedItemWithDataStyle(hstyle);
// 添加一个切片器到工作表并返回切片器实例。
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
// 更改切片器属性。
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 样式信息的字体大小。 |

#### Returns

`any`

如果未设置值，返回样式信息的字体大小；否则返回切片器样式信息。

___

### <a id="fontstyle" name="fontstyle"></a> fontStyle

▸ **fontStyle**(`value?`): `any`

获取或设置字体样式。

**`example`**
```javascript
//这个例子设置字体样式。
// 创建一个表
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
// 样式
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.fontStyle("italic");
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredSelectedItemWithDataStyle(hstyle);
// 添加一个切片器到工作表并返回切片器实例。
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
// 更改切片器属性。
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 样式信息的字体样式。 |

#### Returns

`any`

如果未设置值，返回样式信息的字体样式；否则返回切片器样式信息。

___

### <a id="fontweight" name="fontweight"></a> fontWeight

▸ **fontWeight**(`value?`): `any`

获取或设置字体粗细。

**`example`**
```javascript
//这个例子设置字体粗细。
// 创建一个表
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
// 样式
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.fontWeight("bold");
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredSelectedItemWithDataStyle(hstyle);
// 添加一个切片器到工作表并返回切片器实例。
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
// 更改切片器属性。
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 样式信息的字体粗细。 |

#### Returns

`any`

如果未设置值，返回样式信息的字体粗细；否则返回切片器样式信息。

___

### <a id="forecolor" name="forecolor"></a> foreColor

▸ **foreColor**(`value?`): `any`

获取或设置样式信息的前景色。

**`example`**
```javascript
//这个例子设置切片器的标题样式。
// 创建一个表
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
// 样式
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.foreColor("white");
hstyle.backColor("black");
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.headerStyle(hstyle);
// 添加一个切片器到工作表并返回切片器实例。
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
// 更改切片器属性。
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 样式信息的前景色。 |

#### Returns

`any`

如果未设置值，返回样式信息的前景色；否则返回切片器样式信息。

___

### <a id="setborders" name="setborders"></a> setBorders

▸ **setBorders**(`value`): `void`

设置样式信息的所有边框。

**`example`**
```javascript
//此示例设置切片器的边框。
//创建一个表格
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
// 样式
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.setBorders(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green"));
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.selectedItemWithDataStyle(hstyle);
// 在工作表中添加一个切片器并返回该切片器实例。
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
slicer.style(style1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | [`SlicerBorder`](GC.Spread.Sheets.Slicers.SlicerBorder.md) | 边框设置。 |

#### Returns

`void`

___

### <a id="textdecoration" name="textdecoration"></a> textDecoration

▸ **textDecoration**(`value?`): `any`

获取或设置样式信息的文本装饰。

**`example`**
```javascript
//这个例子为文本添加下划线。
// 创建一个表
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
// 样式
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
// 添加一个切片器到工作表并返回切片器实例。
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
// 更改切片器属性。
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`TextDecorationType`](../enums/GC.Spread.Sheets.TextDecorationType.md) | 样式信息的文本装饰。 |

#### Returns

`any`

如果未设置值，返回样式信息的文本装饰；否则返回切片器样式信息。
