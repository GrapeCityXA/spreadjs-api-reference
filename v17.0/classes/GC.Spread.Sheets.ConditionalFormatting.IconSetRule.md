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

具有指定参数的图标集规则

**`代码示例`**
```
//本示例创建一个新的图标集规则并为其设置区域和图标
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
| `iconSetType` | [`IconSetType`](../enums/GC.Spread.Sheets.ConditionalFormatting.IconSetType.md) | 图标集的类型 |
| `ranges` | [`Range`](GC.Spread.Sheets.Range.md)[] |  |

#### Overrides

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[constructor](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#constructor)

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

如果未设置任何值，则返回规则的基本条件否则，返回条件规则

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[condition](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#condition)

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

如果单元格区域包含指定行和列中的单元格，返回true;否则返回false

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[contains](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#contains)

___

### <a id="createcondition" name="createcondition"></a> createCondition

▸ **createCondition**(): [`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

创建条件规则

#### Returns

[`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

条件

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[createCondition](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#createcondition)

___

### <a id="evaluate" name="evaluate"></a> evaluate

▸ **evaluate**(`evaluator`, `baseRow`, `baseColumn`, `actual`): `any`

如果单元格满足条件，则返回规则的指定值

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
| `evaluator` | `Object` | 计算器 |
| `baseRow` | `number` | 行索引 |
| `baseColumn` | `number` | 列索引 |
| `actual` | `Object` | 当前值 |

#### Returns

`any`

如果单元格满足条件，则为规则的指定值

#### Overrides

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[evaluate](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#evaluate)

___

### <a id="getexpected" name="getexpected"></a> getExpected

▸ **getExpected**(): [`Style`](GC.Spread.Sheets.Style.md)

获取基本规则的样式
**`example`**
```
 //This example uses the getExpected method.
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

获取图标条件

**`代码示例`**
```
//本示例创建一个规则
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,15,3);
activeSheet.setValue(2,0,25,3);
activeSheet.setValue(3,0,-1,3);
//rule
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

返回GC.Spread.Sheets.ConditionalFormatting.IconCriterion的图标集规则

___

### <a id="iconsettype" name="iconsettype"></a> iconSetType

▸ **iconSetType**(`value?`): `any`

获取或设置图标集的类型

**`代码示例`**
```
//本示例创建一个规则
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,15,3);
activeSheet.setValue(2,0,25,3);
activeSheet.setValue(3,0,-1,3);
//rule
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
| `value?` | [`IconSetType`](../enums/GC.Spread.Sheets.ConditionalFormatting.IconSetType.md) | 图标集的类型 |

#### Returns

`any`

如果未设置任何值，则返回图标集的类型否则，返回图标设置规则

___

### <a id="icons" name="icons"></a> icons

▸ **icons**(`value?`): [`IIconInfo`](../interfaces/GC.Spread.Sheets.ConditionalFormatting.IIconInfo.md)[]

获取或设置图标

**`代码示例`**
```
//本示例创建一个规则
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,15,3);
activeSheet.setValue(2,0,25,3);
activeSheet.setValue(3,0,-1,3);

//rule
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

返回iconInfos数组

___

### <a id="intersects" name="intersects"></a> intersects

▸ **intersects**(`row`, `column`, `rowCount`, `columnCount`): `boolean`

此规则的区域是否与另一个区域相交

**`example`**
```
 //This example uses the intersects method.
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
         alert("current selection is intersects with condition formatting range");
     } else {
         alert("current selection is not intersects with condition formatting range");
     }
 });
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |
| `column` | `number` | 列索引 |
| `rowCount` | `number` | 行数 |
| `columnCount` | `number` | 列数 |

#### Returns

`boolean`

