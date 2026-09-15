# Class: ConditionalFormats

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).ConditionalFormats

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.ConditionalFormatting.ConditionalFormats.md#constructor)

### Methods

- [add2ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ConditionalFormats.md#add2scalerule)
- [add3ScaleRule](GC.Spread.Sheets.ConditionalFormatting.ConditionalFormats.md#add3scalerule)
- [addAverageRule](GC.Spread.Sheets.ConditionalFormatting.ConditionalFormats.md#addaveragerule)
- [addCellValueRule](GC.Spread.Sheets.ConditionalFormatting.ConditionalFormats.md#addcellvaluerule)
- [addColumnStateRule](GC.Spread.Sheets.ConditionalFormatting.ConditionalFormats.md#addcolumnstaterule)
- [addDataBarRule](GC.Spread.Sheets.ConditionalFormatting.ConditionalFormats.md#adddatabarrule)
- [addDateOccurringRule](GC.Spread.Sheets.ConditionalFormatting.ConditionalFormats.md#adddateoccurringrule)
- [addDuplicateRule](GC.Spread.Sheets.ConditionalFormatting.ConditionalFormats.md#addduplicaterule)
- [addFormulaRule](GC.Spread.Sheets.ConditionalFormatting.ConditionalFormats.md#addformularule)
- [addIconSetRule](GC.Spread.Sheets.ConditionalFormatting.ConditionalFormats.md#addiconsetrule)
- [addRowStateRule](GC.Spread.Sheets.ConditionalFormatting.ConditionalFormats.md#addrowstaterule)
- [addRule](GC.Spread.Sheets.ConditionalFormatting.ConditionalFormats.md#addrule)
- [addSparklineRule](GC.Spread.Sheets.ConditionalFormatting.ConditionalFormats.md#addsparklinerule)
- [addSpecificTextRule](GC.Spread.Sheets.ConditionalFormatting.ConditionalFormats.md#addspecifictextrule)
- [addTop10Rule](GC.Spread.Sheets.ConditionalFormatting.ConditionalFormats.md#addtop10rule)
- [addUniqueRule](GC.Spread.Sheets.ConditionalFormatting.ConditionalFormats.md#adduniquerule)
- [clearRule](GC.Spread.Sheets.ConditionalFormatting.ConditionalFormats.md#clearrule)
- [containsRule](GC.Spread.Sheets.ConditionalFormatting.ConditionalFormats.md#containsrule)
- [count](GC.Spread.Sheets.ConditionalFormatting.ConditionalFormats.md#count)
- [getRule](GC.Spread.Sheets.ConditionalFormatting.ConditionalFormats.md#getrule)
- [getRules](GC.Spread.Sheets.ConditionalFormatting.ConditionalFormats.md#getrules)
- [removeRule](GC.Spread.Sheets.ConditionalFormatting.ConditionalFormats.md#removerule)
- [removeRuleByRange](GC.Spread.Sheets.ConditionalFormatting.ConditionalFormats.md#removerulebyrange)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new ConditionalFormats**(`worksheet`)

表示格式条件类。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `worksheet` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 工作表。 |

## Methods

### <a id="add2scalerule" name="add2scalerule"></a> add2ScaleRule

▸ **add2ScaleRule**(`minType`, `minValue`, `minColor`, `maxType`, `maxValue`, `maxColor`, `ranges`): [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

将双刻度规则添加到规则集合中。

**`example`**
```javascript
//此示例使用 add2ScaleRule 方法。
activeSheet.conditionalFormats.add2ScaleRule(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number,10,"Red",GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number,100,"Yellow", [new GC.Spread.Sheets.Range(0,0,10,3)]);
activeSheet.setValue(0,0, 1,3);
activeSheet.setValue(1,0, 50,3);
activeSheet.setValue(2,0, 100,3);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `minType` | [`ScaleValueType`](../enums/GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md) | 最小刻度类型。 |
| `minValue` | `number` | 最小刻度值。 |
| `minColor` | `string` | 最小刻度颜色。 |
| `maxType` | [`ScaleValueType`](../enums/GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md) | 最大刻度类型。 |
| `maxValue` | `number` | 最大刻度值。 |
| `maxColor` | `string` | 最大刻度颜色。 |
| `ranges` | [`Range`](GC.Spread.Sheets.Range.md)[] | 应用规则的单元格范围，其项类型为 GC.Spread.Sheets.Range。 |

#### Returns

[`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

添加到规则集合中的双刻度规则。

___

### <a id="add3scalerule" name="add3scalerule"></a> add3ScaleRule

▸ **add3ScaleRule**(`minType`, `minValue`, `minColor`, `midType`, `midValue`, `midColor`, `maxType`, `maxValue`, `maxColor`, `ranges`): [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

将三刻度规则添加到规则集合中。

**`example`**
```javascript
//此示例使用 add3ScaleRule 方法。
activeSheet.setValue(0,0, 1,3);
activeSheet.setValue(1,0, 50,3);
activeSheet.setValue(2,0, 100,3);
activeSheet.conditionalFormats.add3ScaleRule(1, 10, "red", 0, 50, "blue",2, 100, "yellow", [new GC.Spread.Sheets.Range(0, 0, 10, 3)]);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `minType` | [`ScaleValueType`](../enums/GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md) | 最小刻度类型。 |
| `minValue` | `number` | 最小刻度值。 |
| `minColor` | `string` | 最小刻度颜色。 |
| `midType` | [`ScaleValueType`](../enums/GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md) | 中点刻度类型。 |
| `midValue` | `number` | 中点刻度值。 |
| `midColor` | `string` | 中点刻度颜色。 |
| `maxType` | [`ScaleValueType`](../enums/GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md) | 最大刻度类型。 |
| `maxValue` | `number` | 最大刻度值。 |
| `maxColor` | `string` | 最大刻度颜色。 |
| `ranges` | [`Range`](GC.Spread.Sheets.Range.md)[] | 应用规则的单元格范围，其项类型为 GC.Spread.Sheets.Range。 |

#### Returns

[`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

添加到规则集合中的三刻度规则。

___

### <a id="addaveragerule" name="addaveragerule"></a> addAverageRule

▸ **addAverageRule**(`type`, `style`, `ranges`): [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

将平均值规则添加到规则集合中。

**`example`**
```javascript
//此示例使用 addAverageRule 方法。
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
activeSheet.conditionalFormats.addAverageRule(GC.Spread.Sheets.ConditionalFormatting.AverageConditionType.above,style,[new GC.Spread.Sheets.Range(0, 0, 10, 3)]);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | [`AverageConditionType`](../enums/GC.Spread.Sheets.ConditionalFormatting.AverageConditionType.md) | 平均值条件类型。 |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 满足条件时应用于单元格的样式。 |
| `ranges` | [`Range`](GC.Spread.Sheets.Range.md)[] | 应用规则的单元格范围，其项类型为 GC.Spread.Sheets.Range。 |

#### Returns

[`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

添加到规则集合中的平均值规则。

___

### <a id="addcellvaluerule" name="addcellvaluerule"></a> addCellValueRule

▸ **addCellValueRule**(`comparisonOperator`, `value1`, `value2`, `style`, `ranges`): [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

将单元格值规则添加到规则集合中。

**`example`**
```javascript
//此示例使用 addCellValueRule 方法。
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
var ranges=[new GC.Spread.Sheets.Range(0,0,5,1)];
activeSheet.conditionalFormats.addCellValueRule(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.between, 2, 100, style, ranges);
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,45,3);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `comparisonOperator` | [`ComparisonOperators`](../enums/GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.md) | 比较运算符。 |
| `value1` | `Object` | 第一个值。 |
| `value2` | `Object` | 第二个值。 |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 满足条件时应用于单元格的样式。 |
| `ranges` | [`Range`](GC.Spread.Sheets.Range.md)[] | 应用规则的单元格范围，其项类型为 GC.Spread.Sheets.Range。 |

#### Returns

[`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

添加到规则集合中的单元格值规则。

___

### <a id="addcolumnstaterule" name="addcolumnstaterule"></a> addColumnStateRule

▸ **addColumnStateRule**(`state`, `style`, `ranges`): [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

将列状态规则添加到规则集合中。

**`example`**
```javascript
// 在列方向添加悬停状态规则。
activeSheet.conditionalFormats.addColumnStateRule(GC.Spread.Sheets.RowColumnStates.hover, new GC.Spread.Sheets.Style("yellow"), [new GC.Spread.Sheets.Range(-1, -1, -1, -1)]);
activeSheet.conditionalFormats.addColumnStateRule(
     GC.Spread.Sheets.RowColumnStates.hover,
     [new GC.Spread.Sheets.Style("green"), new GC.Spread.Sheets.Style("red")],
     [new GC.Spread.Sheets.Range(1, 1, 10, 5), new GC.Spread.Sheets.Range(13, 1, 10, 5)]
);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `state` | [`RowColumnStates`](../enums/GC.Spread.Sheets.RowColumnStates.md) | 状态类型。 |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) \| [`Style`](GC.Spread.Sheets.Style.md)[] | 当列匹配状态时的行样式。可以是样式数组。 |
| `ranges` | [`Range`](GC.Spread.Sheets.Range.md)[] | 应用规则的范围，其项类型为 GC.Spread.Sheets.Range。 |

#### Returns

[`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

添加到规则集合中的状态规则。

___

### <a id="adddatabarrule" name="adddatabarrule"></a> addDataBarRule

▸ **addDataBarRule**(`minType`, `minValue`, `maxType`, `maxValue`, `color`, `ranges`): [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

将数据条规则添加到规则集合中。

**`example`**
```javascript
//此示例使用 addDataBarRule 方法。
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,15,3);
activeSheet.setValue(2,0,25,3);
activeSheet.setValue(3,0,-1,3);
activeSheet.conditionalFormats.addDataBarRule(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number, -1, GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number, 40, "orange", [new GC.Spread.Sheets.Range(0,0,4,1)]);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `minType` | [`ScaleValueType`](../enums/GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md) | 最小刻度类型。 |
| `minValue` | `number` | 最小刻度值。 |
| `maxType` | [`ScaleValueType`](../enums/GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.md) | 最大刻度类型。 |
| `maxValue` | `number` | 最大刻度值。 |
| `color` | `string` | 在视图中显示的数据条颜色。 |
| `ranges` | [`Range`](GC.Spread.Sheets.Range.md)[] | 应用规则的单元格范围，其项类型为 GC.Spread.Sheets.Range。 |

#### Returns

[`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

添加到规则集合中的数据条规则。

___

### <a id="adddateoccurringrule" name="adddateoccurringrule"></a> addDateOccurringRule

▸ **addDateOccurringRule**(`type`, `style`, `ranges`): [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

将日期出现规则添加到规则集合中。

**`example`**
```javascript
//此示例使用 addDateOccurringRule 方法。
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
var d = new Date();
activeSheet.setValue(0, 0, d);
activeSheet.setValue(1, 0, new Date(d.setDate(d.getDate()+1)));
activeSheet.setValue(2, 0, new Date(d.setDate(d.getDate()+5)));
activeSheet.setValue(3, 0,new Date(d.setDate(d.getDate()+6)));
activeSheet.setValue(4, 0,new Date(d.setDate(d.getDate()+7)));
activeSheet.setValue(5, 0, new Date(d.setDate(d.getDate()+8)));
activeSheet.conditionalFormats.addDateOccurringRule(GC.Spread.Sheets.ConditionalFormatting.DateOccurringType.nextWeek, style, [new GC.Spread.Sheets.Range(0,0,10,1)]);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | [`DateOccurringType`](../enums/GC.Spread.Sheets.ConditionalFormatting.DateOccurringType.md) | 日期出现类型。 |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 满足条件时应用于单元格的样式。 |
| `ranges` | [`Range`](GC.Spread.Sheets.Range.md)[] | 应用规则的单元格范围，其项类型为 GC.Spread.Sheets.Range。 |

#### Returns

[`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

添加到规则集合中的日期出现规则。

___

### <a id="addduplicaterule" name="addduplicaterule"></a> addDuplicateRule

▸ **addDuplicateRule**(`style`, `ranges`): [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

将重复规则添加到规则集合中。

**`example`**
```javascript
//此示例使用 addDuplicateRule 方法。
var style = new GC.Spread.Sheets.Style();
style.backColor = "yellow";
var ranges=[new GC.Spread.Sheets.Range(0,0,10,1)];
activeSheet.conditionalFormats.addDuplicateRule(style, ranges);
activeSheet.setValue(0, 0, 50);
activeSheet.setValue(1, 0, 50);
activeSheet.setValue(2, 0, 11);
activeSheet.setValue(3, 0, 5);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 满足条件时应用于单元格的样式。 |
| `ranges` | [`Range`](GC.Spread.Sheets.Range.md)[] | 应用规则的单元格范围，其项类型为 GC.Spread.Sheets.Range。 |

#### Returns

[`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

添加到规则集合中的重复规则。

___

### <a id="addformularule" name="addformularule"></a> addFormulaRule

▸ **addFormulaRule**(`formula`, `style`, `ranges`): [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

将公式规则添加到规则集合中。

**`example`**
```javascript
//此示例使用 addFormulaRule 方法。
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
var ranges = [new GC.Spread.Sheets.Range(0, 0, 2, 1)];
activeSheet.conditionalFormats.addFormulaRule("=A1=B1+C1", style, ranges);
activeSheet.setValue(0, 0, 2,3);
activeSheet.setValue(0, 1, 1,3);
activeSheet.setValue(0, 2,1,3);
activeSheet.setValue(1, 0, 1,3);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `formula` | `string` | 条件公式。 |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 满足条件时应用于单元格的样式。 |
| `ranges` | [`Range`](GC.Spread.Sheets.Range.md)[] | 应用规则的单元格范围，其项类型为 GC.Spread.Sheets.Range。 |

#### Returns

[`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

添加到规则集合中的公式规则。

___

### <a id="addiconsetrule" name="addiconsetrule"></a> addIconSetRule

▸ **addIconSetRule**(`iconSetTye`, `ranges`): [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

将图标集规则添加到规则集合中。

**`example`**
```javascript
//此示例使用 addIconSetRule 方法。
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,15,3);
activeSheet.setValue(2,0,25,3);
activeSheet.setValue(3,0,-1,3);
activeSheet.conditionalFormats.addIconSetRule(GC.Spread.Sheets.ConditionalFormatting.IconSetType.fourTrafficLights, [new GC.Spread.Sheets.Range(0,0,4,1)]);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `iconSetTye` | [`IconSetType`](../enums/GC.Spread.Sheets.ConditionalFormatting.IconSetType.md) | - |
| `ranges` | [`Range`](GC.Spread.Sheets.Range.md)[] | 应用规则的单元格范围，其项类型为 GC.Spread.Sheets.Range。 |

#### Returns

[`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

添加到规则集合中的图标集规则。

___

### <a id="addrowstaterule" name="addrowstaterule"></a> addRowStateRule

▸ **addRowStateRule**(`state`, `style`, `ranges`): [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

将行状态规则添加到规则集合中。

**`example`**
```javascript
// 添加行方向的悬停状态规则。
activeSheet.conditionalFormats.addRowStateRule(GC.Spread.Sheets.RowColumnStates.hover, new GC.Spread.Sheets.Style("yellow"), [new GC.Spread.Sheets.Range(-1, -1, -1, -1)]);
// 添加具有可变样式的悬停状态规则
activeSheet.conditionalFormats.addRowStateRule(
     GC.Spread.Sheets.RowColumnStates.hover,
     [new GC.Spread.Sheets.Style("green"), new GC.Spread.Sheets.Style("red")],
     [new GC.Spread.Sheets.Range(1, 1, 10, 5), new GC.Spread.Sheets.Range(1, 7, 10, 5)]
);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `state` | [`RowColumnStates`](../enums/GC.Spread.Sheets.RowColumnStates.md) | 状态类型。 |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) \| [`Style`](GC.Spread.Sheets.Style.md)[] | 如果行匹配状态则应用的行样式。可以是样式数组。 |
| `ranges` | [`Range`](GC.Spread.Sheets.Range.md)[] | 应用规则的范围，其项类型为 GC.Spread.Sheets.Range。 |

#### Returns

[`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

添加到规则集合中的状态规则。

___

### <a id="addrule" name="addrule"></a> addRule

▸ **addRule**(`rule`): [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

添加规则。

**`example`**
```javascript
//此示例使用 addRule 方法。
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
| `rule` | [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md) | 要添加的规则。 |

#### Returns

[`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

___

### <a id="addsparklinerule" name="addsparklinerule"></a> addSparklineRule

▸ **addSparklineRule**(`type`, `options?`, `ranges?`): [`SparklineRule`](GC.Spread.Sheets.ConditionalFormatting.SparklineRule.md)

向规则集合中添加迷你图规则。

**`example`**
```javascript
// 示例 1：使用选项对象创建 HBar 迷你图规则
var ranges = [new GC.Spread.Sheets.Range(0, 0, 1, 1)];
activeSheet.setValue(1, 0, 10);
activeSheet.setValue(1, 1, 20);
activeSheet.setValue(1, 2, 30);
var options = {
    'range|percentage': "A2:C2",
    colors: ["red", "green", "blue"]
};
activeSheet.conditionalFormats.addSparklineRule("PieSparkline", options, ranges);

// 示例 2：使用位置参数数组创建 YEARSPARKLINE 规则
// 这将生成：=YEARSPARKLINE(2026, A2:B13, , , "#979797", "#f3f3f3")
var yearRanges = [new GC.Spread.Sheets.Range(0, 0, 1, 1)];
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
activeSheet.conditionalFormats.addSparklineRule("YearSparkline",
    [2026, 'A2:B13', undefined, undefined, '#979797', '#f3f3f3'],
    yearRanges);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | [`SparklineExType`](../modules/GC.Spread.Sheets.Sparklines.md#sparklineextype) | 迷你图类型名称（例如 "PIESPARKLINE"、"LINESPARKLINE"，或自定义迷你图函数名称）。 |
| `options?` | [`ISparklineOptions`](../modules/GC.Spread.Sheets.Sparklines.md#isparklineoptions) \| [`SparklineParameterType`](../modules/GC.Spread.Sheets.Sparklines.md#sparklineparametertype)[] | 迷你图选项，可以是以下两种形式之一：   - 带命名参数的选项对象（适用于参数顺序已知的内置迷你图）。   - 位置参数数组（适用于自定义迷你图，或需要显式参数顺序时）。   支持特殊占位符：`$CF_RANGE$`（会替换为规则区域）和 `@`（当前单元格值或索引）。 |
| `ranges?` | [`Range`](GC.Spread.Sheets.Range.md)[] | 规则应用的单元格区域，其元素类型为 GC.Spread.Sheets.Range。 |

#### Returns

[`SparklineRule`](GC.Spread.Sheets.ConditionalFormatting.SparklineRule.md)

添加到规则集合中的迷你图规则。

___

### <a id="addspecifictextrule" name="addspecifictextrule"></a> addSpecificTextRule

▸ **addSpecificTextRule**(`comparisonOperator`, `text`, `style`, `ranges`): [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

将文本规则添加到规则集合中。

**`example`**
```javascript
//此示例使用 addSpecificTextRule 方法。
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
var ranges=[new GC.Spread.Sheets.Range(0,0,10,1)];
activeSheet.conditionalFormats.addSpecificTextRule(GC.Spread.Sheets.ConditionalFormatting.TextComparisonOperators.contains, "test", style, ranges);
activeSheet.setValue(0, 0, "testing");
activeSheet.setValue(1, 0, "test");
activeSheet.setValue(2, 0, "a");
activeSheet.setValue(3, 0, "t");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `comparisonOperator` | [`TextComparisonOperators`](../enums/GC.Spread.Sheets.ConditionalFormatting.TextComparisonOperators.md) | 比较运算符。 |
| `text` | `string` | 用于比较的文本。 |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 当条件满足时应用于单元格的样式。 |
| `ranges` | [`Range`](GC.Spread.Sheets.Range.md)[] | 应用规则的单元格范围，其项类型为 GC.Spread.Sheets.Range。 |

#### Returns

[`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

添加到规则集合中的文本规则。

___

### <a id="addtop10rule" name="addtop10rule"></a> addTop10Rule

▸ **addTop10Rule**(`type`, `rank`, `style`, `ranges`, `isPercent?`): [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

根据 Top10ConditionType 对象将前10规则或后10规则添加到集合中。

**`example`**
```javascript
//此示例使用 addTop10Rule 方法。
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
var ranges=[new GC.Spread.Sheets.Range(0,0,10,1)];
activeSheet.conditionalFormats.addTop10Rule(GC.Spread.Sheets.ConditionalFormatting.Top10ConditionType.top, 2, style, ranges);
activeSheet.setValue(0, 0, 1);
activeSheet.setValue(1, 0, 50);
activeSheet.setValue(2, 0, 11);
activeSheet.setValue(3, 0, 5);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | [`Top10ConditionType`](../enums/GC.Spread.Sheets.ConditionalFormatting.Top10ConditionType.md) | 前10条件。 |
| `rank` | `number` | 要应用样式的顶部或底部项目的数量。 |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 当条件满足时应用于单元格的样式。 |
| `ranges` | [`Range`](GC.Spread.Sheets.Range.md)[] | 应用规则的单元格范围，其项类型为 GC.Spread.Sheets.Range。 |
| `isPercent?` | `boolean` | - |

#### Returns

[`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

添加到规则集合中的前10规则。

___

### <a id="adduniquerule" name="adduniquerule"></a> addUniqueRule

▸ **addUniqueRule**(`style`, `ranges`): [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

将唯一规则添加到规则集合中。

**`example`**
```javascript
//此示例使用 addUniqueRule 方法。
var style = new GC.Spread.Sheets.Style();
style.backColor = "green";
activeSheet.setValue(0, 0, 50);
activeSheet.setValue(1, 0, 50);
activeSheet.setValue(2, 0, 11);
activeSheet.setValue(3, 0, 5);
activeSheet.conditionalFormats.addUniqueRule(style, [new GC.Spread.Sheets.Range(0,0,10,1)]);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 当条件满足时应用于单元格的样式。 |
| `ranges` | [`Range`](GC.Spread.Sheets.Range.md)[] | 应用规则的单元格范围，其项类型为 GC.Spread.Sheets.Range。 |

#### Returns

[`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

添加到规则集合中的唯一规则。

___

### <a id="clearrule" name="clearrule"></a> clearRule

▸ **clearRule**(): `void`

移除所有规则。

**`example`**
```javascript
//此示例使用 clearRule 方法。
activeSheet.setValue(0,0, 1,3);
activeSheet.setValue(1,0, 50,3);
activeSheet.setValue(2,0, 100,3);
activeSheet.conditionalFormats.add2ScaleRule(GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number, 10, "red", GC.Spread.Sheets.ConditionalFormatting.ScaleValueType.number, 100, "yellow", [new GC.Spread.Sheets.Range(0, 0, 10, 3)]);
// 删除方法前的注释以进行测试
//activeSheet.conditionalFormats.clearRule();
```

#### Returns

`void`

___

### <a id="containsrule" name="containsrule"></a> containsRule

▸ **containsRule**(`rule`, `row`, `column`): `boolean`

确定指定单元格是否包含指定规则。

**`example`**
```javascript
//此示例检查单元格是否具有指定规则。
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
var rule = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
rule.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.cellValueRule);
rule.ranges([new GC.Spread.Sheets.Range(0,0,5,1)]);
rule.operator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.between);
rule.style(style);
rule.value1(2);
rule.value2(100);
activeSheet.conditionalFormats.addRule(rule);
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,45,3);
var ruletest = activeSheet.conditionalFormats.containsRule(rule, 0, 0);
alert(ruletest);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rule` | [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md) | 要检查的规则。 |
| `row` | `number` | 行索引。 |
| `column` | `number` | 列索引。 |

#### Returns

`boolean`

如果指定单元格包含指定规则，则为 `true`；否则为 `false`。

___

### <a id="count" name="count"></a> count

▸ **count**(): `number`

获取集合中规则对象的数量。

**`example`**
```javascript
//此示例计算规则数量。
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
var rule = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
rule.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.cellValueRule);
rule.ranges([new GC.Spread.Sheets.Range(0,0,5,1)]);
rule.operator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.between);
rule.style(style);
rule.value1(2);
rule.value2(100);
activeSheet.conditionalFormats.addRule(rule);
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,45,3);
var ruletest = activeSheet.conditionalFormats.count();
alert(ruletest);
```

#### Returns

`number`

集合中规则对象的数量。

___

### <a id="getrule" name="getrule"></a> getRule

▸ **getRule**(`index`): [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

使用索引获取规则。

**`example`**
```javascript
//此示例使用getRule方法。
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
var rule = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
rule.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.cellValueRule);
rule.ranges([new GC.Spread.Sheets.Range(0,0,5,1)]);
rule.operator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.between);
rule.style(style);
rule.value1(2);
rule.value2(100);
activeSheet.conditionalFormats.addRule(rule);
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,45,3);
var ruletest = activeSheet.conditionalFormats.getRule(0);
alert(ruletest.value1());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 要获取规则的索引。 |

#### Returns

[`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)

从索引获取的规则。

___

### <a id="getrules" name="getrules"></a> getRules

▸ **getRules**(`row`, `column`): [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)[]

获取指定行和列单元格的条件规则。

**`example`**
```javascript
//此示例使用getRules方法。
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
var rule = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
rule.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.cellValueRule);
rule.ranges([new GC.Spread.Sheets.Range(0,0,5,1)]);
rule.operator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.between);
rule.style(style);
rule.value1(2);
rule.value2(100);
activeSheet.conditionalFormats.addRule(rule);
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,45,3);
var ruletest = activeSheet.conditionalFormats.getRules();
alert(ruletest[0].style().backColor);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `column` | `number` | 列索引。 |

#### Returns

[`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md)[]

条件规则。

___

### <a id="removerule" name="removerule"></a> removeRule

▸ **removeRule**(`rule`): `void`

从ConditionalFormats对象中移除规则对象。

**`example`**
```javascript
//此示例使用removeRule方法。
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
var rule = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
rule.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.cellValueRule);
rule.ranges([new GC.Spread.Sheets.Range(0,0,5,1)]);
rule.operator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.between);
rule.style(style);
rule.value1(2);
rule.value2(100);
activeSheet.conditionalFormats.addRule(rule);
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,45,3);
activeSheet.conditionalFormats.removeRule(rule);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rule` | [`ConditionRuleBase`](GC.Spread.Sheets.ConditionalFormatting.ConditionRuleBase.md) | 要从ConditionalFormats对象中移除的规则对象。 |

#### Returns

`void`

___

### <a id="removerulebyrange" name="removerulebyrange"></a> removeRuleByRange

▸ **removeRuleByRange**(`row`, `column`, `rowCount`, `columnCount`): `void`

从指定的单元格范围中移除规则。

**`example`**
```javascript
//此示例使用removeRuleByRange方法。
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
var rule = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
rule.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.cellValueRule);
rule.ranges([new GC.Spread.Sheets.Range(0,0,5,1)]);
rule.operator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.between);
rule.style(style);
rule.value1(2);
rule.value2(100);
activeSheet.conditionalFormats.addRule(rule);
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,45,3);
activeSheet.conditionalFormats.removeRuleByRange(0, 0, 5, 1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 范围中第一个单元格的行索引。 |
| `column` | `number` | 范围中第一个单元格的列索引。 |
| `rowCount` | `number` | 范围中的行数。 |
| `columnCount` | `number` | 范围中的列数。 |

#### Returns

`void`
