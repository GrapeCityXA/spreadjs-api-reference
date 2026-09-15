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

表示数据验证器。

**`example`**
```
//此示例验证单元格数据。
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createTextLengthValidator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.greaterThan, 5);
activeSheet.setDataValidator(0, 0, 1, 1, dv, GC.Spread.Sheets.SheetArea.viewport);
activeSheet.setValue(0, 0, "abcf");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `condition?` | [`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md) |

## Methods

### <a id="comparisonoperator" name="comparisonoperator"></a> comparisonOperator

▸ **comparisonOperator**(`value?`): `any`

获取或设置比较运算符。

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`ComparisonOperators`](../enums/GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.md) |

#### Returns

`any`

如果未设置值，则返回比较运算符；否则返回数据验证器。

___

### <a id="condition" name="condition"></a> condition

▸ **condition**(`value?`): `any`

获取或设置要验证的条件。

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | [`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md) |

#### Returns

`any`

如果未设置值，则返回要验证的条件；否则返回数据验证器。

___

### <a id="errormessage" name="errormessage"></a> errorMessage

▸ **errorMessage**(`value?`): `any`

获取或设置错误消息。

**`example`**
```
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.cellValueCondition);
nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.equalsTo);
nCondition.expected(0);
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
validator.errorMessage('输入错误，请输入一个正数');
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置值，则返回错误消息；否则返回数据验证器。

___

### <a id="errorstyle" name="errorstyle"></a> errorStyle

▸ **errorStyle**(`value?`): `any`

获取或设置要显示的错误样式。

**`example`**
```
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

| Name | Type |
| :------ | :------ |
| `value?` | [`ErrorStyle`](../enums/GC.Spread.Sheets.DataValidation.ErrorStyle.md) |

#### Returns

`any`

如果未设置值，则返回要显示的错误样式；否则返回数据验证器。

___

### <a id="errortitle" name="errortitle"></a> errorTitle

▸ **errorTitle**(`value?`): `any`

获取或设置错误标题。

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置值，则返回错误标题；否则返回数据验证器。

___

### <a id="getvalidlist" name="getvalidlist"></a> getValidList

▸ **getValidList**(`evaluator`, `baseRow`, `baseColumn`): `any`[]

如果数据验证类型为列表，则返回有效数据列表；否则返回 null。

**`example`**
```
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
```
//此示例使用 highlightStyle 方法。
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

| Name | Type |
| :------ | :------ |
| `style?` | [`IHighLightStyle`](../interfaces/GC.Spread.Sheets.DataValidation.IHighLightStyle.md) |

#### Returns

`any`

如果未设置值，则返回高亮样式对象；否则返回数据验证器。

___

### <a id="ignoreblank" name="ignoreblank"></a> ignoreBlank

▸ **ignoreBlank**(`value?`): `any`

获取或设置是否忽略空值。

**`example`**
```
//此示例使用 IgnoreBlank 方法。
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.cellValueCondition);
nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.equalsTo);
nCondition.expected(0);
//当选项为 false 时，验证失败并显示红色警告。
//当选项为 true 时，空白单元格被视为零且验证成功。
nCondition.treatNullValueAsZero(false);
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
validator.ignoreBlank(false);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, null);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置值，则返回是否忽略空值；否则返回数据验证器。

___

### <a id="incelldropdown" name="incelldropdown"></a> inCellDropdown

▸ **inCellDropdown**(`value?`): `any`

获取或设置是否显示下拉按钮。

**`example`**
```
//此示例使用 inCellDropdown 方法。
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

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置值，则返回是否显示下拉按钮；否则返回数据验证器。

___

### <a id="inputmessage" name="inputmessage"></a> inputMessage

▸ **inputMessage**(`value?`): `any`

获取或设置输入消息。

**`example`**
```
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createListValidator("1,2,3");
dv.showInputMessage(true);
dv.inputMessage("值必须为 1、2 或 3");
dv.inputTitle("提示");
activeSheet.setDataValidator(1,1,1,1,dv,GC.Spread.Sheets.SheetArea.viewport);
alert(activeSheet.getDataValidator(1,1).getValidList(activeSheet,1,1));
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置值，则返回输入消息；否则返回数据验证器。

___

### <a id="inputtitle" name="inputtitle"></a> inputTitle

▸ **inputTitle**(`value?`): `any`

获取或设置输入标题。