如果此规则的区域与另一个区域相交，返回true;否则返回false

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[intersects](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#intersects)

___

### <a id="isscalerule" name="isscalerule"></a> isScaleRule

▸ **isScaleRule**(): `boolean`

此规则是否为缩放规则

#### Returns

`boolean`

如果此规则是缩放规则，返回true;否则返回false

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[isScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#isscalerule)

___

### <a id="maxcolor" name="maxcolor"></a> maxColor

▸ **maxColor**(`value?`): `any`

获取或设置最大色阶

**`代码示例`**
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
| `value?` | `string` | 最大色阶 |

#### Returns

`any`

如果未设置任何值，则返回最大色阶；否则，返回刻度规则

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[maxColor](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#maxcolor)

___

### <a id="maxtype" name="maxtype"></a> maxType

▸ **maxType**(`value?`): `any`

获取或设置最大刻度类型

**`代码示例`**
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
| `value?` | [`ScaleValueType`](../enums/GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md) | 最大的比例类型 |

#### Returns

`any`

如果未设置任何值，则返回最大刻度类型否则，返回刻度规则

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[maxType](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#maxtype)

___

### <a id="maxvalue" name="maxvalue"></a> maxValue

▸ **maxValue**(`value?`): `any`

获取或设置最大刻度值

**`代码示例`**
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
| `value?` | `number` | 最大刻度值 |

#### Returns

`any`

如果未设置任何值，则返回最大刻度值否则，返回刻度规则

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[maxValue](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#maxvalue)

___

### <a id="midcolor" name="midcolor"></a> midColor

▸ **midColor**(`value?`): `any`

获取或设置中点刻度颜色

**`代码示例`**
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
| `value?` | `string` | 中点刻度颜色 |

#### Returns

`any`

如果未设置任何值，则返回中点刻度颜色否则，返回刻度规则

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[midColor](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#midcolor)

___

### <a id="midtype" name="midtype"></a> midType

▸ **midType**(`value?`): `any`

获取或设置中点刻度类型

**`代码示例`**
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
| `value?` | [`ScaleValueType`](../enums/GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md) | 中点刻度类型 |

#### Returns

`any`

如果未设置任何值，则返回中点刻度类型否则，返回刻度规则

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[midType](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#midtype)

___

### <a id="midvalue" name="midvalue"></a> midValue

▸ **midValue**(`value?`): `any`

获取或设置中点刻度值

**`代码示例`**
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
| `value?` | `number` | 中点刻度值 |

#### Returns

`any`

如果未设置任何值，则返回中点刻度值否则，返回刻度规则

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[midValue](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#midvalue)

___

### <a id="mincolor" name="mincolor"></a> minColor

▸ **minColor**(`value?`): `any`

获取或设置最小刻度颜色

**`代码示例`**
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
| `value?` | `string` | 最小刻度颜色 |

#### Returns

`any`

如果未设置任何值，则返回最小刻度颜色否则，将返回刻度规则

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[minColor](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#mincolor)

___

### <a id="mintype" name="mintype"></a> minType

▸ **minType**(`value?`): `any`

获取或设置最小刻度的类型

**`代码示例`**
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
| `value?` | [`ScaleValueType`](../enums/GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md) | 最小刻度的类型 |

#### Returns

`any`

如果未设置任何值，则返回最小刻度的类型否则，返回刻度规则

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[minType](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#mintype)

___

### <a id="minvalue" name="minvalue"></a> minValue

▸ **minValue**(`value?`): `any`

获取或设置最小刻度值

**`代码示例`**
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
| `value?` | `number` | 最小刻度值 |

#### Returns

`any`

如果未设置任何值，则返回最小刻度值；否则，返回刻度规则

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[minValue](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#minvalue)

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

如果未设置任何值，则返回规则的优先级否则，返回条件规则

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[priority](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#priority)

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

如果未设置任何值，则返回条件规则区域否则，返回条件规则

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[ranges](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#ranges)

___

### <a id="reset" name="reset"></a> reset

▸ **reset**(): `void`

重置规则

**`代码示例`**
```
//本示例使用reset方法
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,15,3);
activeSheet.setValue(2,0,25,3);
activeSheet.setValue(3,0,-1,3);
//rule
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

获取或设置是否反转图标顺序

**`代码示例`**
```
//本示例创建一个规则
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,15,3);
activeSheet.setValue(2,0,25,3);
activeSheet.setValue(3,0,-1,3);
//rule
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
| `value?` | `boolean` | 是否反转图标顺序 |

#### Returns

`any`

如果未设置任何值，则返回是否反转图标顺序的值；否则，返回图标设置规则

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

如果未设置任何值，则返回条件规则类型否则，返回条件规则

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[ruleType](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#ruletype)

___

### <a id="showicononly" name="showicononly"></a> showIconOnly

▸ **showIconOnly**(`value?`): `any`

获取或设置是否仅显示图标

**`代码示例`**
```
//本示例创建一个规则
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,15,3);
activeSheet.setValue(2,0,25,3);
activeSheet.setValue(3,0,-1,3);
//rule
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
| `value?` | `boolean` | 是否仅显示图标 |

#### Returns

`any`

如果未设置任何值，则返回是否仅显示图标的值；否则，返回图标设置规则

___

### <a id="stopiftrue" name="stopiftrue"></a> stopIfTrue

▸ **stopIfTrue**(`value?`): `boolean`

获取条件计算为true时计算是否停止

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

如果未设置任何值，则返回规则的样式否则，返回条件规则

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[style](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#style)

___

### <a id="geticon" name="geticon"></a> getIcon

▸ `Static` **getIcon**(`iconSetType`, `iconIndex`): `Object`

根据特定的iconSetType和iconIndex对象获取图标

**`static`**

**`代码示例`**
```
//本示例返回图标集规则的图标
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
| `iconSetType` | [`IconSetType`](../enums/GC.Spread.Sheets.ConditionalFormatting.IconSetType.md) | 图标集类型 |
| `iconIndex` | `number` | 图标索引 returns {object} 包含图像的URL字符串，偏移量以及宽度和高度的对象 如果用户要自定义IconSet的图标，则返回图像URL字符串 |

#### Returns

`Object`

包含图像的URL字符串，偏移以及宽度和高度的对象
如果用户想自定义Iconset的图标，则返回图像URL字符串
