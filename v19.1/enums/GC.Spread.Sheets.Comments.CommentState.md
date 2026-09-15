# Enumeration: CommentState

[Sheets](../modules/GC.Spread.Sheets.md).[Comments](../modules/GC.Spread.Sheets.Comments.md).CommentState

定义批注状态。

**`example`**
```javascript
//此示例获取批注状态。
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

指定批注处于活动状态。
在活动状态下，批注当前被选中。
用户可以移动批注的位置或调整批注的大小。

___

### <a id="edit" name="edit"></a> edit

• **edit** = `2`

指定批注处于编辑状态。
批注的编辑状态表示批注正在被修改或更新。
当用户正在更改批注内容时会出现此状态。

___

### <a id="normal" name="normal"></a> normal

• **normal** = `3`

指定批注处于正常状态。
在正常状态下，批注当前未被选中。
用户无法与正常状态下的批注交互。
点击批注将改变状态为活动或编辑。
