# Enumeration: EditorType

[Sheets](../modules/GC.Spread.Sheets.md).[CellTypes](../modules/GC.Spread.Sheets.CellTypes.md).EditorType

文本单元格类型的编辑器类型

**`代码示例`**
```
//本示例说明如何将文本单元格类型的编辑器更改为textarea
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

 使用可编辑的div元素作为文本单元格类型的编辑器

___

### <a id="textarea" name="textarea"></a> textarea

• **textarea** = `0`

 使用textarea元素作为文本单元格类型的编辑器
