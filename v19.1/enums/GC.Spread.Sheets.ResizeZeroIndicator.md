# Enumeration: ResizeZeroIndicator

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).ResizeZeroIndicator

指定当行或列调整到零宽度或高度时绘制策略。

**`example`**
```javascript
//此示例展示当行或列调整到零宽度或高度时绘制策略。
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

使用当前绘制策略当行或列调整到零宽度或高度时。

___

### <a id="enhanced" name="enhanced"></a> enhanced

• **enhanced** = `1`

当行或列调整到零宽度或高度时绘制两条短线条。
