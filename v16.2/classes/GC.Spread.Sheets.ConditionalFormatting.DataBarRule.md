# Class: DataBarRule

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).DataBarRule

## Hierarchy

- [`ScaleRule`](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md)

  ↳ **`DataBarRule`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#constructor)

### Methods

- [axisColor](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#axiscolor)
- [axisPosition](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#axisposition)
- [borderColor](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#bordercolor)
- [color](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#color)
- [condition](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#condition)
- [contains](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#contains)
- [createCondition](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#createcondition)
- [dataBarDirection](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#databardirection)
- [evaluate](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#evaluate)
- [getExpected](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#getexpected)
- [gradient](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#gradient)
- [intersects](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#intersects)
- [isScaleRule](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#isscalerule)
- [maxColor](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#maxcolor)
- [maxType](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#maxtype)
- [maxValue](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#maxvalue)
- [midColor](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#midcolor)
- [midType](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#midtype)
- [midValue](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#midvalue)
- [minColor](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#mincolor)
- [minType](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#mintype)
- [minValue](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#minvalue)
- [negativeBorderColor](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#negativebordercolor)
- [negativeFillColor](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#negativefillcolor)
- [priority](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#priority)
- [ranges](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#ranges)
- [reset](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#reset)
- [ruleType](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#ruletype)
- [showBarOnly](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#showbaronly)
- [showBorder](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#showborder)
- [stopIfTrue](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#stopiftrue)
- [style](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#style)
- [useNegativeBorderColor](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#usenegativebordercolor)
- [useNegativeFillColor](GC.Spread.Sheets.ConditionalFormatting.DataBarRule.md#usenegativefillcolor)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new DataBarRule**(`minType`, `minValue`, `maxType`, `maxValue`, `color`, `ranges`)

具有指定参数的数据条条件规则

**`代码示例`**
```
//本示例创建一个数据条规则
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,15,3);
activeSheet.setValue(2,0,25,3);
activeSheet.setValue(3,0,-1,3);
var dataBarRule = new GC.Spread.Sheets.ConditionalFormatting.DataBarRule(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number, -1, GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number, 40, "green", [new GC.Spread.Sheets.Range(0,0,4,1)]);
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
| `minType` | [`ScaleValueType`](../enums/GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md) | 最小的比例类型 |
| `minValue` | `string` \| `number` | 最小刻度值 |
| `maxType` | [`ScaleValueType`](../enums/GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md) | 最大的比例类型 |
| `maxValue` | `string` \| `number` | 最大刻度值 |
| `color` | `string` | 数据条的填充颜色 |
| `ranges` | [`Range`](GC.Spread.Sheets.Range.md)[] | 数据条规则影响区域 |

#### Overrides

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[constructor](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#constructor)

## Methods

### <a id="axiscolor" name="axiscolor"></a> axisColor

▸ **axisColor**(`value?`): `any`

获取或设置数据条的坐标轴颜色

**`代码示例`**
```
//本示例使用axisColor方法
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,15,3);
activeSheet.setValue(2,0,25,3);
activeSheet.setValue(3,0,-1,3);
 //rule
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
| `value?` | `string` | 数据条的坐标轴颜色 |

#### Returns

`any`

如果未设置任何值,则返回数据条的坐标轴颜色;否则,返回数据条规则

___

### <a id="axisposition" name="axisposition"></a> axisPosition

▸ **axisPosition**(`value?`): `any`

获取或设置数据条的坐标轴位置

**`代码示例`**
```
//本示例使用axisPosition方法
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,15,3);
activeSheet.setValue(2,0,25,3);
activeSheet.setValue(3,0,-1,3);
 //rule
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
| `value?` | [`DataBarAxisPosition`](../enums/GC.Spread.Sheets.ConditionalFormatting.DataBarAxisPosition.md) | 数据条的轴线位置 |

#### Returns

`any`

如果未设置任何值,则返回数据条的坐标轴位置;否则,返回数据条规则

___

### <a id="bordercolor" name="bordercolor"></a> borderColor

▸ **borderColor**(`value?`): `any`

获取或设置边框的颜色

**`代码示例`**
```
//本示例使用borderColor方法
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,15,3);
activeSheet.setValue(2,0,25,3);
activeSheet.setValue(3,0,-1,3);
 //rule
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
| `value?` | `string` | 边框的颜色 |

#### Returns

`any`

如果未设置任何值,则返回边框的颜色;否则,返回数据条规则

___

### <a id="color" name="color"></a> color

▸ **color**(`value?`): `any`

获取或设置数据条的正填充颜色

**`代码示例`**
```
//本示例使用color方法
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,15,3);
activeSheet.setValue(2,0,25,3);
activeSheet.setValue(3,0,-1,3);
 //rule
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
| `value?` | `string` | 填充颜色 |

#### Returns

`any`

如果未设置任何值,则返回数据条的正填充颜色;否则,返回数据条规则

___

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

如果单元格区域包含指定行和列中的单元格,返回true;否则返回false

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

### <a id="databardirection" name="databardirection"></a> dataBarDirection

▸ **dataBarDirection**(`value?`): `any`

获取或设置数据条方向

**`代码示例`**
```
//本示例使用dataBarDirection方法
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,15,3);
activeSheet.setValue(2,0,25,3);
activeSheet.setValue(3,0,-1,3);
 //rule
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
| `value?` | [`BarDirection`](../enums/GC.Spread.Sheets.ConditionalFormatting.BarDirection.md) | 数据条方向 |

#### Returns

`any`

如果未设置任何值,则返回数据条方向;否则,返回数据条规则

___

### <a id="evaluate" name="evaluate"></a> evaluate

▸ **evaluate**(`evaluator`, `baseRow`, `baseColumn`, `actual`): `any`

如果单元格满足条件,则返回规则的指定值

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `evaluator` | `Object` | 计算器 |
| `baseRow` | `number` | 行索引 |
| `baseColumn` | `number` | 列索引 |
| `actual` | `Object` | 当前值 |

#### Returns

`any`

如果单元格满足条件,则为规则的指定值

#### Overrides

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[evaluate](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#evaluate)

___

### <a id="getexpected" name="getexpected"></a> getExpected

▸ **getExpected**(): [`Style`](GC.Spread.Sheets.Style.md)

获取基本规则的样式

#### Returns

[`Style`](GC.Spread.Sheets.Style.md)

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[getExpected](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#getexpected)

___

### <a id="gradient" name="gradient"></a> gradient

▸ **gradient**(`value?`): `any`

获取或设置一个值,该值数据条是否为渐变

**`代码示例`**
```
//本示例使用gradient方法
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
dataBarRule.gradient(false);
activeSheet.conditionalFormats.addRule(dataBarRule);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 数据条是否为渐变 |

#### Returns

`any`

如果未设置任何值,则返回数据条是否为渐变的值;否则,返回数据条规则

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

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[intersects](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#intersects)

___

### <a id="isscalerule" name="isscalerule"></a> isScaleRule

▸ **isScaleRule**(): `boolean`

此规则是否为缩放规则

#### Returns

`boolean`

如果此规则是缩放规则,返回true;否则返回false

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

如果未设置任何值,则返回最大色阶;否则,返回刻度规则

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

如果未设置任何值,则返回最大刻度类型否则,返回刻度规则

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

如果未设置任何值,则返回最大刻度值否则,返回刻度规则

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

如果未设置任何值,则返回中点刻度颜色否则,返回刻度规则

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

如果未设置任何值,则返回中点刻度类型否则,返回刻度规则

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

如果未设置任何值,则返回中点刻度值否则,返回刻度规则

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

如果未设置任何值,则返回最小刻度颜色否则,将返回刻度规则

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

如果未设置任何值,则返回最小刻度的类型否则,返回刻度规则

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

如果未设置任何值,则返回最小刻度值;否则,返回刻度规则

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[minValue](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#minvalue)

___

### <a id="negativebordercolor" name="negativebordercolor"></a> negativeBorderColor

▸ **negativeBorderColor**(`value?`): `any`

获取或设置负边框颜色

**`代码示例`**
```
//本示例使用negativeBorderColor方法
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
| `value?` | `string` | 负边框颜色 |

#### Returns

`any`

如果未设置任何值,则返回负边框颜色;否则,返回数据条规则

___

### <a id="negativefillcolor" name="negativefillcolor"></a> negativeFillColor

▸ **negativeFillColor**(`value?`): `any`

获取或设置负填充颜色

**`代码示例`**
```
//本示例使用negativeFillColor方法
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
| `value?` | `string` | 负填充颜色 |

#### Returns

`any`

如果未设置任何值,则返回负填充颜色;否则,返回数据条规则

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

如果未设置任何值,则返回条件规则区域否则,返回条件规则

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[ranges](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#ranges)

___

### <a id="reset" name="reset"></a> reset

▸ **reset**(): `void`

重置规则

#### Returns

`void`

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[reset](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#reset)

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

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[ruleType](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#ruletype)

___

### <a id="showbaronly" name="showbaronly"></a> showBarOnly

▸ **showBarOnly**(`value?`): `any`

获取或设置是否显示不带文本的数据条

**`代码示例`**
```
//本示例使用showBarOnly方法
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
| `value?` | `boolean` | 是否显示不带文本的数据条 |

#### Returns

`any`

如果未设置任何值,则返回是否显示不带文本的数据条;否则,返回数据条规则

___

### <a id="showborder" name="showborder"></a> showBorder

▸ **showBorder**(`value?`): `any`

获取或设置一个值,该值是否绘制边框

**`代码示例`**
```
//本示例使用showBorder方法
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
| `value?` | `boolean` | 是否绘制边框 |

#### Returns

`any`

如果未设置任何值,则返回是否绘制边框的值;否则,返回数据条规则

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

如果未设置任何值,则返回规则的样式否则,返回条件规则

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[style](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#style)

___

### <a id="usenegativebordercolor" name="usenegativebordercolor"></a> useNegativeBorderColor

▸ **useNegativeBorderColor**(`value?`): `any`

获取或设置一个值,该值是否使用负边框颜色为负值绘制边框

**`代码示例`**
```
//本示例使用useNegativeBorderColor方法
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
| `value?` | `boolean` | 是否使用负边框颜色为负值绘制边框 |

#### Returns

`any`

如果未设置任何值,则返回一个值,该值是否使用负边框颜色为负值绘制边框;否则,返回数据条规则

___

### <a id="usenegativefillcolor" name="usenegativefillcolor"></a> useNegativeFillColor

▸ **useNegativeFillColor**(`value?`): `any`

获取或设置一个值,该值是否使用负填充颜色绘制负值

**`代码示例`**
```
//本示例使用useNegativeFillColor方法
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
| `value?` | `boolean` | 是否使用负填充颜色绘制负值. |

#### Returns

`any`

如果未设置任何值,则返回一个值,该值是否使用负填充色绘制负值;否则,返回数据条规则
