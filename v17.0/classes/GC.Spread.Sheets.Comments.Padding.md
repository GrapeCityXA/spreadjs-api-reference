# Class: Padding

[Sheets](../modules/GC.Spread.Sheets.md).[Comments](../modules/GC.Spread.Sheets.Comments.md).Padding

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Comments.Padding.md#constructor)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Padding**(`top?`, `right?`, `bottom?`, `left?`)

边距信息

**`example`**
```
var comment = activeSheet.comments.add(2, 2, 'this is a comment');
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown)
console.log(comment.padding()); // undefined
comment.padding(new GC.Spread.Sheets.Comments.Padding(10, 20, 30, 40));
console.log(comment.padding()); // Padding {top: 10, right: 20, bottom: 30, left: 40}
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `top?` | `number` | 上边距 |
| `right?` | `number` | 右边距 |
| `bottom?` | `number` | 下边距 |
| `left?` | `number` | 左边距 |
