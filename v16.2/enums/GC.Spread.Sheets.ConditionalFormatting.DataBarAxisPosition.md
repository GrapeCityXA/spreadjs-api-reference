# Enumeration: DataBarAxisPosition

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).DataBarAxisPosition

数据条坐标轴的位置

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

- [automatic](GC.Spread.Sheets.ConditionalFormatting.DataBarAxisPosition.md#automatic)
- [cellMidPoint](GC.Spread.Sheets.ConditionalFormatting.DataBarAxisPosition.md#cellmidpoint)
- [none](GC.Spread.Sheets.ConditionalFormatting.DataBarAxisPosition.md#none)

## Enumeration members

### <a id="automatic" name="automatic"></a> automatic

• **automatic** = `0`

是否基于负值在可变位置显示

___

### <a id="cellmidpoint" name="cellmidpoint"></a> cellMidPoint

• **cellMidPoint** = `1`

是否在单元中点显示

___

### <a id="none" name="none"></a> none

• **none** = `2`

是否按正值条形图相同方向显示负值条形图
