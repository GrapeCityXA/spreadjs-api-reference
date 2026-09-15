# Enumeration: TextDirectionType

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).TextDirectionType

定义文本方向类型。

**`example`**
```
//此示例使用TextDirectionType枚举。
activeSheet.getCell(0, 0).textDirection(GC.Spread.Sheets.TextDirectionType.rightToLeft);
activeSheet.getRange(1, -1, 1, -1).textDirection(GC.Spread.Sheets.TextDirectionType.rightToLeft);
var style = new GC.Spread.Sheets.Style();
style.textDirection = GC.Spread.Sheets.TextDirectionType.rightToLeft;
activeSheet.setStyle(1, 1, style, GC.Spread.Sheets.SheetArea.viewport);
```

## Table of contents

### Enumeration members

- [context](GC.Spread.Sheets.TextDirectionType.md#context)
- [leftToRight](GC.Spread.Sheets.TextDirectionType.md#lefttoright)
- [rightToLeft](GC.Spread.Sheets.TextDirectionType.md#righttoleft)

## Enumeration members

### <a id="context" name="context"></a> context

• **context** = `0`

指定文本方向取决于上下文，通过扫描文本的第一个非空白字符来确定：如果是强从右到左的字符，则文本方向为从右到左；否则，文本方向为从左到右。

___

### <a id="lefttoright" name="lefttoright"></a> leftToRight

• **leftToRight** = `1`

指定单元格中的文本方向为从左到右，如英语。

___

### <a id="righttoleft" name="righttoleft"></a> rightToLeft

• **rightToLeft** = `2`

指定单元格中的文本方向为从右到左，如阿拉伯语或希伯来语。
