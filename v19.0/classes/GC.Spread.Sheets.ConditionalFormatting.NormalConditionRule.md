# Class: NormalConditionRule

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).NormalConditionRule

## Hierarchy

- [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

  ↳ **`NormalConditionRule`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule.md#constructor)

### Methods

- [condition](GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule.md#condition)
- [contains](GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule.md#contains)
- [createCondition](GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule.md#createcondition)
- [evaluate](GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule.md#evaluate)
- [formula](GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule.md#formula)
- [getExpected](GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule.md#getexpected)
- [intersects](GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule.md#intersects)
- [isScaleRule](GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule.md#isscalerule)
- [operator](GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule.md#operator)
- [priority](GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule.md#priority)
- [ranges](GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule.md#ranges)
- [rank](GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule.md#rank)
- [reset](GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule.md#reset)
- [ruleType](GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule.md#ruletype)
- [stopIfTrue](GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule.md#stopiftrue)
- [style](GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule.md#style)
- [text](GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule.md#text)
- [type](GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule.md#type)
- [value1](GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule.md#value1)
- [value2](GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule.md#value2)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new NormalConditionRule**(`ruleType`, `ranges`, `style`, `operator`, `value1`, `value2`, `text`, `formula`, `type`, `rank`)

表示一个普通条件规则。

**`example`**
```
activeSheet.setArray(0,0,[1,2,3,4,5,6,7,8,9,10]);
var cell = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
cell.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.cellValueRule);
cell.operator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.greaterThan);
cell.value1(5);
cell.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 1)]);
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
cell.style(style);
activeSheet.conditionalFormats.addRule(cell);
//button
$("#button1").click(function () {
     cell.reset();
     activeSheet.suspendPaint();
     activeSheet.resumePaint();
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ruleType` | [`RuleType`](../enums/GC.Spread.Sheets.ConditionalFormatting.RuleType.md) | 条件格式规则的类型。 |
| `ranges` | [`Range`](GC.Spread.Sheets.Range.md)[] | 应用规则的单元格范围，其项目类型为 GC.Spread.Sheets.Range。 |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 满足条件时应用于单元格的样式。 |
| `operator` | [`LogicalOperators`](../enums/GC.Spread.Sheets.ConditionalFormatting.LogicalOperators.md) \| [`ComparisonOperators`](../enums/GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.md) \| [`TextComparisonOperators`](../enums/GC.Spread.Sheets.ConditionalFormatting.TextComparisonOperators.md) | 比较运算符。 |
| `value1` | `Object` | 第一个值。 |
| `value2` | `Object` | 第二个值。 |
| `text` | `string` | 用于比较的文本。 |
| `formula` | `string` | 条件公式。 |
| `type` | [`AverageConditionType`](../enums/GC.Spread.Sheets.ConditionalFormatting.AverageConditionType.md) \| [`DateOccurringType`](../enums/GC.Spread.Sheets.ConditionalFormatting.DateOccurringType.md) \| [`Top10ConditionType`](../enums/GC.Spread.Sheets.ConditionalFormatting.Top10ConditionType.md) | 平均条件类型。 |
| `rank` | `number` | 要应用样式的顶部或底部项目的数量。 |

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

**`example`**
```javascript
var rule = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
rule.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.formulaRule);
rule.formula("=A1=B1+C1");
var condition = rule.createCondition();
console.log(condition.evaluate(activeSheet));
```

#### Returns

[`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

条件。

#### Overrides

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[createCondition](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#createcondition)

___

### <a id="evaluate" name="evaluate"></a> evaluate

▸ **evaluate**(`evaluator`, `baseRow`, `baseColumn`, `actual`): [`Style`](GC.Spread.Sheets.Style.md)

如果单元格满足条件，则返回规则的单元格样式。

**`example`**
```javascript
 activeSheet.setValue(0, 0, 1, 3);
 activeSheet.setValue(1, 0, 15, 3);
 activeSheet.setValue(2, 0, 25, 3);
 activeSheet.setValue(3, 0, -1, 3);
 var iconSetRule = new GC.Spread.Sheets.ConditionalFormatting.IconSetRule();
 iconSetRule.ranges([new GC.Spread.Sheets.Range(0, 0, 4, 1)]);
 iconSetRule.iconSetType(GC.Spread.Sheets.ConditionalFormatting.IconSetType.fourTrafficLights);
 activeSheet.conditionalFormats.addRule(iconSetRule);
 for (var i = 1; i < 5; i++) {
     var evaluateResult = iconSetRule.evaluate(activeSheet, i, 0, activeSheet.getValue(i, 0));
     console.log(evaluateResult);
 }
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `evaluator` | `Object` | 可以评估条件的对象。 |
| `baseRow` | `number` | 行索引。 |
| `baseColumn` | `number` | 列索引。 |
| `actual` | `Object` | 实际值。 |

#### Returns

[`Style`](GC.Spread.Sheets.Style.md)

规则的单元格样式。

#### Inherited from

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[evaluate](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#evaluate)

___

### <a id="formula" name="formula"></a> formula

▸ **formula**(`formulaOrBaseRow?`, `baseColumn?`): `any`

获取或设置条件公式。

**`example`**
```
//此示例使用 formula 方法。
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
var rule = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
rule.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.formulaRule);
rule.formula("=A1=B1+C1");
rule.ranges([new GC.Spread.Sheets.Range(0, 0, 2, 1)]);
rule.style(style);
activeSheet.conditionalFormats.addRule(rule);
activeSheet.setValue(0, 0, 2,3);
activeSheet.setValue(0, 1, 1,3);
activeSheet.setValue(0, 2,1,3);
activeSheet.setValue(1, 0, 1,3);
var formulaOfTheTopLeftCell = rule.formula();
var formulaOfA1 = rule.formula(0, 0);
var formulaOfA2 = rule.formula(1, 0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `formulaOrBaseRow?` | `string` \| `number` | 条件公式或基准行。 |
| `baseColumn?` | `number` | 基准列。 |

#### Returns

`any`

如果未设置值或设置了 baseRow 和 baseColumn，则返回条件公式；否则返回数字条件规则。

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

### <a id="operator" name="operator"></a> operator

▸ **operator**(`value?`): `any`

Gets or sets the comparison operator.

**`example`**
```
//This example creates multiple rules.
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
| `value?` | [`ComparisonOperators`](../enums/GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.md) | The comparison operator. |

#### Returns

`any`

If no value is set, returns the comparison operator; otherwise, returns the number condition rule.

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

### <a id="rank" name="rank"></a> rank

▸ **rank**(`value?`): `any`

获取或设置要应用样式的顶部或底部项目的数量。

**`example`**
```
//此示例创建多个规则。
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
| `value?` | `number` | 要应用样式的顶部或底部项目的数量。 |

#### Returns

`any`

如果未设置值，则返回要应用样式的顶部或底部项目的数量；否则返回数字条件规则。

___

### <a id="reset" name="reset"></a> reset

▸ **reset**(): `void`

重置规则。

**`example`**
```
activeSheet.setValue(0,0, 1,3);
activeSheet.setValue(1,0, 50,3);
activeSheet.setValue(2,0, 100,3);
activeSheet.setValue(3,0, 2,3);
activeSheet.setValue(4,0, 60,3);
activeSheet.setValue(5,0, 90,3);
activeSheet.setValue(6,0, 3,3);
activeSheet.setValue(7,0, 40,3);
activeSheet.setValue(8,0, 70,3);
activeSheet.setValue(9,0, 5,3);
activeSheet.setValue(10,0, 35,3);
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
style.borderLeft =new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderTop = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderRight = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderBottom = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
var rule = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
rule.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.averageRule);
rule.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 3)]);
rule.style(style);
rule.type(GC.Spread.Sheets.ConditionalFormatting.AverageConditionType.above);
activeSheet.conditionalFormats.addRule(rule);
rule.reset();
```

#### Returns

`void`

#### Overrides

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

▸ **stopIfTrue**(`value?`): `any`

获取或设置是否在规则之前应用优先级较低的规则。

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
| `value?` | `boolean` | 是否在规则之前应用优先级较低的规则。 |

#### Returns

`any`

如果未设置值，则返回是否不应用优先级较低的规则；否则返回条件规则。

#### Inherited from

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

___

### <a id="text" name="text"></a> text

▸ **text**(`value?`): `any`

获取或设置用于比较的文本。

**`example`**
```
//此示例创建一个规则。
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
var rule = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
rule.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.specificTextRule);
rule.style(style);
rule.text("test");
rule.operator(GC.Spread.Sheets.ConditionalFormatting.TextComparisonOperators.contains);
rule.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 1)]);
activeSheet.conditionalFormats.addRule(rule);
activeSheet.setValue(0, 0, "testing");
activeSheet.setValue(1, 0, "test");
activeSheet.setValue(2, 0, "a");
activeSheet.setValue(3, 0, "t");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 用于比较的文本。 |

#### Returns

`any`

如果未设置值，则返回用于比较的文本；否则返回数字条件规则。

___

### <a id="type" name="type"></a> type

▸ **type**(`value?`): `any`

获取或设置平均值条件类型。

**`example`**
```
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
| `value?` | [`AverageConditionType`](../enums/GC.Spread.Sheets.ConditionalFormatting.AverageConditionType.md) | 平均值条件类型。 |

#### Returns

`any`

如果未设置值，则返回平均值条件类型；否则返回数字条件规则。

___

### <a id="value1" name="value1"></a> value1

▸ **value1**(`valueOrBaseRow?`, `baseColumn?`): `any`

获取或设置第一个值。

**`example`**
```
//此示例创建多个规则。
activeSheet.setArray(0,0,[[1,10],[2,9], [3,8],[4,7],[5,6],[6,5],[7,4],[8,3],[9,2],[10,1]]);
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
style.foreColor = "black";
var cell = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
cell.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.cellValueRule);
cell.operator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.greaterThan);
cell.value1("=B1");
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
var formulaOfTheTopLeftCell = cell.value1();
var formulaOfA5 = cell.value1(4, 0);
var formulaOfA10 = cell.value1(9, 0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `valueOrBaseRow?` | `any` | 第一个值或基准行。 |
| `baseColumn?` | `number` | 基准列。 |

#### Returns

`any`

如果未设置值或设置了baseRow和baseColumn，则返回第一个值；否则返回数字条件规则。

___

### <a id="value2" name="value2"></a> value2

▸ **value2**(`valueOrBaseRow?`, `baseColumn?`): `any`

获取或设置第二个值。

**`example`**
```
//此示例使用value2方法。
activeSheet.setArray(0,0,[1,2,3,4,5,6,7,8,9,10]);
var cell = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
cell.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.cellValueRule);
cell.operator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.between);
cell.value1(5);
cell.value2(7);
cell.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 1)]);
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
style.foreColor = "black";
cell.style(style);
activeSheet.conditionalFormats.addRule(cell);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `valueOrBaseRow?` | `any` | 第二个值或基准行。 |
| `baseColumn?` | `number` | 基准列。 |

#### Returns

`any`

如果未设置值或设置了baseRow和baseColumn，则返回第二个值；否则返回数字条件规则。
