# Enumeration: SortState

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).SortState

要执行的排序类型

**`代码示例`**
``` javascript
//本示例设置切片器中项的排序顺序
//创建一个表
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
//创建样式
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.light4();
//向工作表添加切片器并返回切片器实例
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Height");
//设置切片器属性
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.sortState(GC.Spread.Sheets.SortState.descending);
slicer.style(style1);
```

## Table of contents

### Enumeration members

- [ascending](GC.Spread.Sheets.SortState.md#ascending)
- [descending](GC.Spread.Sheets.SortState.md#descending)
- [none](GC.Spread.Sheets.SortState.md#none)

## Enumeration members

### <a id="ascending" name="ascending"></a> ascending

• **ascending** = `1`

升序

___

### <a id="descending" name="descending"></a> descending

• **descending** = `2`

降序

___

### <a id="none" name="none"></a> none

• **none** = `0`

禁用排序
