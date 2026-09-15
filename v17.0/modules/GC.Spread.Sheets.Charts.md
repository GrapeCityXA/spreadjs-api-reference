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
- [ILegacyChartPaintCallBack](../interfaces/GC.Spread.Sheets.Charts.ILegacyChartPaintCallBack.md)
- [ILineStyle](../interfaces/GC.Spread.Sheets.Charts.ILineStyle.md)
- [IPaintCallBack](../interfaces/GC.Spread.Sheets.Charts.IPaintCallBack.md)
- [IPatternFillBackColor](../interfaces/GC.Spread.Sheets.Charts.IPatternFillBackColor.md)
- [IScaling](../interfaces/GC.Spread.Sheets.Charts.IScaling.md)
- [ISeries](../interfaces/GC.Spread.Sheets.Charts.ISeries.md)
- [ISeriesItemBase](../interfaces/GC.Spread.Sheets.Charts.ISeriesItemBase.md)
- [ISeriesItemBorder](../interfaces/GC.Spread.Sheets.Charts.ISeriesItemBorder.md)
- [ISeriesSymbolBorder](../interfaces/GC.Spread.Sheets.Charts.ISeriesSymbolBorder.md)
- [ISymbol](../interfaces/GC.Spread.Sheets.Charts.ISymbol.md)
- [ITrendline](../interfaces/GC.Spread.Sheets.Charts.ITrendline.md)
- [TrendlineItem](../interfaces/GC.Spread.Sheets.Charts.TrendlineItem.md)

### Type aliases

- [IDataPointStyle](GC.Spread.Sheets.Charts.md#idatapointstyle)
- [IFormatOver](GC.Spread.Sheets.Charts.md#iformatover)
- [IFormatOvers](GC.Spread.Sheets.Charts.md#iformatovers)

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

**`property`** {number} symbolSize 数据点的符号大小

**`property`** {GC.Spread.Sheets.Charts.SymbolShape} symbolShape 数据点的符号

**`property`** {GC.Spread.Sheets.Charts.ISeriesItemBorder} symbolBorder 数据点的符号边界

**`property`** {string} symbolBorder.color 数据点的符号边框颜色

**`property`** {number} symbolBorder.colorTransparency 数据点符号边框颜色的透明度

**`property`** {number} symbolBorder.width 数据点的符号边框宽度

**`property`** {GC.Spread.Sheets.Charts.LineType} symbolBorder.lineType 数据点的符号边界线类型

#### Type declaration

| Name | Type |
| :------ | :------ |
| `backColor` | `string` \| [`IPatternFillBackColor`](../interfaces/GC.Spread.Sheets.Charts.IPatternFillBackColor.md) |
| `backColorTransparency?` | `number` |
| `border?` | [`ISeriesItemBorder`](../interfaces/GC.Spread.Sheets.Charts.ISeriesItemBorder.md) |

___

### <a id="iformatover" name="iformatover"></a> IFormatOver

Ƭ **IFormatOver**: `Object`

**`property`** {string | GC.Spread.Sheets.Charts.IPatternFillBackColor} backColor 特定数据点集的背景颜色

**`property`** {number} backColorTransparency 特定数据点集的背景颜色透明度

**`property`** {GC.Spread.Sheets.Charts.ISeriesItemBorder} borderStyle 特定数据点集的边框样式

**`property`** {Object} borderStyle.color 特定数据点集的边框颜色

**`property`** {number} borderStyle.transparency 特定数据点集的边框颜色透明度

**`property`** {number} borderStyle.width 特定数据点集的边框宽度

**`property`** {GC.Spread.Sheets.Charts.LineType} borderStyle.lineType 特定数据点集的边框线型

#### Type declaration

| Name | Type |
| :------ | :------ |
| `backColor?` | `string` \| [`IPatternFillBackColor`](../interfaces/GC.Spread.Sheets.Charts.IPatternFillBackColor.md) |
| `backColorTransparency?` | `number` |
| `borderStyle?` | [`ISeriesItemBorder`](../interfaces/GC.Spread.Sheets.Charts.ISeriesItemBorder.md) |

___

### <a id="iformatovers" name="iformatovers"></a> IFormatOvers

Ƭ **IFormatOvers**: `Object`

**`property`** {Object.<number, GC.Spread.Sheets.Charts.IFormatOver>}  - 键为数字类型的对象类型
对于瀑布图，0代表增加，1代表减少，2代表总计，键值为IFormatOver类型

#### Index signature

▪ [key: `number`]: [`IFormatOver`](GC.Spread.Sheets.Charts.md#iformatover)
