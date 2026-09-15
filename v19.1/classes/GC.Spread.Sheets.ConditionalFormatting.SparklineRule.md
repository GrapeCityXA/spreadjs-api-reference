# Class: SparklineRule

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).SparklineRule

## Hierarchy

- [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

  ↳ **`SparklineRule`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.ConditionalFormatting.SparklineRule.md#constructor)

### Methods

- [condition](GC.Spread.Sheets.ConditionalFormatting.SparklineRule.md#condition)
- [contains](GC.Spread.Sheets.ConditionalFormatting.SparklineRule.md#contains)
- [createCondition](GC.Spread.Sheets.ConditionalFormatting.SparklineRule.md#createcondition)
- [evaluate](GC.Spread.Sheets.ConditionalFormatting.SparklineRule.md#evaluate)
- [getExpected](GC.Spread.Sheets.ConditionalFormatting.SparklineRule.md#getexpected)
- [intersects](GC.Spread.Sheets.ConditionalFormatting.SparklineRule.md#intersects)
- [isScaleRule](GC.Spread.Sheets.ConditionalFormatting.SparklineRule.md#isscalerule)
- [priority](GC.Spread.Sheets.ConditionalFormatting.SparklineRule.md#priority)
- [ranges](GC.Spread.Sheets.ConditionalFormatting.SparklineRule.md#ranges)
- [reset](GC.Spread.Sheets.ConditionalFormatting.SparklineRule.md#reset)
- [ruleType](GC.Spread.Sheets.ConditionalFormatting.SparklineRule.md#ruletype)
- [showSparklineOnly](GC.Spread.Sheets.ConditionalFormatting.SparklineRule.md#showsparklineonly)
- [sparklineOptions](GC.Spread.Sheets.ConditionalFormatting.SparklineRule.md#sparklineoptions)
- [sparklineType](GC.Spread.Sheets.ConditionalFormatting.SparklineRule.md#sparklinetype)
- [stopIfTrue](GC.Spread.Sheets.ConditionalFormatting.SparklineRule.md#stopiftrue)
- [style](GC.Spread.Sheets.ConditionalFormatting.SparklineRule.md#style)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new SparklineRule**(`type`, `sparklineOptions?`, `ranges?`)

表示一种迷你图规则，用于基于条件格式在单元格中呈现迷你图。

**`example`**
```javascript
// 示例 1：使用选项对象创建 HBar 迷你图规则
activeSheet.setArray(0, 0, [[0.2], [0.5], [0.75], [1.0], [0.6]]);
var rule = new GC.Spread.Sheets.ConditionalFormatting.SparklineRule('HBARSPARKLINE', {
    value: '@',
    colorScheme: 'green'
}, [new GC.Spread.Sheets.Range(0, 0, 5, 1)]);
activeSheet.conditionalFormats.addRule(rule);

// 示例 2：使用位置参数数组创建 YEARSPARKLINE 规则
// 这将生成：=YEARSPARKLINE(2026, A2:B13, , , "#979797", "#f3f3f3")
// 模拟全年活动高峰，夏季和秋季更为繁忙。
activeSheet.setArray(1, 0, [
    [new Date(2026, 0, 5), 2],
    [new Date(2026, 1, 14), 3],
    [new Date(2026, 2, 27), 4],
    [new Date(2026, 3, 10), 6],
    [new Date(2026, 4, 22), 5],
    [new Date(2026, 5, 18), 8],
    [new Date(2026, 6, 9), 7],
    [new Date(2026, 7, 25), 6],
    [new Date(2026, 8, 16), 9],
    [new Date(2026, 9, 28), 10],
    [new Date(2026, 10, 11), 7],
    [new Date(2026, 11, 20), 4]
]);
var rule2 = new GC.Spread.Sheets.ConditionalFormatting.SparklineRule('YEARSPARKLINE',
    [2026, 'A2:B13', undefined, undefined, '#979797', '#f3f3f3'],
    [new GC.Spread.Sheets.Range(0, 0, 1, 1)]);
activeSheet.conditionalFormats.addRule(rule2);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | [`SparklineExType`](../modules/GC.Spread.Sheets.Sparklines.md#sparklineextype) | 迷你图函数名称（例如 'PIESPARKLINE'、'BULLETSPARKLINE'、'HBARSPARKLINE'，或自定义迷你图函数名称）。 |
| `sparklineOptions?` | [`ISparklineOptions`](../modules/GC.Spread.Sheets.Sparklines.md#isparklineoptions) \| [`SparklineParameterType`](../modules/GC.Spread.Sheets.Sparklines.md#sparklineparametertype)[] | - |
| `ranges?` | [`Range`](GC.Spread.Sheets.Range.md)[] | - |

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

▸ **evaluate**(`evaluator`, `baseRow`, `baseColumn`, `actual`): `any`

如果单元格位于规则区域内，则返回该规则的迷你图值。

**`example`**
```javascript
var rule = new GC.Spread.Sheets.ConditionalFormatting.SparklineRule('HBARSPARKLINE', {value: '@'}, [new GC.Spread.Sheets.Range(0, 0, 5, 1)]);
activeSheet.setArray(0, 0, [[0.2], [0.5], [0.75], [1.0], [0.6]]);
activeSheet.conditionalFormats.addRule(rule);
var result = rule.evaluate(activeSheet, 0, 0, 0.5);
console.log(result);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `evaluator` | `Object` | 计算器（工作表）。 |
| `baseRow` | `number` | 行索引。 |
| `baseColumn` | `number` | 列索引。 |
| `actual` | `Object` | 单元格的实际值。 |

#### Returns

`any`

如果单元格在区域内，则返回值对象；否则返回 null。

#### Overrides

[ConditionRuleBase](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md).[evaluate](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md#evaluate)

___

### <a id="getexpected" name="getexpected"></a> getExpected

▸ **getExpected**(): [`Style`](GC.Spread.Sheets.Style.md)

获取基础规则的样式。

**`example`**
```javascript
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
```javascript
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
```javascript
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

将规则重置为默认状态。

**`example`**
```javascript
activeSheet.setArray(0, 0, [[0.2], [0.5], [0.75], [1.0], [0.6], [0.25], [0.35], [0.15], [0.45], [0.3]]);
var rule = new GC.Spread.Sheets.ConditionalFormatting.SparklineRule('HBARSPARKLINE', {value: '@'}, [new GC.Spread.Sheets.Range(0, 0, 5, 1)]);
activeSheet.conditionalFormats.addRule(rule);
rule.reset();
rule.sparklineOptions({
   value: '@',
   colorScheme: 'blue'
});
rule.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 1)]);
activeSheet.refresh();
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
```javascript
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

### <a id="showsparklineonly" name="showsparklineonly"></a> showSparklineOnly

▸ **showSparklineOnly**(`value?`): `any`

获取或设置是否仅显示迷你图而不显示单元格文本。

**`example`**
```javascript
// 此示例使用 showSparklineOnly 方法。
activeSheet.setValue(0, 0, 50);
activeSheet.setValue(1, 0, 75);
activeSheet.setValue(2, 0, 25);
var sparklineRule = new GC.Spread.Sheets.ConditionalFormatting.SparklineRule('HBARSPARKLINE', {
    value: '@',
    colorScheme: 'green'
}, [new GC.Spread.Sheets.Range(0, 0, 3, 1)]);
sparklineRule.showSparklineOnly(true);
activeSheet.conditionalFormats.addRule(sparklineRule);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否仅显示迷你图而不显示单元格文本。 |

#### Returns

`any`

如果未设置值，则返回是否仅显示迷你图而不显示单元格文本；否则返回迷你图规则。

___

### <a id="sparklineoptions" name="sparklineoptions"></a> sparklineOptions

▸ **sparklineOptions**(`value?`): `any`

获取或设置迷你图选项。

**`example`**
```javascript
// 示例 1：使用选项对象创建 HBar 迷你图规则
activeSheet.setArray(0, 0, [[0.2], [0.3], [0.5], [0.1], [0.4], [0.25], [0.35], [0.15], [0.45], [0.3]]);
var rule = new GC.Spread.Sheets.ConditionalFormatting.SparklineRule('PIESPARKLINE', {
    'range|percentage': '@',
    colors: ['red', 'green', 'blue']
}, [new GC.Spread.Sheets.Range(0, 0, 10, 1)]);
activeSheet.conditionalFormats.addRule(rule);
console.log(rule.sparklineOptions()); // { 'range|percentage': '@', colors: ['red', 'green', 'blue'] }

// 示例 2：使用位置参数数组创建 YEARSPARKLINE 规则
rule.sparklineOptions(['@', 'skyblue', 'orange', 'lightgray']);
activeSheet.refresh();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`ISparklineOptions`](../modules/GC.Spread.Sheets.Sparklines.md#isparklineoptions) \| [`SparklineParameterType`](../modules/GC.Spread.Sheets.Sparklines.md#sparklineparametertype)[] | 迷你图选项，可以是以下两种形式之一：   - 带命名参数的选项对象（适用于参数顺序已知的内置迷你图）。   - 位置参数数组（用于自定义迷你图或显式参数排序）。   支持特殊占位符：`$CF_RANGE$`（会替换为规则的区域字符串）和 `@`（会替换为当前单元格值，或在 pointIndex 等索引参数中替换为当前单元格索引）。 |

#### Returns

`any`

如果未设置值，则返回迷你图选项；否则返回迷你图规则。

___

### <a id="sparklinetype" name="sparklinetype"></a> sparklineType

▸ **sparklineType**(): [`SparklineExType`](../modules/GC.Spread.Sheets.Sparklines.md#sparklineextype)

获取迷你图函数类型名称。

**`example`**
```javascript
activeSheet.setArray(0, 0, [[0.2], [0.5], [0.75], [1.0], [0.6]]);
var rule = new GC.Spread.Sheets.ConditionalFormatting.SparklineRule('HBARSPARKLINE', {value: '@'}, [new GC.Spread.Sheets.Range(0, 0, 5, 1)]);
activeSheet.conditionalFormats.addRule(rule);
console.log(rule.sparklineType()); // 'HBARSPARKLINE'
```

#### Returns

[`SparklineExType`](../modules/GC.Spread.Sheets.Sparklines.md#sparklineextype)

迷你图类型名称（例如 'PIESPARKLINE'）。

___

### <a id="stopiftrue" name="stopiftrue"></a> stopIfTrue

▸ **stopIfTrue**(`value?`): `any`

获取或设置是否在规则之前应用优先级较低的规则。

**`example`**
```javascript
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
```javascript
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
