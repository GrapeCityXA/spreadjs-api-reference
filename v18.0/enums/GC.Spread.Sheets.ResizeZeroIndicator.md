# Enumeration: ResizeZeroIndicator

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).ResizeZeroIndicator

将行或列的大小调整为零时的绘制策略

**`代码示例`**
``` javascript
//本示例显示宽度或高度为零的列或行的双网格线
spread.options.resizeZeroIndicator = GC.Spread.Sheets.ResizeZeroIndicator.enhanced;
activeSheet.getRange(-1, 2, -1, 1).width(0);
activeSheet.getRange(1, -1, 1, -1).height(0);
```

## Table of contents

### Enumeration members

- [default](GC.Spread.Sheets.ResizeZeroIndicator.md#default)
- [enhanced](GC.Spread.Sheets.ResizeZeroIndicator.md#enhanced)

## Enumeration members

### <a id="default" name="default"></a> default

• **default** = `0`

 当行或列的大小调整为零时，使用当前的绘图策略

___

### <a id="enhanced" name="enhanced"></a> enhanced

• **enhanced** = `1`

当行或列的大小调整为零时，绘制两条短线
