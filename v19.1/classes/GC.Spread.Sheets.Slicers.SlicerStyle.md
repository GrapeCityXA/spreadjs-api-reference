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

表示切片器样式设置。

**`example`**
```javascript
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

// 设置自定义样式
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

从指定的JSON字符串加载对象状态。

**`example`**
```javascript
// 这个例子使用fromJSON方法。
const light1 = GC.Spread.Sheets.Slicers.SlicerStyles.light1();
// 导出
const jsonStr = JSON.stringify(light1.toJSON());
// 导入
const newTheme = new GC.Spread.Sheets.Slicers.SlicerStyle();
newTheme.fromJSON(JSON.parse(jsonStr));
newTheme.name('custom1');
alert(jsonStr);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `Object` | 从反序列化中获取的项目切片器主题数据。 |

#### Returns

`void`

___

### <a id="headerstyle" name="headerstyle"></a> headerStyle

▸ **headerStyle**(`value?`): `any`

获取或设置切片器标题的样式。

**`example`**
```javascript
// 这个例子设置标题背景颜色。
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
// 切片器信息
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
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) | 切片器标题的样式。 |

#### Returns

`any`

如果未设置值，返回切片器标题的样式；否则返回切片器样式。

___

### <a id="hoveredselecteditemwithdatastyle" name="hoveredselecteditemwithdatastyle"></a> hoveredSelectedItemWithDataStyle

▸ **hoveredSelectedItemWithDataStyle**(`value?`): `any`

获取或设置鼠标悬停时选中项的样式。

**`example`**
```javascript
// 这个例子使用hoveredSelectedItemWithDataStyle方法。
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
// 切片器信息
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
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) | 鼠标悬停时选中项的样式。 |

#### Returns

`any`

如果未设置值，返回鼠标悬停时选中项的样式；否则返回切片器样式。

___

### <a id="hoveredselecteditemwithnodatastyle" name="hoveredselecteditemwithnodatastyle"></a> hoveredSelectedItemWithNoDataStyle

▸ **hoveredSelectedItemWithNoDataStyle**(`value?`): `any`

获取或设置悬停时已选中但无数据的切片器项的显示样式，包括背景颜色、边框和字体样式。无数据项指的是在当前筛选器和数据上下文中被判定为没有对应数据的切片器项（可能是由于其他切片器应用的筛选导致）。

**`example`**
```javascript
// 请将鼠标悬停在切片器中的项目上，查看样式效果。
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
// 添加表格
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, datasource);
var condition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.textCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.TextCompareType.equalsTo,expected: 'Dairy'});
table.rowFilter().addFilterItem(2, condition);
table.rowFilter().filter();
// 在工作表中添加一个切片器并返回该切片器实例。
var slicer = activeSheet.slicers.add("slicer",table.name(),"Name");
// 更改切片器属性。
var slicerStyleInfo = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
slicerStyleInfo.backColor("magenta");
var slicerStyle = slicer.style();
slicerStyle.hoveredSelectedItemWithNoDataStyle(slicerStyleInfo);
slicer.style(slicerStyle);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) | 鼠标悬停时选中项的样式。 |

#### Returns

`any`

如果未设置值，返回鼠标悬停时选中项的样式；否则返回切片器样式。

___

### <a id="hoveredunselecteditemwithdatastyle" name="hoveredunselecteditemwithdatastyle"></a> hoveredUnSelectedItemWithDataStyle

▸ **hoveredUnSelectedItemWithDataStyle**(`value?`): `any`

获取或设置鼠标悬停时未选中项的样式。

**`example`**
```javascript
// 这个例子使用hoveredUnSelectedItemWithDataStyle方法。
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
// 切片器样式
var hstyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
hstyle.backColor("red");
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyle();
style1.hoveredUnSelectedItemWithDataStyle(hstyle);
// 添加一个切片器到工作表并返回切片器实例。
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
// 更改切片器属性。
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) | 鼠标悬停时未选中项的样式。 |

#### Returns

`any`

如果未设置值，返回鼠标悬停时未选中项的样式；否则返回切片器样式。

___

### <a id="hoveredunselecteditemwithnodatastyle" name="hoveredunselecteditemwithnodatastyle"></a> hoveredUnSelectedItemWithNoDataStyle

▸ **hoveredUnSelectedItemWithNoDataStyle**(`value?`): `any`

获取或设置切片器中悬停的未选中项（即当前筛选条件下没有对应数据的项）的显示样式，包括颜色、字体和边框。NoDataItems表示在当前筛选和数据上下文中被判定为没有对应数据的切片器项（可能是由于其他切片器应用的筛选）。

**`example`**
```javascript
// 请将鼠标悬停在切片器中的项目上，查看样式效果。
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
var condition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.textCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.TextCompareType.equalsTo,expected: 'Apple'});
table.rowFilter().addFilterItem(1, condition);
var condition1 = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.textCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.TextCompareType.equalsTo,expected: 'Fruit'});
table.rowFilter().addFilterItem(2, condition1);
table.rowFilter().filter();
// 在工作表中添加一个切片器并返回该切片器实例。
var slicer = activeSheet.slicers.add("slicer",table.name(),"Category");
// 修改切片器的属性
var slicerStyleInfo = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
slicerStyleInfo.backColor("magenta");
var slicerStyle = slicer.style();
slicerStyle.hoveredUnSelectedItemWithNoDataStyle(slicerStyleInfo);
slicer.style(slicerStyle);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) | 鼠标悬停时未选中项的样式。 |

#### Returns

`any`

如果未设置值，返回鼠标悬停时未选中项的样式；否则返回切片器样式。

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置样式名称。

**`example`**
```javascript
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
// 在工作表中添加一个切片器并返回该切片器实例。
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Height");
// 设置自定义样式
var style = new GC.Spread.Sheets.Slicers.SlicerStyle();
var styleInfo1 = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
styleInfo1.backColor("orange");
style.wholeSlicerStyle(styleInfo1);
console.log(style.name()); // ''
style.name("orangeStyle");
slicer.style(style);
console.log(slicer.style().name()); // 'orangeStyle'
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 切片器样式名称。 |

