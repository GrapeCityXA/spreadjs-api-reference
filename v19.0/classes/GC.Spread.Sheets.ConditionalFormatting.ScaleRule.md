# Class: ScaleRule

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).ScaleRule

## Hierarchy

- [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

  ↳ **`ScaleRule`**

  ↳↳ [`DataBarRule`](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md)

  ↳↳ [`IconSetRule`](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md)

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#constructor)

### Methods

- [condition](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#condition)
- [contains](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#contains)
- [createCondition](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#createcondition)
- [evaluate](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#evaluate)
- [getExpected](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#getexpected)
- [intersects](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#intersects)
- [isScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#isscalerule)
- [maxColor](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#maxcolor)
- [maxType](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#maxtype)
- [maxValue](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#maxvalue)
- [midColor](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#midcolor)
- [midType](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#midtype)
- [midValue](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#midvalue)
- [minColor](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#mincolor)
- [minType](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#mintype)
- [minValue](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#minvalue)
- [priority](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#priority)
- [ranges](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#ranges)
- [reset](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#reset)
- [ruleType](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#ruletype)
- [stopIfTrue](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#stopiftrue)
- [style](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#style)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new ScaleRule**(`ruleType`, `minType?`, `minValue?`, `minColor?`, `midType?`, `midValue?`, `midColor?`, `maxType?`, `maxValue?`, `maxColor?`, `ranges?`)

表示一个比例条件规则。

**`@extends`** GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase

**`example`**
```
var scale = new GC.Spread.Sheets.ConditionalFormatting.ScaleRule();
scale.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.threeScaleRule);
scale.midColor("red");
scale.midType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
scale.midValue(50);
scale.maxColor("blue");
scale.maxType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
scale.maxValue(100);
scale.minColor("yellow");
scale.minType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
scale.minValue(10);
scale.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 3)]);
activeSheet.conditionalFormats.addRule(scale);
activeSheet.setValue(0,0, 1,3);
activeSheet.setValue(1,0, 50,3);
activeSheet.setValue(2,0, 100,3);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ruleType` | [`RuleType`](../enums/GC.Spread.Sheets.ConditionalFormatting.RuleType.md) | 规则类型。 |
| `minType?` | [`ScaleValueType`](../enums/GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md) | 最小比例类型。 |
| `minValue?` | `number` | 最小比例值。 |
| `minColor?` | `string` | 最小比例颜色。 |
| `midType?` | [`ScaleValueType`](../enums/GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md) | 中点比例类型。 |
| `midValue?` | `number` | 中点比例值。 |
| `midColor?` | `string` | 中点比例颜色。 |
| `maxType?` | [`ScaleValueType`](../enums/GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md) | 最大比例类型。 |
| `maxValue?` | `number` | 最大比例值。 |
| `maxColor?` | `string` | 最大比例颜色。 |
| `ranges?` | [`Range`](GC.Spread.Sheets.Range.md)[] | 范围。 |

#### Overrides

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[constructor](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#constructor)

## Methods

### <a id="condition" name="condition"></a> condition

▸ **condition**(`value?`): `any`

获取或设置规则的基础条件。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md) | 规则的基础条件。 |

#### Returns

`any`

如果未设置值，则返回规则的基础条件；否则返回条件规则。

#### Inherited from

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[condition](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#condition)

___

### <a id="contains" name="contains"></a> contains

▸ **contains**(`row`, `column`): `boolean`

确定单元格范围是否包含指定行和列的单元格。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `column` | `number` | 列索引。 |

#### Returns

`boolean`

如果单元格范围包含指定行和列的单元格，则为 `true`；否则为 `false`。

#### Inherited from

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[contains](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#contains)

___

### <a id="createcondition" name="createcondition"></a> createCondition

▸ **createCondition**(): [`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

为规则创建条件。

#### Returns

[`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

条件。

#### Overrides

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[createCondition](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#createcondition)

___

### <a id="evaluate" name="evaluate"></a> evaluate

▸ **evaluate**(`evaluator`, `baseRow`, `baseColumn`, `actual`): `any`

如果单元格满足条件，则返回规则的指定值。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `evaluator` | `Object` | 评估器。 |
| `baseRow` | `number` | 行索引。 |
| `baseColumn` | `number` | 列索引。 |
| `actual` | `Object` | 用于评估的实际值对象。 |

#### Returns

`any`

如果单元格满足条件，则返回规则的指定值。

#### Overrides

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[evaluate](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#evaluate)

___

### <a id="getexpected" name="getexpected"></a> getExpected

▸ **getExpected**(): [`Style`](GC.Spread.Sheets.Style.md)

获取基础规则的样式。

**`example`**
```
 //此示例使用getExpected方法。
 activeSheet.suspendPaint();
 var style = new GC.Spread.Sheets.Style();
 style.backColor = "green";
 var ranges = [new GC.Spread.Sheets.Range(0, 0, 10, 1)];
 activeSheet.conditionalFormats.addUniqueRule(style, ranges);
 var data = [50, 50, 11, 5, 3, 6, 7, 8, 7, 11];
 var condition = activeSheet.conditionalFormats.getRules()[0];
 for (var i = 0; i < 10;i++){
     activeSheet.setValue(i, 0, data[i]);
 }
 activeSheet.resumePaint();
 console.log(condition.getExpected());
```

#### Returns

[`Style`](GC.Spread.Sheets.Style.md)

#### Inherited from

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[getExpected](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#getexpected)

___

### <a id="intersects" name="intersects"></a> intersects

▸ **intersects**(`row`, `column`, `rowCount`, `columnCount`): `boolean`

指定此规则的范围是否与另一个范围相交。

**`example`**
```
 //此示例使用intersects方法。
 activeSheet.suspendPaint();
 var style = new GC.Spread.Sheets.Style();
 style.backColor = "green";
 var ranges = [new GC.Spread.Sheets.Range(0, 0, 10, 1)];
 activeSheet.conditionalFormats.addUniqueRule(style, ranges);
 var data = [50, 50, 11, 5, 3, 6, 7, 8, 7, 11];
 var condition = activeSheet.conditionalFormats.getRules()[0];
 for (var i = 0; i < 10; i++) {
     activeSheet.setValue(i, 0, data[i]);
 }
 activeSheet.resumePaint();
 activeSheet.bind(GC.Spread.Sheets.Events.SelectionChanged, function(e, info) {
     var selection = info.newSelections[0];
     var result = condition.intersects(selection.row, selection.col, selection.rowCount, selection.colCount);
     if (result) {
         alert("当前选择与条件格式化范围相交");
     } else {
         alert("当前选择与条件格式化范围不相交");
     }
 });
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `column` | `number` | 列索引。 |
| `rowCount` | `number` | 行数。 |
| `columnCount` | `number` | 列数。 |

#### Returns

`boolean`

如果此规则的范围与另一个范围相交，则为 `true`；否则为 `false`。

#### Inherited from

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[intersects](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#intersects)

___

### <a id="isscalerule" name="isscalerule"></a> isScaleRule

▸ **isScaleRule**(): `boolean`

指定此规则是否为比例规则。

#### Returns

`boolean`

如果此规则是比例规则，则为 `true`；否则为 `false`。

#### Inherited from

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[isScaleRule](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#isscalerule)

___

### <a id="maxcolor" name="maxcolor"></a> maxColor

▸ **maxColor**(`value?`): `any`

获取或设置最大颜色比例。

**`example`**
```
var rule = new GC.Spread.Sheets.ConditionalFormatting.ScaleRule();
rule.ranges([new GC.Spread.Sheets.Range(0,0,10,3)]);
rule.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.twoScaleRule);
rule.minType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
rule.minValue(10);
rule.minColor("Yellow");
rule.maxType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
rule.maxValue(100);
rule.maxColor("Blue");
activeSheet.conditionalFormats.addRule(rule);
activeSheet.setValue(0,0, 1,3);
activeSheet.setValue(1,0, 50,3);
activeSheet.setValue(2,0, 100,3);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 最大颜色比例。 |

#### Returns

`any`

如果未设置值，则返回最大颜色比例；否则返回比例规则。

___

### <a id="maxtype" name="maxtype"></a> maxType

▸ **maxType**(`value?`): `any`

获取或设置最大比例类型。

**`example`**
```
var scale = new GC.Spread.Sheets.ConditionalFormatting.ScaleRule();
scale.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.threeScaleRule);
scale.midColor("red");
scale.midType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
scale.midValue(50);
scale.maxColor("blue");
scale.maxType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
scale.maxValue(100);
scale.minColor("yellow");
scale.minType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
scale.minValue(10);
scale.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 3)]);
activeSheet.conditionalFormats.addRule(scale);
activeSheet.setValue(0,0, 1,3);
activeSheet.setValue(1,0, 50,3);
activeSheet.setValue(2,0, 100,3);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`ScaleValueType`](../enums/GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md) | 最大比例类型。 |

#### Returns

`any`

如果未设置值，则返回最大比例类型；否则返回比例规则。

___

### <a id="maxvalue" name="maxvalue"></a> maxValue

▸ **maxValue**(`value?`): `any`

获取或设置最大比例值。

**`example`**
```
var scale = new GC.Spread.Sheets.ConditionalFormatting.ScaleRule();
scale.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.twoScaleRule);
scale.maxColor("blue");
scale.maxType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
scale.maxValue(100);
scale.minColor("yellow");
scale.minType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
scale.minValue(10);
scale.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 3)]);
activeSheet.conditionalFormats.addRule(scale);
activeSheet.setValue(0,0, 1,3);
activeSheet.setValue(1,0, 50,3);
activeSheet.setValue(2,0, 100,3);
alert("Color: " + scale.maxColor() + " Type: " + scale.maxType() + " Value: " + scale.maxValue());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 最大比例值。 |

#### Returns

`any`

如果未设置值，则返回最大比例值；否则返回比例规则。

___

### <a id="midcolor" name="midcolor"></a> midColor

▸ **midColor**(`value?`): `any`

获取或设置中点比例颜色。

**`example`**
```
var scale = new GC.Spread.Sheets.ConditionalFormatting.ScaleRule();
scale.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.threeScaleRule);
scale.midColor("red");
scale.midType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
scale.midValue(50);
scale.maxColor("blue");
scale.maxType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
scale.maxValue(100);
scale.minColor("yellow");
scale.minType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
scale.minValue(10);
scale.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 3)]);
activeSheet.conditionalFormats.addRule(scale);
activeSheet.setValue(0,0, 1,3);
activeSheet.setValue(1,0, 50,3);
activeSheet.setValue(2,0, 100,3);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 中点比例颜色。 |

#### Returns

`any`

如果未设置值，则返回中点比例颜色；否则返回比例规则。

___

### <a id="midtype" name="midtype"></a> midType

▸ **midType**(`value?`): `any`

获取或设置中点比例类型。

**`example`**
```
var scale = new GC.Spread.Sheets.ConditionalFormatting.ScaleRule();
scale.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.threeScaleRule);
scale.midColor("red");
scale.midType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
scale.midValue(50);
scale.maxColor("blue");
scale.maxType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
scale.maxValue(100);
scale.minColor("yellow");
scale.minType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
scale.minValue(10);
scale.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 3)]);
activeSheet.conditionalFormats.addRule(scale);
activeSheet.setValue(0,0, 1,3);
activeSheet.setValue(1,0, 50,3);
activeSheet.setValue(2,0, 100,3);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`ScaleValueType`](../enums/GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md) | 中点比例类型。 |

#### Returns

`any`

如果未设置值，则返回中点比例类型；否则返回比例规则。

___

### <a id="midvalue" name="midvalue"></a> midValue

▸ **midValue**(`value?`): `any`

获取或设置中点比例值。

**`example`**
```
var scale = new GC.Spread.Sheets.ConditionalFormatting.ScaleRule();
scale.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.threeScaleRule);
scale.midColor("red");
scale.midType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
scale.midValue(50);
scale.maxColor("blue");
scale.maxType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
scale.maxValue(100);
scale.minColor("yellow");
scale.minType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
scale.minValue(10);
scale.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 3)]);
activeSheet.conditionalFormats.addRule(scale);
activeSheet.setValue(0,0, 1,3);
activeSheet.setValue(1,0, 50,3);
activeSheet.setValue(2,0, 100,3);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 中点比例值。 |

#### Returns

`any`

如果未设置值，则返回中点比例值；否则返回比例规则。

___

### <a id="mincolor" name="mincolor"></a> minColor

▸ **minColor**(`value?`): `any`

获取或设置最小比例颜色。

**`example`**
```
var rule = new GC.Spread.Sheets.ConditionalFormatting.ScaleRule();
rule.ranges([new GC.Spread.Sheets.Range(0,0,10,3)]);
rule.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.twoScaleRule);
rule.minType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
rule.minValue(10);
rule.minColor("Yellow");
rule.maxType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
rule.maxValue(100);
rule.maxColor("Blue");
activeSheet.conditionalFormats.addRule(rule);
activeSheet.setValue(0,0, 1,3);
activeSheet.setValue(1,0, 50,3);
activeSheet.setValue(2,0, 100,3);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 最小比例颜色。 |

#### Returns

`any`

如果未设置值，则返回最小比例颜色；否则返回比例规则。

___

### <a id="mintype" name="mintype"></a> minType

▸ **minType**(`value?`): `any`

获取或设置最小比例类型。

**`example`**
```
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

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`ScaleValueType`](../enums/GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md) | 最小比例类型。 |

#### Returns

`any`

如果未设置值，则返回最小比例类型；否则返回比例规则。

___

### <a id="minvalue" name="minvalue"></a> minValue

▸ **minValue**(`value?`): `any`

获取或设置最小比例值。

**`example`**
```
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

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 最小比例值。 |

#### Returns

`any`

如果未设置值，则返回最小比例值；否则返回比例规则。

___

### <a id="priority" name="priority"></a> priority

▸ **priority**(`value?`): `any`

获取或设置规则的优先级。

**`example`**
```javascript
// 示例：创建多个不同优先级的条件格式规则
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
var rule = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
rule.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.cellValueRule);
rule.operator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.greaterThan);
rule.value1(10);
rule.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 1)]);
rule.style(style);
rule.priority(1); // 将优先级设置为 1（最高优先级）
activeSheet.conditionalFormats.addRule(rule);
var style2 = new GC.Spread.Sheets.Style();
style2.backColor = "blue";
var rule2 = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
rule2.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.cellValueRule);
rule2.operator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.greaterThan);
rule2.value1(100);
rule2.ranges([new GC.Spread.Sheets.Range(5, 0, 10, 1)]);
rule2.style(style2);
rule2.priority(2); // 将优先级设置为 2
activeSheet.conditionalFormats.addRule(rule2);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 规则的优先级。 |

#### Returns

`any`

如果未设置值，则返回规则的优先级；否则返回条件规则。

#### Inherited from

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[priority](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#priority)

___

### <a id="ranges" name="ranges"></a> ranges

▸ **ranges**(`value?`): `any`

获取或设置规则的范围。

**`example`**
```
var style = new GC.Spread.Sheets.Style();
style.backColor = "green";
var ranges = [new GC.Spread.Sheets.Range(0, 0, 10, 1)];
activeSheet.conditionalFormats.addUniqueRule(style, ranges);
activeSheet.setValue(0, 0, 50);
activeSheet.setValue(1, 0, 50);
activeSheet.setValue(2, 0, 11);
activeSheet.setValue(3, 0, 5);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`Range`](GC.Spread.Sheets.Range.md)[] | 规则的范围。 |

#### Returns

`any`

若未设置参数值，返回条件格式规则范围的副本；若已设置参数值，返回该条件格式规则对象。

#### Inherited from

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[ranges](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#ranges)

___

### <a id="reset" name="reset"></a> reset

▸ **reset**(): `void`

重置规则。

**`example`**
```
 activeSheet.setArray(0, 0, [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]);
 var style = new GC.Spread.Sheets.Style();
 style.backColor = "red";
 style.foreColor = "black";
 var cell = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
 cell.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.cellValueRule);
 cell.operator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.greaterThan);
 cell.value1(2);
 cell.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 1)]);
 cell.style(style);
 activeSheet.conditionalFormats.addRule(cell);
 var style = new GC.Spread.Sheets.Style();
 style.cellButtons = [{
     caption: "Reset",
     useButtonStyle: true,
     width: 60,
     command: function(sheet) {
         cell.reset();
         sheet.resumePaint();
     }
 }];
 activeSheet.setStyle(16, 4, style);
```

#### Returns

`void`

#### Inherited from

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[reset](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#reset)

___

### <a id="ruletype" name="ruletype"></a> ruleType

▸ **ruleType**(`value?`): `any`

获取或设置规则的类型。

**`example`**
```
//此示例使用ruleType方法。
activeSheet.setArray(0,0,[1,2,3,4,5,6,7,8,9,10]);
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
style.foreColor = "black";
var cell = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
cell.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.cellValueRule);
cell.operator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.greaterThan);
cell.value1(5);
cell.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 1)]);
cell.style(style);
activeSheet.conditionalFormats.addRule(cell);
var style1 = new GC.Spread.Sheets.Style();
style1.foreColor = "red";
var top = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
top.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.top10Rule);
top.type(GC.Spread.Sheets.ConditionalFormatting.Top10ConditionType.top);
top.rank(3);
top.style(style1);
top.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 1)]);
top.stopIfTrue(true);
activeSheet.conditionalFormats.addRule(top);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`RuleType`](../enums/GC.Spread.Sheets.ConditionalFormatting.RuleType.md) | 规则的类型。 |

#### Returns

`any`

如果未设置值，则返回规则的类型；否则返回条件规则。

#### Inherited from

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[ruleType](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#ruletype)

___

### <a id="stopiftrue" name="stopiftrue"></a> stopIfTrue

▸ **stopIfTrue**(`value?`): `boolean`

获取条件评估为 `true` 时是否应停止评估。

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`boolean`

#### Overrides

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[stopIfTrue](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#stopiftrue)

___

### <a id="style" name="style"></a> style

▸ **style**(`value?`): `any`

获取或设置规则的样式。

**`example`**
```
//此示例应用多个规则。
activeSheet.setArray(0,0,[1,2,3,4,5,6,7,8,9,10]);
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
style.foreColor = "black";
var cell = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
cell.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.cellValueRule);
cell.operator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.greaterThan);
cell.value1(5);
cell.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 1)]);
cell.style(style);
activeSheet.conditionalFormats.addRule(cell);
var style1 = new GC.Spread.Sheets.Style();
style1.foreColor = "red";
var top = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
top.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.top10Rule);
top.type(GC.Spread.Sheets.ConditionalFormatting.Top10ConditionType.top);
top.rank(3);
top.style(style1);
top.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 1)]);
top.stopIfTrue(true);
activeSheet.conditionalFormats.addRule(top);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`Style`](GC.Spread.Sheets.Style.md) | 规则的样式。 |

#### Returns

`any`

如果未设置值，则返回规则的样式；否则返回条件规则。

#### Inherited from

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[style](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#style)
