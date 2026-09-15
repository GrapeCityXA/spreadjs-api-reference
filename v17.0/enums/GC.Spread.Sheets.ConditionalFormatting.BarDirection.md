# Enumeration: BarDirection

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).BarDirection

数据条方向

**`代码示例`**
```
//本示例创建一个数据条规则
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

- [leftToRight](GC.Spread.Sheets.ConditionalFormatting.BarDirection.md#lefttoright)
- [rightToLeft](GC.Spread.Sheets.ConditionalFormatting.BarDirection.md#righttoleft)

## Enumeration members

### <a id="lefttoright" name="lefttoright"></a> leftToRight

• **leftToRight** = `0`

是否从左到右显示数据条

___

### <a id="righttoleft" name="righttoleft"></a> rightToLeft

• **rightToLeft** = `1`

是否从右到左显示数据条
