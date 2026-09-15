# Enumeration: EditorType

[Sheets](../modules/GC.Spread.Sheets.md).[CellTypes](../modules/GC.Spread.Sheets.CellTypes.md).EditorType

表示文本单元格类型的编辑器类型。

**`example`**
```
//此示例展示如何将文本单元格类型的编辑器更改为文本区域。
var tempStyle = new GC.Spread.Sheets.Style();
tempStyle.cellType = new GC.Spread.Sheets.CellTypes.Text(GC.Spread.Sheets.CellTypes.EditorType.textarea);
activeSheet.setDefaultStyle(tempStyle);
```

## Table of contents

### Enumeration members

- [editableDiv](GC.Spread.Sheets.CellTypes.EditorType.md#editablediv)
- [textarea](GC.Spread.Sheets.CellTypes.EditorType.md#textarea)

## Enumeration members

### <a id="editablediv" name="editablediv"></a> editableDiv

• **editableDiv** = `1`

使用可编辑的 div 元素作为文本单元格类型的编辑器。

___

### <a id="textarea" name="textarea"></a> textarea

• **textarea** = `0`

使用 textarea 元素作为文本单元格类型的编辑器。
