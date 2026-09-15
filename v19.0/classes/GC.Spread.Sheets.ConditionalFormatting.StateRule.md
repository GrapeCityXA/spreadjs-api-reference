# Class: StateRule

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).StateRule

## Hierarchy

- [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

  ↳ **`StateRule`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.ConditionalFormatting.StateRule.md#constructor)

### Methods

- [condition](GC.Spread.Sheets.ConditionalFormatting.StateRule.md#condition)
- [contains](GC.Spread.Sheets.ConditionalFormatting.StateRule.md#contains)
- [createCondition](GC.Spread.Sheets.ConditionalFormatting.StateRule.md#createcondition)
- [evaluate](GC.Spread.Sheets.ConditionalFormatting.StateRule.md#evaluate)
- [getExpected](GC.Spread.Sheets.ConditionalFormatting.StateRule.md#getexpected)
- [intersects](GC.Spread.Sheets.ConditionalFormatting.StateRule.md#intersects)
- [isRow](GC.Spread.Sheets.ConditionalFormatting.StateRule.md#isrow)
- [isScaleRule](GC.Spread.Sheets.ConditionalFormatting.StateRule.md#isscalerule)
- [priority](GC.Spread.Sheets.ConditionalFormatting.StateRule.md#priority)
- [ranges](GC.Spread.Sheets.ConditionalFormatting.StateRule.md#ranges)
- [reset](GC.Spread.Sheets.ConditionalFormatting.StateRule.md#reset)
- [ruleType](GC.Spread.Sheets.ConditionalFormatting.StateRule.md#ruletype)
- [state](GC.Spread.Sheets.ConditionalFormatting.StateRule.md#state)
- [stopIfTrue](GC.Spread.Sheets.ConditionalFormatting.StateRule.md#stopiftrue)
- [style](GC.Spread.Sheets.ConditionalFormatting.StateRule.md#style)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new StateRule**(`ruleType`, `state`, `style?`, `ranges?`)

表示一个状态规则。

**`example`**
```
// 在整个工作表中添加一个带有红色背景的行状态规则
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
var stateRule = new GC.Spread.Sheets.ConditionalFormatting.StateRule(
     GC.Spread.Sheets.ConditionalFormatting.RuleType.rowStateRule,
     GC.Spread.Sheets.RowColumnStates.active,
     style, [new GC.Spread.Sheets.Range(-1, -1, -1, -1)]
);
activeSheet.conditionalFormats.addRule(stateRule);
// 添加一个行状态规则，为不同的对应范围设置两种样式。
var stateRule2 = new GC.Spread.Sheets.ConditionalFormatting.StateRule(
     GC.Spread.Sheets.ConditionalFormatting.RuleType.rowStateRule,
     GC.Spread.Sheets.RowColumnStates.dirty,
     [new GC.Spread.Sheets.Style("green"), new GC.Spread.Sheets.Style("red")],
     [new GC.Spread.Sheets.Range(1, 1, 10, 5), new GC.Spread.Sheets.Range(1, 7, 10, 5)]
);
activeSheet.conditionalFormats.addRule(stateRule2);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ruleType` | [`RuleType`](../enums/GC.Spread.Sheets.ConditionalFormatting.RuleType.md) | 状态规则类型，可以是 GC.Spread.Sheets.ConditionalFormatting.RuleType.rowStateRule 或 GC.Spread.Sheets.ConditionalFormatting.RuleType.columnStateRule。 |
| `state` | [`RowColumnStates`](../enums/GC.Spread.Sheets.RowColumnStates.md) | 状态。 |
| `style?` | [`Style`](GC.Spread.Sheets.Style.md) \| [`Style`](GC.Spread.Sheets.Style.md)[] | 当满足状态条件时应用于单元格的样式。可以是样式数组。 |
| `ranges?` | [`Range`](GC.Spread.Sheets.Range.md)[] | 应用规则的单元格范围，其项类型为 GC.Spread.Sheets.Range。 |

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

#### Inherited from

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

### <a id="isrow" name="isrow"></a> isRow

▸ **isRow**(): `boolean`

获取此状态规则是否应用于行方向。

**`example`**
```javascript
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
var stateRule = new GC.Spread.Sheets.ConditionalFormatting.StateRule(
     GC.Spread.Sheets.ConditionalFormatting.RuleType.rowStateRule,
     GC.Spread.Sheets.RowColumnStates.active,
     style, [new GC.Spread.Sheets.Range(-1, -1, -1, -1)]
);
activeSheet.conditionalFormats.addRule(stateRule);
console.log(stateRule.isRow());
var stateRule2 = new GC.Spread.Sheets.ConditionalFormatting.StateRule(
     GC.Spread.Sheets.ConditionalFormatting.RuleType.columnStateRule,
     GC.Spread.Sheets.RowColumnStates.active,
     style, [new GC.Spread.Sheets.Range(-1, -1, -1, -1)]
);
activeSheet.conditionalFormats.addRule(stateRule2);
console.log(stateRule2.isRow());
```

#### Returns

`boolean`

此状态规则是否应用于行方向，否则将应用于列方向。

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

### <a id="state" name="state"></a> state

▸ **state**(`value?`): [`RowColumnStates`](../enums/GC.Spread.Sheets.RowColumnStates.md)

获取或设置规则状态。

**`example`**
```javascript
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
var stateRule = new GC.Spread.Sheets.ConditionalFormatting.StateRule(
     GC.Spread.Sheets.ConditionalFormatting.RuleType.rowStateRule,
     GC.Spread.Sheets.RowColumnStates.active,
     style, [new GC.Spread.Sheets.Range(-1, -1, -1, -1)]
);
activeSheet.conditionalFormats.addRule(stateRule);
console.log(stateRule.state()); // 获取当前状态
stateRule.state(GC.Spread.Sheets.ConditionalFormatting.RuleType.columnStateRule); // 修改状态为列状态规则
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`RowColumnStates`](../enums/GC.Spread.Sheets.RowColumnStates.md) | 状态。 |

#### Returns

[`RowColumnStates`](../enums/GC.Spread.Sheets.RowColumnStates.md)

规则状态。

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
