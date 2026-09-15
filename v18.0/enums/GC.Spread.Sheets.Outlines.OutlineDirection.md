# Enumeration: OutlineDirection

[Sheets](../modules/GC.Spread.Sheets.md).[Outlines](../modules/GC.Spread.Sheets.Outlines.md).OutlineDirection

行区域分组或列区域分组位置

**`代码示例`**
``` javascript
sheet.suspendPaint();
sheet.rowOutlines.group(3,2);
sheet.columnOutlines.group(4,1);
sheet.rowOutlines.direction(GC.Spread.Sheets.Outlines.OutlineDirection.backward);
sheet.columnOutlines.direction(GC.Spread.Sheets.Outlines.OutlineDirection.forward);
sheet.resumePaint();
```

## Table of contents

### Enumeration members

- [backward](GC.Spread.Sheets.Outlines.OutlineDirection.md#backward)
- [forward](GC.Spread.Sheets.Outlines.OutlineDirection.md#forward)

## Enumeration members

### <a id="backward" name="backward"></a> backward

• **backward** = `0`

摘要行位于组详细信息的上方或左侧

___

### <a id="forward" name="forward"></a> forward

• **forward** = `1`

摘要行位于组详细信息的下方或右侧
