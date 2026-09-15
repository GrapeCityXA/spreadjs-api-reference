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

表示具有指定参数的数据条规则。

**`example`**
```
//此示例创建一个数据条规则。
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
| `minType` | [`ScaleValueType`](../enums/GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md) | 最小比例类型。 |
| `minValue` | `string` \| `number` | 最小比例值。 |
| `maxType` | [`ScaleValueType`](../enums/GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md) | 最大比例类型。 |
| `maxValue` | `string` \| `number` | 最大比例值。 |
| `color` | `string` | 数据条的填充颜色。 |
| `ranges` | [`Range`](GC.Spread.Sheets.Range.md)[] | 数据条规则影响的范围。 |

#### Overrides

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[constructor](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#constructor)

## Methods

### <a id="axiscolor" name="axiscolor"></a> axisColor

▸ **axisColor**(`value?`): `any`

获取或设置数据条的轴颜色。

**`example`**
```
//此示例使用axisColor方法。
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
| `value?` | `string` | 数据条的轴颜色。 |

#### Returns

`any`

如果未设置值，则返回数据条的轴颜色；否则返回数据条规则。

___

### <a id="axisposition" name="axisposition"></a> axisPosition

▸ **axisPosition**(`value?`): `any`

获取或设置数据条的轴位置。

**`example`**
```
//此示例使用axisPosition方法。
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
| `value?` | [`DataBarAxisPosition`](../enums/GC.Spread.Sheets.ConditionalFormatting.DataBarAxisPosition.md) | 数据条的轴位置。 |

#### Returns

`any`

如果未设置值，则返回数据条的轴位置；否则返回数据条规则。

___

### <a id="bordercolor" name="bordercolor"></a> borderColor

▸ **borderColor**(`value?`): `any`

获取或设置边框的颜色。

**`example`**
```
//此示例使用borderColor方法。
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
| `value?` | `string` | 边框的颜色。 |

#### Returns

`any`

如果未设置值，则返回边框的颜色；否则返回数据条规则。

___

### <a id="color" name="color"></a> color

▸ **color**(`value?`): `any`

获取或设置数据条的正填充颜色。

**`example`**
```
//此示例使用color方法。
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
| `value?` | `string` | 填充颜色。 |

#### Returns

`any`

如果未设置值，则返回数据条的正填充颜色；否则返回数据条规则。

___

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

### <a id="databardirection" name="databardirection"></a> dataBarDirection

▸ **dataBarDirection**(`value?`): `any`

获取或设置数据条的方向。

**`example`**
```
//此示例使用dataBarDirection方法。
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
| `value?` | [`BarDirection`](../enums/GC.Spread.Sheets.ConditionalFormatting.BarDirection.md) | 数据条的方向。 |

#### Returns

`any`

如果未设置值，则返回数据条的方向；否则返回数据条规则。

___

### <a id="evaluate" name="evaluate"></a> evaluate

▸ **evaluate**(`evaluator`, `baseRow`, `baseColumn`, `actual`): `any`

返回指定值，如果单元格满足条件。

**`example`**
```
 //此示例使用evaluate方法。
 var data = ["data", 1, 15, 25, -10];
 activeSheet.setArray(0, 0, data);
 activeSheet.setValue(0, 1, "fillColor");
 activeSheet.setValue(0, 2, "borderColor");
 activeSheet.setColumnWidth(0, 200);

 var dataBarRule = new GC.Spread.Sheets.ConditionalFormatting.DataBarRule();
 dataBarRule.ranges([new GC.Spread.Sheets.Range(0, 0, 5, 1)]);
 dataBarRule.minType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
 dataBarRule.minValue(-10);
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
 for (var i = 1; i < 5; i++) {
     var evaluateResult = dataBarRule.evaluate(activeSheet, i, 0, activeSheet.getValue(i, 0));
     activeSheet.setValue(i, 1, evaluateResult.fillColor);
     activeSheet.setValue(i, 2, evaluateResult.borderColor);
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

### <a id="gradient" name="gradient"></a> gradient

▸ **gradient**(`value?`): `any`

获取或设置是否为渐变。

**`example`**
```
//此示例使用gradient方法。
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
| `value?` | `boolean` | 是否为渐变。 |

