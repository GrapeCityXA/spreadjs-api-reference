# Interface: ISparklineSetting

[Sheets](../modules/GC.Spread.Sheets.md).[Sparklines](../modules/GC.Spread.Sheets.Sparklines.md).ISparklineSetting

## Table of contents

### Properties

- [axisColor](GC.Spread.Sheets.Sparklines.ISparklineSetting.md#axiscolor)
- [displayEmptyCellsAs](GC.Spread.Sheets.Sparklines.ISparklineSetting.md#displayemptycellsas)
- [displayHidden](GC.Spread.Sheets.Sparklines.ISparklineSetting.md#displayhidden)
- [displayXAxis](GC.Spread.Sheets.Sparklines.ISparklineSetting.md#displayxaxis)
- [firstMarkerColor](GC.Spread.Sheets.Sparklines.ISparklineSetting.md#firstmarkercolor)
- [groupMaxValue](GC.Spread.Sheets.Sparklines.ISparklineSetting.md#groupmaxvalue)
- [groupMinValue](GC.Spread.Sheets.Sparklines.ISparklineSetting.md#groupminvalue)
- [highMarkerColor](GC.Spread.Sheets.Sparklines.ISparklineSetting.md#highmarkercolor)
- [lastMarkerColor](GC.Spread.Sheets.Sparklines.ISparklineSetting.md#lastmarkercolor)
- [lineWeight](GC.Spread.Sheets.Sparklines.ISparklineSetting.md#lineweight)
- [lowMarkerColor](GC.Spread.Sheets.Sparklines.ISparklineSetting.md#lowmarkercolor)
- [manualMax](GC.Spread.Sheets.Sparklines.ISparklineSetting.md#manualmax)
- [manualMin](GC.Spread.Sheets.Sparklines.ISparklineSetting.md#manualmin)
- [markersColor](GC.Spread.Sheets.Sparklines.ISparklineSetting.md#markerscolor)
- [maxAxisType](GC.Spread.Sheets.Sparklines.ISparklineSetting.md#maxaxistype)
- [minAxisType](GC.Spread.Sheets.Sparklines.ISparklineSetting.md#minaxistype)
- [negativeColor](GC.Spread.Sheets.Sparklines.ISparklineSetting.md#negativecolor)
- [rightToLeft](GC.Spread.Sheets.Sparklines.ISparklineSetting.md#righttoleft)
- [seriesColor](GC.Spread.Sheets.Sparklines.ISparklineSetting.md#seriescolor)
- [showFirst](GC.Spread.Sheets.Sparklines.ISparklineSetting.md#showfirst)
- [showHigh](GC.Spread.Sheets.Sparklines.ISparklineSetting.md#showhigh)
- [showLast](GC.Spread.Sheets.Sparklines.ISparklineSetting.md#showlast)
- [showLow](GC.Spread.Sheets.Sparklines.ISparklineSetting.md#showlow)
- [showMarkers](GC.Spread.Sheets.Sparklines.ISparklineSetting.md#showmarkers)
- [showNegative](GC.Spread.Sheets.Sparklines.ISparklineSetting.md#shownegative)

## Properties

### <a id="axiscolor" name="axiscolor"></a> axisColor

• `Optional` **axisColor**: `string`

轴线的颜色

___

### <a id="displayemptycellsas" name="displayemptycellsas"></a> displayEmptyCellsAs

• `Optional` **displayEmptyCellsAs**: [`EmptyValueStyle`](../enums/GC.Spread.Sheets.Sparklines.EmptyValueStyle.md)

指示如何显示空单元格

___

### <a id="displayhidden" name="displayhidden"></a> displayHidden

• `Optional` **displayHidden**: `boolean`

指示是否为此迷你图组中的迷你图绘制隐藏单元格中的数据

___

### <a id="displayxaxis" name="displayxaxis"></a> displayXAxis

• `Optional` **displayXAxis**: `boolean`

指示是否为此迷你图组中的每个迷你图显示水平轴

___

### <a id="firstmarkercolor" name="firstmarkercolor"></a> firstMarkerColor

• `Optional` **firstMarkerColor**: `string`

此迷你图组中每个迷你图的第一个数据点的颜色

___

### <a id="groupmaxvalue" name="groupmaxvalue"></a> groupMaxValue

• `Optional` **groupMaxValue**: `number`

获取迷你图组的最大值

___

### <a id="groupminvalue" name="groupminvalue"></a> groupMinValue

• `Optional` **groupMinValue**: `number`

获取迷你图组的最小值

___

### <a id="highmarkercolor" name="highmarkercolor"></a> highMarkerColor

• `Optional` **highMarkerColor**: `string`

此迷你图组中每个迷你图的最高数据点的颜色

___

### <a id="lastmarkercolor" name="lastmarkercolor"></a> lastMarkerColor

• `Optional` **lastMarkerColor**: `string`

此迷你图组中每个迷你图的最后一个数据点的颜色

___

### <a id="lineweight" name="lineweight"></a> lineWeight

• `Optional` **lineWeight**: `number`

指示迷你图组中每个迷你图的线条粗细，以磅为单位。粗细必须大于或等于零，且必须小于或等于3（LineSeries仅支持0.0-3.0范围内的线条粗细值）

___

### <a id="lowmarkercolor" name="lowmarkercolor"></a> lowMarkerColor

• `Optional` **lowMarkerColor**: `string`

此迷你图组中每个迷你图的最低数据点的颜色

___

### <a id="manualmax" name="manualmax"></a> manualMax

• `Optional` **manualMax**: `number`

指示此迷你图组中所有迷你图共享的垂直轴的最大值。如果maxAxisType不等于custom，则轴为零

___

### <a id="manualmin" name="manualmin"></a> manualMin

• `Optional` **manualMin**: `number`

指示此迷你图组中所有迷你图共享的垂直轴的最小值。如果minAxisType不等于custom，则轴为零

___

### <a id="markerscolor" name="markerscolor"></a> markersColor

• `Optional` **markersColor**: `string`

指定此迷你图组中每个迷你图的数据标记的颜色

___

### <a id="maxaxistype" name="maxaxistype"></a> maxAxisType

• `Optional` **maxAxisType**: [`SparklineAxisMinMax`](../enums/GC.Spread.Sheets.Sparklines.SparklineAxisMinMax.md)

指示如何计算此迷你图组中迷你图的垂直轴最大值

___

### <a id="minaxistype" name="minaxistype"></a> minAxisType

• `Optional` **minAxisType**: [`SparklineAxisMinMax`](../enums/GC.Spread.Sheets.Sparklines.SparklineAxisMinMax.md)

指示如何计算此迷你图组中迷你图的垂直轴最小值

___

### <a id="negativecolor" name="negativecolor"></a> negativeColor

• `Optional` **negativeColor**: `string`

指定此迷你图组中每个迷你图的负数据点的颜色

___

### <a id="righttoleft" name="righttoleft"></a> rightToLeft

• `Optional` **rightToLeft**: `boolean`

指示迷你图组中的每个迷你图是否以从右到左的方式显示

___

### <a id="seriescolor" name="seriescolor"></a> seriesColor

• `Optional` **seriesColor**: `string`

指定此迷你图组中每个迷你图的颜色

___

### <a id="showfirst" name="showfirst"></a> showFirst

• `Optional` **showFirst**: `boolean`

指示是否为此迷你图组中的每个迷你图以不同方式格式化第一个数据点

___

### <a id="showhigh" name="showhigh"></a> showHigh

• `Optional` **showHigh**: `boolean`

指示是否为此迷你图组中的每个迷你图以不同方式格式化具有最高值的数据点

___

### <a id="showlast" name="showlast"></a> showLast

• `Optional` **showLast**: `boolean`

指示是否为此迷你图组中的每个迷你图以不同方式格式化最后一个数据点

___

### <a id="showlow" name="showlow"></a> showLow

• `Optional` **showLow**: `boolean`

指示是否为此迷你图组中的每个迷你图以不同方式格式化具有最低值的数据点

___

### <a id="showmarkers" name="showmarkers"></a> showMarkers

• `Optional` **showMarkers**: `boolean`

指示是否为此迷你图组中的每个迷你图显示数据标记

___

### <a id="shownegative" name="shownegative"></a> showNegative

• `Optional` **showNegative**: `boolean`

指示是否为此迷你图组中的每个迷你图以不同方式格式化负数据点
