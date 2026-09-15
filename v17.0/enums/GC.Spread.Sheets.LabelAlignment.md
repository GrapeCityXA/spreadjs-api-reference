# Enumeration: LabelAlignment

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).LabelAlignment

单元格标签的位置

**`代码示例`**
```
//本示例设置单元格填充，对齐方式和其他选项
var type = new GC.Spread.Sheets.Style();
type.watermark = "User name";
type.cellPadding = "20";
type.labelOptions = {alignment:GC.Spread.Sheets.LabelAlignment.topLeft, visibility: GC.Spread.Sheets.LabelVisibility.visible};
activeSheet.setStyle(0, 1, type);
activeSheet.getRange(0, -1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).height(60);
activeSheet.getRange(-1, 1, -1, 1).width(150);
var combo = new GC.Spread.Sheets.CellTypes.ComboBox();
combo.items([{ text: "Oranges", value: "11k" }, { text: "Apples", value: "15k" }, { text: "Grape", value: "100k" }]);
combo.editorValueType(GC.Spread.Sheets.CellTypes.EditorValueType.text);
activeSheet.setCellType(2, 1, combo, GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(2, 1, GC.Spread.Sheets.SheetArea.viewport).watermark("ComboBox Cell Type").cellPadding('10 10 20 10');
activeSheet.getCell(2, 1, GC.Spread.Sheets.SheetArea.viewport).labelOptions({alignment: GC.Spread.Sheets.LabelAlignment.bottomCenter, foreColor: 'yellowgreen', font: 'bold 15px Arial'});
activeSheet.getRange(2, -1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).height(60);
```

## Table of contents

### Enumeration members

- [bottomCenter](GC.Spread.Sheets.LabelAlignment.md#bottomcenter)
- [bottomLeft](GC.Spread.Sheets.LabelAlignment.md#bottomleft)
- [bottomRight](GC.Spread.Sheets.LabelAlignment.md#bottomright)
- [topCenter](GC.Spread.Sheets.LabelAlignment.md#topcenter)
- [topLeft](GC.Spread.Sheets.LabelAlignment.md#topleft)
- [topRight](GC.Spread.Sheets.LabelAlignment.md#topright)

## Enumeration members

### <a id="bottomcenter" name="bottomcenter"></a> bottomCenter

• **bottomCenter** = `4`

 单元格标签的位置是底端中心对齐

___

### <a id="bottomleft" name="bottomleft"></a> bottomLeft

• **bottomLeft** = `3`

 单元格标签的位置是左下角对齐

___

### <a id="bottomright" name="bottomright"></a> bottomRight

• **bottomRight** = `5`

 单元格标签的位置是右下角对齐

___

### <a id="topcenter" name="topcenter"></a> topCenter

• **topCenter** = `1`

 单元格标签的位置是顶端居中对齐

___

### <a id="topleft" name="topleft"></a> topLeft

• **topLeft** = `0`

 单元格标签的位置是左上角对齐

___

### <a id="topright" name="topright"></a> topRight

• **topRight** = `2`

 单元格标签的位置是右上角对齐
