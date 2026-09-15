# Interface: IPlotConfigOption

[Sheets](../modules/GC.Spread.Sheets.md).[DataCharts](../modules/GC.Spread.Sheets.DataCharts.md).IPlotConfigOption

## Table of contents

### Properties

- [funnel](GC.Spread.Sheets.DataCharts.IPlotConfigOption.md#funnel)
- [hoverAnimation](GC.Spread.Sheets.DataCharts.IPlotConfigOption.md#hoveranimation)
- [hoverStyle](GC.Spread.Sheets.DataCharts.IPlotConfigOption.md#hoverstyle)
- [innerRadius](GC.Spread.Sheets.DataCharts.IPlotConfigOption.md#innerradius)
- [lineAspect](GC.Spread.Sheets.DataCharts.IPlotConfigOption.md#lineaspect)
- [outerRadius](GC.Spread.Sheets.DataCharts.IPlotConfigOption.md#outerradius)
- [palette](GC.Spread.Sheets.DataCharts.IPlotConfigOption.md#palette)
- [startAngle](GC.Spread.Sheets.DataCharts.IPlotConfigOption.md#startangle)
- [style](GC.Spread.Sheets.DataCharts.IPlotConfigOption.md#style)
- [swapAxes](GC.Spread.Sheets.DataCharts.IPlotConfigOption.md#swapaxes)
- [sweep](GC.Spread.Sheets.DataCharts.IPlotConfigOption.md#sweep)
- [symbols](GC.Spread.Sheets.DataCharts.IPlotConfigOption.md#symbols)
- [text](GC.Spread.Sheets.DataCharts.IPlotConfigOption.md#text)
- [tooltip](GC.Spread.Sheets.DataCharts.IPlotConfigOption.md#tooltip)
- [treemap](GC.Spread.Sheets.DataCharts.IPlotConfigOption.md#treemap)
- [updateAnimation](GC.Spread.Sheets.DataCharts.IPlotConfigOption.md#updateanimation)
- [waterfall](GC.Spread.Sheets.DataCharts.IPlotConfigOption.md#waterfall)

## Properties

### <a id="funnel" name="funnel"></a> funnel

• `Optional` **funnel**: [`IFunnelOption`](GC.Spread.Sheets.DataCharts.IFunnelOption.md)

___

### <a id="hoveranimation" name="hoveranimation"></a> hoverAnimation

• `Optional` **hoverAnimation**: [`IAnimationOption`](GC.Spread.Sheets.DataCharts.IAnimationOption.md)

___

### <a id="hoverstyle" name="hoverstyle"></a> hoverStyle

• `Optional` **hoverStyle**: [`IDataPointStyleOption`](GC.Spread.Sheets.DataCharts.IDataPointStyleOption.md)

___

### <a id="innerradius" name="innerradius"></a> innerRadius

• `Optional` **innerRadius**: `number`

___

### <a id="lineaspect" name="lineaspect"></a> lineAspect

• `Optional` **lineAspect**: [`LineAspect`](../enums/GC.Spread.Sheets.DataCharts.LineAspect.md)

___

### <a id="outerradius" name="outerradius"></a> outerRadius

• `Optional` **outerRadius**: `number`

___

### <a id="palette" name="palette"></a> palette

• `Optional` **palette**: `string`[]

___

### <a id="startangle" name="startangle"></a> startAngle

• `Optional` **startAngle**: `number`

___

### <a id="style" name="style"></a> style

• `Optional` **style**: [`IDataPointStyleOption`](GC.Spread.Sheets.DataCharts.IDataPointStyleOption.md)

___

### <a id="swapaxes" name="swapaxes"></a> swapAxes

• `Optional` **swapAxes**: `boolean`

**`deprecated`** 坐标轴方向由图表绘图区的 `type` 属性定义，请不要依赖 `swapAxes` 属性。为保证兼容性，较新版本的渲染器将会忽略 `swapAxes` 属性。

___

### <a id="sweep" name="sweep"></a> sweep

• `Optional` **sweep**: `number`

___

### <a id="symbols" name="symbols"></a> symbols

• `Optional` **symbols**: `boolean`

___

### <a id="text" name="text"></a> text

• `Optional` **text**: [`IPlotConfigTextOption`](GC.Spread.Sheets.DataCharts.IPlotConfigTextOption.md)[]

___

### <a id="tooltip" name="tooltip"></a> tooltip

• `Optional` **tooltip**: [`IPlotConfigTooltipOption`](GC.Spread.Sheets.DataCharts.IPlotConfigTooltipOption.md)[]

___

### <a id="treemap" name="treemap"></a> treemap

• `Optional` **treemap**: [`ITreemapOption`](GC.Spread.Sheets.DataCharts.ITreemapOption.md)

___

### <a id="updateanimation" name="updateanimation"></a> updateAnimation

• `Optional` **updateAnimation**: [`IAnimationOption`](GC.Spread.Sheets.DataCharts.IAnimationOption.md)

___

### <a id="waterfall" name="waterfall"></a> waterfall

• `Optional` **waterfall**: [`IWaterfallOption`](GC.Spread.Sheets.DataCharts.IWaterfallOption.md)
