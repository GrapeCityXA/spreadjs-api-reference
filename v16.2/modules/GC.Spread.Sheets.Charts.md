# Namespace: Charts

[Spread](GC.Spread.md).[Sheets](GC.Spread.Sheets.md).Charts

## Table of contents

### Enumerations

- [AxisCrossPoint](../enums/GC.Spread.Sheets.Charts.AxisCrossPoint.md)
- [AxisGroup](../enums/GC.Spread.Sheets.Charts.AxisGroup.md)
- [AxisOrientation](../enums/GC.Spread.Sheets.Charts.AxisOrientation.md)
- [ChartType](../enums/GC.Spread.Sheets.Charts.ChartType.md)
- [DataLabelPosition](../enums/GC.Spread.Sheets.Charts.DataLabelPosition.md)
- [DisplayBlanksAs](../enums/GC.Spread.Sheets.Charts.DisplayBlanksAs.md)
- [DisplayUnit](../enums/GC.Spread.Sheets.Charts.DisplayUnit.md)
- [ErrorBarType](../enums/GC.Spread.Sheets.Charts.ErrorBarType.md)
- [ErrorBarValueType](../enums/GC.Spread.Sheets.Charts.ErrorBarValueType.md)
- [LegendPosition](../enums/GC.Spread.Sheets.Charts.LegendPosition.md)
- [LineType](../enums/GC.Spread.Sheets.Charts.LineType.md)
- [PatternType](../enums/GC.Spread.Sheets.Charts.PatternType.md)
- [RowCol](../enums/GC.Spread.Sheets.Charts.RowCol.md)
- [SymbolShape](../enums/GC.Spread.Sheets.Charts.SymbolShape.md)
- [TickLabelPosition](../enums/GC.Spread.Sheets.Charts.TickLabelPosition.md)
- [TickMark](../enums/GC.Spread.Sheets.Charts.TickMark.md)
- [TrendlineType](../enums/GC.Spread.Sheets.Charts.TrendlineType.md)

### Classes

- [Chart](../classes/GC.Spread.Sheets.Charts.Chart.md)
- [ChartCollection](../classes/GC.Spread.Sheets.Charts.ChartCollection.md)
- [Points](../classes/GC.Spread.Sheets.Charts.Points.md)
- [SeriesCollection](../classes/GC.Spread.Sheets.Charts.SeriesCollection.md)

### Interfaces

- [ErrorBarItem](../interfaces/GC.Spread.Sheets.Charts.ErrorBarItem.md)
- [ErrorBarItems](../interfaces/GC.Spread.Sheets.Charts.ErrorBarItems.md)
- [IAxes](../interfaces/GC.Spread.Sheets.Charts.IAxes.md)
- [IAxis](../interfaces/GC.Spread.Sheets.Charts.IAxis.md)
- [IAxisStyle](../interfaces/GC.Spread.Sheets.Charts.IAxisStyle.md)
- [IAxisTitle](../interfaces/GC.Spread.Sheets.Charts.IAxisTitle.md)
- [IBorder](../interfaces/GC.Spread.Sheets.Charts.IBorder.md)
- [IChartArea](../interfaces/GC.Spread.Sheets.Charts.IChartArea.md)
- [IChartLegend](../interfaces/GC.Spread.Sheets.Charts.IChartLegend.md)
- [IChartTextStyle](../interfaces/GC.Spread.Sheets.Charts.IChartTextStyle.md)
- [IChartTitle](../interfaces/GC.Spread.Sheets.Charts.IChartTitle.md)
- [IDataLabels](../interfaces/GC.Spread.Sheets.Charts.IDataLabels.md)
- [IDataPoint](../interfaces/GC.Spread.Sheets.Charts.IDataPoint.md)
- [IDisplayUnit](../interfaces/GC.Spread.Sheets.Charts.IDisplayUnit.md)
- [IGridLine](../interfaces/GC.Spread.Sheets.Charts.IGridLine.md)
- [IHoverStyle](../interfaces/GC.Spread.Sheets.Charts.IHoverStyle.md)
- [IHoverSymbolStyle](../interfaces/GC.Spread.Sheets.Charts.IHoverSymbolStyle.md)
- [ILineStyle](../interfaces/GC.Spread.Sheets.Charts.ILineStyle.md)
- [IPaintCallBack](../interfaces/GC.Spread.Sheets.Charts.IPaintCallBack.md)
- [IPatternFillBackColor](../interfaces/GC.Spread.Sheets.Charts.IPatternFillBackColor.md)
- [IScaling](../interfaces/GC.Spread.Sheets.Charts.IScaling.md)
- [ISeries](../interfaces/GC.Spread.Sheets.Charts.ISeries.md)
- [ISeriesItemBorder](../interfaces/GC.Spread.Sheets.Charts.ISeriesItemBorder.md)
- [ISeriesSymbolBorder](../interfaces/GC.Spread.Sheets.Charts.ISeriesSymbolBorder.md)
- [ISymbol](../interfaces/GC.Spread.Sheets.Charts.ISymbol.md)
- [ITrendline](../interfaces/GC.Spread.Sheets.Charts.ITrendline.md)
- [TrendlineItem](../interfaces/GC.Spread.Sheets.Charts.TrendlineItem.md)

### Type aliases

- [IDataPointStyle](GC.Spread.Sheets.Charts.md#idatapointstyle)

## Type aliases

### <a id="idatapointstyle" name="idatapointstyle"></a> IDataPointStyle

Ƭ **IDataPointStyle**: `Object`

**`property`** {string | GC.Spread.Sheets.Charts.IPatternFillBackColor} backColor 数据点的背景颜色

**`property`** {number} backColorTransparency 数据点的背景颜色透明度

**`property`** {GC.Spread.Sheets.Charts.ISeriesItemBorder} border 数据点的边框样式

**`property`** {Object} border.color 数据点的边框颜色

**`property`** {number} border.transparency 数据点的边框颜色透明度

**`property`** {number} border.width 数据点的边框宽度

**`property`** {GC.Spread.Sheets.Charts.LineType} border.lineType 数据点的边框线类型

**`param`** 该数据点是否启用了invertIfNegative。


#### Type declaration

| Name | Type |
| :------ | :------ |
| `backColor` | `string` \| [`IPatternFillBackColor`](../interfaces/GC.Spread.Sheets.Charts.IPatternFillBackColor.md) |
| `backColorTransparency?` | `number` |
| `border?` | [`ISeriesItemBorder`](../interfaces/GC.Spread.Sheets.Charts.ISeriesItemBorder.md) |
