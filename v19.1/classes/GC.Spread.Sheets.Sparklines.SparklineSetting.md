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

创建迷你图设置。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `setting?` | [`ISparklineSetting`](../interfaces/GC.Spread.Sheets.Sparklines.ISparklineSetting.md) | 设置项。 |

## Properties

### <a id="options" name="options"></a> options

• **options**: [`ISparklineSetting`](../interfaces/GC.Spread.Sheets.Sparklines.ISparklineSetting.md)

表示迷你图的选项。

**`example`**
```javascript
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

克隆迷你图设置。

#### Returns

[`SparklineSetting`](GC.Spread.Sheets.Sparklines.SparklineSetting.md)

克隆的迷你图设置。
