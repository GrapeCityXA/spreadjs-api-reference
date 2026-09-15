# Class: SlicerStyle

[Sheets](../modules/GC.Spread.Sheets.md).[Slicers](../modules/GC.Spread.Sheets.Slicers.md).SlicerStyle

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Slicers.SlicerStyle.md#constructor)

### Methods

- [fromJSON](GC.Spread.Sheets.Slicers.SlicerStyle.md#fromjson)
- [headerStyle](GC.Spread.Sheets.Slicers.SlicerStyle.md#headerstyle)
- [hoveredSelectedItemWithDataStyle](GC.Spread.Sheets.Slicers.SlicerStyle.md#hoveredselecteditemwithdatastyle)
- [hoveredSelectedItemWithNoDataStyle](GC.Spread.Sheets.Slicers.SlicerStyle.md#hoveredselecteditemwithnodatastyle)
- [hoveredUnSelectedItemWithDataStyle](GC.Spread.Sheets.Slicers.SlicerStyle.md#hoveredunselecteditemwithdatastyle)
- [hoveredUnSelectedItemWithNoDataStyle](GC.Spread.Sheets.Slicers.SlicerStyle.md#hoveredunselecteditemwithnodatastyle)
- [name](GC.Spread.Sheets.Slicers.SlicerStyle.md#name)
- [selectedItemWithDataStyle](GC.Spread.Sheets.Slicers.SlicerStyle.md#selecteditemwithdatastyle)
- [selectedItemWithNoDataStyle](GC.Spread.Sheets.Slicers.SlicerStyle.md#selecteditemwithnodatastyle)
- [toJSON](GC.Spread.Sheets.Slicers.SlicerStyle.md#tojson)
- [unSelectedItemWithDataStyle](GC.Spread.Sheets.Slicers.SlicerStyle.md#unselecteditemwithdatastyle)
- [unSelectedItemWithNoDataStyle](GC.Spread.Sheets.Slicers.SlicerStyle.md#unselecteditemwithnodatastyle)
- [wholeSlicerStyle](GC.Spread.Sheets.Slicers.SlicerStyle.md#wholeslicerstyle)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new SlicerStyle**()

代表切片器样式设置。

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datas = [
    ["1", "NewYork", "1968/6/8"],
    ["4", "NewYork", "1972/7/3"],
    ["4", "NewYork", "1964/3/2"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
var dataColumns = ["Name", "City", "Birthday"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");

//set customized style
var style = new GC.Spread.Sheets.Slicers.SlicerStyle();
var styleInfo1 = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
styleInfo1.backColor("orange");
styleInfo1.borderBottom(new GC.Spread.Sheets.Slicers.SlicerBorder(2,"solid","green"));
style.wholeSlicerStyle(styleInfo1);
var styleInfo2 = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
styleInfo2.backColor("red");
styleInfo2.borderBottom(new GC.Spread.Sheets.Slicers.SlicerBorder(4,"solid","gray"));
style.hoveredSelectedItemWithDataStyle(styleInfo2);
slicer.style(style);
```

## Methods

### <a id="fromjson" name="fromjson"></a> fromJSON

▸ **fromJSON**(`data`): `void`

从指定的 JSON 字符串加载对象状态。

**`example`**
```
//This example uses the fromJSON method.
const light1 = GC.Spread.Sheets.Slicers.SlicerStyles.light1();
//export
const jsonStr = JSON.stringify(light1.toJSON());
//import
const newTheme = new GC.Spread.Sheets.Slicers.SlicerStyle();
newTheme.fromJSON(JSON.parse(jsonStr));
newTheme.name('custom1');
alert(jsonStr);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `Object` | 来自反序列化的项目切片器主题数据。 |

#### Returns

`void`

___

### <a id="headerstyle" name="headerstyle"></a> headerStyle

▸ **headerStyle**(`value?`): `any`

获取或设置切片器头部的样式

**`代码示例`**
``` javascript
//本示例设置标题背景色
//create a table
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
//切片器信息
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
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) |

#### Returns

`any`

如果未设置任何值，则返回切片器头部的样式；否则，返回切片器样式

___

### <a id="hoveredselecteditemwithdatastyle" name="hoveredselecteditemwithdatastyle"></a> hoveredSelectedItemWithDataStyle

▸ **hoveredSelectedItemWithDataStyle**(`value?`): `any`

获取或设置切片器的带有数据的悬停所选项目的样式.

**`代码示例`**
``` javascript
//This example sets the hoveredSelectedItemWithDataStyle method.
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
// 切片器信息
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
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) |

#### Returns

`any`

如果没有设置值，则返回带有数据的悬停所选项目的样式；否则，返回切片器样式.

___

### <a id="hoveredselecteditemwithnodatastyle" name="hoveredselecteditemwithnodatastyle"></a> hoveredSelectedItemWithNoDataStyle

▸ **hoveredSelectedItemWithNoDataStyle**(`value?`): `any`

获取或设置没有数据的悬停所选项的样式

**`代码示例`**
``` javascript
//This example uses the hoveredSelectedItemWithNoDataStyle method.
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datasource = [
    { Name: "Apple", Category: "Fruit" },
    { Name: "Orange", Category: "Fruit" },
    { Name: "Broccoli", Category: "Vegetable" },
    { Name: "Kiwi", Category: "Fruit" },
    { Name: "Rice", Category: "Cereal" },
    { Name: "Strawberry", Category: "Fruit" },
    { Name: "Yogurt", Category: "Dairy" },
    { Name: "Plum", Category: "Fruit" },
    { Name: "Celery", Category: "Vegetable" },
    { Name: "Grape", Category: "Fruit" },
    { Name: "Oats", Category: "Cereal" },
    { Name: "Quinoa", Category: "Cereal" },
    { Name: "Maize", Category: "Cereal" },
    { Name: "Okra", Category: "Vegetable" },
    { Name: "Corn", Category: "Vegetable" },
    { Name: "Wheat", Category: "Cereal" },
    { Name: "Barley", Category: "Cereal" },
    { Name: "Cream", Category: "Dairy" },
    { Name: "Millet", Category: "Cereal" },
    { Name: "Rye", Category: "Cereal" },
    { Name: "Artichoke", Category: "Vegetable" },
    { Name: "Buckwheat", Category: "Cereal" },
    { Name: "Gooseberry", Category: "Fruit" },
    { Name: "Amaranth", Category: "Cereal" },
    { Name: "Carrot", Category: "Vegetable" },
    { Name: "Cheese", Category: "Dairy" },
    { Name: "Fig", Category: "Fruit" },
    { Name: "Milk", Category: "Dairy" },
    { Name: "Butter", Category: "Dairy" },
               ];
//add table
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, datasource);
//向工作表添加一个切片器并返回切片器实例
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Category");
 //改变切片器的属性
slicer.width(200);
slicer.height(200);
slicer.position(new GC.Spread.Sheets.Point(300, 50));
var slicer2 = activeSheet.slicers.add("slicer2", table.name(), "Name");
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.backColor("red");
hstyle.borderBottom(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green"));
var hstyle1 = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle1.borderTop(new GC.Spread.Sheets.Slicers.SlicerBorder(2, "dashed", "blue"));
hstyle1.backColor("yellow");
var hstyle2 = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle2.backColor("green");
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredSelectedItemWithDataStyle(hstyle);
style1.hoveredUnSelectedItemWithDataStyle(hstyle);
style1.unSelectedItemWithDataStyle(hstyle1);
style1.selectedItemWithDataStyle(hstyle2);
slicer.style(style1);
// 切片器样式
var hstyle2nd = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle2nd.backColor("red");
hstyle2nd.borderBottom(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "double", "orange"));
var hstyle12nd = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle12nd.borderTop(new GC.Spread.Sheets.Slicers.SlicerBorder(2, "double", "blue"));
hstyle12nd.backColor("yellow");
var hstyle22nd = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle22nd.backColor("magenta");
var style1two = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1two.hoveredSelectedItemWithNoDataStyle(hstyle2nd);
style1two.hoveredUnSelectedItemWithNoDataStyle(hstyle2nd);
style1two.unSelectedItemWithNoDataStyle(hstyle12nd);
style1two.selectedItemWithNoDataStyle(hstyle22nd);
slicer2.style(style1two);
activeSheet.setColumnWidth(1, 100);
activeSheet.setColumnWidth(2, 100);
activeSheet.setColumnWidth(3, 100);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) |

#### Returns

`any`

如果未设置任何值，则返回没有数据的悬停所选项的样式；否则，返回切片器样式

___

### <a id="hoveredunselecteditemwithdatastyle" name="hoveredunselecteditemwithdatastyle"></a> hoveredUnSelectedItemWithDataStyle

▸ **hoveredUnSelectedItemWithDataStyle**(`value?`): `any`

获取或设置切片器的style of the hovered unselected item with data.

**`代码示例`**
``` javascript
//This example uses the hoveredUnSelectedItemWithDataStyle method.
//create a table
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
// 切片器样式
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.backColor("red");
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredUnSelectedItemWithDataStyle(hstyle);
//向工作表添加一个切片器并返回切片器实例
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
 //改变切片器的属性
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) |

#### Returns

`any`

如果没有设置值，则返回悬停未选中的带有数据的项目的样式；否则，返回切片器样式.

___

### <a id="hoveredunselecteditemwithnodatastyle" name="hoveredunselecteditemwithnodatastyle"></a> hoveredUnSelectedItemWithNoDataStyle

▸ **hoveredUnSelectedItemWithNoDataStyle**(`value?`): `any`

获取或设置没有数据的悬停未选择项的样式

**`代码示例`**
``` javascript
//This example uses the hoveredUnSelectedItemWithNoDataStyle method.
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datasource = [
    { Name: "Apple", Category: "Fruit" },
    { Name: "Orange", Category: "Fruit" },
    { Name: "Broccoli", Category: "Vegetable" },
    { Name: "Kiwi", Category: "Fruit" },
    { Name: "Rice", Category: "Cereal" },
    { Name: "Strawberry", Category: "Fruit" },
    { Name: "Yogurt", Category: "Dairy" },
    { Name: "Plum", Category: "Fruit" },
    { Name: "Celery", Category: "Vegetable" },
    { Name: "Grape", Category: "Fruit" },
    { Name: "Oats", Category: "Cereal" },
    { Name: "Quinoa", Category: "Cereal" },
    { Name: "Maize", Category: "Cereal" },
    { Name: "Okra", Category: "Vegetable" },
    { Name: "Corn", Category: "Vegetable" },
    { Name: "Wheat", Category: "Cereal" },
    { Name: "Barley", Category: "Cereal" },
    { Name: "Cream", Category: "Dairy" },
    { Name: "Millet", Category: "Cereal" },
    { Name: "Rye", Category: "Cereal" },
    { Name: "Artichoke", Category: "Vegetable" },
    { Name: "Buckwheat", Category: "Cereal" },
    { Name: "Gooseberry", Category: "Fruit" },
    { Name: "Amaranth", Category: "Cereal" },
    { Name: "Carrot", Category: "Vegetable" },
    { Name: "Cheese", Category: "Dairy" },
    { Name: "Fig", Category: "Fruit" },
    { Name: "Milk", Category: "Dairy" },
    { Name: "Butter", Category: "Dairy" },
              ];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, datasource);
//向工作表添加一个切片器并返回切片器实例
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Category");
 //改变切片器的属性
slicer.width(200);
slicer.height(200);
slicer.position(new GC.Spread.Sheets.Point(300, 50));
var slicer2 = activeSheet.slicers.add("slicer2", table.name(), "Name");
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.backColor("red");
hstyle.borderBottom(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green"));
var hstyle1 = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle1.borderTop(new GC.Spread.Sheets.Slicers.SlicerBorder(2, "dashed", "blue"));
hstyle1.backColor("yellow");
var hstyle2 = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle2.backColor("green");
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredSelectedItemWithDataStyle(hstyle);
style1.hoveredUnSelectedItemWithDataStyle(hstyle);
style1.unSelectedItemWithDataStyle(hstyle1);
style1.selectedItemWithDataStyle(hstyle2);
slicer.style(style1);
var hstyle2nd = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle2nd.backColor("red");
hstyle2nd.borderBottom(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "double", "orange"));
var hstyle12nd = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle12nd.borderTop(new GC.Spread.Sheets.Slicers.SlicerBorder(2, "double", "blue"));
hstyle12nd.backColor("yellow");
var hstyle22nd = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle22nd.backColor("magenta");
var style1two = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1two.hoveredSelectedItemWithNoDataStyle(hstyle2nd);
style1two.hoveredUnSelectedItemWithNoDataStyle(hstyle2nd);
style1two.unSelectedItemWithNoDataStyle(hstyle12nd);
style1two.selectedItemWithNoDataStyle(hstyle22nd);
slicer2.style(style1two);
activeSheet.setColumnWidth(1, 100);
activeSheet.setColumnWidth(2, 100);
activeSheet.setColumnWidth(3, 100);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) |

#### Returns

`any`

如果未设置任何值，则返回没有数据的悬停的未选择项的样式；否则，返回切片器样式

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置样式的名称

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置任何值，则返回样式的名称；否则，返回切片器样式

___

### <a id="selecteditemwithdatastyle" name="selecteditemwithdatastyle"></a> selectedItemWithDataStyle

▸ **selectedItemWithDataStyle**(`value?`): `any`

获取或设置带有数据的所选项的样式

**`代码示例`**
``` javascript
//This example uses the hoveredUnSelectedItemWithNoDataStyle method.
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datasource = [
    { Name: "Apple", Category: "Fruit" },
    { Name: "Orange", Category: "Fruit" },
    { Name: "Broccoli", Category: "Vegetable" },
    { Name: "Kiwi", Category: "Fruit" },
    { Name: "Rice", Category: "Cereal" },
    { Name: "Strawberry", Category: "Fruit" },
    { Name: "Yogurt", Category: "Dairy" },
    { Name: "Plum", Category: "Fruit" },
    { Name: "Celery", Category: "Vegetable" },
    { Name: "Grape", Category: "Fruit" },
    { Name: "Oats", Category: "Cereal" },
    { Name: "Quinoa", Category: "Cereal" },
    { Name: "Maize", Category: "Cereal" },
    { Name: "Okra", Category: "Vegetable" },
    { Name: "Corn", Category: "Vegetable" },
    { Name: "Wheat", Category: "Cereal" },
    { Name: "Barley", Category: "Cereal" },
    { Name: "Cream", Category: "Dairy" },
    { Name: "Millet", Category: "Cereal" },
    { Name: "Rye", Category: "Cereal" },
    { Name: "Artichoke", Category: "Vegetable" },
    { Name: "Buckwheat", Category: "Cereal" },
    { Name: "Gooseberry", Category: "Fruit" },
    { Name: "Amaranth", Category: "Cereal" },
    { Name: "Carrot", Category: "Vegetable" },
    { Name: "Cheese", Category: "Dairy" },
    { Name: "Fig", Category: "Fruit" },
    { Name: "Milk", Category: "Dairy" },
    { Name: "Butter", Category: "Dairy" },
              ];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, datasource);
//向工作表添加一个切片器并返回切片器实例
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Category");
 //改变切片器的属性
slicer.width(200);
slicer.height(200);
slicer.position(new GC.Spread.Sheets.Point(300, 50));
var slicer2 = activeSheet.slicers.add("slicer2", table.name(), "Name");
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.backColor("red");
hstyle.borderBottom(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green"));
var hstyle1 = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle1.borderTop(new GC.Spread.Sheets.Slicers.SlicerBorder(2, "dashed", "blue"));
hstyle1.backColor("yellow");
var hstyle2 = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle2.backColor("green");
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredSelectedItemWithDataStyle(hstyle);
style1.hoveredUnSelectedItemWithDataStyle(hstyle);
style1.unSelectedItemWithDataStyle(hstyle1);
style1.selectedItemWithDataStyle(hstyle2);
slicer.style(style1);
var hstyle2nd = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle2nd.backColor("red");
hstyle2nd.borderBottom(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "double", "orange"));
var hstyle12nd = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle12nd.borderTop(new GC.Spread.Sheets.Slicers.SlicerBorder(2, "double", "blue"));
hstyle12nd.backColor("yellow");
var hstyle22nd = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle22nd.backColor("magenta");
var style1two = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1two.hoveredSelectedItemWithNoDataStyle(hstyle2nd);
style1two.hoveredUnSelectedItemWithNoDataStyle(hstyle2nd);
style1two.unSelectedItemWithNoDataStyle(hstyle12nd);
style1two.selectedItemWithNoDataStyle(hstyle22nd);
slicer2.style(style1two);
activeSheet.setColumnWidth(1, 100);
activeSheet.setColumnWidth(2, 100);
activeSheet.setColumnWidth(3, 100);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) |

#### Returns

`any`

如果未设置任何值，则返回带有数据的所选项的样式；否则，返回切片器样式

___

### <a id="selecteditemwithnodatastyle" name="selecteditemwithnodatastyle"></a> selectedItemWithNoDataStyle

▸ **selectedItemWithNoDataStyle**(`value?`): `any`

获取或设置没有数据的所选项的样式

**`代码示例`**
``` javascript
//本示例使用hoveredUnSelectedItemWithNoDataStyle方法
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datasource = [
    { Name: "Apple", Category: "Fruit" },
    { Name: "Orange", Category: "Fruit" },
    { Name: "Broccoli", Category: "Vegetable" },
    { Name: "Kiwi", Category: "Fruit" },
    { Name: "Rice", Category: "Cereal" },
    { Name: "Strawberry", Category: "Fruit" },
    { Name: "Yogurt", Category: "Dairy" },
    { Name: "Plum", Category: "Fruit" },
    { Name: "Celery", Category: "Vegetable" },
    { Name: "Grape", Category: "Fruit" },
    { Name: "Oats", Category: "Cereal" },
    { Name: "Quinoa", Category: "Cereal" },
    { Name: "Maize", Category: "Cereal" },
    { Name: "Okra", Category: "Vegetable" },
    { Name: "Corn", Category: "Vegetable" },
    { Name: "Wheat", Category: "Cereal" },
    { Name: "Barley", Category: "Cereal" },
    { Name: "Cream", Category: "Dairy" },
    { Name: "Millet", Category: "Cereal" },
    { Name: "Rye", Category: "Cereal" },
    { Name: "Artichoke", Category: "Vegetable" },
    { Name: "Buckwheat", Category: "Cereal" },
    { Name: "Gooseberry", Category: "Fruit" },
    { Name: "Amaranth", Category: "Cereal" },
    { Name: "Carrot", Category: "Vegetable" },
    { Name: "Cheese", Category: "Dairy" },
    { Name: "Fig", Category: "Fruit" },
    { Name: "Milk", Category: "Dairy" },
    { Name: "Butter", Category: "Dairy" },
              ];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, datasource);
//向工作表添加一个切片器并返回切片器实例
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Category");
 //改变切片器的属性
slicer.width(200);
slicer.height(200);
slicer.position(new GC.Spread.Sheets.Point(300, 50));
var slicer2 = activeSheet.slicers.add("slicer2", table.name(), "Name");
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.backColor("red");
hstyle.borderBottom(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green"));
var hstyle1 = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle1.borderTop(new GC.Spread.Sheets.Slicers.SlicerBorder(2, "dashed", "blue"));
hstyle1.backColor("yellow");
var hstyle2 = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle2.backColor("green");
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredSelectedItemWithDataStyle(hstyle);
style1.hoveredUnSelectedItemWithDataStyle(hstyle);
style1.unSelectedItemWithDataStyle(hstyle1);
style1.selectedItemWithDataStyle(hstyle2);
slicer.style(style1);
var hstyle2nd = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle2nd.backColor("red");
hstyle2nd.borderBottom(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "double", "orange"));
var hstyle12nd = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle12nd.borderTop(new GC.Spread.Sheets.Slicers.SlicerBorder(2, "double", "blue"));
hstyle12nd.backColor("yellow");
var hstyle22nd = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle22nd.backColor("magenta");
var style1two = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1two.hoveredSelectedItemWithNoDataStyle(hstyle2nd);
style1two.hoveredUnSelectedItemWithNoDataStyle(hstyle2nd);
style1two.unSelectedItemWithNoDataStyle(hstyle12nd);
style1two.selectedItemWithNoDataStyle(hstyle22nd);
slicer2.style(style1two);
activeSheet.setColumnWidth(1, 100);
activeSheet.setColumnWidth(2, 100);
activeSheet.setColumnWidth(3, 100);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) |

#### Returns

`any`

如果未设置任何值，则返回没有数据的所选项的样式；否则，返回切片器样式

### <a id="tojson" name="tojson"></a> toJSON

▸ **toJSON**(): `Object`

Saves the object state to a JSON string.

**`example`**
```
//This example uses the toJSON method.
const light1 = GC.Spread.Sheets.Slicers.SlicerStyles.light1();
//export
const jsonStr = JSON.stringify(light1.toJSON());
//import
const newTheme = new GC.Spread.Sheets.Slicers.SlicerStyle();
newTheme.fromJSON(JSON.parse(jsonStr));
newTheme.name('custom1');
alert(jsonStr);
```

#### Returns

`Object`

The item slicer theme data.

___

### <a id="unselecteditemwithdatastyle" name="unselecteditemwithdatastyle"></a> unSelectedItemWithDataStyle

▸ **unSelectedItemWithDataStyle**(`value?`): `any`

获取或设置带有数据的未选中项的样式

**`代码示例`**
``` javascript
//本示例使用hoveredUnSelectedItemWithNoDataStyle方法
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datasource = [
    { Name: "Apple", Category: "Fruit" },
    { Name: "Orange", Category: "Fruit" },
    { Name: "Broccoli", Category: "Vegetable" },
    { Name: "Kiwi", Category: "Fruit" },
    { Name: "Rice", Category: "Cereal" },
    { Name: "Strawberry", Category: "Fruit" },
    { Name: "Yogurt", Category: "Dairy" },
    { Name: "Plum", Category: "Fruit" },
    { Name: "Celery", Category: "Vegetable" },
    { Name: "Grape", Category: "Fruit" },
    { Name: "Oats", Category: "Cereal" },
    { Name: "Quinoa", Category: "Cereal" },
    { Name: "Maize", Category: "Cereal" },
    { Name: "Okra", Category: "Vegetable" },
    { Name: "Corn", Category: "Vegetable" },
    { Name: "Wheat", Category: "Cereal" },
    { Name: "Barley", Category: "Cereal" },
    { Name: "Cream", Category: "Dairy" },
    { Name: "Millet", Category: "Cereal" },
    { Name: "Rye", Category: "Cereal" },
    { Name: "Artichoke", Category: "Vegetable" },
    { Name: "Buckwheat", Category: "Cereal" },
    { Name: "Gooseberry", Category: "Fruit" },
    { Name: "Amaranth", Category: "Cereal" },
    { Name: "Carrot", Category: "Vegetable" },
    { Name: "Cheese", Category: "Dairy" },
    { Name: "Fig", Category: "Fruit" },
    { Name: "Milk", Category: "Dairy" },
    { Name: "Butter", Category: "Dairy" },
              ];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, datasource);
//向工作表添加一个切片器并返回切片器实例
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Category");
 //改变切片器的属性
slicer.width(200);
slicer.height(200);
slicer.position(new GC.Spread.Sheets.Point(300, 50));
var slicer2 = activeSheet.slicers.add("slicer2", table.name(), "Name");
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.backColor("red");
hstyle.borderBottom(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green"));
var hstyle1 = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle1.borderTop(new GC.Spread.Sheets.Slicers.SlicerBorder(2, "dashed", "blue"));
hstyle1.backColor("yellow");
var hstyle2 = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle2.backColor("green");
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredSelectedItemWithDataStyle(hstyle);
style1.hoveredUnSelectedItemWithDataStyle(hstyle);
style1.unSelectedItemWithDataStyle(hstyle1);
style1.selectedItemWithDataStyle(hstyle2);
slicer.style(style1);
var hstyle2nd = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle2nd.backColor("red");
hstyle2nd.borderBottom(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "double", "orange"));
var hstyle12nd = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle12nd.borderTop(new GC.Spread.Sheets.Slicers.SlicerBorder(2, "double", "blue"));
hstyle12nd.backColor("yellow");
var hstyle22nd = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle22nd.backColor("magenta");
var style1two = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1two.hoveredSelectedItemWithNoDataStyle(hstyle2nd);
style1two.hoveredUnSelectedItemWithNoDataStyle(hstyle2nd);
style1two.unSelectedItemWithNoDataStyle(hstyle12nd);
style1two.selectedItemWithNoDataStyle(hstyle22nd);
slicer2.style(style1two);
activeSheet.setColumnWidth(1, 100);
activeSheet.setColumnWidth(2, 100);
activeSheet.setColumnWidth(3, 100);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) |

#### Returns

`any`

如果未设置任何值，则返回未选中项的样式以及数据；否则，返回切片器样式

___

### <a id="unselecteditemwithnodatastyle" name="unselecteditemwithnodatastyle"></a> unSelectedItemWithNoDataStyle

▸ **unSelectedItemWithNoDataStyle**(`value?`): `any`

获取或设置没有数据的未选择项的样式

**`代码示例`**
``` javascript
//本示例使用hoveredUnSelectedItemWithNoDataStyle方法
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 2 });
var activeSheet = spread.getActiveSheet();
var datasource = [
    { Name: "Apple", Category: "Fruit" },
    { Name: "Orange", Category: "Fruit" },
    { Name: "Broccoli", Category: "Vegetable" },
    { Name: "Kiwi", Category: "Fruit" },
    { Name: "Rice", Category: "Cereal" },
    { Name: "Strawberry", Category: "Fruit" },
    { Name: "Yogurt", Category: "Dairy" },
    { Name: "Plum", Category: "Fruit" },
    { Name: "Celery", Category: "Vegetable" },
    { Name: "Grape", Category: "Fruit" },
    { Name: "Oats", Category: "Cereal" },
    { Name: "Quinoa", Category: "Cereal" },
    { Name: "Maize", Category: "Cereal" },
    { Name: "Okra", Category: "Vegetable" },
    { Name: "Corn", Category: "Vegetable" },
    { Name: "Wheat", Category: "Cereal" },
    { Name: "Barley", Category: "Cereal" },
    { Name: "Cream", Category: "Dairy" },
    { Name: "Millet", Category: "Cereal" },
    { Name: "Rye", Category: "Cereal" },
    { Name: "Artichoke", Category: "Vegetable" },
    { Name: "Buckwheat", Category: "Cereal" },
    { Name: "Gooseberry", Category: "Fruit" },
    { Name: "Amaranth", Category: "Cereal" },
    { Name: "Carrot", Category: "Vegetable" },
    { Name: "Cheese", Category: "Dairy" },
    { Name: "Fig", Category: "Fruit" },
    { Name: "Milk", Category: "Dairy" },
    { Name: "Butter", Category: "Dairy" },
              ];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, datasource);
//向工作表添加一个切片器并返回切片器实例
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Category");
 //改变切片器的属性
slicer.width(200);
slicer.height(200);
slicer.position(new GC.Spread.Sheets.Point(300, 50));
var slicer2 = activeSheet.slicers.add("slicer2", table.name(), "Name");
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.backColor("red");
hstyle.borderBottom(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "dashed", "green"));
var hstyle1 = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle1.borderTop(new GC.Spread.Sheets.Slicers.SlicerBorder(2, "dashed", "blue"));
hstyle1.backColor("yellow");
var hstyle2 = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle2.backColor("green");
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredSelectedItemWithDataStyle(hstyle);
style1.hoveredUnSelectedItemWithDataStyle(hstyle);
style1.unSelectedItemWithDataStyle(hstyle1);
style1.selectedItemWithDataStyle(hstyle2);
slicer.style(style1);
var hstyle2nd = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle2nd.backColor("red");
hstyle2nd.borderBottom(new GC.Spread.Sheets.Slicers.SlicerBorder(3, "double", "orange"));
var hstyle12nd = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle12nd.borderTop(new GC.Spread.Sheets.Slicers.SlicerBorder(2, "double", "blue"));
hstyle12nd.backColor("yellow");
var hstyle22nd = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle22nd.backColor("magenta");
var style1two = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1two.hoveredSelectedItemWithNoDataStyle(hstyle2nd);
style1two.hoveredUnSelectedItemWithNoDataStyle(hstyle2nd);
style1two.unSelectedItemWithNoDataStyle(hstyle12nd);
style1two.selectedItemWithNoDataStyle(hstyle22nd);
slicer2.style(style1two);
activeSheet.setColumnWidth(1, 100);
activeSheet.setColumnWidth(2, 100);
activeSheet.setColumnWidth(3, 100);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) |

#### Returns

`any`

如果未设置任何值，则返回没有数据的未选择项的样式；否则，返回切片器样式

___

### <a id="wholeslicerstyle" name="wholeslicerstyle"></a> wholeSlicerStyle

▸ **wholeSlicerStyle**(`value?`): `any`

获取或设置整个切片器的样式

**`代码示例`**
``` javascript
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
//向工作表添加一个切片器并返回切片器实例
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Height");
slicer.position(new GC.Spread.Sheets.Point(100, 200));
//设置自定义样式
var style = new GC.Spread.Sheets.Slicers.SlicerStyle();
var styleInfo1 = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
styleInfo1.backColor("orange");
styleInfo1.borderBottom(new GC.Spread.Sheets.Slicers.SlicerBorder(2,"solid","green"));
style.wholeSlicerStyle(styleInfo1);
var styleInfo2 = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
styleInfo2.backColor("red");
styleInfo2.borderBottom(new GC.Spread.Sheets.Slicers.SlicerBorder(4,"solid","gray"));
style.hoveredSelectedItemWithDataStyle(styleInfo2);
slicer.style(style);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) |

#### Returns

`any`

如果未设置任何值，则返回整个切片器的样式；否则，返回切片器样式
