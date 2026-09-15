# Class: SlicerStyles

[Sheets](../modules/GC.Spread.Sheets.md).[Slicers](../modules/GC.Spread.Sheets.Slicers.md).SlicerStyles

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Slicers.SlicerStyles.md#constructor)

### Methods

- [dark1](GC.Spread.Sheets.Slicers.SlicerStyles.md#dark1)
- [dark2](GC.Spread.Sheets.Slicers.SlicerStyles.md#dark2)
- [dark3](GC.Spread.Sheets.Slicers.SlicerStyles.md#dark3)
- [dark4](GC.Spread.Sheets.Slicers.SlicerStyles.md#dark4)
- [dark5](GC.Spread.Sheets.Slicers.SlicerStyles.md#dark5)
- [dark6](GC.Spread.Sheets.Slicers.SlicerStyles.md#dark6)
- [light1](GC.Spread.Sheets.Slicers.SlicerStyles.md#light1)
- [light2](GC.Spread.Sheets.Slicers.SlicerStyles.md#light2)
- [light3](GC.Spread.Sheets.Slicers.SlicerStyles.md#light3)
- [light4](GC.Spread.Sheets.Slicers.SlicerStyles.md#light4)
- [light5](GC.Spread.Sheets.Slicers.SlicerStyles.md#light5)
- [light6](GC.Spread.Sheets.Slicers.SlicerStyles.md#light6)
- [other1](GC.Spread.Sheets.Slicers.SlicerStyles.md#other1)
- [other2](GC.Spread.Sheets.Slicers.SlicerStyles.md#other2)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new SlicerStyles**()

一个内置的切片器样式集合

**`代码示例`**
``` javascript
//本示例使用内置样式
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
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.light4();
//向工作表添加一个切片器并返回切片器实例
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
 //改变切片器的属性
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

## Methods

### <a id="dark1" name="dark1"></a> dark1

▸ `Static` **dark1**(): [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

dark1风格

**`代码示例`**
``` javascript
//本示例使用内置样式
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
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.dark1();
 //创建切片器
//将切片器添加到工作表
var slicer = activeSheet.slicers.add("slicer1", table.name(),"Height");
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Returns

[`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

___

### <a id="dark2" name="dark2"></a> dark2

▸ `Static` **dark2**(): [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

dark2风格

**`代码示例`**
``` javascript
//本示例使用内置样式
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
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.dark2();
 //创建切片器
//将切片器添加到工作表
var slicer = activeSheet.slicers.add("slicer1", table.name(),"Height");
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Returns

[`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

___

### <a id="dark3" name="dark3"></a> dark3

▸ `Static` **dark3**(): [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

dark3风格

**`代码示例`**
``` javascript
//本示例使用内置样式
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
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.dark3();
 //创建切片器
//将切片器添加到工作表
var slicer = activeSheet.slicers.add("slicer1", table.name(),"Height");
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Returns

[`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

___

### <a id="dark4" name="dark4"></a> dark4

▸ `Static` **dark4**(): [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

dark4风格

**`代码示例`**
``` javascript
//本示例使用内置样式
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
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.dark4();
 //创建切片器
//将切片器添加到工作表
var slicer = activeSheet.slicers.add("slicer1", table.name(),"Height");
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Returns

[`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

___

### <a id="dark5" name="dark5"></a> dark5

▸ `Static` **dark5**(): [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

dark5风格

**`代码示例`**
``` javascript
//本示例使用内置样式
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
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.dark5();
 //创建切片器
//将切片器添加到工作表
var slicer = activeSheet.slicers.add("slicer1", table.name(),"Height");
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Returns

[`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

___

### <a id="dark6" name="dark6"></a> dark6

▸ `Static` **dark6**(): [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

dark6风格

**`代码示例`**
``` javascript
//本示例使用内置样式
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
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.dark6();
 //创建切片器
//将切片器添加到工作表
var slicer = activeSheet.slicers.add("slicer1", table.name(),"Height");
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Returns

[`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

___

### <a id="light1" name="light1"></a> light1

▸ `Static` **light1**(): [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

light1风格

**`代码示例`**
``` javascript
//本示例使用内置样式
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
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.light1();
 //创建切片器
//将切片器添加到工作表
var slicer = activeSheet.slicers.add("slicer1", table.name(),"Height");
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Returns

[`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

___

### <a id="light2" name="light2"></a> light2

▸ `Static` **light2**(): [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

light2风格

**`代码示例`**
``` javascript
//本示例使用内置样式
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
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.light2();
 //创建切片器
//将切片器添加到工作表
var slicer = activeSheet.slicers.add("slicer1", table.name(),"Height");
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Returns

[`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

___

### <a id="light3" name="light3"></a> light3

▸ `Static` **light3**(): [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

light3风格

**`代码示例`**
``` javascript
//本示例使用内置样式
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
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.light3();
 //创建切片器
//将切片器添加到工作表
var slicer = activeSheet.slicers.add("slicer1", table.name(),"Height");
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Returns

[`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

___

### <a id="light4" name="light4"></a> light4

▸ `Static` **light4**(): [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

light4风格

**`代码示例`**
``` javascript
//本示例使用内置样式
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
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.light4();
 //创建切片器
//将切片器添加到工作表
var slicer = activeSheet.slicers.add("slicer1", table.name(),"Height");
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Returns

[`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

___

### <a id="light5" name="light5"></a> light5

▸ `Static` **light5**(): [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

light5风格

**`代码示例`**
``` javascript
//本示例使用内置样式
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
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.light5();
 //创建切片器
//将切片器添加到工作表
var slicer = activeSheet.slicers.add("slicer1", table.name(),"Height");
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Returns

[`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

___

### <a id="light6" name="light6"></a> light6

▸ `Static` **light6**(): [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

light6风格

**`代码示例`**
``` javascript
//本示例使用内置样式
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
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.light6();
 //创建切片器
//将切片器添加到工作表
var slicer = activeSheet.slicers.add("slicer1", table.name(),"Height");
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Returns

[`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

___

### <a id="other1" name="other1"></a> other1

▸ `Static` **other1**(): [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

获取other1样式

**`代码示例`**
``` javascript
//本示例使用内置样式
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
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.other1();
 //创建切片器
//将切片器添加到工作表
var slicer = activeSheet.slicers.add("slicer1", table.name(),"Height");
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Returns

[`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

___

### <a id="other2" name="other2"></a> other2

▸ `Static` **other2**(): [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

获取other2样式

**`代码示例`**
``` javascript
//本示例使用内置样式
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
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.other2();
 //创建切片器
//将切片器添加到工作表
var slicer = activeSheet.slicers.add("slicer1", table.name(),"Height");
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(style1);
```

#### Returns

[`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)
