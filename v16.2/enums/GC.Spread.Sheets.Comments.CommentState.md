# Enumeration: CommentState

[Sheets](../modules/GC.Spread.Sheets.md).[Comments](../modules/GC.Spread.Sheets.Comments.md).CommentState

定义批注状态.

**`代码示例`**
```
//本示例使用了批注状态.
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
activeSheet.getCell(5,5).comment(comment);
alert(comment.commentState());
```

## Table of contents

### Enumeration members

- [active](GC.Spread.Sheets.Comments.CommentState.md#active)
- [edit](GC.Spread.Sheets.Comments.CommentState.md#edit)
- [normal](GC.Spread.Sheets.Comments.CommentState.md#normal)

## Enumeration members

### <a id="active" name="active"></a> active

• **active** = `1`

批注处于活动状态

___

### <a id="edit" name="edit"></a> edit

• **edit** = `2`

批注处于编辑状态

___

### <a id="normal" name="normal"></a> normal

• **normal** = `3`

批注处于正常状态