#### Returns

`any`

如果未设置值，则返回是否为渐变；否则返回数据条规则。

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

### <a id="negativebordercolor" name="negativebordercolor"></a> negativeBorderColor

▸ **negativeBorderColor**(`value?`): `any`

获取或设置负边框的颜色。

**`example`**
```
//此示例使用negativeBorderColor方法。
activeSheet.setColumnWidth(0,400);
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,15,3);
activeSheet.setValue(2,0,25,3);
activeSheet.setValue(3,0,-10,3);
var dataBarRule = new GC.Spread.Sheets.ConditionalFormatting.DataBarRule();
dataBarRule.ranges([new GC.Spread.Sheets.Range(0,0,4,1)]);
dataBarRule.minType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
dataBarRule.minValue(-10);
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
| `value?` | `string` | 负边框的颜色。 |

#### Returns

`any`

如果未设置值，则返回负边框的颜色；否则返回数据条规则。

___

### <a id="negativefillcolor" name="negativefillcolor"></a> negativeFillColor

▸ **negativeFillColor**(`value?`): `any`

获取或设置负填充的颜色。

**`example`**
```
//此示例使用negativeFillColor方法。
activeSheet.setColumnWidth(0,400);
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,15,3);
activeSheet.setValue(2,0,25,3);
activeSheet.setValue(3,0,-10,3);
var dataBarRule = new GC.Spread.Sheets.ConditionalFormatting.DataBarRule();
dataBarRule.ranges([new GC.Spread.Sheets.Range(0,0,4,1)]);
dataBarRule.minType(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number);
dataBarRule.minValue(-10);
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
| `value?` | `string` | 负填充的颜色。 |

#### Returns

`any`

如果未设置值，则返回负填充的颜色；否则返回数据条规则。

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

若未设置参数值，返回条件格式规则范围的副本；若已设置参数值，返回该条件格式规则对象。

#### Inherited from

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[ranges](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#ranges)

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

[ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md).[reset](GC.Spread.Sheets.ConditionalFormatting.ScaleRule.md#reset)

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

### <a id="showbaronly" name="showbaronly"></a> showBarOnly

▸ **showBarOnly**(`value?`): `any`

获取或设置是否显示数据条而不显示文本。

**`example`**
```
//此示例使用showBarOnly方法。
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
| `value?` | `boolean` | 是否显示数据条而不显示文本。 |

#### Returns

`any`

如果未设置值，则返回是否显示数据条而不显示文本；否则返回数据条规则。

___

### <a id="showborder" name="showborder"></a> showBorder

▸ **showBorder**(`value?`): `any`

获取或设置是否绘制边框。

**`example`**
```
//此示例使用showBorder方法。
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
| `value?` | `boolean` | 是否绘制边框。 |

#### Returns

`any`

如果未设置值，则返回是否绘制边框；否则返回数据条规则。

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

### <a id="usenegativebordercolor" name="usenegativebordercolor"></a> useNegativeBorderColor

▸ **useNegativeBorderColor**(`value?`): `any`

获取或设置是否使用负边框颜色绘制负值的边框。

**`example`**
```
//此示例使用useNegativeBorderColor方法。
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
| `value?` | `boolean` | 是否使用负边框颜色绘制负值的边框。 |

#### Returns

`any`

如果未设置值，则返回是否使用负边框颜色绘制负值的边框；否则返回数据条规则。

___

### <a id="usenegativefillcolor" name="usenegativefillcolor"></a> useNegativeFillColor

▸ **useNegativeFillColor**(`value?`): `any`

获取或设置是否使用负填充颜色绘制负值。

**`example`**
```
//此示例使用useNegativeFillColor方法。
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
| `value?` | `boolean` | 是否使用负填充颜色绘制负值。 |

#### Returns

`any`

如果未设置值，则返回是否使用负填充颜色绘制负值；否则返回数据条规则。
