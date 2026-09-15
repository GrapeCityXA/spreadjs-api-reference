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

状态规则

**`代码示例`**
```
// 在整个工作表中添加一个红色背景的行状态规则
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
var stateRule = new GC.Spread.Sheets.ConditionalFormatting.StateRule(GC.Spread.Sheets.ConditionalFormatting.RuleType.rowStateRule, style, [new GC.Spread.Sheets.Range(-1, -1, -1, -1)]);
activeSheet.conditionalFormats.addRule(cell);
// add a row state rule with two styles to different corresponding ranges
var stateRule = new GC.Spread.Sheets.ConditionalFormatting.StateRule(
     GC.Spread.Sheets.ConditionalFormatting.RuleType.rowStateRule,
     [new GC.Spread.Sheets.Style("green"), new GC.Spread.Sheets.Style("red")],
     [new GC.Spread.Sheets.Range(1, 1, 10, 5)\uff0c new GC.Spread.Sheets.Range(1, 7, 10, 5)]
);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ruleType` | [`RuleType`](../enums/GC.Spread.Sheets.ConditionalFormatting.RuleType.md) | 状态规则类型,它将是GC.Spread.Sheet.ConditionalFormatting.RuleType.rowStateRule或GC.Spread.Sheet.ConditionalFormatting.RuleType.columnStateRule |
| `state` | [`RowColumnStates`](../enums/GC.Spread.Sheets.RowColumnStates.md) | 状态 |
| `style?` | [`Style`](GC.Spread.Sheets.Style.md) \| [`Style`](GC.Spread.Sheets.Style.md)[] | 满足状态时应用于单元格的样式 It could an array of styles. |
| `ranges?` | [`Range`](GC.Spread.Sheets.Range.md)[] | 项类型为GC.Spread.Sheets.Range的应用规则的单元格区域 |

#### Overrides

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[constructor](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#constructor)

## Methods

### <a id="condition" name="condition"></a> condition

▸ **condition**(`value?`): `any`

获取或设置规则的基本条件

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md) | 规则的基本条件 |

#### Returns

`any`

如果未设置任何值,则返回规则的基本条件否则,返回条件规则

#### Inherited from

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[condition](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#condition)

___

### <a id="contains" name="contains"></a> contains

▸ **contains**(`row`, `column`): `boolean`

确定单元格区域是否包含指定行和列的单元格

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |
| `column` | `number` | 列索引 |

#### Returns

`boolean`

如果单元格区域包含指定行和列中的单元格,返回true;否则返回false

#### Inherited from

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[contains](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#contains)

___

### <a id="createcondition" name="createcondition"></a> createCondition

▸ **createCondition**(): [`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

为规则创建条件

#### Returns

[`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

条件

#### Inherited from

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[createCondition](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#createcondition)

___

### <a id="evaluate" name="evaluate"></a> evaluate

▸ **evaluate**(`evaluator`, `baseRow`, `baseColumn`, `actual`): [`Style`](GC.Spread.Sheets.Style.md)

如果单元格满足条件,则返回规则的单元格样式

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `evaluator` | `Object` | 可以计算条件的对象 |
| `baseRow` | `number` | 行索引 |
| `baseColumn` | `number` | 列索引 |
| `actual` | `Object` | 实际值 |

#### Returns

[`Style`](GC.Spread.Sheets.Style.md)

规则的单元格样式

#### Inherited from

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[evaluate](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#evaluate)

___

### <a id="getexpected" name="getexpected"></a> getExpected

▸ **getExpected**(): [`Style`](GC.Spread.Sheets.Style.md)

获取基本规则的样式

#### Returns

[`Style`](GC.Spread.Sheets.Style.md)

#### Inherited from

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[getExpected](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#getexpected)

___

### <a id="intersects" name="intersects"></a> intersects

▸ **intersects**(`row`, `column`, `rowCount`, `columnCount`): `boolean`

此规则的区域是否与另一个区域相交

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |
| `column` | `number` | 列索引 |
| `rowCount` | `number` | 行数 |
| `columnCount` | `number` | 列数 |

#### Returns

`boolean`

如果此规则的区域与另一个区域相交,返回true;否则返回false

#### Inherited from

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[intersects](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#intersects)

___

### <a id="isrow" name="isrow"></a> isRow

▸ **isRow**(): `boolean`

获取此状态规则是否将应用于行的方向

#### Returns

`boolean`

该状态规则是否适用于行方向,否则,将适用于列方向

___

### <a id="isscalerule" name="isscalerule"></a> isScaleRule

▸ **isScaleRule**(): `boolean`

此规则是否为缩放规则

#### Returns

`boolean`

如果此规则是缩放规则,返回true;否则返回false

#### Inherited from

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[isScaleRule](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#isscalerule)

___

### <a id="priority" name="priority"></a> priority

▸ **priority**(`value?`): `any`

获取或设置规则的优先级

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 规则的优先级 |

#### Returns

`any`

如果未设置任何值,则返回规则的优先级否则,返回条件规则

#### Inherited from

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[priority](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#priority)

___

### <a id="ranges" name="ranges"></a> ranges

▸ **ranges**(`value?`): `any`

获取或设置条件规则区域

**`代码示例`**
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
| `value?` | [`Range`](GC.Spread.Sheets.Range.md)[] | 条件规则区域 |

#### Returns

`any`

如果未设置任何值,则返回条件规则区域否则,返回条件规则

#### Inherited from

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[ranges](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#ranges)

___

### <a id="reset" name="reset"></a> reset

▸ **reset**(): `void`

重置规则

#### Returns

`void`

#### Inherited from

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[reset](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#reset)

___

### <a id="ruletype" name="ruletype"></a> ruleType

▸ **ruleType**(`value?`): `any`

获取或设置条件规则类型

**`代码示例`**
```
//本示例使用ruleType方法
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
| `value?` | [`RuleType`](../enums/GC.Spread.Sheets.ConditionalFormatting.RuleType.md) | 条件规则类型 |

#### Returns

`any`

如果未设置任何值,则返回条件规则类型否则,返回条件规则

#### Inherited from

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[ruleType](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#ruletype)

___

### <a id="state" name="state"></a> state

▸ **state**(`value?`): [`RowColumnStates`](../enums/GC.Spread.Sheets.RowColumnStates.md)

获取或设置规则状态

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`RowColumnStates`](../enums/GC.Spread.Sheets.RowColumnStates.md) | 状态 |

#### Returns

[`RowColumnStates`](../enums/GC.Spread.Sheets.RowColumnStates.md)

规则状态

___

### <a id="stopiftrue" name="stopiftrue"></a> stopIfTrue

▸ **stopIfTrue**(`value?`): `any`

获取或设置是否在此规则之前应用优先级较低的规则

**`代码示例`**
```
//本示例应用了多个规则
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
| `value?` | `boolean` | 是否在此规则之前应用优先级较低的规则 |

#### Returns

`any`

如果未设置任何值,则返回在此规则之前是否应用优先级较低的规则;否则,返回条件规则

#### Inherited from

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[stopIfTrue](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#stopiftrue)

___

### <a id="style" name="style"></a> style

▸ **style**(`value?`): `any`

获取或设置规则的样式

**`代码示例`**
```
//本示例应用了多个规则
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
| `value?` | [`Style`](GC.Spread.Sheets.Style.md) | 规则的样式 |

#### Returns

`any`

如果未设置任何值,则返回规则的样式否则,返回条件规则

#### Inherited from

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[style](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#style)
