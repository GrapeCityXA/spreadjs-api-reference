# Class: DefaultDataValidator

[Sheets](../modules/GC.Spread.Sheets.md).[DataValidation](../modules/GC.Spread.Sheets.DataValidation.md).DefaultDataValidator

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md#constructor)

### Methods

- [comparisonOperator](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md#comparisonoperator)
- [condition](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md#condition)
- [errorMessage](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md#errormessage)
- [errorStyle](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md#errorstyle)
- [errorTitle](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md#errortitle)
- [getValidList](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md#getvalidlist)
- [highlightStyle](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md#highlightstyle)
- [ignoreBlank](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md#ignoreblank)
- [inCellDropdown](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md#incelldropdown)
- [inputMessage](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md#inputmessage)
- [inputTitle](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md#inputtitle)
- [isValid](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md#isvalid)
- [preciseCompareDate](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md#precisecomparedate)
- [reset](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md#reset)
- [showErrorMessage](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md#showerrormessage)
- [showInputMessage](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md#showinputmessage)
- [type](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md#type)
- [value1](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md#value1)
- [value2](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md#value2)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new DefaultDataValidator**(`condition?`)

表示一个定义单元格数据验证规则的数据验证器。
DefaultDataValidator 类允许你指定验证条件，以此限制用户在单个单元格或单元格区域中输入的数据类型或数值范围。
它支持多种验证类型，包括整数、小数、列表、日期、时间、文本长度限制以及自定义公式。

**`example`**
```javascript
// 示例 1：本示例用于验证单元格数据。
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createTextLengthValidator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.greaterThan, 5);
activeSheet.setDataValidator(0, 0, 2, 1, dv, GC.Spread.Sheets.SheetArea.viewport);
activeSheet.setValue(0, 0, "abc");
activeSheet.setValue(1, 0, "abcdef");
```

**`example`**
```javascript
// 示例 2：创建一个整数验证器
var numberValidator = GC.Spread.Sheets.DataValidation.createNumberValidator(
    GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.between, 1, 100, true);
numberValidator.inputMessage("请输入一个 1 到 100 之间的整数");
numberValidator.errorMessage("输入值必须是 1 到 100 之间的整数");
activeSheet.setDataValidator(1, 0, 1, 1, numberValidator);
```

**`example`**
```javascript
// 示例 3：创建一个列表验证器
var listValidator = GC.Spread.Sheets.DataValidation.createListValidator("Apple,Banana,Orange");
listValidator.showInputMessage(true);
listValidator.inputTitle("水果选择");
listValidator.inputMessage("请从下拉列表中选择一种水果");
activeSheet.setDataValidator(2, 0, 1, 1, listValidator);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `condition?` | [`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md) | 定义验证规则的条件对象。 |

## Methods

### <a id="comparisonoperator" name="comparisonoperator"></a> comparisonOperator

▸ **comparisonOperator**(`value?`): `any`

获取或设置比较运算符。

**`example`**
```javascript
// 示例：为数字验证器设置比较运算符
var validator = GC.Spread.Sheets.DataValidation.createNumberValidator(
    GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.between, 1, 100);

// 获取当前比较运算符
console.log(validator.comparisonOperator()); // 输出：6（对应 between 运算符）
// 应用到单元格
activeSheet.setDataValidator(0, 0, validator);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`ComparisonOperators`](../enums/GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.md) | 比较运算符。 |

#### Returns

`any`

如果未设置值，则返回当前比较运算符；否则返回当前数据验证器对象。

___

### <a id="condition" name="condition"></a> condition

▸ **condition**(`value?`): `any`

获取或设置要验证的条件。

**`example`**
```javascript
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.averageCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.AverageConditionType.above});
nCondition.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 3)]);
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator();
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
validator.condition(nCondition);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, 5);
activeSheet.setValue(1, 0, 15);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md) | 要验证的条件。 |

#### Returns

`any`

如果未设置值，则返回当前验证条件；否则返回当前数据验证器对象。

___

### <a id="errormessage" name="errormessage"></a> errorMessage

▸ **errorMessage**(`value?`): `any`

获取或设置错误消息。

**`example`**
```javascript
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.cellValueCondition);
nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.equalsTo);
nCondition.expected(0);
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
validator.errorMessage('输入错误，请输入一个正数');
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 错误消息。 |

#### Returns

`any`

如果未设置值，则返回当前错误消息；否则返回当前数据验证器对象。

___

### <a id="errorstyle" name="errorstyle"></a> errorStyle

▸ **errorStyle**(`value?`): `any`

获取或设置要显示的错误样式。

**`example`**
```javascript
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.averageCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.AverageConditionType.above});
nCondition.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 3)]);
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
validator.errorStyle(GC.Spread.Sheets.DataValidation.ErrorStyle.warning);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, 5);
activeSheet.setValue(1, 0, 15);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`ErrorStyle`](../enums/GC.Spread.Sheets.DataValidation.ErrorStyle.md) | 要显示的错误样式。 |

#### Returns

`any`

如果未设置值，则返回当前错误样式；否则返回当前数据验证器对象。

___

### <a id="errortitle" name="errortitle"></a> errorTitle

▸ **errorTitle**(`value?`): `any`

获取或设置错误标题。

**`example`**
```javascript
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createListValidator("1,2,3");
dv.showErrorMessage(true);
dv.errorMessage("值必须为 1、2 或 3");
dv.errorTitle("自定义错误标题");
activeSheet.setDataValidator(1,1,1,1,dv,GC.Spread.Sheets.SheetArea.viewport);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 错误标题。 |

#### Returns

`any`

如果未设置值，则返回当前错误标题；否则返回当前数据验证器对象。

___

### <a id="getvalidlist" name="getvalidlist"></a> getValidList

▸ **getValidList**(`evaluator`, `baseRow`, `baseColumn`): `any`[]

如果数据验证类型为列表，则返回有效数据列表；否则返回 null。

**`example`**
```javascript
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createListValidator("1,2,3");
dv.showInputMessage(true);
dv.inputMessage("值必须为 1、2 或 3");
dv.inputTitle("提示");
activeSheet.setDataValidator(1,1,1,1,dv, GC.Spread.Sheets.SheetArea.viewport);
alert(activeSheet.getDataValidator(1,1).getValidList(activeSheet,1,1));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `evaluator` | `Object` | 可以评估条件的对象。 |
| `baseRow` | `number` | 基准行。 |
| `baseColumn` | `number` | 基准列。 |

#### Returns

`any`[]

有效数据列表或 null。

___

### <a id="highlightstyle" name="highlightstyle"></a> highlightStyle

▸ **highlightStyle**(`style?`): `any`

获取或设置无效数据单元格的高亮样式。

**`example`**
```javascript
// 此示例使用 highlightStyle 方法。
sheet.setValue(1, 1, "sss");
var dv = GC.Spread.Sheets.DataValidation.createListValidator('Fruit,Vegetable,Food');
dv.highlightStyle({
   type:GC.Spread.Sheets.DataValidation.HighlightType.dogEar,
   color:'blue',
   position:GC.Spread.Sheets.DataValidation.HighlightPosition.topLeft
});
sheet.setDataValidator(1,1, dv);
spread.options.highlightInvalidData = true;
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `style?` | [`IHighLightStyle`](../interfaces/GC.Spread.Sheets.DataValidation.IHighLightStyle.md) | 无效数据单元格的样式。 |

#### Returns

`any`

如果未设置值，则返回当前高亮样式对象；否则返回当前数据验证器对象。

___

### <a id="ignoreblank" name="ignoreblank"></a> ignoreBlank

▸ **ignoreBlank**(`value?`): `any`

获取或设置是否忽略空值。

**`example`**
```javascript
// 此示例使用 ignoreBlank 方法。
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.cellValueCondition);
nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.equalsTo);
nCondition.expected(0);
// 当选项为 false 时，验证失败并显示红色警告。
// 当选项为 true 时，空白单元格被视为零且验证成功。
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
| `value?` | `boolean` | 指示是否忽略空值。 |

#### Returns

`any`

如果未设置值，则返回当前是否忽略空值的状态；否则返回当前数据验证器对象。

___

### <a id="incelldropdown" name="incelldropdown"></a> inCellDropdown

▸ **inCellDropdown**(`value?`): `any`

获取或设置是否显示下拉按钮。

**`example`**
```javascript
// 此示例使用 inCellDropdown 方法。
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createListValidator("1,2,3");
dv.showInputMessage(true);
dv.inputMessage("值必须为 1、2 或 3");
dv.inputTitle("提示");
dv.inCellDropdown(true);
activeSheet.setDataValidator(1,1,1,1,dv,GC.Spread.Sheets.SheetArea.viewport);
var validList = activeSheet.getDataValidator(1, 1).getValidList(activeSheet, 1, 1);
alert(validList);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 指示是否显示下拉按钮。 |

#### Returns

`any`

如果未设置值，则返回当前是否显示下拉按钮的状态；否则返回当前数据验证器对象。

___

### <a id="inputmessage" name="inputmessage"></a> inputMessage

▸ **inputMessage**(`value?`): `any`

获取或设置输入消息。

**`example`**
```javascript
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createListValidator("1,2,3");
dv.showInputMessage(true);
dv.inputMessage("值必须为 1、2 或 3");
dv.inputTitle("提示");
activeSheet.setDataValidator(1,1,1,1,dv,GC.Spread.Sheets.SheetArea.viewport);
alert(activeSheet.getDataValidator(1,1).getValidList(activeSheet,1,1));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 输入消息。 |

#### Returns

`any`

如果未设置值，则返回当前输入消息；否则返回当前数据验证器对象。

___

### <a id="inputtitle" name="inputtitle"></a> inputTitle

▸ **inputTitle**(`value?`): `any`

获取或设置输入标题。

**`example`**
```javascript
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createListValidator("1,2,3");
dv.showInputMessage(true);
dv.inputMessage("值必须为 1、2 或 3");
dv.inputTitle("提示");
activeSheet.setDataValidator(1,1,1,1,dv,GC.Spread.Sheets.SheetArea.viewport);
alert(activeSheet.getDataValidator(1,1).getValidList(activeSheet,1,1));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 输入标题。 |

#### Returns

`any`

如果未设置值，则返回当前输入标题；否则返回当前数据验证器对象。

___

### <a id="isvalid" name="isvalid"></a> isValid

▸ **isValid**(`evaluator`, `baseRow`, `baseColumn`, `actual`): `boolean`

确定当前值是否有效。

**`example`**
```javascript
sheet.setArray(0, 0,
    [
        [ 3.4 ],
        [ 102.8 ]
    ]);
var expression1 = 1.1;
var expression2 = 101.2;
var dv = GC.Spread.Sheets.DataValidation.createNumberValidator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.between, expression1, expression2, false);
sheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(dv);
dv = sheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(); // SDM 的限制，设置样式时会复制 dv。
console.log(dv.isValid(sheet, 0, 0, 3)); // true
console.log(dv.isValid(sheet, 0, 0, 1)); // false
console.log(dv.isValid(sheet, 0, 0, 101)); // true
console.log(dv.isValid(sheet, 0, 0, 0)); // false
console.log(dv.isValid(sheet, 0, 0, 120.0)); // false
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `evaluator` | `Object` | 评估器。 |
| `baseRow` | `number` | 基准行。 |
| `baseColumn` | `number` | 基准列。 |
| `actual` | `Object` | 当前值。 |

#### Returns

`boolean`

如果值有效则返回 `true`；否则返回 `false`。

___

### <a id="precisecomparedate" name="precisecomparedate"></a> preciseCompareDate

▸ **preciseCompareDate**(`value?`): `any`

获取或设置是否比较整天或精确日期时间。

**`example`**
```javascript
// 此示例使用 preciseCompareDate 方法。
var dateCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.dateCondition);
dateCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.DateCompareType.after);
dateCondition.expected(new Date(2020, 4, 22, 6));
// 当选项为 false 时，验证器比较整天，日期相同因此验证失败并显示红色警告。
// 当选项为 true 时，7 点的时间大于 6 点，因此验证成功。
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

如果未设置值，则返回当前是否启用精确日期时间比较的状态；否则返回当前数据验证器对象。

___

### <a id="reset" name="reset"></a> reset

▸ **reset**(): `void`

重置数据验证器。

**`example`**
```javascript
// 此示例使用 reset 方法。
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.cellValueCondition);
nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.equalsTo);
nCondition.expected(0);
// 当选项为 false 时，验证失败并显示红色警告。
// 当选项为 true 时，空白单元格被视为零，验证成功。
nCondition.treatNullValueAsZero(false);
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
validator.ignoreBlank(false);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, null);
validator.reset();
```

#### Returns

`void`

___

### <a id="showerrormessage" name="showerrormessage"></a> showErrorMessage

▸ **showErrorMessage**(`value?`): `any`

获取或设置是否显示错误消息。

**`example`**
```javascript
spread.options.highlightInvalidData = true;
// 如果公式条件返回 true，则公式验证器判定为有效。
var dv = GC.Spread.Sheets.DataValidation.createFormulaValidator("A1&gt;0");
dv.showInputMessage(true);
dv.inputMessage("在 A1 中输入大于 0 的值。");
dv.inputTitle("提示");
dv.showErrorMessage(true);
dv.errorMessage("值不正确");
activeSheet.setDataValidator(0, 0, 1, 1, dv, GC.Spread.Sheets.SheetArea.viewport);
// 绑定事件
activeSheet.bind(GC.Spread.Sheets.Events.ValidationError, function (sender, args) {
    if (args.validator.showErrorMessage()) {
        if (confirm(args.validator.errorMessage())) {
            args.validationResult = GC.Spread.Sheets.DataValidation.DataValidationResult.retry;
        } else {
            args.validationResult = GC.Spread.Sheets.DataValidation.DataValidationResult.forceApply;
        }
    }
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 指示是否显示错误消息。 |

#### Returns

`any`

如果未设置值，则返回当前是否显示错误消息的状态；否则返回当前数据验证器对象。

___

### <a id="showinputmessage" name="showinputmessage"></a> showInputMessage

▸ **showInputMessage**(`value?`): `any`

获取或设置是否显示输入标题和输入消息。

**`example`**
```javascript
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createListValidator("1,2,3");
dv.showInputMessage(true);
dv.inputMessage("值必须为 1、2 或 3");
dv.inputTitle("提示");
activeSheet.setDataValidator(1,1,1,1,dv,GC.Spread.Sheets.SheetArea.viewport);
alert(activeSheet.getDataValidator(1,1).getValidList(activeSheet,1,1));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 指示是否显示输入标题和输入消息。 |

#### Returns

`any`

如果未设置值，则返回当前是否显示输入标题和输入消息的状态；否则返回当前数据验证器对象。

___

### <a id="type" name="type"></a> type

▸ **type**(`value?`): `any`

获取或设置此数据验证器的条件类型。

**`example`**
```javascript
// 此示例使用 preciseCompareDate 方法。
var dateCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.dateCondition);
dateCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.DateCompareType.after);
dateCondition.expected(new Date(2020, 4, 22, 6));
// 当选项为 false 时，验证器比较整个日期，日期相同因此验证失败并显示红色警告。
// 当选项为 true 时，日期时间 7 点大于 6 点，因此验证成功。
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
| `value?` | [`CriteriaType`](../enums/GC.Spread.Sheets.DataValidation.CriteriaType.md) | 此数据验证器的条件类型。 |

