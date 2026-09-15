# Class: IconCriterion

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).IconCriterion

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.ConditionalFormatting.IconCriterion.md#constructor)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new IconCriterion**(`isGreaterThanOrEqualTo`, `iconValueType`, `iconValue`)

表示具有指定参数的图标条件。

**`example`**
```
//此示例创建一个图标规则。
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,15,3);
activeSheet.setValue(2,0,25,3);
activeSheet.setValue(3,0,-1,3);
//规则
var iconSetRule = new GC.Spread.Sheets.ConditionalFormatting.IconSetRule();
iconSetRule.ranges([new GC.Spread.Sheets.Range(0,0,4,1)]);
iconSetRule.iconSetType(GC.Spread.Sheets.ConditionalFormatting.IconSetType.fourTrafficLights);
var iconCriteria = iconSetRule.iconCriteria();
iconCriteria[0] = new GC.Spread.Sheets.ConditionalFormatting.IconCriterion(true, GC.Spread.Sheets.ConditionalFormatting.IconValueType.number, 1);
iconCriteria[1] = new GC.Spread.Sheets.ConditionalFormatting.IconCriterion(true, GC.Spread.Sheets.ConditionalFormatting.IconValueType.number, 10);
iconCriteria[2] = new GC.Spread.Sheets.ConditionalFormatting.IconCriterion(true, GC.Spread.Sheets.ConditionalFormatting.IconValueType.number, 20);
iconSetRule.iconCriteria(iconCriteria);
iconSetRule.reverseIconOrder(false);
iconSetRule.showIconOnly(false);
activeSheet.conditionalFormats.addRule(iconSetRule);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `isGreaterThanOrEqualTo` | `boolean` | 如果设置为true，则使用大于或等于运算符计算值。 |
| `iconValueType` | [`IconValueType`](../enums/GC.Spread.Sheets.ConditionalFormatting.IconValueType.md) | 比例值的类型。 |
| `iconValue` | `Object` | 比例值。 |
