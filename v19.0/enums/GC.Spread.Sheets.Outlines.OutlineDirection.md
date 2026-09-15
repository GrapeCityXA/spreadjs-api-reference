# Enumeration: OutlineDirection

[Sheets](../modules/GC.Spread.Sheets.md).[Outlines](../modules/GC.Spread.Sheets.Outlines.md).OutlineDirection

指定大纲（范围组）汇总行或列的位置状态。

**`example`**
```
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

汇总行位于组详情的上方或左侧。

___

### <a id="forward" name="forward"></a> forward

• **forward** = `1`

汇总行位于组详情的下方或右侧。
