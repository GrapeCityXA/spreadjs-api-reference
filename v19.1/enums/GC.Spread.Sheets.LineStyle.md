# Enumeration: LineStyle

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).LineStyle

指定边框的线条绘制样式。

**`example`**
```javascript
//此示例创建边框。
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

表示点划线边框线。

___

### <a id="dashdotdot" name="dashdotdot"></a> dashDotDot

• **dashDotDot** = `11`

表示点点划线边框线。

___

### <a id="dashed" name="dashed"></a> dashed

• **dashed** = `3`

表示虚线边框线。

___

### <a id="dotted" name="dotted"></a> dotted

• **dotted** = `4`

表示点线边框线。

___

### <a id="double" name="double"></a> double

• **double** = `6`

表示双线边框线。

___

### <a id="empty" name="empty"></a> empty

• **empty** = `0`

表示无样式的边框线。

___

### <a id="hair" name="hair"></a> hair

• **hair** = `7`

表示全点边框线。

___

### <a id="medium" name="medium"></a> medium

• **medium** = `2`

表示实心中等粗细的边框线。

___

### <a id="mediumdashdot" name="mediumdashdot"></a> mediumDashDot

• **mediumDashDot** = `10`

表示中等粗细的点划线边框线。

___

### <a id="mediumdashdotdot" name="mediumdashdotdot"></a> mediumDashDotDot

• **mediumDashDotDot** = `12`

表示中等粗细的点点划线边框线。

___

### <a id="mediumdashed" name="mediumdashed"></a> mediumDashed

• **mediumDashed** = `8`

表示中等粗细的虚线边框线。

___

### <a id="slanteddashdot" name="slanteddashdot"></a> slantedDashDot

• **slantedDashDot** = `13`

表示斜点划线边框线。

___

### <a id="thick" name="thick"></a> thick

• **thick** = `5`

表示实心粗线边框线。

___

### <a id="thin" name="thin"></a> thin

• **thin** = `1`

表示实心细线的边框线。
