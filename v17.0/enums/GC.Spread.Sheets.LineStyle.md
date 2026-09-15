# Enumeration: LineStyle

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).LineStyle

边框的线条绘制样式

**`代码示例`**
```
//本示例创建一个边框
var border = new GC.Spread.Sheets.LineBorder
border.color = "#7FFFD4";
border.style = GC.Spread.Sheets.LineStyle.double;
var cell = activeSheet.getCell(1, 1, GC.Spread.Sheets.SheetArea.viewport);
cell.borderLeft(border);
```

## Table of contents

### Enumeration members

- [dashDot](GC.Spread.Sheets.LineStyle.md#dashdot)
- [dashDotDot](GC.Spread.Sheets.LineStyle.md#dashdotdot)
- [dashed](GC.Spread.Sheets.LineStyle.md#dashed)
- [dotted](GC.Spread.Sheets.LineStyle.md#dotted)
- [double](GC.Spread.Sheets.LineStyle.md#double)
- [empty](GC.Spread.Sheets.LineStyle.md#empty)
- [hair](GC.Spread.Sheets.LineStyle.md#hair)
- [medium](GC.Spread.Sheets.LineStyle.md#medium)
- [mediumDashDot](GC.Spread.Sheets.LineStyle.md#mediumdashdot)
- [mediumDashDotDot](GC.Spread.Sheets.LineStyle.md#mediumdashdotdot)
- [mediumDashed](GC.Spread.Sheets.LineStyle.md#mediumdashed)
- [slantedDashDot](GC.Spread.Sheets.LineStyle.md#slanteddashdot)
- [thick](GC.Spread.Sheets.LineStyle.md#thick)
- [thin](GC.Spread.Sheets.LineStyle.md#thin)

## Enumeration members

### <a id="dashdot" name="dashdot"></a> dashDot

• **dashDot** = `9`

 带点划线的边框线

___

### <a id="dashdotdot" name="dashdotdot"></a> dashDotDot

• **dashDotDot** = `11`

 带点划线的边框线

___

### <a id="dashed" name="dashed"></a> dashed

• **dashed** = `3`

 用虚线表示边框线

___

### <a id="dotted" name="dotted"></a> dotted

• **dotted** = `4`

 带点的边框

___

### <a id="double" name="double"></a> double

• **double** = `6`

 双边框线

___

### <a id="empty" name="empty"></a> empty

• **empty** = `0`

没有样式的边框线

___

### <a id="hair" name="hair"></a> hair

• **hair** = `7`

 用点组成的边框线

___

### <a id="medium" name="medium"></a> medium

• **medium** = `2`

 用实线表示中边框线

___

### <a id="mediumdashdot" name="mediumdashdot"></a> mediumDashDot

• **mediumDashDot** = `10`

 带点划线的中等边框线

___

### <a id="mediumdashdotdot" name="mediumdashdotdot"></a> mediumDashDotDot

• **mediumDashDotDot** = `12`

 带点划线的中等边框线

___

### <a id="mediumdashed" name="mediumdashed"></a> mediumDashed

• **mediumDashed** = `8`

 带虚线的中等边框线

___

### <a id="slanteddashdot" name="slanteddashdot"></a> slantedDashDot

• **slantedDashDot** = `13`

 带点划线的倾斜边框线

___

### <a id="thick" name="thick"></a> thick

• **thick** = `5`

 用实线表示粗边框线

___

### <a id="thin" name="thin"></a> thin

• **thin** = `1`

 带有实线的边框线
