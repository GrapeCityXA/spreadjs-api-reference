# Enumeration: DisplayMode

[Sheets](../modules/GC.Spread.Sheets.md).[Comments](../modules/GC.Spread.Sheets.Comments.md).DisplayMode

定义何时显示批注

**`代码示例`**
``` javascript
//本示例使用DisplayMode枚举
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

 始终显示批注

___

### <a id="hovershown" name="hovershown"></a> hoverShown

• **hoverShown** = `2`

 仅当指针悬停在批注的所在单元上方时才显示注释
