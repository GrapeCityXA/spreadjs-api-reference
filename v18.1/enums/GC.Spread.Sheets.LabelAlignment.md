# Enumeration: LabelAlignment

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).LabelAlignment

指定单元格标签位置。

**`example`**
```
//此示例设置单元格内边距、对齐方式和其他选项。
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

表示单元格标签位置在底部居中。

___

### <a id="bottomleft" name="bottomleft"></a> bottomLeft

• **bottomLeft** = `3`

表示单元格标签位置在左下角。

___

### <a id="bottomright" name="bottomright"></a> bottomRight

• **bottomRight** = `5`

表示单元格标签位置在右下角。

___

### <a id="topcenter" name="topcenter"></a> topCenter

• **topCenter** = `1`

表示单元格标签位置在顶部居中。

___

### <a id="topleft" name="topleft"></a> topLeft

• **topLeft** = `0`

表示单元格标签位置在左上角。

___

### <a id="topright" name="topright"></a> topRight

• **topRight** = `2`

表示单元格标签位置在右上角。
