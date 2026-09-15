# Interface: ISeries

[Sheets](../modules/GC.Spread.Sheets.md).[Charts](../modules/GC.Spread.Sheets.Charts.md).ISeries

## Table of contents

### Properties

- [axisGroup](GC.Spread.Sheets.Charts.ISeries.md#axisgroup)
- [backColor](GC.Spread.Sheets.Charts.ISeries.md#backcolor)
- [backColorTransparency](GC.Spread.Sheets.Charts.ISeries.md#backcolortransparency)
- [border](GC.Spread.Sheets.Charts.ISeries.md#border)
- [bubbleScale](GC.Spread.Sheets.Charts.ISeries.md#bubblescale)
- [bubbleSizes](GC.Spread.Sheets.Charts.ISeries.md#bubblesizes)
- [chartType](GC.Spread.Sheets.Charts.ISeries.md#charttype)
- [dataLabels](GC.Spread.Sheets.Charts.ISeries.md#datalabels)
- [dataPoints](GC.Spread.Sheets.Charts.ISeries.md#datapoints)
- [doughnutHoleSize](GC.Spread.Sheets.Charts.ISeries.md#doughnutholesize)
- [errorBars](GC.Spread.Sheets.Charts.ISeries.md#errorbars)
- [gapWidth](GC.Spread.Sheets.Charts.ISeries.md#gapwidth)
- [invertColor](GC.Spread.Sheets.Charts.ISeries.md#invertcolor)
- [invertIfNegative](GC.Spread.Sheets.Charts.ISeries.md#invertifnegative)
- [name](GC.Spread.Sheets.Charts.ISeries.md#name)
- [overlap](GC.Spread.Sheets.Charts.ISeries.md#overlap)
- [plotVisibleOnly](GC.Spread.Sheets.Charts.ISeries.md#plotvisibleonly)
- [showConnectorLines](GC.Spread.Sheets.Charts.ISeries.md#showconnectorlines)
- [smooth](GC.Spread.Sheets.Charts.ISeries.md#smooth)
- [startAngle](GC.Spread.Sheets.Charts.ISeries.md#startangle)
- [subtotals](GC.Spread.Sheets.Charts.ISeries.md#subtotals)
- [symbol](GC.Spread.Sheets.Charts.ISeries.md#symbol)
- [trendlines](GC.Spread.Sheets.Charts.ISeries.md#trendlines)
- [xValues](GC.Spread.Sheets.Charts.ISeries.md#xvalues)
- [yValues](GC.Spread.Sheets.Charts.ISeries.md#yvalues)

## Properties

### <a id="axisgroup" name="axisgroup"></a> axisGroup

• `Optional` **axisGroup**: [`AxisGroup`](../enums/GC.Spread.Sheets.Charts.AxisGroup.md)

系列轴组。

___

### <a id="backcolor" name="backcolor"></a> backColor

• `Optional` **backColor**: `string` \| [`IPatternFillBackColor`](GC.Spread.Sheets.Charts.IPatternFillBackColor.md)

系列背景颜色。

___

### <a id="backcolortransparency" name="backcolortransparency"></a> backColorTransparency

• `Optional` **backColorTransparency**: `number`

系列背景颜色的透明度。

___

### <a id="border" name="border"></a> border

• `Optional` **border**: [`ISeriesItemBorder`](GC.Spread.Sheets.Charts.ISeriesItemBorder.md)

系列边框样式。

___

### <a id="bubblescale" name="bubblescale"></a> bubbleScale

• `Optional` **bubbleScale**: `number`

气泡图的缩放因子。可以是从 0 到 300 的整数值，对应于默认大小的百分比。默认值为 100。

___

### <a id="bubblesizes" name="bubblesizes"></a> bubbleSizes

• `Optional` **bubbleSizes**: `string`

系列气泡大小公式。此参数用于气泡图。

___

### <a id="charttype" name="charttype"></a> chartType

• `Optional` **chartType**: [`ChartType`](../enums/GC.Spread.Sheets.Charts.ChartType.md)

系列图表类型。

___

### <a id="datalabels" name="datalabels"></a> dataLabels

• `Optional` **dataLabels**: [`IDataLabels`](GC.Spread.Sheets.Charts.IDataLabels.md)

系列数据标签。

___

### <a id="datapoints" name="datapoints"></a> dataPoints

• `Optional` **dataPoints**: [`IDataPoints`](GC.Spread.Sheets.Charts.IDataPoints.md)

系列数据点。

___

### <a id="doughnutholesize" name="doughnutholesize"></a> doughnutHoleSize

• `Optional` **doughnutHoleSize**: `number`

饼图的空洞大小。此参数用于饼图，最大值为 0.9，最小值为 0。

___

### <a id="errorbars" name="errorbars"></a> errorBars

• `Optional` **errorBars**: [`ErrorBarItems`](GC.Spread.Sheets.Charts.ErrorBarItems.md)

系列误差线。

___

### <a id="gapwidth" name="gapwidth"></a> gapWidth

• `Optional` **gapWidth**: `number`

柱状图或条形图组的间隙宽度。最大值为 5，最小值为 0。

___

### <a id="invertcolor" name="invertcolor"></a> invertColor

• `Optional` **invertColor**: `string`

当系列图表类型为柱状图或条形图且 invertIfNegative 为 true 时，系列点值为负的颜色。

___

### <a id="invertifnegative" name="invertifnegative"></a> invertIfNegative

• `Optional` **invertIfNegative**: `boolean`

当系列图表类型为柱状图或条形图且 invertIfNegative 为 true 时，系列点值为负的颜色。

___

### <a id="name" name="name"></a> name

• `Optional` **name**: `string`

系列名称公式。

___

### <a id="overlap" name="overlap"></a> overlap

• `Optional` **overlap**: `number`

柱状图或条形图组的堆叠重叠。最大值为 1，最小值为 -1。

___

### <a id="plotvisibleonly" name="plotvisibleonly"></a> plotVisibleOnly

• `Optional` **plotVisibleOnly**: `boolean`

是否显示隐藏行和列中的数据。

___

### <a id="showconnectorlines" name="showconnectorlines"></a> showConnectorLines

• `Optional` **showConnectorLines**: `boolean`

是否显示系列连接线。此参数用于瀑布图，默认值为 false.

___

### <a id="smooth" name="smooth"></a> smooth

• `Optional` **smooth**: `boolean`

是否显示平滑线。此参数用于折线图和散点图。

___

### <a id="startangle" name="startangle"></a> startAngle

• `Optional` **startAngle**: `number`

图表类型为饼图时，系列第一个切片的角度。默认值为 0，表示 12 点钟位置。

___

### <a id="subtotals" name="subtotals"></a> subtotals

• `Optional` **subtotals**: `number`[]

瀑布图设置为总计点索引数组（0 基）。此参数用于瀑布图，默认值为空数组。

___

### <a id="symbol" name="symbol"></a> symbol

• `Optional` **symbol**: [`ISymbol`](GC.Spread.Sheets.Charts.ISymbol.md)

系列符号。

___

### <a id="trendlines" name="trendlines"></a> trendlines

• `Optional` **trendlines**: [`TrendlineItem`](GC.Spread.Sheets.Charts.TrendlineItem.md)[]

系列趋势线。

___

### <a id="xvalues" name="xvalues"></a> xValues

• `Optional` **xValues**: `string`

系列x值公式。

___

### <a id="yvalues" name="yvalues"></a> yValues

• `Optional` **yValues**: `string`

系列y值公式。
