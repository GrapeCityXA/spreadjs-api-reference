# Class: IconSetRule

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).IconSetRule

## Hierarchy

- [`ScaleRule`](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md)

  ↳ **`IconSetRule`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#constructor)

### Methods

- [condition](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#condition)
- [contains](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#contains)
- [createCondition](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#createcondition)
- [evaluate](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#evaluate)
- [getExpected](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#getexpected)
- [iconCriteria](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#iconcriteria)
- [iconSetType](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#iconsettype)
- [icons](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#icons)
- [intersects](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#intersects)
- [isScaleRule](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#isscalerule)
- [maxColor](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#maxcolor)
- [maxType](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#maxtype)
- [maxValue](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#maxvalue)
- [midColor](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#midcolor)
- [midType](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#midtype)
- [midValue](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#midvalue)
- [minColor](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#mincolor)
- [minType](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#mintype)
- [minValue](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#minvalue)
- [priority](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#priority)
- [ranges](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#ranges)
- [reset](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#reset)
- [reverseIconOrder](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#reverseiconorder)
- [ruleType](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#ruletype)
- [showIconOnly](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#showicononly)
- [stopIfTrue](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#stopiftrue)
- [style](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#style)
- [getIcon](GC.Spread.Sheets.ConditionalFormatting.IconSetRule.md#geticon)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new IconSetRule**(`iconSetType`, `ranges`)

表示具有指定参数的图标集规则。

**`example`**
```
//此示例创建一个新的图标集规则并设置其范围和图标。
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,15,3);
activeSheet.setValue(2,0,25,3);
activeSheet.setValue(3,0,-1,3);
var iconSetRule = new GC.Spread.Sheets.ConditionalFormatting.IconSetRule();
iconSetRule.ranges([new GC.Spread.Sheets.Range(0,0,4,1)]);
iconSetRule.iconSetType(GC.Spread.Sheets.ConditionalFormatting.IconSetType.fourTrafficLights);
var icons = iconSetRule.icons();
icons[0] = {iconSetType: GC.Spread.Sheets.ConditionalFormatting.IconSetType.fiveArrowsColored, iconIndex: 1};
icons[1] = {iconSetType: GC.Spread.Sheets.ConditionalFormatting.IconSetType.fiveArrowsColored, iconIndex: 2};
icons[2] = {iconSetType: GC.Spread.Sheets.ConditionalFormatting.IconSetType.noIcons, iconIndex: 0};

var iconCriteria = iconSetRule.iconCriteria();
iconCriteria[0] = new GC.Spread.Sheets.ConditionalFormatting.IconCriterion(true, GC.Spread.Sheets.ConditionalFormatting.IconValueType.number, 1);
iconCriteria[1] = new GC.Spread.Sheets.ConditionalFormatting.IconCriterion(true, GC.Spread.Sheets.ConditionalFormatting.IconValueType.number, 10);
iconCriteria[2] = new GC.Spread.Sheets.ConditionalFormatting.IconCriterion(true, GC.Spread.Sheets.ConditionalFormatting.IconValueType.number, 20);
iconSetRule.reverseIconOrder(false);
iconSetRule.showIconOnly(false);
activeSheet.conditionalFormats.addRule(iconSetRule);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `iconSetType` | [`IconSetType`](../enums/GC.Spread.Sheets.ConditionalFormatting.IconSetType.md) | 图标集的类型。 |
| `ranges` | [`Range`](GC.Spread.Sheets.Range.md)[] |  |

#### Overrides

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[constructor](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#constructor)

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

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[condition](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#condition)

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

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[contains](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#contains)

___

### <a id="createcondition" name="createcondition"></a> createCondition

▸ **createCondition**(): [`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

为规则创建条件。

#### Returns

[`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

条件。

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[createCondition](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#createcondition)

___

### <a id="evaluate" name="evaluate"></a> evaluate

▸ **evaluate**(`evaluator`, `baseRow`, `baseColumn`, `actual`): `any`

如果单元格满足条件，则返回指定值。

**`example`**
```
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
| `evaluator` | `Object` | 评估器。 |
| `baseRow` | `number` | 行索引。 |
| `baseColumn` | `number` | 列索引。 |
| `actual` | `Object` | 当前值。 |

#### Returns

`any`

如果单元格满足条件，则返回指定值。

#### Overrides

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[evaluate](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#evaluate)

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

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[getExpected](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#getexpected)

___

### <a id="iconcriteria" name="iconcriteria"></a> iconCriteria

▸ **iconCriteria**(): [`IconCriterion`](GC.Spread.Sheets.ConditionalFormatting.IconCriterion.md)[]

获取图标条件。

**`example`**
```
//此示例创建一个规则。
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
iconSetRule.reverseIconOrder(false);
iconSetRule.showIconOnly(false);
activeSheet.conditionalFormats.addRule(iconSetRule);
```

#### Returns

[`IconCriterion`](GC.Spread.Sheets.ConditionalFormatting.IconCriterion.md)[]

返回的图标条件类型为GC.Spread.Sheets.ConditionalFormatting.IconCriterion。

___

### <a id="iconsettype" name="iconsettype"></a> iconSetType

▸ **iconSetType**(`value?`): `any`

获取或设置图标集的类型。

**`example`**
```
//此示例创建一个规则。
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
iconSetRule.reverseIconOrder(false);
iconSetRule.showIconOnly(false);
activeSheet.conditionalFormats.addRule(iconSetRule);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`IconSetType`](../enums/GC.Spread.Sheets.ConditionalFormatting.IconSetType.md) | 图标集的类型。 |

#### Returns

`any`

如果未设置值，则返回图标集的类型；否则返回图标集规则。

___

### <a id="icons" name="icons"></a> icons

▸ **icons**(`value?`): [`IIconInfo`](../interfaces/GC.Spread.Sheets.ConditionalFormatting.IIconInfo.md)[]

获取或设置图标。

**`example`**
```
//此示例创建一个规则。
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,15,3);
activeSheet.setValue(2,0,25,3);
activeSheet.setValue(3,0,-1,3);

//规则
var iconSetRule = new GC.Spread.Sheets.ConditionalFormatting.IconSetRule();
iconSetRule.ranges([new GC.Spread.Sheets.Range(0,0,4,1)]);
iconSetRule.iconSetType(GC.Spread.Sheets.ConditionalFormatting.IconSetType.fourTrafficLights);
var icons = iconSetRule.icons();
icons[0] = {iconSetType: GC.Spread.Sheets.ConditionalFormatting.IconSetType.fiveArrowsColored, iconIndex: 1};
icons[1] = {iconSetType: GC.Spread.Sheets.ConditionalFormatting.IconSetType.fiveArrowsColored, iconIndex: 2};
icons[2] = {iconSetType: GC.Spread.Sheets.ConditionalFormatting.IconSetType.noIcons, iconIndex: 0};
iconSetRule.reverseIconOrder(false);
iconSetRule.showIconOnly(false);
activeSheet.conditionalFormats.addRule(iconSetRule);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`IIconInfo`](../interfaces/GC.Spread.Sheets.ConditionalFormatting.IIconInfo.md)[] |

#### Returns

[`IIconInfo`](../interfaces/GC.Spread.Sheets.ConditionalFormatting.IIconInfo.md)[]

返回iconInfos数组。

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

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[intersects](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#intersects)

___

### <a id="isscalerule" name="isscalerule"></a> isScaleRule

▸ **isScaleRule**(): `boolean`

指定此规则是否为比例规则。

#### Returns

`boolean`

如果此规则是比例规则，则为 `true`；否则为 `false`。

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[isScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#isscalerule)

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

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[maxColor](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#maxcolor)

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

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[maxType](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#maxtype)

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

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[maxValue](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#maxvalue)

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

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[midColor](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#midcolor)

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

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[midType](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#midtype)

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

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[midValue](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#midvalue)

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

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[minColor](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#mincolor)

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

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[minType](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#mintype)

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

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[minValue](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#minvalue)

___

### <a id="priority" name="priority"></a> priority

▸ **priority**(`value?`): `any`

获取或设置规则的优先级。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 规则的优先级。 |

#### Returns

`any`

如果未设置值，则返回规则的优先级；否则返回条件规则。

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[priority](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#priority)

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

如果未设置值，则返回规则的范围；否则返回条件规则。

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[ranges](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#ranges)

___

### <a id="reset" name="reset"></a> reset

▸ **reset**(): `void`

重置规则。

**`example`**
```
//此示例使用reset方法。
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
iconSetRule.reverseIconOrder(false);
iconSetRule.showIconOnly(false);
activeSheet.conditionalFormats.addRule(iconSetRule);
iconSetRule.reset();
```

#### Returns

`void`

#### Overrides

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[reset](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#reset)

___

### <a id="reverseiconorder" name="reverseiconorder"></a> reverseIconOrder

▸ **reverseIconOrder**(`value?`): `any`

获取或设置是否反转图标顺序。

**`example`**
```
//此示例创建一个规则。
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
iconSetRule.reverseIconOrder(false);
iconSetRule.showIconOnly(false);
activeSheet.conditionalFormats.addRule(iconSetRule);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否反转图标顺序。 |

#### Returns

`any`

如果未设置值，则返回是否反转图标顺序；否则返回图标集规则。

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

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[ruleType](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#ruletype)

___

### <a id="showicononly" name="showicononly"></a> showIconOnly

▸ **showIconOnly**(`value?`): `any`

获取或设置是否仅显示图标。

**`example`**
```
//此示例创建一个规则。
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
iconSetRule.reverseIconOrder(false);
iconSetRule.showIconOnly(false);
activeSheet.conditionalFormats.addRule(iconSetRule);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否仅显示图标。 |

#### Returns

`any`

如果未设置值，则返回是否仅显示图标；否则返回图标集规则。

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

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[stopIfTrue](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#stopiftrue)

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

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[style](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#style)

___

### <a id="geticon" name="geticon"></a> getIcon

▸ `Static` **getIcon**(`iconSetType`, `iconIndex`): `Object`

根据特定的iconSetType和iconIndex对象获取图标。

**`static`**

**`example`**
```
//此示例返回一个图标集规则的图标。
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,15,3);
activeSheet.setValue(2,0,25,3);
activeSheet.setValue(3,0,-1,3);
//获取图标
var base = GC.Spread.Sheets.ConditionalFormatting.IconSetRule.getIcon;
GC.Spread.Sheets.ConditionalFormatting.IconSetRule.getIcon = function (iconSetType, iconIndex) {
     var icon = base.apply(this, arguments);
     if (iconSetType === GC.Spread.Sheets.ConditionalFormatting.IconSetType.threeArrowsColored) {
         if (iconIndex === 0) {
             return "images/Star2.png";
         } else if (iconIndex === 1){
             return "images/Rating4.png";
         } else if (iconIndex === 2) {
             return "images/Box4.png";
         }
     }
     return icon;
};
var iconSetRule = new GC.Spread.Sheets.ConditionalFormatting.IconSetRule();
iconSetRule.ranges([new GC.Spread.Sheets.Range(0,0,4,1)]);
iconSetRule.iconSetType(GC.Spread.Sheets.ConditionalFormatting.IconSetType.threeArrowsColored);
var iconCriteria = iconSetRule.iconCriteria();
iconCriteria[0] = new GC.Spread.Sheets.ConditionalFormatting.IconCriterion(true, GC.Spread.Sheets.ConditionalFormatting.IconValueType.number, 1);
iconCriteria[1] = new GC.Spread.Sheets.ConditionalFormatting.IconCriterion(true, GC.Spread.Sheets.ConditionalFormatting.IconValueType.number, 10);
iconCriteria[2] = new GC.Spread.Sheets.ConditionalFormatting.IconCriterion(true, GC.Spread.Sheets.ConditionalFormatting.IconValueType.number, 20);
iconSetRule.reverseIconOrder(false);
iconSetRule.showIconOnly(false);
activeSheet.conditionalFormats.addRule(iconSetRule);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `iconSetType` | [`IconSetType`](../enums/GC.Spread.Sheets.ConditionalFormatting.IconSetType.md) | 图标集的类型。 |
| `iconIndex` | `number` | 图标索引。 |

#### Returns

`Object`

一个包含图像的URL字符串、偏移量和宽度高度的对象。如果用户想要自定义图标，则返回图像URL字符串。
