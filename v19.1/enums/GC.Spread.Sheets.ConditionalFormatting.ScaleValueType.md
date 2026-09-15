# Enumeration: ScaleValueType

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).ScaleValueType

指定刻度值类型。

**`example`**
```javascript
//此示例创建数据条规则。
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,15,3);
activeSheet.setValue(2,0,25,3);
activeSheet.setValue(3,0,-1,3);
var dataBarRule = new GC.Spread.Sheets.ConditionalFormatting.DataBarRule();
dataBarRule.ranges([new GC.Spread.Sheets.Range(0,0,4,1)]);
dataBarRule.minType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
dataBarRule.minValue(-1);
dataBarRule.maxType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
dataBarRule.maxValue(40);
dataBarRule.color("green");
dataBarRule.showBorder(true);
dataBarRule.borderColor("orange");
dataBarRule.dataBarDirection(GC.Spread.Sheets.ConditionalFormatting.BarDirection.leftToRight);
dataBarRule.negativeFillColor("yellow");
dataBarRule.useNegativeFillColor(true);
dataBarRule.negativeBorderColor("red");
dataBarRule.useNegativeBorderColor(true);
dataBarRule.axisPosition(GC.Spread.Sheets.ConditionalFormatting.DataBarAxisPosition.automatic);
dataBarRule.axisColor("blue");
dataBarRule.showBarOnly(false);
activeSheet.conditionalFormats.addRule(dataBarRule);
```

## Table of contents

### Enumeration members

- [automax](GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md#automax)
- [automin](GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md#automin)
- [formula](GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md#formula)
- [highestValue](GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md#highestvalue)
- [lowestValue](GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md#lowestvalue)
- [number](GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md#number)
- [percent](GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md#percent)
- [percentile](GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md#percentile)

## Enumeration members

### <a id="automax" name="automax"></a> automax

• **automax** = `7`

指示是否返回指定范围内的自动最大值。

___

### <a id="automin" name="automin"></a> automin

• **automin** = `5`

指示是否返回指定范围内的自动最小值。

___

### <a id="formula" name="formula"></a> formula

• **formula** = `6`

指示是否返回公式计算的结果。

___

### <a id="highestvalue" name="highestvalue"></a> highestValue

• **highestValue** = `2`

指示是否返回指定单元格范围内的最高值。

___

### <a id="lowestvalue" name="lowestvalue"></a> lowestValue

• **lowestValue** = `1`

指示是否返回指定单元格范围内的最低值。

___

### <a id="number" name="number"></a> number

• **number** = `0`

指示是否直接返回指定数字。

___

### <a id="percent" name="percent"></a> percent

• **percent** = `3`

指示是否返回指定单元格范围内单元格值的百分比。

___

### <a id="percentile" name="percentile"></a> percentile

• **percentile** = `4`

指示是否返回指定单元格范围内单元格值的百分位数。
