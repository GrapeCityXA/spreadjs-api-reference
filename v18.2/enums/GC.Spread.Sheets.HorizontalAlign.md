# Enumeration: HorizontalAlign

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).HorizontalAlign

指定水平对齐方式。

**`example`**
```
//此示例使用HorizontalAlign类型。
var style = new GC.Spread.Sheets.Style();
style.font = "8pt Arial";
style.hAlign = GC.Spread.Sheets.HorizontalAlign.center;
style.vAlign = GC.Spread.Sheets.VerticalAlign.center;
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(1,1).value("B2");
```

## Table of contents

### Enumeration members

- [center](GC.Spread.Sheets.HorizontalAlign.md#center)
- [centerContinuous](GC.Spread.Sheets.HorizontalAlign.md#centercontinuous)
- [distributed](GC.Spread.Sheets.HorizontalAlign.md#distributed)
- [general](GC.Spread.Sheets.HorizontalAlign.md#general)
- [left](GC.Spread.Sheets.HorizontalAlign.md#left)
- [right](GC.Spread.Sheets.HorizontalAlign.md#right)

## Enumeration members

### <a id="center" name="center"></a> center

• **center** = `1`

表示单元格内容居中对齐。

___

### <a id="centercontinuous" name="centercontinuous"></a> centerContinuous

• **centerContinuous** = `4`

表示单元格内容在选定范围内居中。

___

### <a id="distributed" name="distributed"></a> distributed

• **distributed** = `5`

表示单元格内每行文本中的每个"单词"均匀分布在单元格宽度上，左右边距对齐。

___

### <a id="general" name="general"></a> general

• **general** = `3`

表示水平对齐方式基于值类型。

___

### <a id="left" name="left"></a> left

• **left** = `0`

表示单元格内容左对齐。

___

### <a id="right" name="right"></a> right

• **right** = `2`

表示单元格内容右对齐。
