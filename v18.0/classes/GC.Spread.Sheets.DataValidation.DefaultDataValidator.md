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

数据验证器

**`代码示例`**
``` javascript
//本示例验证单元数据
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

获取或设置比较运算符

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`ComparisonOperators`](../enums/GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.md) |

#### Returns

`any`

如果未设置任何值，则返回比较运算符；否则，返回数据验证器

___

### <a id="condition" name="condition"></a> condition

▸ **condition**(`value?`): `any`

获取或设置要验证的条件

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

如果未设置任何值，则返回条件以进行验证；否则，返回数据验证器

___

### <a id="errormessage" name="errormessage"></a> errorMessage

▸ **errorMessage**(`value?`): `any`

获取或设置错误消息

**`example`**
```
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.cellValueCondition);
nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.equalsTo);
nCondition.expected(0);
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.custom);
validator.errorMessage('Incorrect input, please input a positive number');
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置任何值，则返回错误消息否则，返回数据验证器

___

### <a id="errorstyle" name="errorstyle"></a> errorStyle

▸ **errorStyle**(`value?`): `any`

获取或设置要显示的错误样式

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

如果未设置任何值，则返回要显示的错误样式否则，返回数据验证器

___

### <a id="errortitle" name="errortitle"></a> errorTitle

▸ **errorTitle**(`value?`): `any`

获取或设置错误标题

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置任何值，则返回错误标题否则，返回数据验证器

___

### <a id="getvalidlist" name="getvalidlist"></a> getValidList

▸ **getValidList**(`evaluator`, `baseRow`, `baseColumn`): `any`[]

如果数据验证类型为列表，则返回有效数据列表；否则，返回null

**`example`**
```
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createListValidator("1,2,3");
dv.showInputMessage(true);
dv.inputMessage("Value must be 1,2 or 3");
dv.inputTitle("tip");
activeSheet.setDataValidator(1,1,1,1,dv, GC.Spread.Sheets.SheetArea.viewport);
alert(activeSheet.getDataValidator(1,1).getValidList(activeSheet,1,1));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `evaluator` | `Object` | 可以计算条件的对象 |
| `baseRow` | `number` | 基行 |
| `baseColumn` | `number` | 基列 |

#### Returns

`any`[]

有效数据列表或null

___

### <a id="highlightstyle" name="highlightstyle"></a> highlightStyle

▸ **highlightStyle**(`style?`): `Object`

获取或设置无效的数据单元格高亮显示样式

**`代码示例`**
``` javascript
//本示例使用highlightStyle方法
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

如果未设置任何值，则返回高亮显示样式对象；否则，返回数据验证器

___

### <a id="ignoreblank" name="ignoreblank"></a> ignoreBlank

▸ **ignoreBlank**(`value?`): `any`

获取或设置是否忽略空值

**`代码示例`**
``` javascript
//本示例使用IgnoreBlank方法
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.cellValueCondition);
nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.equalsTo);
nCondition.expected(0);
//当选项为false时，验证失败并显示红色警报
//当选项为true时，将把空白单元格视为零，验证成功
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

如果未设置任何值，则返回是否忽略空值否则，返回数据验证器

___

### <a id="incelldropdown" name="incelldropdown"></a> inCellDropdown

▸ **inCellDropdown**(`value?`): `any`

获取或设置是否显示下拉按钮

**`代码示例`**
``` javascript
//本示例使用inCellDropdown方法
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createListValidator("1,2,3");
dv.showInputMessage(true);
dv.inputMessage("Value must be 1,2 or 3");
dv.inputTitle("tip");
dv.inCellDropdown(true);
activeSheet.setDataValidator(1,1,1,1,dv,GC.Spread.Sheets.SheetArea.viewport);
var validList = activeSheet.getDataValidator(1, 1).getValidList(activeSheet, 1, 1);
alert(validList);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否显示下拉按钮 |

#### Returns

`any`

如果未设置任何值，则返回是否显示下拉按钮；否则，返回数据验证器

___

### <a id="inputmessage" name="inputmessage"></a> inputMessage

▸ **inputMessage**(`value?`): `any`

获取或设置输入消息

**`代码示例`**
``` javascript
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createListValidator("1,2,3");
dv.showInputMessage(true);
dv.inputMessage("Value must be 1,2 or 3");
dv.inputTitle("tip");
activeSheet.setDataValidator(1,1,1,1,dv,GC.Spread.Sheets.SheetArea.viewport);
alert(activeSheet.getDataValidator(1,1).getValidList(activeSheet,1,1));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 输入消息 |

#### Returns

`any`

如果未设置任何值，则返回输入消息否则，返回数据验证器

___

### <a id="inputtitle" name="inputtitle"></a> inputTitle

▸ **inputTitle**(`value?`): `any`

获取或设置输入标题

**`代码示例`**
``` javascript
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createListValidator("1,2,3");
dv.showInputMessage(true);
dv.inputMessage("Value must be 1,2 or 3");
dv.inputTitle("tip");
activeSheet.setDataValidator(1,1,1,1,dv,GC.Spread.Sheets.SheetArea.viewport);
alert(activeSheet.getDataValidator(1,1).getValidList(activeSheet,1,1));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 输入标题 |

#### Returns

`any`

如果未设置任何值，则返回输入标题否则，返回数据验证器

___

