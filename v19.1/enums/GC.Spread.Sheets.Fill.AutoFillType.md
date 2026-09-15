# Enumeration: AutoFillType

[Sheets](../modules/GC.Spread.Sheets.md).[Fill](../modules/GC.Spread.Sheets.Fill.md).AutoFillType

表示拖拽填充的类型。

**`example`**
```javascript
//此示例使用 AutoFillType 枚举。
console.log(spread.options.defaultDragFillType); // 等于 GC.Spread.Sheets.Fill.AutoFillType.auto
spread.options.defaultDragFillType = GC.Spread.Sheets.Fill.AutoFillType.copyCells;
```

## Table of contents

### Enumeration members

- [auto](GC.Spread.Sheets.Fill.AutoFillType.md#auto)
- [clearValues](GC.Spread.Sheets.Fill.AutoFillType.md#clearvalues)
- [copyCells](GC.Spread.Sheets.Fill.AutoFillType.md#copycells)
- [fillFormattingOnly](GC.Spread.Sheets.Fill.AutoFillType.md#fillformattingonly)
- [fillSeries](GC.Spread.Sheets.Fill.AutoFillType.md#fillseries)
- [fillWithoutFormatting](GC.Spread.Sheets.Fill.AutoFillType.md#fillwithoutformatting)

## Enumeration members

### <a id="auto" name="auto"></a> auto

• **auto** = `5`

自动填充单元格。

___

### <a id="clearvalues" name="clearvalues"></a> clearValues

• **clearValues** = `4`

清除单元格值。

___

### <a id="copycells" name="copycells"></a> copyCells

• **copyCells** = `0`

使用所有数据对象填充单元格，包括值、格式和公式。

___

### <a id="fillformattingonly" name="fillformattingonly"></a> fillFormattingOnly

• **fillFormattingOnly** = `2`

仅使用格式填充单元格。

___

### <a id="fillseries" name="fillseries"></a> fillSeries

• **fillSeries** = `1`

使用序列填充单元格。

___

### <a id="fillwithoutformatting" name="fillwithoutformatting"></a> fillWithoutFormatting

• **fillWithoutFormatting** = `3`

使用值填充单元格，不使用格式。
