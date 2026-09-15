# Enumeration: DisplayMode

[Sheets](../modules/GC.Spread.Sheets.md).[Comments](../modules/GC.Spread.Sheets.Comments.md).DisplayMode

定义批注的显示时机。

**`example`**
```
//此示例使用DisplayMode枚举。
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
activeSheet.getCell(5,5).comment(comment);
```

## Table of contents

### Enumeration members

- [alwaysShown](GC.Spread.Sheets.Comments.DisplayMode.md#alwaysshown)
- [hoverShown](GC.Spread.Sheets.Comments.DisplayMode.md#hovershown)

## Enumeration members

### <a id="alwaysshown" name="alwaysshown"></a> alwaysShown

• **alwaysShown** = `1`

指定批注始终显示。

___

### <a id="hovershown" name="hovershown"></a> hoverShown

• **hoverShown** = `2`

指定批注仅在鼠标悬停在批注所属单元格上时显示。
