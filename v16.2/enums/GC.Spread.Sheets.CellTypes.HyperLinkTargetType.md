# Enumeration: HyperLinkTargetType

[Sheets](../modules/GC.Spread.Sheets.md).[CellTypes](../modules/GC.Spread.Sheets.CellTypes.md).HyperLinkTargetType

指定超链接的目标类型

**`代码示例`**
```
//本示例创建一个超链接单元格
var cellType = new GC.Spread.Sheets.CellTypes.HyperLink();
cellType.linkColor("blue");
cellType.visitedLinkColor("#FFFF00");
cellType.text("GrapeCity");
cellType.linkToolTip("Company Web Site");
cellType.target(GC.Spread.Sheets.CellTypes.HyperLinkTargetType.self);
activeSheet.getCell(0, 2).cellType(cellType).value("http://www.grapecity.com/");
```

## Table of contents

### Enumeration members

- [blank](GC.Spread.Sheets.CellTypes.HyperLinkTargetType.md#blank)
- [parent](GC.Spread.Sheets.CellTypes.HyperLinkTargetType.md#parent)
- [self](GC.Spread.Sheets.CellTypes.HyperLinkTargetType.md#self)
- [top](GC.Spread.Sheets.CellTypes.HyperLinkTargetType.md#top)

## Enumeration members

### <a id="blank" name="blank"></a> blank

• **blank** = `0`

在新窗口或选项卡中打开超链接

___

### <a id="parent" name="parent"></a> parent

• **parent** = `2`

在父框架中打开超链接

___

### <a id="self" name="self"></a> self

• **self** = `1`

在用户单击的同一框架中打开超链接

___

### <a id="top" name="top"></a> top

• **top** = `3`

在整个窗口中打开超链接
