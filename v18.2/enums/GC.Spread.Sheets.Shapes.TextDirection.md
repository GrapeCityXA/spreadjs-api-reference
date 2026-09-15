# Enumeration: TextDirection

[Sheets](../modules/GC.Spread.Sheets.md).[Shapes](../modules/GC.Spread.Sheets.Shapes.md).TextDirection

定义形状的文本方向。

**`example`**
```
// 此示例为形状设置文本方向。
var rectangleShape = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 100, 60, 200, 160);
var oldStyle = rectangleShape.style();
oldStyle.textFrame.textDirection = GC.Spread.Sheets.Shapes.TextDirection.wordArtVertRtl;
rectangleShape.style(oldStyle);
```

## Table of contents

### Enumeration members

- [eaVert](GC.Spread.Sheets.Shapes.TextDirection.md#eavert)
- [eaVertLtr](GC.Spread.Sheets.Shapes.TextDirection.md#eavertltr)
- [horz](GC.Spread.Sheets.Shapes.TextDirection.md#horz)
- [vert](GC.Spread.Sheets.Shapes.TextDirection.md#vert)
- [vert270](GC.Spread.Sheets.Shapes.TextDirection.md#vert270)
- [wordArtVert](GC.Spread.Sheets.Shapes.TextDirection.md#wordartvert)
- [wordArtVertRtl](GC.Spread.Sheets.Shapes.TextDirection.md#wordartvertrtl)

## Enumeration members

### <a id="eavert" name="eavert"></a> eaVert

• **eaVert** = `4`

指定文本以东亚垂直从右到左显示。

___

### <a id="eavertltr" name="eavertltr"></a> eaVertLtr

• **eaVertLtr** = `5`

指定文本以东亚垂直从左到右显示。

___

### <a id="horz" name="horz"></a> horz

• **horz** = `0`

指定文本水平显示。

___

### <a id="vert" name="vert"></a> vert

• **vert** = `1`

指定文本垂直90度显示。

___

### <a id="vert270" name="vert270"></a> vert270

• **vert270** = `2`

指定文本垂直270度显示。

___

### <a id="wordartvert" name="wordartvert"></a> wordArtVert

• **wordArtVert** = `3`

指定文本以艺术字垂直从左到右显示。

___

### <a id="wordartvertrtl" name="wordartvertrtl"></a> wordArtVertRtl

• **wordArtVertRtl** = `6`

指定文本以艺术字垂直从右到左显示。