#### Returns

`any`

如果未设置值，返回样式名称；否则返回切片器样式。

___

### <a id="selecteditemwithdatastyle" name="selecteditemwithdatastyle"></a> selectedItemWithDataStyle

▸ **selectedItemWithDataStyle**(`value?`): `any`

获取或设置选中项的样式。

**`example`**
```javascript
// 这个例子使用hoveredUnSelectedItemWithNoDataStyle方法。
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
// 添加一个切片器到工作表并返回切片器实例。
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Category");
// 更改切片器属性。
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

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) | 选中项的样式。 |

#### Returns

`any`

如果未设置值，返回选中项的样式；否则返回切片器样式。

___

### <a id="selecteditemwithnodatastyle" name="selecteditemwithnodatastyle"></a> selectedItemWithNoDataStyle

▸ **selectedItemWithNoDataStyle**(`value?`): `any`

获取或设置无数据的选定项的样式。无数据项（NoDataItems）指的是在当前筛选器和数据上下文中被判定为没有对应数据的切片器项（可能是由于其他切片器应用的筛选所致）。

**`example`**
```javascript
// 这个例子使用hoveredUnSelectedItemWithNoDataStyle方法。
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
var condition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.textCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.TextCompareType.equalsTo,expected: 'Dairy'});
table.rowFilter().addFilterItem(2, condition);
table.rowFilter().filter();
// 在工作表中添加一个切片器并返回该切片器实例。
var slicer = activeSheet.slicers.add("slicer",table.name(),"Name");
// 修改切片器的属性
var slicerStyleInfo = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
slicerStyleInfo.backColor("magenta");
var slicerStyle = slicer.style();
slicerStyle.selectedItemWithNoDataStyle(slicerStyleInfo);
slicer.style(slicerStyle);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) | 未选中项的样式。 |

#### Returns

`any`

如果未设置值，返回未选中项的样式；否则返回切片器样式。

___

### <a id="tojson" name="tojson"></a> toJSON

▸ **toJSON**(): `Object`

将对象状态保存为JSON字符串。

**`example`**
```javascript
// 这个例子使用toJSON方法。
const light1 = GC.Spread.Sheets.Slicers.SlicerStyles.light1();
// 导出
const jsonStr = JSON.stringify(light1.toJSON());
// 导入
const newTheme = new GC.Spread.Sheets.Slicers.SlicerStyle();
newTheme.fromJSON(JSON.parse(jsonStr));
newTheme.name('custom1');
alert(jsonStr);
```

#### Returns

`Object`

项目切片器主题数据。

___

### <a id="unselecteditemwithdatastyle" name="unselecteditemwithdatastyle"></a> unSelectedItemWithDataStyle

▸ **unSelectedItemWithDataStyle**(`value?`): `any`

获取或设置未选中项的样式。

**`example`**
```javascript
// 这个例子使用hoveredUnSelectedItemWithNoDataStyle方法。
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
// 添加一个切片器到工作表并返回切片器实例。
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Category");
// 更改切片器属性。
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

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) | 未选中项的样式。 |

#### Returns

`any`

如果未设置值，返回未选中项的样式；否则返回切片器样式。

___

### <a id="unselecteditemwithnodatastyle" name="unselecteditemwithnodatastyle"></a> unSelectedItemWithNoDataStyle

▸ **unSelectedItemWithNoDataStyle**(`value?`): `any`

获取或设置切片器中未选中项（即当前筛选条件下没有对应数据的项）的显示样式，包括颜色、字体和边框。NoDataItems指的是在当前筛选和数据上下文中被确定为没有对应数据的切片器项（可能是由于其他切片器应用的筛选）。

**`example`**
```javascript
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
var condition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.textCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.TextCompareType.equalsTo,expected: 'Apple'});
table.rowFilter().addFilterItem(1, condition);
var condition1 = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.textCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.TextCompareType.equalsTo,expected: 'Fruit'});
table.rowFilter().addFilterItem(2, condition1);
table.rowFilter().filter();
// 在工作表中添加一个切片器并返回该切片器实例。
var slicer = activeSheet.slicers.add("slicer",table.name(),"Category");
// 修改切片器的属性
var slicerStyleInfo = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
slicerStyleInfo.backColor("magenta");
var slicerStyle = slicer.style();
slicerStyle.unSelectedItemWithNoDataStyle(slicerStyleInfo);
slicer.style(slicerStyle);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) | 未选中项的样式。 |

#### Returns

`any`

如果未设置值，返回未选中项的样式；否则返回切片器样式。

___

### <a id="wholeslicerstyle" name="wholeslicerstyle"></a> wholeSlicerStyle

▸ **wholeSlicerStyle**(`value?`): `any`

获取或设置切片器样式。

**`example`**
```javascript
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
// 添加一个切片器到工作表并返回切片器实例。
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Height");
slicer.position(new GC.Spread.Sheets.Point(100, 200));
// 设置自定义样式
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

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SlicerStyleInfo`](GC.Spread.Sheets.Slicers.SlicerStyleInfo.md) | 切片器样式。 |

#### Returns

`any`

如果未设置值，返回切片器样式；否则返回切片器样式。
