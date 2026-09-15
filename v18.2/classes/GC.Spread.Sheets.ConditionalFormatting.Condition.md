# Class: Condition

[Sheets](../modules/GC.Spread.Sheets.md).[ConditionalFormatting](../modules/GC.Spread.Sheets.ConditionalFormatting.md).Condition

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.ConditionalFormatting.Condition.md#constructor)

### Methods

- [compareType](GC.Spread.Sheets.ConditionalFormatting.Condition.md#comparetype)
- [evaluate](GC.Spread.Sheets.ConditionalFormatting.Condition.md#evaluate)
- [expected](GC.Spread.Sheets.ConditionalFormatting.Condition.md#expected)
- [formula](GC.Spread.Sheets.ConditionalFormatting.Condition.md#formula)
- [getExpected](GC.Spread.Sheets.ConditionalFormatting.Condition.md#getexpected)
- [getValidList](GC.Spread.Sheets.ConditionalFormatting.Condition.md#getvalidlist)
- [ignoreBlank](GC.Spread.Sheets.ConditionalFormatting.Condition.md#ignoreblank)
- [ignoreCase](GC.Spread.Sheets.ConditionalFormatting.Condition.md#ignorecase)
- [item1](GC.Spread.Sheets.ConditionalFormatting.Condition.md#item1)
- [item2](GC.Spread.Sheets.ConditionalFormatting.Condition.md#item2)
- [preciseCompareDate](GC.Spread.Sheets.ConditionalFormatting.Condition.md#precisecomparedate)
- [ranges](GC.Spread.Sheets.ConditionalFormatting.Condition.md#ranges)
- [reset](GC.Spread.Sheets.ConditionalFormatting.Condition.md#reset)
- [treatNullValueAsZero](GC.Spread.Sheets.ConditionalFormatting.Condition.md#treatnullvalueaszero)
- [useWildCards](GC.Spread.Sheets.ConditionalFormatting.Condition.md#usewildcards)
- [fromDay](GC.Spread.Sheets.ConditionalFormatting.Condition.md#fromday)
- [fromFormula](GC.Spread.Sheets.ConditionalFormatting.Condition.md#fromformula)
- [fromMonth](GC.Spread.Sheets.ConditionalFormatting.Condition.md#frommonth)
- [fromQuarter](GC.Spread.Sheets.ConditionalFormatting.Condition.md#fromquarter)
- [fromSource](GC.Spread.Sheets.ConditionalFormatting.Condition.md#fromsource)
- [fromWeek](GC.Spread.Sheets.ConditionalFormatting.Condition.md#fromweek)
- [fromYear](GC.Spread.Sheets.ConditionalFormatting.Condition.md#fromyear)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Condition**(`conditionType`, `args`)

使用参数对象表示条件项。

**`example`**
```
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.averageCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.AverageConditionType.above});
nCondition.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 3)]);
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, 5);
activeSheet.setValue(1, 0, 15);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `conditionType` | [`ConditionType`](../enums/GC.Spread.Sheets.ConditionalFormatting.ConditionType.md) |
| `args` | `Object` |

## Methods

### <a id="comparetype" name="comparetype"></a> compareType

▸ **compareType**(`value?`): `any`

获取或设置规则比较类型。

**`example`**
```
 var data = ["testing", 'est', 'testtest', 'tesla', 'taste'];
 activeSheet.setArray(0,0,data);
 //此示例将高亮显示不包含'test'的单元格
 var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.textCondition);
 nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.TextCompareType.contains);
 nCondition.expected("test");
 var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
 validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
 activeSheet.getRange(0, 0, 5,1).validator(validator);
 spread.options.highlightInvalidData = true;
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`LogicalOperators`](../enums/GC.Spread.Sheets.ConditionalFormatting.LogicalOperators.md) \| [`GeneralComparisonOperators`](../enums/GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.md) \| [`TextCompareType`](../enums/GC.Spread.Sheets.ConditionalFormatting.TextCompareType.md) \| [`ColorCompareType`](../enums/GC.Spread.Sheets.ConditionalFormatting.ColorCompareType.md) \| [`DateCompareType`](../enums/GC.Spread.Sheets.ConditionalFormatting.DateCompareType.md) | 规则比较类型。 |

#### Returns

`any`

如果未设置值，则返回规则比较类型；否则返回条件。

___

### <a id="evaluate" name="evaluate"></a> evaluate

▸ **evaluate**(`evaluator`, `baseRow`, `baseColumn`, `actualObj`): `boolean`

使用指定的评估器评估条件。

**`example`**
```
 //此示例将高亮显示不包含'test'的单元格
 var data = ["testing", 'est', 'testtest', 'tesla', 'taste'];
 activeSheet.setArray(0, 0, data);
 var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.textCondition);
 nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.TextCompareType.contains);
 nCondition.expected("test");
 var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
 validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
 activeSheet.getRange(0, 0, 5, 1).validator(validator);
 spread.options.highlightInvalidData = true;
 for (var i = 0; i < 10; i++) {
     var result = nCondition.evaluate(activeSheet, i, 0, data[i]);
     console.log(result);
 }
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `evaluator` | `Object` | 可以评估表达式或函数的评估器。 |
| `baseRow` | `number` | 评估的基础行索引。 |
| `baseColumn` | `number` | 评估的基础列索引。 |
| `actualObj` | `Object` | 用于评估的object1的实际值。 |

#### Returns

`boolean`

如果结果成功则返回`true`；否则返回`false`。

___

### <a id="expected" name="expected"></a> expected

▸ **expected**(`value?`): `any`

获取或设置期望值。

**`example`**
```
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.dateCondition);
nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.DateCompareType.before);
nCondition.expected(new Date(2012, 11, 31));
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, new Date(2012, 12, 12));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `any` | 期望值。 |

#### Returns

`any`

如果未设置值，则返回期望值；否则返回条件。

___

### <a id="formula" name="formula"></a> formula

▸ **formula**(`formulaOrBaseRow?`, `baseColumn?`): `any`

获取或设置期望的公式。

**`example`**
```
var textLengthCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.textLengthCondition);
textLengthCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.greaterThan);
textLengthCondition.formula("$C$1"); // 用于计算数字的公式。
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(textLengthCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, "abcf");
//在$C$1中设置值3，执行此代码后，Cell(0,0)中的值有效。
activeSheet.setValue(0, 2, 3);
//在$C$1中设置值5，执行此代码后，Cell(0,0)中的值无效。
// activeSheet.setValue(0, 2, 5);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `formulaOrBaseRow?` | `string` \| `number` | 期望的公式或基础行。 |
| `baseColumn?` | `number` | 基础列。 |

#### Returns

`any`

如果未设置值或设置了baseRow和baseColumn，则返回期望的公式；否则返回条件。

___

### <a id="getexpected" name="getexpected"></a> getExpected

▸ **getExpected**(`evaluator`, `baseRow`, `baseColumn`): `Object`

获取期望值。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `evaluator` | `Object` | 可以计算表达式或函数的计算器。 |
| `baseRow` | `number` | 用于计算的基准行索引。 |
| `baseColumn` | `number` | 用于计算的基准列索引。 |

#### Returns

`Object`

期望值。

___

### <a id="getvalidlist" name="getvalidlist"></a> getValidList

▸ **getValidList**(`evaluator`, `baseRow`, `baseColumn`): `any`[]

返回有效数据项列表。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `evaluator` | `Object` | 可以计算表达式或函数的计算器。 |
| `baseRow` | `number` | 用于计算的基准行索引。 |
| `baseColumn` | `number` | 用于计算的基准列索引。 |

#### Returns

`any`[]

有效数据项列表。

___

### <a id="ignoreblank" name="ignoreblank"></a> ignoreBlank

▸ **ignoreBlank**(`value?`): `any`

获取或设置是否忽略空白单元格。

**`example`**
```
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.textCondition);
nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.TextCompareType.contains);
nCondition.expected("te?t");
nCondition.ignoreBlank(true);
nCondition.ignoreCase(true);
nCondition.useWildCards(true);
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, "testing");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否忽略空白单元格。 |

#### Returns

`any`

如果未设置值，则返回是否忽略空白单元格；否则返回条件。

___

### <a id="ignorecase" name="ignorecase"></a> ignoreCase

▸ **ignoreCase**(`value?`): `any`

获取或设置执行比较时是否忽略大小写。

**`example`**
```
//此示例创建文本条件。
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.textCondition);
nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.TextCompareType.contains);
nCondition.expected("te?t");
nCondition.ignoreBlank(true);
nCondition.ignoreCase(true);
nCondition.useWildCards(true);
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, "testing");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 执行比较时是否忽略大小写。 |

#### Returns

`any`

如果未设置值，则返回执行比较时是否忽略大小写；否则返回条件。

___

### <a id="item1" name="item1"></a> item1

▸ **item1**(`value?`): [`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

获取或设置第一个条件。

**`example`**
```
//此示例验证日期。
var condition1 = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.dateCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.DateCompareType.afterEqualsTo, expected: new Date(2012, 11, 31)});
var condition2 = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.dateCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.DateCompareType.beforeEqualsTo, expected: new Date(2013, 11, 31)});
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.relationCondition);
nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.LogicalOperators.and);
nCondition.item1(condition1);
nCondition.item2(condition2);
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, new Date(2012, 11, 25));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md) | 第一个条件。 |

#### Returns

[`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

如果未设置值，则返回第一个条件；否则返回关系条件。

___

### <a id="item2" name="item2"></a> item2

▸ **item2**(`value?`): [`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

获取或设置第二个条件。

**`example`**
```
//此示例验证日期。
var condition1 = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.dateCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.DateCompareType.afterEqualsTo, expected: new Date(2012, 11, 31)});
var condition2 = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.dateCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.DateCompareType.beforeEqualsTo, expected: new Date(2013, 11, 31)});
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.relationCondition);
nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.LogicalOperators.and);
nCondition.item1(condition1);
nCondition.item2(condition2);
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, new Date(2012, 11, 25));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md) | 第二个条件。 |

#### Returns

[`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

如果未设置值，则返回第二个条件；否则返回关系条件。

___

### <a id="precisecomparedate" name="precisecomparedate"></a> preciseCompareDate

▸ **preciseCompareDate**(`value?`): `any`

获取或设置是否比较整天或精确日期时间。

**`example`**
```
//此示例使用preciseCompareDate方法。
var dateCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.dateCondition);
dateCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.DateCompareType.after);
dateCondition.expected(new Date(2020, 4, 22, 6));
//当选项为false时，验证器比较整天，它们相同，所以验证失败并显示红色警告。
//当选项为true时，日期时间7点大于6点，所以结果成功。
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(dateCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.date);
validator.preciseCompareDate(true);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, new Date(2020, 4, 22, 7));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 指示是否比较整天或精确日期时间。 |

#### Returns

`any`

如果未设置值，则返回是否比较整天或精确日期时间；否则返回数据验证器。

___

### <a id="ranges" name="ranges"></a> ranges

▸ **ranges**(`value?`): `any`

获取或设置条件范围。

**`example`**
```
//此示例创建唯一条件。
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.uniqueCondition);
nCondition.expected(true);
nCondition.ranges([new GC.Spread.Sheets.Range(0, 0, 5, 1)]);
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, 5);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`Range`](GC.Spread.Sheets.Range.md)[] | 条件范围。 |

#### Returns

`any`

如果未设置值，则返回条件范围；否则返回条件。

___

### <a id="reset" name="reset"></a> reset

▸ **reset**(): `void`

重置此实例。

**`example`**
```
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.numberCondition);
nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.greaterThan);
nCondition.expected(5);
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, 5);
//创建按钮
$("#button1").click(function () {
activeSheet.suspendPaint();
nCondition.reset();
activeSheet.resumePaint();
    });
```

#### Returns

`void`

___

### <a id="treatnullvalueaszero" name="treatnullvalueaszero"></a> treatNullValueAsZero

▸ **treatNullValueAsZero**(`value?`): `any`

获取或设置是否将单元格中的空值视为零。

**`example`**
```
//此示例设置treatNullValueAsZero方法。
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.cellValueCondition);
nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.equalsTo);
nCondition.expected(0);
//当选项为false时，验证失败并显示红色警告。
//当选项为true时，空单元格被视为零且验证成功。
nCondition.treatNullValueAsZero(false);
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
validator.ignoreBlank(false);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, null);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否将单元格中的空值视为零。 |

