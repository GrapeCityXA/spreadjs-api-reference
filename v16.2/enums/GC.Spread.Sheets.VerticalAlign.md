# Enumeration: VerticalAlign

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).VerticalAlign

垂直对齐方式

**`代码示例`**
```
//本示例使用了垂直对齐类型
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

 单元格内容是底部对齐的

___

### <a id="center" name="center"></a> center

• **center** = `1`

 单元格内容居中

___

### <a id="top" name="top"></a> top

• **top** = `0`

 单元格内容是顶对齐的
