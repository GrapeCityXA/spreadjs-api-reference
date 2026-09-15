# Enumeration: Direction

[Sheets](../modules/GC.Spread.Sheets.md).[CellTypes](../modules/GC.Spread.Sheets.CellTypes.md).Direction

指定单选按钮列表单元格的扩展方向。

**`example`**
```javascript
//此示例创建一个单选按钮列表单元格。
var cellType2 = new GC.Spread.Sheets.CellTypes.RadioButtonList();
cellType2.items([{text:"a",value:1},{text:"b",value:2},{text:"c",value:3}]);
cellType2.direction(GC.Spread.Sheets.CellTypes.Direction.vertical);
activeSheet.getCell(2, 2).cellType(cellType2);
```

## Table of contents

### Enumeration members

- [horizontal](GC.Spread.Sheets.CellTypes.Direction.md#horizontal)
- [vertical](GC.Spread.Sheets.CellTypes.Direction.md#vertical)

## Enumeration members

### <a id="horizontal" name="horizontal"></a> horizontal

• **horizontal** = `0`

指定项目水平扩展。

___

### <a id="vertical" name="vertical"></a> vertical

• **vertical** = `1`

指定项目垂直扩展。
