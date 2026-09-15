# Class: ItemSlicer

[Sheets](../modules/GC.Spread.Sheets.md).[Slicers](../modules/GC.Spread.Sheets.Slicers.md).ItemSlicer

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Slicers.ItemSlicer.md#constructor)

### Methods

- [captionName](GC.Spread.Sheets.Slicers.ItemSlicer.md#captionname)
- [columnCount](GC.Spread.Sheets.Slicers.ItemSlicer.md#columncount)
- [getDOMElement](GC.Spread.Sheets.Slicers.ItemSlicer.md#getdomelement)
- [getStyleName](GC.Spread.Sheets.Slicers.ItemSlicer.md#getstylename)
- [height](GC.Spread.Sheets.Slicers.ItemSlicer.md#height)
- [itemHeight](GC.Spread.Sheets.Slicers.ItemSlicer.md#itemheight)
- [name](GC.Spread.Sheets.Slicers.ItemSlicer.md#name)
- [showHeader](GC.Spread.Sheets.Slicers.ItemSlicer.md#showheader)
- [showNoDataItems](GC.Spread.Sheets.Slicers.ItemSlicer.md#shownodataitems)
- [showNoDataItemsInLast](GC.Spread.Sheets.Slicers.ItemSlicer.md#shownodataitemsinlast)
- [sortState](GC.Spread.Sheets.Slicers.ItemSlicer.md#sortstate)
- [style](GC.Spread.Sheets.Slicers.ItemSlicer.md#style)
- [visuallyNoDataItems](GC.Spread.Sheets.Slicers.ItemSlicer.md#visuallynodataitems)
- [width](GC.Spread.Sheets.Slicers.ItemSlicer.md#width)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new ItemSlicer**(`name`, `slicerData`, `columnName`)

项切片器

**`代码示例`**
``` javascript
//本示例创建一个项切片器
//创建表格
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: "1968/6/8" },
    { Name: "Betty", City: "NewYork", Birthday: "1972/7/3" },
    { Name: "Alice", City: "Washington", Birthday: "2012/2/15" },

var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var slicerData = new GC.Spread.Sheets.Slicers.TableSlicerData(table)
//给项切片器设置项切片器数据
var slicer = new GC.Spread.Sheets.Slicers.ItemSlicer("slicer", slicerData, "Name");
//将项切片器添加到dom树
//The "slicerHost" is the div you want to add the slicer's dom to.
$("#slicerHost").append(slicer.getDOMElement());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 项切片器名称 |
| `slicerData` | [`GeneralSlicerData`](GC.Spread.Slicers.GeneralSlicerData.md) | GeneralSlicerData或TableSlicerData的实例 |
| `columnName` | `string` | 与项切片器相关的列名称 |

## Methods

### <a id="captionname" name="captionname"></a> captionName

▸ **captionName**(`value?`): `any`

获取或设置项切片器头部名称

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: "1968/6/8" },
    { Name: "Betty", City: "NewYork", Birthday: "1972/7/3" },
    { Name: "Alice", City: "Washington", Birthday: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var slicerData = new GC.Spread.Sheets.Slicers.TableSlicerData(table)
//Set slicer data to item slicer.
var slicer = new GC.Spread.Sheets.Slicers.ItemSlicer("slicer", slicerData, "Name");
var oldValue = slicer.captionName();
console.log(oldValue);
slicer.captionName('Slicer_Caption');
var newValue = slicer.captionName();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置任何值，则返回项切片器头部名称；否则，返回项切片器

___

### <a id="columncount" name="columncount"></a> columnCount

▸ **columnCount**(`value?`): `any`

获取或设置项切片器的列数

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: "1968/6/8" },
    { Name: "Betty", City: "NewYork", Birthday: "1972/7/3" },
    { Name: "Alice", City: "Washington", Birthday: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var slicerData = new GC.Spread.Sheets.Slicers.TableSlicerData(table)
//Set slicer data to item slicer.
var slicer = new GC.Spread.Sheets.Slicers.ItemSlicer("slicer", slicerData, "Name");
var oldValue = slicer.columnCount();
console.log(oldValue);
slicer.columnCount(3);
var newValue = slicer.columnCount();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置任何值，则返回项切片器的列数；否则，返回项切片器

___

### <a id="getdomelement" name="getdomelement"></a> getDOMElement

▸ **getDOMElement**(): `HTMLElement`

获取项切片器的dom元素

**`example`**
```
//This example creates an item slicer.
//create table
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: "1968/6/8" },
    { Name: "Betty", City: "NewYork", Birthday: "1972/7/3" },
    { Name: "Alice", City: "Washington", Birthday: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var slicerData = new GC.Spread.Sheets.Slicers.TableSlicerData(table)
//Set slicer data to item slicer.
var slicer = new GC.Spread.Sheets.Slicers.ItemSlicer("slicer", slicerData, "Name");
//Add the item slicer to the dom tree.
//The "slicerHost" is the div you want to add the slicer's dom to.
$("#slicerHost").append(slicer.getDOMElement());
```

#### Returns

`HTMLElement`

项切片器的dom元素

### <a id="getstylename" name="getstylename"></a> getStyleName

▸ **getStyleName**(): `undefined` \| `string`

获取或设置表项切片器的样式名称。

#### Returns

`undefined` \| `string`

返回表项切片器样式名称。

___

### <a id="height" name="height"></a> height

▸ **height**(`value?`): `any`

获取或设置项切片器的高度

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: "1968/6/8" },
    { Name: "Betty", City: "NewYork", Birthday: "1972/7/3" },
    { Name: "Alice", City: "Washington", Birthday: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var slicerData = new GC.Spread.Sheets.Slicers.TableSlicerData(table)
//Set slicer data to item slicer.
var slicer = new GC.Spread.Sheets.Slicers.ItemSlicer("slicer", slicerData, "Name");
var oldValue = slicer.height();
console.log(oldValue);
slicer.height(120);
var newValue = slicer.height();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置任何值，则返回项切片器的高度；否则，返回项切片器

___

### <a id="itemheight" name="itemheight"></a> itemHeight

▸ **itemHeight**(`value?`): `any`

获取或设置项切片器的项高度

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: "1968/6/8" },
    { Name: "Betty", City: "NewYork", Birthday: "1972/7/3" },
    { Name: "Alice", City: "Washington", Birthday: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var slicerData = new GC.Spread.Sheets.Slicers.TableSlicerData(table)
//Set slicer data to item slicer.
var slicer = new GC.Spread.Sheets.Slicers.ItemSlicer("slicer", slicerData, "Name");
var oldValue = slicer.itemHeight();
console.log(oldValue);
slicer.itemHeight(34);
var newValue = slicer.itemHeight();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置任何值，则返回项切片器的项高度；否则，返回项切片器

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置项切片器的名称

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: "1968/6/8" },
    { Name: "Betty", City: "NewYork", Birthday: "1972/7/3" },
    { Name: "Alice", City: "Washington", Birthday: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var slicerData = new GC.Spread.Sheets.Slicers.TableSlicerData(table)
//Set slicer data to item slicer.
var slicer = new GC.Spread.Sheets.Slicers.ItemSlicer("slicer", slicerData, "Name");
var oldValue = slicer.name();
console.log(oldValue);
slicer.name('SlicerA');
var newValue = slicer.name();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置任何值，则返回项切片器的名称；否则，返回项切片器

___

### <a id="showheader" name="showheader"></a> showHeader

▸ **showHeader**(`value?`): `any`

获取或设置是否显示项切片器头部

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: "1968/6/8" },
    { Name: "Betty", City: "NewYork", Birthday: "1972/7/3" },
    { Name: "Alice", City: "Washington", Birthday: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var slicerData = new GC.Spread.Sheets.Slicers.TableSlicerData(table)
//Set slicer data to item slicer.
var slicer = new GC.Spread.Sheets.Slicers.ItemSlicer("slicer", slicerData, "Name");
var oldValue = slicer.showHeader();
console.log(oldValue);
slicer.showHeader(false);
var newValue = slicer.showHeader();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置任何值，则返回是否显示项切片器头部；否则，返回项切片器

___

### <a id="shownodataitems" name="shownodataitems"></a> showNoDataItems

▸ **showNoDataItems**(`value?`): `any`

获取或设置是否显示项切片器的无数据项

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: "1968/6/8" },
    { Name: "Betty", City: "NewYork", Birthday: "1972/7/3" },
    { Name: "Alice", City: "Washington", Birthday: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var slicerData = new GC.Spread.Sheets.Slicers.TableSlicerData(table)
//Set slicer data to item slicer.
var slicer = new GC.Spread.Sheets.Slicers.ItemSlicer("slicer", slicerData, "Name");
var oldValue = slicer.showNoDataItems();
console.log(oldValue);
slicer.showNoDataItems(false);
var newValue = slicer.showNoDataItems();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置任何值，则返回是否显示项切片器的无数据项；否则，返回项切片器

___

### <a id="shownodataitemsinlast" name="shownodataitemsinlast"></a> showNoDataItemsInLast

▸ **showNoDataItemsInLast**(`value?`): `any`

获取或设置是否最后显示无数据项

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: "1968/6/8" },
    { Name: "Betty", City: "NewYork", Birthday: "1972/7/3" },
    { Name: "Alice", City: "Washington", Birthday: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var slicerData = new GC.Spread.Sheets.Slicers.TableSlicerData(table)
//Set slicer data to item slicer.
var slicer = new GC.Spread.Sheets.Slicers.ItemSlicer("slicer", slicerData, "Name");
var oldValue = slicer.showNoDataItemsInLast();
console.log(oldValue);
slicer.showNoDataItemsInLast(false);
var newValue = slicer.showNoDataItemsInLast();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置任何值，则返回是否最后显示无数据项；否则，返回项切片器

___

### <a id="sortstate" name="sortstate"></a> sortState

▸ **sortState**(`value?`): `any`

获取或设置项切片器的排序状态

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: "1968/6/8" },
    { Name: "Betty", City: "NewYork", Birthday: "1972/7/3" },
    { Name: "Alice", City: "Washington", Birthday: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var slicerData = new GC.Spread.Sheets.Slicers.TableSlicerData(table)
//Set slicer data to item slicer.
var slicer = new GC.Spread.Sheets.Slicers.ItemSlicer("slicer", slicerData, "Name");
var oldValue = slicer.sortState();
console.log(oldValue);
slicer.sortState(GC.Spread.Sheets.SortState.descending);
var newValue = slicer.sortState();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SortState`](../enums/GC.Spread.Sheets.SortState.md) |

#### Returns

`any`

如果未设置任何值，则返回项切片器的排序状态；否则，返回项切片器

___

### <a id="style" name="style"></a> style

▸ **style**(`value?`): `any`

获取或设置项切片器的样式

**`代码示例`**
``` javascript
样式是json数据，其json模式如下：
{
     "$schema" : "http://json-schema.org/draft-04/schema#",
     "title" : "style",
     "type" : "object",
     "properties" : {
         "wholeSlicerStyle" : {
             "$ref" : "#/definitions/StyleInfo"
         },
         "headerStyle" : {
             "$ref" : "#/definitions/StyleInfo"
         },
         "selectedItemWithDataStyle" : {
             "$ref" : "#/definitions/StyleInfo"
         },
         "selectedItemWithNoDataStyle" : {
             "$ref" : "#/definitions/StyleInfo"
         },
         "unSelectedItemWithDataStyle" : {
             "$ref" : "#/definitions/StyleInfo"
         },
         "unSelectedItemWithNoDataStyle" : {
             "$ref" : "#/definitions/StyleInfo"
         },
         "hoveredSelectedItemWithDataStyle" : {
             "$ref" : "#/definitions/StyleInfo"
         },
         "hoveredSelectedItemWithNoDataStyle" : {
             "$ref" : "#/definitions/StyleInfo"
         },
         "hoveredUnSelectedItemWithDataStyle" : {
             "$ref" : "#/definitions/StyleInfo"
         },
         "hoveredUnSelectedItemWithNoDataStyle" : {
             "$ref" : "#/definitions/StyleInfo"
         }
     },
     "definitions" : {
         "StyleInfo" : {
             "type" : "object",
             "properties" : {
                     "backColor" : {
                             "type" : "string"
                     },
                     "foreColor" : {
                             "type" : "string"
                     },
                     "font" : {
                             "type" : "string"
                     },
                     "borderLeft" : {
                             "$ref" : "#/definitions/SlicerBorder"
                     },
                     "borderTop" : {
                             "$ref" : "#/definitions/SlicerBorder"
                     },
                     "borderRight" : {
                             "$ref" : "#/definitions/SlicerBorder"
                     },
                     "borderBottom" : {
                             "$ref" : "#/definitions/SlicerBorder"
                     },
                 "textDecoration":{
                     "type" : "string"
                 }
             }
         },
         "SlicerBorder":{
             "type":"object",
             "properties":{
                 "borderWidth":{
                         "type":"number"
                 },
                 "borderStyle":{
                         "type":"string"
                 },
                 "borderColor":{
                         "type":"string"
                 }
          }
         }
     }
 }
using sample:
var style = new GC.Spread.Sheets.Slicers.SlicerStyle();
style.wholeSlicerStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo('red', 'blue', '16pt Calibri'));
style.headerStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo(undefined, 'green'));
style.selectedItemWithDataStyle(new GC.Spread.Sheets.Slicers.SlicerStyleInfo(undefined, undefined, undefined, new GC.Spread.Sheets.LineBorder('pink', GC.Spread.Sheets.LineStyle.double)));
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: "1968/6/8" },
    { Name: "Betty", City: "NewYork", Birthday: "1972/7/3" },
    { Name: "Alice", City: "Washington", Birthday: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var slicerData = new GC.Spread.Sheets.Slicers.TableSlicerData(table)
//Set slicer data to item slicer.
var slicer = new GC.Spread.Sheets.Slicers.ItemSlicer("slicer", slicerData, "Name");
var oldValue = slicer.style();
console.log(oldValue);
slicer.style(style);
var newValue = slicer.style();
console.log(newValue);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `any` | 项切片器的样式 |

#### Returns

`any`

如果未设置任何值，则返回项切片器的样式；否则，返回项切片器

___

### <a id="visuallynodataitems" name="visuallynodataitems"></a> visuallyNoDataItems

▸ **visuallyNoDataItems**(`value?`): `any`

获取或设置是否在视觉上区分没有数据的项

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: "1968/6/8" },
    { Name: "Betty", City: "NewYork", Birthday: "1972/7/3" },
    { Name: "Alice", City: "Washington", Birthday: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var slicerData = new GC.Spread.Sheets.Slicers.TableSlicerData(table)
//Set slicer data to item slicer.
var slicer = new GC.Spread.Sheets.Slicers.ItemSlicer("slicer", slicerData, "Name");
var oldValue = slicer.visuallyNoDataItems();
console.log(oldValue);
slicer.visuallyNoDataItems(false);
var newValue = slicer.visuallyNoDataItems();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置任何值，则返回是否在视觉上区分没有数据的项；否则，返回项切片器

___

### <a id="width" name="width"></a> width

▸ **width**(`value?`): `any`

获取或设置项切片器的宽度

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook('ss');
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: "1968/6/8" },
    { Name: "Betty", City: "NewYork", Birthday: "1972/7/3" },
    { Name: "Alice", City: "Washington", Birthday: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var slicerData = new GC.Spread.Sheets.Slicers.TableSlicerData(table)
//Set slicer data to item slicer.
var slicer = new GC.Spread.Sheets.Slicers.ItemSlicer("slicer", slicerData, "Name");
var oldValue = slicer.width();
console.log(oldValue);
slicer.width(120);
var newValue = slicer.width();
console.log(newValue);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置任何值，则返回项切片器的宽度；否则，返回项切片器
