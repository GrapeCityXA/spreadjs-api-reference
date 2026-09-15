# Enumeration: TextAlign

[Sheets](../modules/GC.Spread.Sheets.md).[CellTypes](../modules/GC.Spread.Sheets.CellTypes.md).TextAlign

指定复选框单元格的文本对齐方式。

**`example`**
```javascript
//此示例创建一个复选框单元格。
var cellType = new GC.Spread.Sheets.CellTypes.RadioButtonList();
cellType.items([{text:"a",value:1},{text:"b",value:2},{text:"c",value:3}]);
cellType.textAlign(GC.Spread.Sheets.CellTypes.TextAlign.left);
activeSheet.getCell(2, 2).cellType(cellType);
```

## Table of contents

### Enumeration members

- [inside](GC.Spread.Sheets.CellTypes.TextAlign.md#inside)
- [left](GC.Spread.Sheets.CellTypes.TextAlign.md#left)
- [right](GC.Spread.Sheets.CellTypes.TextAlign.md#right)

## Enumeration members

### <a id="inside" name="inside"></a> inside

• **inside** = `4`

指定文本位于切换按钮内部。

___

### <a id="left" name="left"></a> left

• **left** = `2`

指定文本在左侧。

___

### <a id="right" name="right"></a> right

• **right** = `3`

指定文本在右侧。
