# Class: SlicerCollection

[Sheets](../modules/GC.Spread.Sheets.md).[Slicers](../modules/GC.Spread.Sheets.Slicers.md).SlicerCollection

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Slicers.SlicerCollection.md#constructor)

### Methods

- [add](GC.Spread.Sheets.Slicers.SlicerCollection.md#add)
- [all](GC.Spread.Sheets.Slicers.SlicerCollection.md#all)
- [clear](GC.Spread.Sheets.Slicers.SlicerCollection.md#clear)
- [get](GC.Spread.Sheets.Slicers.SlicerCollection.md#get)
- [remove](GC.Spread.Sheets.Slicers.SlicerCollection.md#remove)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new SlicerCollection**(`sheet`)

表示一个切片器管理器，管理工作表中的所有切片器。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheet` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 工作表。 |

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`slicerName`, `targetName`, `itemName`, `style?`, `type?`): [`ISlicer`](../interfaces/GC.Spread.Sheets.Slicers.ISlicer.md)

添加一个切片器到工作表。

**`example`**
```
// 这个例子使用add方法。
// 创建一个表
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
// 添加一个切片器到工作表并返回切片器实例。
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
 // 更改切片器属性。
slicer.position(new GC.Spread.Sheets.Point(100, 200));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `slicerName` | `string` | 切片器名称。 |
| `targetName` | `string` | 切片器关联的表或透视表的名称。 |
| `itemName` | `string` | 切片器关联的表列或透视表字段的名称。 |
| `style?` | `string` \| [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md) \| [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md) | 切片器样式。 |
| `type?` | [`SlicerType`](../enums/GC.Spread.Sheets.Slicers.SlicerType.md) | - |

#### Returns

[`ISlicer`](../interfaces/GC.Spread.Sheets.Slicers.ISlicer.md)

添加到工作表的切片器。

___

### <a id="all" name="all"></a> all

▸ **all**(`targetName?`, `itemName?`): [`ISlicer`](../interfaces/GC.Spread.Sheets.Slicers.ISlicer.md)[]

获取工作表中具有指示的表名称和列名称的所有切片器。

**`example`**
```
// 创建一个表
var datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var activeSheet = spread.getActiveSheet();
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
// 添加一个切片器到工作表并返回切片器实例。
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");

var allSlicers = activeSheet.slicers.all();
console.log(allSlicers.length); // 1;
console.log(allSlicers[0] === slicer); // true
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `targetName?` | `string` |
| `itemName?` | `string` |

#### Returns

[`ISlicer`](../interfaces/GC.Spread.Sheets.Slicers.ISlicer.md)[]

切片器集合。

___

### <a id="clear" name="clear"></a> clear

▸ **clear**(): `void`

从工作表中删除所有切片器。

**`example`**
```
// 创建一个表
var datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var activeSheet = spread.getActiveSheet();
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
// 添加一个切片器到工作表并返回切片器实例。
var slicer1 = activeSheet.slicers.add("slicer1",table.name(),"Name");
var slicer2 = activeSheet.slicers.add("slicer2",table.name(),"City");

var allSlicers = activeSheet.slicers.all();
console.log(allSlicers.length); // 2;

activeSheet.slicers.clear();
allSlicers = activeSheet.slicers.all();
console.log(allSlicers.length); // 0;
```

#### Returns

`void`

___

### <a id="get" name="get"></a> get

▸ **get**(`name`): [`ISlicer`](../interfaces/GC.Spread.Sheets.Slicers.ISlicer.md)

获取工作表中具有指示的名称的切片器。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 切片器名称。 |

#### Returns

[`ISlicer`](../interfaces/GC.Spread.Sheets.Slicers.ISlicer.md)

具有指示名称的切片器。

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`name`): `void`

使用指示的切片器名称从工作表中删除切片器。

**`example`**
```
// 创建一个表
var datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var activeSheet = spread.getActiveSheet();
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
// 添加一个切片器到工作表并返回切片器实例。
var slicer1 = activeSheet.slicers.add("slicer1",table.name(),"Name");
var slicer2 = activeSheet.slicers.add("slicer2",table.name(),"City");

var allSlicers = activeSheet.slicers.all();
console.log(allSlicers.length); // 2;

activeSheet.slicers.remove('slicer1');
allSlicers = activeSheet.slicers.all();
console.log(allSlicers.length); // 1;
console.log(allSlicers[0] === slicer2); // true;
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 切片器名称。 |

#### Returns

`void`