#### Returns

`any`

如果未设置值，则返回当前数据验证器的条件类型；否则返回当前数据验证器对象。

___

### <a id="value1" name="value1"></a> value1

▸ **value1**(`baseRow?`, `baseColumn?`): `any`

获取数据验证的第一个值。

**`example`**
```javascript
// 此示例验证单元格值。
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.cellValueCondition);
nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.equalsTo);
nCondition.expected(0);
// 当选项为 false 时，验证失败并显示红色警告。
// 当选项为 true 时，空白单元格被视为零，验证成功。
nCondition.treatNullValueAsZero(false);
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
validator.ignoreBlank(false);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, null);
alert(validator.value1());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `baseRow?` | `number` | 基准行。 |
| `baseColumn?` | `number` | 基准列。 |

#### Returns

`any`

第一个值。

___

### <a id="value2" name="value2"></a> value2

▸ **value2**(`baseRow?`, `baseColumn?`): `any`

获取数据验证的第二个值。

**`example`**
```javascript
// 本示例演示如何获取数据验证的第二个值。
spread.options.highlightInvalidData = true;
// 创建一个使用 between 运算符的数字验证器（范围 10 到 100）
var validator = GC.Spread.Sheets.DataValidation.createNumberValidator(
    GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.between,
    10,  // 第一个值：最小值
    100  // 第二个值：最大值
);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
activeSheet.setValue(0,0,5);
// 此时 value1() 和 value2() 会返回不同的值
console.log(validator.value2()); // 输出：100（最大值）
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `baseRow?` | `number` | 基准行。 |
| `baseColumn?` | `number` | 基准列。 |

#### Returns

`any`

第二个值。