#### Returns

`any`

如果未设置值，则返回是否将单元格中的空值视为零；否则返回条件。

___

### <a id="usewildcards" name="usewildcards"></a> useWildCards

▸ **useWildCards**(`value?`): `any`

获取或设置是否使用通配符比较字符串。

**`example`**
```
//此示例允许使用通配符。
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.textCondition);
nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.TextCompareType.contains);
nCondition.expected("te?t");
nCondition.ignoreBlank(true);
nCondition.ignoreCase(true);
nCondition.useWildCards(true);
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, "testing");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否使用通配符比较字符串。 |

#### Returns

`any`

如果未设置值，则返回是否使用通配符比较字符串；否则返回条件。

___

### <a id="fromday" name="fromday"></a> fromDay

▸ `Static` **fromDay**(`day`): [`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

从指定的日期创建日期扩展条件对象。

**`static`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `day` | `number` | 日期。 |

#### Returns

[`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

日期扩展条件对象。

___

### <a id="fromformula" name="fromformula"></a> fromFormula

▸ `Static` **fromFormula**(`formula`): [`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

从公式数据创建区域条件。

**`static`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `formula` | `string` | 指定包含数据项范围的公式。 |

#### Returns

[`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

区域条件。

___

### <a id="frommonth" name="frommonth"></a> fromMonth

▸ `Static` **fromMonth**(`month`): [`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

从指定的月份创建日期扩展条件对象。

**`static`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `month` | `number` | 月份。第一个月为0。 |

#### Returns

[`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

日期扩展条件对象。

___

### <a id="fromquarter" name="fromquarter"></a> fromQuarter

▸ `Static` **fromQuarter**(`quarter`): [`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

从指定的季度创建日期扩展条件对象。

**`static`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `quarter` | [`QuarterType`](../enums/GC.Spread.Sheets.ConditionalFormatting.QuarterType.md) | 季度。 |

#### Returns

[`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

日期扩展条件对象。

___

### <a id="fromsource" name="fromsource"></a> fromSource

▸ `Static` **fromSource**(`expected`): [`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

从源数据创建区域条件。

**`static`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `expected` | `string` | 期望的源，用逗号(",")分隔每个数据项。 |

#### Returns

[`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

区域条件。

___

### <a id="fromweek" name="fromweek"></a> fromWeek

▸ `Static` **fromWeek**(`week`): [`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

从指定的周创建日期扩展条件对象。

**`static`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `week` | `number` | 周数。 |

#### Returns

[`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

日期扩展条件对象。

___

### <a id="fromyear" name="fromyear"></a> fromYear

▸ `Static` **fromYear**(`year`): [`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

从指定的年份创建日期扩展条件对象。

**`static`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `year` | `number` | 年份。 |

#### Returns

[`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)

日期扩展条件对象。