**`example`**
```
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createListValidator("1,2,3");
dv.showInputMessage(true);
dv.inputMessage("值必须为 1、2 或 3");
dv.inputTitle("提示");
activeSheet.setDataValidator(1,1,1,1,dv,GC.Spread.Sheets.SheetArea.viewport);
alert(activeSheet.getDataValidator(1,1).getValidList(activeSheet,1,1));
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置值，则返回输入标题；否则返回数据验证器。

___

### <a id="isvalid" name="isvalid"></a> isValid

▸ **isValid**(`evaluator`, `baseRow`, `baseColumn`, `actual`): `boolean`

确定当前值是否有效。

**`example`**
```
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
```
//此示例使用 preciseCompareDate 方法。
var dateCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.dateCondition);
dateCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.DateCompareType.after);
dateCondition.expected(new Date(2020, 4, 22, 6));
//当选项为 false 时，验证器比较整天，它们相同，所以验证失败并显示红色警告。
//当选项为 true 时，7 点的时间大于 6 点，所以结果为成功。
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(dateCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.date);
validator.preciseCompareDate(true);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, new Date(2020, 4, 22, 7));
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置值，则返回是否比较整天或精确日期时间；否则返回数据验证器。

___

### <a id="reset" name="reset"></a> reset

▸ **reset**(): `void`

重置数据验证器。

**`example`**
```
//此示例使用 reset 方法。
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.cellValueCondition);
nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.equalsTo);
nCondition.expected(0);
//当选项为 false 时，验证失败并显示红色警告。
//当选项为 true 时，空白单元格被视为零，验证成功。
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
```
spread.options.highlightInvalidData = true;
//如果公式条件返回 true，则公式验证器有效。
var dv = GC.Spread.Sheets.DataValidation.createFormulaValidator("A1&gt;0");
dv.showInputMessage(true);
dv.inputMessage("在 A1 中输入大于 0 的值。");
dv.inputTitle("提示");
dv.showErrorMessage(true);
dv.errorMessage("值不正确");
activeSheet.setDataValidator(0, 0, 1, 1, dv, GC.Spread.Sheets.SheetArea.viewport);
//绑定
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

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置值，则返回是否显示错误消息；否则返回数据验证器。

___

### <a id="showinputmessage" name="showinputmessage"></a> showInputMessage

▸ **showInputMessage**(`value?`): `any`

获取或设置是否显示输入标题和输入消息。

**`example`**
```
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createListValidator("1,2,3");
dv.showInputMessage(true);
dv.inputMessage("值必须为 1、2 或 3");
dv.inputTitle("提示");
activeSheet.setDataValidator(1,1,1,1,dv,GC.Spread.Sheets.SheetArea.viewport);
alert(activeSheet.getDataValidator(1,1).getValidList(activeSheet,1,1));
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置值，则返回是否显示输入标题和输入消息；否则返回数据验证器。

___

### <a id="type" name="type"></a> type

▸ **type**(`value?`): `any`

获取或设置此数据验证器的条件类型。

**`example`**
```
//此示例使用 preciseCompareDate 方法。
var dateCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.dateCondition);
dateCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.DateCompareType.after);
dateCondition.expected(new Date(2020, 4, 22, 6));
//当选项为 false 时，验证器比较整个日期，它们相同，因此验证失败并显示红色警告。
//当选项为 true 时，日期时间 7 点大于 6 点，因此结果成功。
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(dateCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.date);
validator.preciseCompareDate(true);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, new Date(2020, 4, 22, 7));
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`CriteriaType`](../enums/GC.Spread.Sheets.DataValidation.CriteriaType.md) |

#### Returns

`any`

如果未设置值，则返回此数据验证器的条件类型；否则返回数据验证器。

___

### <a id="value1" name="value1"></a> value1

▸ **value1**(`baseRow?`, `baseColumn?`): `any`

获取数据验证的第一个值。

**`example`**
```
//此示例验证单元格值。
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.cellValueCondition);
nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.equalsTo);
nCondition.expected(0);
//当选项为 false 时，验证失败并显示红色警告。
//当选项为 true 时，空白单元格被视为零，验证成功。
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

| Name | Type |
| :------ | :------ |
| `baseRow?` | `number` |
| `baseColumn?` | `number` |

#### Returns

`any`

第一个值。

___

### <a id="value2" name="value2"></a> value2

▸ **value2**(`baseRow?`, `baseColumn?`): `any`

获取数据验证的第二个值。

**`example`**
```
//此示例验证单元格值。
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.cellValueCondition);
nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.equalsTo);
nCondition.expected(0);
//当选项为 false 时，验证失败并显示红色警告。
//当选项为 true 时，空白单元格被视为零，验证成功。
nCondition.treatNullValueAsZero(false);
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
validator.ignoreBlank(false);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, null);
alert(validator.value2());
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `baseRow?` | `number` |
| `baseColumn?` | `number` |

#### Returns

`any`

第二个值。
