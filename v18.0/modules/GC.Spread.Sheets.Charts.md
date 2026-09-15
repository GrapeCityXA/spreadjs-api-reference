# Namespace: Charts

[Spread](GC.Spread.md).[Sheets](GC.Spread.Sheets.md).Charts

## Table of contents

### Enumerations

- [AxisCrossPoint](../enums/GC.Spread.Sheets.Charts.AxisCrossPoint.md)
- [AxisGroup](../enums/GC.Spread.Sheets.Charts.AxisGroup.md)
- [AxisOrientation](../enums/GC.Spread.Sheets.Charts.AxisOrientation.md)
- [ChartType](../enums/GC.Spread.Sheets.Charts.ChartType.md)
- [ColorRule](../enums/GC.Spread.Sheets.Charts.ColorRule.md)
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
- [TimeUnit](../enums/GC.Spread.Sheets.Charts.TimeUnit.md)
- [TrendlineType](../enums/GC.Spread.Sheets.Charts.TrendlineType.md)

### Classes

- [Chart](../classes/GC.Spread.Sheets.Charts.Chart.md)
- [ChartCollection](../classes/GC.Spread.Sheets.Charts.ChartCollection.md)
- [ColorSchemes](../classes/GC.Spread.Sheets.Charts.ColorSchemes.md)
- [Points](../classes/GC.Spread.Sheets.Charts.Points.md)
- [SeriesCollection](../classes/GC.Spread.Sheets.Charts.SeriesCollection.md)

### Interfaces

- [ErrorBarItem](../interfaces/GC.Spread.Sheets.Charts.ErrorBarItem.md)
- [ErrorBarItemCustom](../interfaces/GC.Spread.Sheets.Charts.ErrorBarItemCustom.md)
- [ErrorBarItemStyle](../interfaces/GC.Spread.Sheets.Charts.ErrorBarItemStyle.md)
- [ErrorBarItems](../interfaces/GC.Spread.Sheets.Charts.ErrorBarItems.md)
- [IAxes](../interfaces/GC.Spread.Sheets.Charts.IAxes.md)
- [IAxis](../interfaces/GC.Spread.Sheets.Charts.IAxis.md)
- [IAxisStyle](../interfaces/GC.Spread.Sheets.Charts.IAxisStyle.md)
- [IAxisTitle](../interfaces/GC.Spread.Sheets.Charts.IAxisTitle.md)
- [IBorder](../interfaces/GC.Spread.Sheets.Charts.IBorder.md)
- [IChartArea](../interfaces/GC.Spread.Sheets.Charts.IChartArea.md)
- [IChartLegend](../interfaces/GC.Spread.Sheets.Charts.IChartLegend.md)
- [IChartLegendLayout](../interfaces/GC.Spread.Sheets.Charts.IChartLegendLayout.md)
- [IChartTextStyle](../interfaces/GC.Spread.Sheets.Charts.IChartTextStyle.md)
- [IChartTitle](../interfaces/GC.Spread.Sheets.Charts.IChartTitle.md)
- [IDataLabels](../interfaces/GC.Spread.Sheets.Charts.IDataLabels.md)
- [IDataPoint](../interfaces/GC.Spread.Sheets.Charts.IDataPoint.md)
- [IDataPoints](../interfaces/GC.Spread.Sheets.Charts.IDataPoints.md)
- [IDisplayUnit](../interfaces/GC.Spread.Sheets.Charts.IDisplayUnit.md)
- [IFormatOver](../interfaces/GC.Spread.Sheets.Charts.IFormatOver.md)
- [IFormatOvers](../interfaces/GC.Spread.Sheets.Charts.IFormatOvers.md)
- [IGridLine](../interfaces/GC.Spread.Sheets.Charts.IGridLine.md)
- [IHoverStyle](../interfaces/GC.Spread.Sheets.Charts.IHoverStyle.md)
- [IHoverSymbolStyle](../interfaces/GC.Spread.Sheets.Charts.IHoverSymbolStyle.md)
- [ILegacyChartPaintCallBack](../interfaces/GC.Spread.Sheets.Charts.ILegacyChartPaintCallBack.md)
- [ILineStyle](../interfaces/GC.Spread.Sheets.Charts.ILineStyle.md)
- [IPaintCallBack](../interfaces/GC.Spread.Sheets.Charts.IPaintCallBack.md)
- [IPatternFillBackColor](../interfaces/GC.Spread.Sheets.Charts.IPatternFillBackColor.md)
- [IScaling](../interfaces/GC.Spread.Sheets.Charts.IScaling.md)
- [ISeries](../interfaces/GC.Spread.Sheets.Charts.ISeries.md)
- [ISeriesItemBorder](../interfaces/GC.Spread.Sheets.Charts.ISeriesItemBorder.md)
- [ISeriesSymbolBorder](../interfaces/GC.Spread.Sheets.Charts.ISeriesSymbolBorder.md)
- [ISymbol](../interfaces/GC.Spread.Sheets.Charts.ISymbol.md)
- [TrendlineItem](../interfaces/GC.Spread.Sheets.Charts.TrendlineItem.md)

### Type aliases

- [ColorScheme](GC.Spread.Sheets.Charts.md#colorscheme)

### Functions

- [getColor](GC.Spread.Sheets.Charts.md#getcolor)

## Type aliases

### <a id="colorscheme" name="colorscheme"></a> ColorScheme

Ƭ **ColorScheme**: ([`ColorRule`](../enums/GC.Spread.Sheets.Charts.ColorRule.md) \| `string`[])[]

**`property`** {GC.Spread.Sheets.Charts.ColorRule} 0 - 颜色规则

**`property`** {string[]} 1 - 颜色列表

## Functions

### <a id="getcolor" name="getcolor"></a> getColor

▸ **getColor**(`colorScheme`, `index`, `count?`): `string`

通过colorScheme、index获取指定颜色

**`example`**
```
GC.Spread.Sheets.Charts.getColor([GC.Spread.Sheets.Charts.ColorRule.acrossLinear, ['Accent 1', 'Accent 4']], 6, 10); // return 'Accent 1 23'
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `colorScheme` | [`ColorScheme`](GC.Spread.Sheets.Charts.md#colorscheme) | 配色方案。 |
| `index` | `number` | The specified index. |
| `count?` | `number` | - |

#### Returns

`string`

返回指定的颜色。
