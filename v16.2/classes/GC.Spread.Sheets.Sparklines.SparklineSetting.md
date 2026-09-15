# Class: SparklineSetting

[Sheets](../modules/GC.Spread.Sheets.md).[Sparklines](../modules/GC.Spread.Sheets.Sparklines.md).SparklineSetting

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Sparklines.SparklineSetting.md#constructor)

### Properties

- [options](GC.Spread.Sheets.Sparklines.SparklineSetting.md#options)

### Methods

- [clone](GC.Spread.Sheets.Sparklines.SparklineSetting.md#clone)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new SparklineSetting**(`setting?`)

创建迷你图设置

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `setting?` | [`ISparklineSetting`](../interfaces/GC.Spread.Sheets.Sparklines.ISparklineSetting.md) | 设置 |

## Properties

### <a id="options" name="options"></a> options

• **options**: [`ISparklineSetting`](../interfaces/GC.Spread.Sheets.Sparklines.ISparklineSetting.md)

Indicates the options for the sparkline.
options.axisColor {string} the color of the axis
options.firstMarkerColor {string} the color of the first data point for each sparkline in this sparkline group
options.highMarkerColor {string} the color of the highest data point for each sparkline in this sparkline group
options.lastMarkerColor {string} the color of the last data point for each sparkline in this sparkline group
options.lowMarkerColor {string} the color of the lowest data point for each sparkline in this sparkline group
options.markersColor {string} a value that specifies the color of the data markers for each sparkline in this sparkline group
options.negativeColor {string} a value that specifies the color of the negative data points for each sparkline in this sparkline group
options.seriesColor {string} a value that specifies the color for each sparkline in this sparkline group
options.displayEmptyCellsAs {GC.Spread.Sheets.Sparklines.EmptyValueStyle} Indicates how to display the empty cells
options.rightToLeft {boolean} Indicates whether each sparkline in the sparkline group is displayed in a right-to-left manner
options.displayHidden {boolean} Indicates whether data in hidden cells is plotted for the sparklines in this sparkline group
options.displayXAxis {boolean} Indicates whether the horizontal axis is displayed for each sparkline in this sparkline group
options.showFirst {boolean} a value that indicates whether the first data point is formatted differently for each sparkline in this sparkline group
options.showHigh {boolean} a value that specifies whether the data points with the highest value are formatted differently for each sparkline in this sparkline group
options.showLast {boolean} a value that indicates whether the last data point is formatted differently for each sparkline in this sparkline group
options.showLow {boolean} a value that specifies whether the data points with the lowest value are formatted differently for each sparkline in this sparkline group
options.showNegative {boolean} a value that specifies whether the negative data points are formatted differently for each sparkline in this sparkline group
options.showMarkers {boolean} a value that specifies whether data markers are displayed for each sparkline in this sparkline group
options.manualMax {number} Indicates the maximum for the vertical axis that is shared across all sparklines in this sparkline group. The axis is zero if maxAxisType does not equal custom
options.manualMin {number} Indicates the minimum for the vertical axis that is shared across all sparklines in this sparkline group. The axis is zero if minAxisType does not equal custom
options.maxAxisType {GC.Spread.Sheets.Sparklines.SparklineAxisMinMax} Indicates how the vertical axis maximum is calculated for the sparklines in this sparkline group
options.minAxisType {GC.Spread.Sheets.Sparklines.SparklineAxisMinMax} Indicates how the vertical axis minimum is calculated for the sparklines in this sparkline group
options.groupMaxValue {number} Gets the maximum value of the sparkline group
options.groupMinValue {number} Gets the minimum value of the sparkline group
options.lineWeight {number} Indicates the line weight for each sparkline in the sparkline group, where the line weight is measured in points. The weight must be greater than or equal to zero, and must be less than or equal to 3 (LineSeries only supports line weight values in the range of 0.0-3.0)

**`代码示例`**
```
var data = new GC.Spread.Sheets.Range(1, 0, 8, 1);
var setting = new GC.Spread.Sheets.Sparklines.SparklineSetting();
setting.options.showMarkers = true;
setting.options.lineWeight = 3;
setting.options.displayXAxis = true;
setting.options.showFirst = true;
setting.options.showLast = true;
setting.options.showLow = true;
setting.options.showHigh = true;
setting.options.showNegative = true;
setting.options.seriesColor = "Text 2 1";
setting.options.firstMarkerColor = "Text 2 3";
setting.options.negativeColor = "Accent 2 1";
setting.options.markersColor = "Accent 3 1";
setting.options.lowMarkerColor = "Accent 4 1";
setting.options.highMarkerColor = "Accent 6 1";
setting.options.lastMarkerColor = "Accent 6 6";
setting.options.axisColor ="Text 1 1";
sheet.addSpan(13, 0, 4, 3, null);
sheet.setSparkline(13, 0, data, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
sheet.setValue(1, 0, 1);
sheet.setValue(2, 0, -2);
sheet.setValue(3, 0, -1);
sheet.setValue(4, 0, 6);
sheet.setValue(5, 0, 4);
sheet.setValue(6, 0, -4);
sheet.setValue(7, 0, 3);
```

## Methods

### <a id="clone" name="clone"></a> clone

▸ **clone**(): [`SparklineSetting`](GC.Spread.Sheets.Sparklines.SparklineSetting.md)

克隆迷你图设置

#### Returns

[`SparklineSetting`](GC.Spread.Sheets.Sparklines.SparklineSetting.md)

克隆的迷你图设置
