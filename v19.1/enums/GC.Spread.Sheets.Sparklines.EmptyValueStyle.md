# Enumeration: EmptyValueStyle

[Sheets](../modules/GC.Spread.Sheets.md).[Sparklines](../modules/GC.Spread.Sheets.Sparklines.md).EmptyValueStyle

指定如何在图表中显示数据系列中的空值。

**`example`**
```javascript
//此示例使用EmptyValueStyle枚举。
var data = new GC.Spread.Sheets.Range(1, 0, 8, 1);
var setting = new GC.Spread.Sheets.Sparklines.SparklineSetting
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
setting.options.axisColor = "Text 1 1";
setting.options.displayEmptyCellsAs =  GC.Spread.Sheets.Sparklines.EmptyValueStyle.Zero;
activeSheet.addSpan(13, 0, 4, 3, null);
activeSheet.setSparkline(13, 0, data, GC.Spread.Sheets.Sparklines.DataOrientation.vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
activeSheet.setValue(1, 0, 1);
activeSheet.setValue(2, 0, -2);
activeSheet.setValue(3, 0, -1);
activeSheet.setValue(4, 0, 6);
activeSheet.setValue(5, 0, 4);
activeSheet.setValue(6, 0, -4);
activeSheet.setValue(7, 0, 3);
activeSheet.setValue(8, 0, 8);
```

## Table of contents

### Enumeration members

- [connect](GC.Spread.Sheets.Sparklines.EmptyValueStyle.md#connect)
- [gaps](GC.Spread.Sheets.Sparklines.EmptyValueStyle.md#gaps)
- [zero](GC.Spread.Sheets.Sparklines.EmptyValueStyle.md#zero)

## Enumeration members

### <a id="connect" name="connect"></a> connect

• **connect** = `2`

用连接元素填充间隙，而不是在数据系列中为空值留出间隙。

___

### <a id="gaps" name="gaps"></a> gaps

• **gaps** = `0`

在数据系列中为空值留出间隙，这会导致线条分段。

___

### <a id="zero" name="zero"></a> zero

• **zero** = `1`

将数据系列中的空值作为零值处理，使线条在零值数据点处降至零。
