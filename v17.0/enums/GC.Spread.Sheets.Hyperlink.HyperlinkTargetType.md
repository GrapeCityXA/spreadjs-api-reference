# Enumeration: HyperlinkTargetType

[Sheets](../modules/GC.Spread.Sheets.md).[Hyperlink](../modules/GC.Spread.Sheets.Hyperlink.md).HyperlinkTargetType

用户打开超链接文档的方式默认是空白

**`代码示例`**
```
//本示例使用HyperlinkTargetType
sheet.setHyperlink(1, 1, {
   url: 'https://www.grapecity.com/spreadjs',
   tooltip: 'baidu',
   target: GC.Spread.Sheets.Hyperlink.HyperlinkTargetType.top,
}, GC.Spread.Sheets.SheetArea.viewport);
```

## Table of contents

### Enumeration members

- [blank](GC.Spread.Sheets.Hyperlink.HyperlinkTargetType.md#blank)
- [parent](GC.Spread.Sheets.Hyperlink.HyperlinkTargetType.md#parent)
- [self](GC.Spread.Sheets.Hyperlink.HyperlinkTargetType.md#self)
- [top](GC.Spread.Sheets.Hyperlink.HyperlinkTargetType.md#top)

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
