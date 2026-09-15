# Enumeration: SelectionMode

[Sheets](../modules/GC.Spread.Sheets.md).[CellTypes](../modules/GC.Spread.Sheets.CellTypes.md).SelectionMode

指定按钮列表单元格的文本选择模式。

**`example`**
```javascript
//此示例创建一个按钮列表单元格。
var cellType2 = new GC.Spread.Sheets.CellTypes.ButtonList();
cellType2.items([{text:"a",value:1},{text:"b",value:2},{text:"c",value:3}]);
cellType2.selectionMode(GC.Spread.Sheets.CellTypes.SelectionMode.single);
activeSheet.getCell(2, 2).cellType(cellType2);
```

## Table of contents

### Enumeration members

- [multiple](GC.Spread.Sheets.CellTypes.SelectionMode.md#multiple)
- [single](GC.Spread.Sheets.CellTypes.SelectionMode.md#single)

## Enumeration members

### <a id="multiple" name="multiple"></a> multiple

• **multiple** = `1`

指定选择模式为多选。

___

### <a id="single" name="single"></a> single

• **single** = `0`

指定选择模式为单选。
