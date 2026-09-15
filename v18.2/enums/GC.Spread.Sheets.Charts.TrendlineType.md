# Enumeration: TrendlineType

[Sheets](../modules/GC.Spread.Sheets.md).[Charts](../modules/GC.Spread.Sheets.Charts.md).TrendlineType

指定用于平滑数据波动的趋势线的计算方法。

## Table of contents

### Enumeration members

- [exponential](GC.Spread.Sheets.Charts.TrendlineType.md#exponential)
- [linear](GC.Spread.Sheets.Charts.TrendlineType.md#linear)
- [logarithmic](GC.Spread.Sheets.Charts.TrendlineType.md#logarithmic)
- [movingAverage](GC.Spread.Sheets.Charts.TrendlineType.md#movingaverage)
- [polynomial](GC.Spread.Sheets.Charts.TrendlineType.md#polynomial)
- [power](GC.Spread.Sheets.Charts.TrendlineType.md#power)

## Enumeration members

### <a id="exponential" name="exponential"></a> exponential

• **exponential** = `0`

使用方程计算通过点的最小二乘拟合。

___

### <a id="linear" name="linear"></a> linear

• **linear** = `1`

使用线性方程 y = mx + b 计算通过点的最小二乘拟合。

___

### <a id="logarithmic" name="logarithmic"></a> logarithmic

• **logarithmic** = `2`

使用方程 y = c ln x + b 计算通过点的最小二乘拟合。

___

### <a id="movingaverage" name="movingaverage"></a> movingAverage

• **movingAverage** = `3`

使用从数据系列部分计算的平均值序列。点数等于系列中的总点数减去为周期指定的数字。

___

### <a id="polynomial" name="polynomial"></a> polynomial

• **polynomial** = `4`

使用方程计算通过点的最小二乘拟合。

___

### <a id="power" name="power"></a> power

• **power** = `5`

使用方程计算通过点的最小二乘拟合。
