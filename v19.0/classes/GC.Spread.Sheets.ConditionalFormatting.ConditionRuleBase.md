# Class: ConditionRuleBase

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).ConditionRuleBase

## Hierarchy

- **`ConditionRuleBase`**

  ↳ [`NormalConditionRule`](GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule.md)

  ↳ [`ScaleRule`](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md)

  ↳ [`StateRule`](GC.Spread.Sheets.ConditionalFormatting.StateRule.md)

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#constructor)

### Methods

- [condition](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#condition)
- [contains](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#contains)
- [createCondition](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#createcondition)
- [evaluate](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#evaluate)
- [getExpected](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#getexpected)
- [intersects](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#intersects)
- [isScaleRule](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#isscalerule)
- [priority](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#priority)
- [ranges](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#ranges)
- [reset](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#reset)
- [ruleType](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#ruletype)
- [stopIfTrue](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#stopiftrue)
- [style](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#style)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new ConditionRuleBase**(`ruleType`, `style`, `ranges`)

表示具有指定样式的格式化基础规则类。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ruleType` | [`RuleType`](../enums/GC.Spread.Sheets.ConditionalFormatting.RuleType.md) | 条件格式化规则的类型。 |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 规则的样式。 |
| `ranges` | [`Range`](GC.Spread.Sheets.Range.md)[] | 范围数组。 |

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

___

### <a id="isscalerule" name="isscalerule"></a> isScaleRule

▸ **isScaleRule**(): `boolean`

指定此规则是否为比例规则。

#### Returns

`boolean`

如果此规则是比例规则，则为 `true`；否则为 `false`。

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
