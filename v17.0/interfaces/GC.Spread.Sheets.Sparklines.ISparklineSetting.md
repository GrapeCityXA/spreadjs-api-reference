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

the color of the axis

___

### <a id="displayemptycellsas" name="displayemptycellsas"></a> displayEmptyCellsAs

• `Optional` **displayEmptyCellsAs**: [`EmptyValueStyle`](../enums/GC.Spread.Sheets.Sparklines.EmptyValueStyle.md)

Indicates how to display the empty cells

___

### <a id="displayhidden" name="displayhidden"></a> displayHidden

• `Optional` **displayHidden**: `boolean`

Indicates whether data in hidden cells is plotted for the sparklines in this sparkline group

___

### <a id="displayxaxis" name="displayxaxis"></a> displayXAxis

• `Optional` **displayXAxis**: `boolean`

Indicates whether the horizontal axis is displayed for each sparkline in this sparkline group

___

### <a id="firstmarkercolor" name="firstmarkercolor"></a> firstMarkerColor

• `Optional` **firstMarkerColor**: `string`

the color of the first data point for each sparkline in this sparkline group

___

### <a id="groupmaxvalue" name="groupmaxvalue"></a> groupMaxValue

• `Optional` **groupMaxValue**: `number`

Gets the maximum value of the sparkline group

___

### <a id="groupminvalue" name="groupminvalue"></a> groupMinValue

• `Optional` **groupMinValue**: `number`

Gets the minimum value of the sparkline group

___

### <a id="highmarkercolor" name="highmarkercolor"></a> highMarkerColor

• `Optional` **highMarkerColor**: `string`

the color of the highest data point for each sparkline in this sparkline group

___

### <a id="lastmarkercolor" name="lastmarkercolor"></a> lastMarkerColor

• `Optional` **lastMarkerColor**: `string`

the color of the last data point for each sparkline in this sparkline group

___

### <a id="lineweight" name="lineweight"></a> lineWeight

• `Optional` **lineWeight**: `number`

Indicates the line weight for each sparkline in the sparkline group, where the line weight is measured in points. The weight must be greater than or equal to zero, and must be less than or equal to 3 (LineSeries only supports line weight values in the range of 0.0-3.0)

___

### <a id="lowmarkercolor" name="lowmarkercolor"></a> lowMarkerColor

• `Optional` **lowMarkerColor**: `string`

the color of the lowest data point for each sparkline in this sparkline group

___

### <a id="manualmax" name="manualmax"></a> manualMax

• `Optional` **manualMax**: `number`

Indicates the maximum for the vertical axis that is shared across all sparklines in this sparkline group. The axis is zero if maxAxisType does not equal custom

___

### <a id="manualmin" name="manualmin"></a> manualMin

• `Optional` **manualMin**: `number`

Indicates the minimum for the vertical axis that is shared across all sparklines in this sparkline group. The axis is zero if minAxisType does not equal custom

___

### <a id="markerscolor" name="markerscolor"></a> markersColor

• `Optional` **markersColor**: `string`

a value that specifies the color of the data markers for each sparkline in this sparkline group

___

### <a id="maxaxistype" name="maxaxistype"></a> maxAxisType

• `Optional` **maxAxisType**: [`SparklineAxisMinMax`](../enums/GC.Spread.Sheets.Sparklines.SparklineAxisMinMax.md)

Indicates how the vertical axis maximum is calculated for the sparklines in this sparkline group

___

### <a id="minaxistype" name="minaxistype"></a> minAxisType

• `Optional` **minAxisType**: [`SparklineAxisMinMax`](../enums/GC.Spread.Sheets.Sparklines.SparklineAxisMinMax.md)

Indicates how the vertical axis minimum is calculated for the sparklines in this sparkline group

___

### <a id="negativecolor" name="negativecolor"></a> negativeColor

• `Optional` **negativeColor**: `string`

a value that specifies the color of the negative data points for each sparkline in this sparkline group

___

### <a id="righttoleft" name="righttoleft"></a> rightToLeft

• `Optional` **rightToLeft**: `boolean`

Indicates whether each sparkline in the sparkline group is displayed in a right-to-left manner

___

### <a id="seriescolor" name="seriescolor"></a> seriesColor

• `Optional` **seriesColor**: `string`

a value that specifies the color for each sparkline in this sparkline group

___

### <a id="showfirst" name="showfirst"></a> showFirst

• `Optional` **showFirst**: `boolean`

a value that indicates whether the first data point is formatted differently for each sparkline in this sparkline group

___

### <a id="showhigh" name="showhigh"></a> showHigh

• `Optional` **showHigh**: `boolean`

a value that specifies whether the data points with the highest value are formatted differently for each sparkline in this sparkline group

___

### <a id="showlast" name="showlast"></a> showLast

• `Optional` **showLast**: `boolean`

a value that indicates whether the last data point is formatted differently for each sparkline in this sparkline group

___

### <a id="showlow" name="showlow"></a> showLow

• `Optional` **showLow**: `boolean`

a value that specifies whether the data points with the lowest value are formatted differently for each sparkline in this sparkline group

___

### <a id="showmarkers" name="showmarkers"></a> showMarkers

• `Optional` **showMarkers**: `boolean`

a value that specifies whether data markers are displayed for each sparkline in this sparkline group

___

### <a id="shownegative" name="shownegative"></a> showNegative

• `Optional` **showNegative**: `boolean`

a value that specifies whether the negative data points are formatted differently for each sparkline in this sparkline group
