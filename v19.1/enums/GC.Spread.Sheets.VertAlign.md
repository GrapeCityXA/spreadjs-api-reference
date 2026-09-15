# Enumeration: VertAlign

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).VertAlign

定义文本垂直对齐类型。

**`example`**
```javascript
//此示例使用VertAlign枚举。
activeSheet.setValue(1, 1, {richText:[{style:{vertAlign:GC.Spread.Sheets.VertAlign.subscript},text:'SpreadJS'}]}, GC.Spread.Sheets.SheetArea.viewport);
```

## Table of contents

### Enumeration members

- [normal](GC.Spread.Sheets.VertAlign.md#normal)
- [subscript](GC.Spread.Sheets.VertAlign.md#subscript)
- [superscript](GC.Spread.Sheets.VertAlign.md#superscript)

## Enumeration members

### <a id="normal" name="normal"></a> normal

• **normal** = `0`

表示普通文本对齐。

___

### <a id="subscript" name="subscript"></a> subscript

• **subscript** = `2`

表示下标。

___

### <a id="superscript" name="superscript"></a> superscript

• **superscript** = `1`

表示上标。
