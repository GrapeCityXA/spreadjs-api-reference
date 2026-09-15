# Enumeration: HorizontalAlign

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).HorizontalAlign

水平对齐

**`代码示例`**
```
//本例使用的是HorizontalAlign类型
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

 单元格内容居中

___

### <a id="centercontinuous" name="centercontinuous"></a> centerContinuous

• **centerContinuous** = `4`

 单元格内容跨列居中

___

### <a id="distributed" name="distributed"></a> distributed

• **distributed** = `5`

指示单元格内每行文本的每个“单词”均匀分布在单元格的宽度上，并在左右两侧对齐

___

### <a id="general" name="general"></a> general

• **general** = `3`

 水平对齐基于值类型

___

### <a id="left" name="left"></a> left

• **left** = `0`

 单元格内容左对齐

___

### <a id="right" name="right"></a> right

• **right** = `2`

 单元格内容右对齐
