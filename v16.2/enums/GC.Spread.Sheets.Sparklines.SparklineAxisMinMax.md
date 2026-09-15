# Enumeration: SparklineAxisMinMax

[Sheets](../modules/GC.Spread.Sheets.md).[Sparklines](../modules/GC.Spread.Sheets.Sparklines.md).SparklineAxisMinMax

一个枚举,它指定关于如何为迷你图组计算垂直轴的最小值或最大值的信息

**`代码示例`**
```
//本示例使用SparklineAxisMinMax枚举
activeSheet.setValue(0, 0, "Data Range is A2-A9");
activeSheet.setValue(1, 0, 1);
activeSheet.setValue(2, 0, -2);
activeSheet.setValue(3, 0, -1);
activeSheet.setValue(4, 0, 6);
activeSheet.setValue(5, 0, 4);
activeSheet.setValue(6, 0, -4);
activeSheet.setValue(7, 0, 3);
activeSheet.setValue(8, 0, 8);
var data = new GC.Spread.Sheets.Range(1, 0, 8, 1);
var setting = new GC.Spread.Sheets.Sparklines.SparklineSetting();
setting.options.minAxisType = GC.Spread.Sheets.Sparklines.SparklineAxisMinMax.custom;
setting.options.manualMin = -2;
setting.options.maxAxisType = GC.Spread.Sheets.Sparklines.SparklineAxisMinMax.custom;
setting.options.manualMax = 10;
var s1=  activeSheet.setSparkline(11, 0, data, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
var s2 =activeSheet.setSparkline(11, 3, data, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.column, setting);
var s3=  activeSheet.setSparkline(11, 6, data, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.winloss, setting);
var group = activeSheet.groupSparkline([s1,s2,s3]);
```

## Table of contents

### Enumeration members

- [custom](GC.Spread.Sheets.Sparklines.SparklineAxisMinMax.md#custom)
- [group](GC.Spread.Sheets.Sparklines.SparklineAxisMinMax.md#group)
- [individual](GC.Spread.Sheets.Sparklines.SparklineAxisMinMax.md#individual)

## Enumeration members

### <a id="custom" name="custom"></a> custom

• **custom** = `2`

由该迷你图组的manualMin属性或manualMax属性指定该迷你图组中每个迷你图的垂直轴的最小值或最大值

___

### <a id="group" name="group"></a> group

• **group** = `1`

垂直轴的最小值或最大值在该迷你图组中的所有迷你图上共享,并且是自动计算的,因此可以在绘图区域中显示具有最小值或最大值的数据点

___

### <a id="individual" name="individual"></a> individual

• **individual** = `0`

自动计算此迷你图组中每个迷你图的垂直轴的最小值或最大值,以便可以在绘图区域中显示具有最小值或最大值的数据点