### <a id="isvalid" name="isvalid"></a> isValid

▸ **isValid**(`evaluator`, `baseRow`, `baseColumn`, `actual`): `boolean`

确定当前值是否有效

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
dv = sheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(); // Limitation of SDM, the dv is copied when set to style.
console.log(dv.isValid(sheet, 0, 0, 3)); // true
console.log(dv.isValid(sheet, 0, 0, 1)); // false
console.log(dv.isValid(sheet, 0, 0, 101)); // true
console.log(dv.isValid(sheet, 0, 0, 0)); // false
console.log(dv.isValid(sheet, 0, 0, 120.0)); // false
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `evaluator` | `Object` | 计算器 |
| `baseRow` | `number` | 基行 |
| `baseColumn` | `number` | 基列 |
| `actual` | `Object` | 当前值 |

#### Returns

`boolean`

` true `该值有效；否则为` false `

___

### <a id="precisecomparedate" name="precisecomparedate"></a> preciseCompareDate

▸ **preciseCompareDate**(`value?`): `any`

获取或设置是比较整天还是精确日期时间

**`代码示例`**
``` javascript
//本示例使用preciseCompareDate方法
var dateCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.dateCondition);
dateCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.DateCompareType.after);
dateCondition.expected(new Date(2020, 4, 22, 6));
//When the option is false, the validator compares the whole day, and they are the same, so validation fails and the red alert is displayed.
//When the option is true, the date time 7 o'clock is greater than 6 o'clock, so the result is successful.
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(dateCondition);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.date);
validator.preciseCompareDate(true);
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, new Date(2020, 4, 22, 07));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 比较整天或精确日期时间 |

#### Returns

`any`

如果未设置值，则返回比较全天或精确日期时间；否则，返回数据验证

___

### <a id="reset" name="reset"></a> reset

▸ **reset**(): `void`

重置数据验证器

**`代码示例`**
``` javascript
//本示例使用reset方法
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.cellValueCondition);
nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.equalsTo);
nCondition.expected(0);
//When the option is false, the validation fails and the red alert is displayed.
//When the option is true, the blank cell is treated as zero and the validation is successful.
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

获取或设置是否显示错误消息

**`代码示例`**
``` javascript
spread.options.highlightInvalidData = true;
//如果公式条件返回true,则公式验证有效
var dv = GC.Spread.Sheets.DataValidation.createFormulaValidator("A1&gt;0");
dv.showInputMessage(true);
dv.inputMessage("Enter a value greater than 0 in A1.");
dv.inputTitle("Tip");
dv.showErrorMessage(true);
dv.errorMessage("Incorrect Value");
activeSheet.setDataValidator(0, 0, 1, 1, dv, GC.Spread.Sheets.SheetArea.viewport);
//bind
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
| `value?` | `boolean` | 是否显示错误消息 |

#### Returns

`any`

如果未设置任何值，则返回是否显示错误消息否则，返回数据验证器

___

### <a id="showinputmessage" name="showinputmessage"></a> showInputMessage

▸ **showInputMessage**(`value?`): `any`

获取或设置是否显示输入标题和输入消息

**`代码示例`**
``` javascript
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createListValidator("1,2,3");
dv.showInputMessage(true);
dv.inputMessage("Value must be 1,2 or 3");
dv.inputTitle("tip");
activeSheet.setDataValidator(1,1,1,1,dv,GC.Spread.Sheets.SheetArea.viewport);
alert(activeSheet.getDataValidator(1,1).getValidList(activeSheet,1,1));
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置任何值，则返回是否显示输入标题和输入消息否则，返回数据验证器

___

### <a id="type" name="type"></a> type

▸ **type**(`value?`): `any`

获取或设置此数据验证器的条件类型

**`example`**
```
//This example uses the preciseCompareDate method.
var dateCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.dateCondition);
dateCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.DateCompareType.after);
dateCondition.expected(new Date(2020, 4, 22, 6));
//When the option is false, the validator compares the whole day, and they are the same, so validation fails and the red alert is displayed.
//When the option is true, the date time 7 o'clock is greater than 6 o'clock, so the result is successful.
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

如果未设置任何值，则返回此数据验证器的条件类型；否则，返回数据验证器

___

### <a id="value1" name="value1"></a> value1

▸ **value1**(`baseRow?`, `baseColumn?`): `any`

获取数据验证的第一个值

**`代码示例`**
``` javascript
//本示例验证单元格值
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.cellValueCondition);
nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.equalsTo);
nCondition.expected(0);
//当选项为false时，验证失败并显示红色警报
//当选项为true时，将把空白单元格视为零，验证成功
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
| `baseRow?` | `number` | 基行 |
| `baseColumn?` | `number` | 基列 |

#### Returns

`any`

第一个值

___

### <a id="value2" name="value2"></a> value2

▸ **value2**(`baseRow?`, `baseColumn?`): `any`

获取数据验证的第二个值

**`代码示例`**
``` javascript
//本示例验证单元格值
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.cellValueCondition);
nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.equalsTo);
nCondition.expected(0);
//当选项为false时，验证失败并显示红色警报
//当选项为true时，将把空白单元格视为零，验证成功
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

| Name | Type | Description |
| :------ | :------ | :------ |
| `baseRow?` | `number` | 基行 |
| `baseColumn?` | `number` | 基列 |

#### Returns

`any`

第二个值
