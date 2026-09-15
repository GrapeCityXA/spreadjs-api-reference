# Interface: IAxis

[Sheets](../modules/GC.Spread.Sheets.md).[Charts](../modules/GC.Spread.Sheets.Charts.md).IAxis

## Table of contents

### Properties

- [baseUnit](GC.Spread.Sheets.Charts.IAxis.md#baseunit)
- [crossPoint](GC.Spread.Sheets.Charts.IAxis.md#crosspoint)
- [displayUnit](GC.Spread.Sheets.Charts.IAxis.md#displayunit)
- [format](GC.Spread.Sheets.Charts.IAxis.md#format)
- [labelAngle](GC.Spread.Sheets.Charts.IAxis.md#labelangle)
- [lineStyle](GC.Spread.Sheets.Charts.IAxis.md#linestyle)
- [majorGridLine](GC.Spread.Sheets.Charts.IAxis.md#majorgridline)
- [majorTickPosition](GC.Spread.Sheets.Charts.IAxis.md#majortickposition)
- [majorUnit](GC.Spread.Sheets.Charts.IAxis.md#majorunit)
- [majorUnitScale](GC.Spread.Sheets.Charts.IAxis.md#majorunitscale)
- [max](GC.Spread.Sheets.Charts.IAxis.md#max)
- [min](GC.Spread.Sheets.Charts.IAxis.md#min)
- [minorGridLine](GC.Spread.Sheets.Charts.IAxis.md#minorgridline)
- [minorTickPosition](GC.Spread.Sheets.Charts.IAxis.md#minortickposition)
- [minorUnit](GC.Spread.Sheets.Charts.IAxis.md#minorunit)
- [minorUnitScale](GC.Spread.Sheets.Charts.IAxis.md#minorunitscale)
- [numberFormatLinked](GC.Spread.Sheets.Charts.IAxis.md#numberformatlinked)
- [scaling](GC.Spread.Sheets.Charts.IAxis.md#scaling)
- [style](GC.Spread.Sheets.Charts.IAxis.md#style)
- [tickLabelPosition](GC.Spread.Sheets.Charts.IAxis.md#ticklabelposition)
- [tickLabelSpacing](GC.Spread.Sheets.Charts.IAxis.md#ticklabelspacing)
- [title](GC.Spread.Sheets.Charts.IAxis.md#title)
- [visible](GC.Spread.Sheets.Charts.IAxis.md#visible)

## Properties

### <a id="baseunit" name="baseunit"></a> baseUnit

• `Optional` **baseUnit**: [`TimeUnit`](../enums/GC.Spread.Sheets.Charts.TimeUnit.md)

日期分类轴的基础单位刻度。

___

### <a id="crosspoint" name="crosspoint"></a> crossPoint

• `Optional` **crossPoint**: `number` \| [`AxisCrossPoint`](../enums/GC.Spread.Sheets.Charts.AxisCrossPoint.md)

指示轴的交叉值。

___

### <a id="displayunit" name="displayunit"></a> displayUnit

• `Optional` **displayUnit**: [`IDisplayUnit`](GC.Spread.Sheets.Charts.IDisplayUnit.md)

轴的显示单位信息。

___

### <a id="format" name="format"></a> format

• `Optional` **format**: `string`

轴的格式。

___

### <a id="labelangle" name="labelangle"></a> labelAngle

• `Optional` **labelAngle**: `number`

轴的标签角度。

___

### <a id="linestyle" name="linestyle"></a> lineStyle

• `Optional` **lineStyle**: [`IBorder`](GC.Spread.Sheets.Charts.IBorder.md)

轴线样式。

___

### <a id="majorgridline" name="majorgridline"></a> majorGridLine

• `Optional` **majorGridLine**: [`IGridLine`](GC.Spread.Sheets.Charts.IGridLine.md)

轴的主网格线。

___

### <a id="majortickposition" name="majortickposition"></a> majorTickPosition

• `Optional` **majorTickPosition**: [`TickMark`](../enums/GC.Spread.Sheets.Charts.TickMark.md)

轴主刻度位置。

___

### <a id="majorunit" name="majorunit"></a> majorUnit

• `Optional` **majorUnit**: `number`

主分类轴的主要单位刻度。

___

### <a id="majorunitscale" name="majorunitscale"></a> majorUnitScale

• `Optional` **majorUnitScale**: [`TimeUnit`](../enums/GC.Spread.Sheets.Charts.TimeUnit.md)

日期分类轴的主要单位刻度。

___

### <a id="max" name="max"></a> max

• `Optional` **max**: `number` \| `Date`

相关轴的最大值。（仅适用于值/日期轴）

___

### <a id="min" name="min"></a> min

• `Optional` **min**: `number` \| `Date`

相关轴的最小值。（仅适用于值/日期轴）

___

### <a id="minorgridline" name="minorgridline"></a> minorGridLine

• `Optional` **minorGridLine**: [`IGridLine`](GC.Spread.Sheets.Charts.IGridLine.md)

轴的次网格线。

___

### <a id="minortickposition" name="minortickposition"></a> minorTickPosition

• `Optional` **minorTickPosition**: [`TickMark`](../enums/GC.Spread.Sheets.Charts.TickMark.md)

轴次刻度位置。

___

### <a id="minorunit" name="minorunit"></a> minorUnit

• `Optional` **minorUnit**: `number`

主分类轴的次要单位刻度。

___

### <a id="minorunitscale" name="minorunitscale"></a> minorUnitScale

• `Optional` **minorUnitScale**: [`TimeUnit`](../enums/GC.Spread.Sheets.Charts.TimeUnit.md)

日期分类轴的次要单位刻度。

___

### <a id="numberformatlinked" name="numberformatlinked"></a> numberFormatLinked

• `Optional` **numberFormatLinked**: `boolean`

是否应用链接数据源的格式。

___

### <a id="scaling" name="scaling"></a> scaling

• `Optional` **scaling**: [`IScaling`](GC.Spread.Sheets.Charts.IScaling.md)

轴的缩放信息。

___

### <a id="style" name="style"></a> style

• `Optional` **style**: [`IAxisStyle`](GC.Spread.Sheets.Charts.IAxisStyle.md)

轴样式。

___

### <a id="ticklabelposition" name="ticklabelposition"></a> tickLabelPosition

• `Optional` **tickLabelPosition**: [`TickLabelPosition`](../enums/GC.Spread.Sheets.Charts.TickLabelPosition.md)

轴刻度标签位置。

___

### <a id="ticklabelspacing" name="ticklabelspacing"></a> tickLabelSpacing

• `Optional` **tickLabelSpacing**: `number`

轴刻度标签间距。

___

### <a id="title" name="title"></a> title

• `Optional` **title**: [`IAxisTitle`](GC.Spread.Sheets.Charts.IAxisTitle.md)

轴的标题。

___

### <a id="visible" name="visible"></a> visible

• `Optional` **visible**: `boolean`

指定轴是否显示。
