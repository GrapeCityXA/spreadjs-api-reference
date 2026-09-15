# Enumeration: VerticalAlign

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).VerticalAlign

指定垂直对齐方式。

**`example`**
```
//此示例使用VerticalAlign类型。
var style = new GC.Spread.Sheets.Style();
style.font = "8pt Arial";
style.hAlign = GC.Spread.Sheets.HorizontalAlign.center;
style.vAlign = GC.Spread.Sheets.VerticalAlign.center;
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(1,1).value("B2");
```

## Table of contents

### Enumeration members

- [bottom](GC.Spread.Sheets.VerticalAlign.md#bottom)
- [center](GC.Spread.Sheets.VerticalAlign.md#center)
- [top](GC.Spread.Sheets.VerticalAlign.md#top)

## Enumeration members

### <a id="bottom" name="bottom"></a> bottom

• **bottom** = `2`

表示单元格内容底部对齐。

___

### <a id="center" name="center"></a> center

• **center** = `1`

表示单元格内容居中对齐。

___

### <a id="top" name="top"></a> top

• **top** = `0`

表示单元格内容顶部对齐。
