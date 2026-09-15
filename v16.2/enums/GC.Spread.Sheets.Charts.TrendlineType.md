# Enumeration: TrendlineType

[Sheets](../modules/GC.Spread.Sheets.md).[Charts](../modules/GC.Spread.Sheets.Charts.md).TrendlineType

指定如何计算可消除数据波动的趋势线

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

使用方程式计算通过点的最小二乘拟合

___

### <a id="linear" name="linear"></a> linear

• **linear** = `1`

使用线性方程y = mx + b计算通过点的最小二乘拟合

___

### <a id="logarithmic" name="logarithmic"></a> logarithmic

• **logarithmic** = `2`

使用等式y = c ln x + b计算通过点的最小二乘拟合

___

### <a id="movingaverage" name="movingaverage"></a> movingAverage

• **movingAverage** = `3`

使用从数据系列的各个部分计算出的一系列平均值
of points equals the total number of points in the series less the number
specified for the period.

___

### <a id="polynomial" name="polynomial"></a> polynomial

• **polynomial** = `4`

使用方程式计算通过点的最小二乘拟合

___

### <a id="power" name="power"></a> power

• **power** = `5`

使用方程式计算通过点的最小二乘拟合
