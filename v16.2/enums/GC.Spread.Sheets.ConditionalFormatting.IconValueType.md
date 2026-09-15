# Enumeration: IconValueType

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).IconValueType

图标值类型

**`代码示例`**
```
//本示例创建一个规则
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,15,3);
activeSheet.setValue(2,0,25,3);
activeSheet.setValue(3,0,-1,3);
var iconSetRule = new GC.Spread.Sheets.ConditionalFormatting.IconSetRule();
iconSetRule.ranges([new GC.Spread.Sheets.Range(0,0,4,1)]);
iconSetRule.iconSetType(GC.Spread.Sheets.ConditionalFormatting.IconSetType.fourTrafficLights);
var iconCriteria = iconSetRule.iconCriteria();
iconCriteria[0] = new GC.Spread.Sheets.ConditionalFormatting.IconCriterion(true, GC.Spread.Sheets.ConditionalFormatting.IconValueType.number, 1);
iconCriteria[1] = new GC.Spread.Sheets.ConditionalFormatting.IconCriterion(true, GC.Spread.Sheets.ConditionalFormatting.IconValueType.number, 10);
iconCriteria[2] = new GC.Spread.Sheets.ConditionalFormatting.IconCriterion(true, GC.Spread.Sheets.ConditionalFormatting.IconValueType.number, 20);
iconSetRule.reverseIconOrder(false);
iconSetRule.showIconOnly(false);
activeSheet.conditionalFormats.addRule(iconSetRule);
```

## Table of contents

### Enumeration members

- [formula](GC.Spread.Sheets.ConditionalFormatting.IconValueType.md#formula)
- [number](GC.Spread.Sheets.ConditionalFormatting.IconValueType.md#number)
- [percent](GC.Spread.Sheets.ConditionalFormatting.IconValueType.md#percent)
- [percentile](GC.Spread.Sheets.ConditionalFormatting.IconValueType.md#percentile)

## Enumeration members

### <a id="formula" name="formula"></a> formula

• **formula** = `7`

是否返回公式计算的结果

___

### <a id="number" name="number"></a> number

• **number** = `1`

是否直接返回指定的数字

___

### <a id="percent" name="percent"></a> percent

• **percent** = `4`

是否返回指定单元格区域内的单元格值的百分比

___

### <a id="percentile" name="percentile"></a> percentile

• **percentile** = `5`

是否返回指定单元格区域内的单元格值的百分位数
