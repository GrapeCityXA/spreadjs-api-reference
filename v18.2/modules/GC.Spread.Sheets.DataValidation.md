# Namespace: DataValidation

[Spread](GC.Spread.md).[Sheets](GC.Spread.Sheets.md).DataValidation

## Table of contents

### Enumerations

- [CriteriaType](../enums/GC.Spread.Sheets.DataValidation.CriteriaType.md)
- [DataValidationResult](../enums/GC.Spread.Sheets.DataValidation.DataValidationResult.md)
- [ErrorStyle](../enums/GC.Spread.Sheets.DataValidation.ErrorStyle.md)
- [HighlightPosition](../enums/GC.Spread.Sheets.DataValidation.HighlightPosition.md)
- [HighlightType](../enums/GC.Spread.Sheets.DataValidation.HighlightType.md)

### Classes

- [DefaultDataValidator](../classes/GC.Spread.Sheets.DataValidation.DefaultDataValidator.md)

### Interfaces

- [IHighLightStyle](../interfaces/GC.Spread.Sheets.DataValidation.IHighLightStyle.md)

### Functions

- [createDateValidator](GC.Spread.Sheets.DataValidation.md#createdatevalidator)
- [createFormulaListValidator](GC.Spread.Sheets.DataValidation.md#createformulalistvalidator)
- [createFormulaValidator](GC.Spread.Sheets.DataValidation.md#createformulavalidator)
- [createListValidator](GC.Spread.Sheets.DataValidation.md#createlistvalidator)
- [createNumberValidator](GC.Spread.Sheets.DataValidation.md#createnumbervalidator)
- [createTextLengthValidator](GC.Spread.Sheets.DataValidation.md#createtextlengthvalidator)
- [createTimeValidator](GC.Spread.Sheets.DataValidation.md#createtimevalidator)

## Functions

### <a id="createdatevalidator" name="createdatevalidator"></a> createDateValidator

▸ **createDateValidator**(`typeOperator`, `v1`, `v2?`): [`DefaultDataValidator`](../classes/GC.Spread.Sheets.DataValidation.DefaultDataValidator.md)

基于数据创建验证器。

**`static`**

**`example`**
```
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createDateValidator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.between, new Date(2012, 11, 31), new Date(2013, 11, 31));
dv.showInputMessage(true);
dv.inputMessage("Enter a date between 12/31/2012 and 12/31/2013.");
dv.inputTitle("Tip");
activeSheet.getCell(1, -1).validator(dv);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `typeOperator` | [`ComparisonOperators`](../enums/GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.md) | 比较运算符类型。该属性的可能值由 GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators 定义。 |
| `v1` | `Object` | 第一个对象。 |
| `v2?` | `Object` | - |

#### Returns

[`DefaultDataValidator`](../classes/GC.Spread.Sheets.DataValidation.DefaultDataValidator.md)

验证器。

___

### <a id="createformulalistvalidator" name="createformulalistvalidator"></a> createFormulaListValidator

▸ **createFormulaListValidator**(`formula`): [`DefaultDataValidator`](../classes/GC.Spread.Sheets.DataValidation.DefaultDataValidator.md)

基于公式列表创建验证器。

**`static`**

**`example`**
```
activeSheet.setValue(0, 2, 5);
activeSheet.setValue(1, 2, 4);
activeSheet.setValue(2, 2, 5);
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createFormulaListValidator("$C$1:$C$3");
dv.showInputMessage(true);
dv.inputMessage("Pick a value from the list.");
dv.inputTitle("tip");
activeSheet.setDataValidator(1, 1, 1,1,dv,GC.Spread.Sheets.SheetArea.viewport);
var validList = activeSheet.getDataValidator(1, 1).getValidList(activeSheet, 1, 1);
alert(validList);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `formula` | `string` | 公式列表。 |

#### Returns

[`DefaultDataValidator`](../classes/GC.Spread.Sheets.DataValidation.DefaultDataValidator.md)

验证器。

___

### <a id="createformulavalidator" name="createformulavalidator"></a> createFormulaValidator

▸ **createFormulaValidator**(`formula`): [`DefaultDataValidator`](../classes/GC.Spread.Sheets.DataValidation.DefaultDataValidator.md)

基于公式创建验证器。

**`static`**

**`example`**
```
spread.options.highlightInvalidData = true;
//如果公式条件返回true，则公式验证器有效。
var dv = GC.Spread.Sheets.DataValidation.createFormulaValidator("A1>0");
dv.showInputMessage(true);
dv.inputMessage("Enter a value greater than 0 in A1.");
dv.inputTitle("Tip");
activeSheet.setDataValidator(0, 0, 1,1,dv,GC.Spread.Sheets.SheetArea.viewport);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `formula` | `string` | 公式条件。 |

#### Returns

[`DefaultDataValidator`](../classes/GC.Spread.Sheets.DataValidation.DefaultDataValidator.md)

验证器。

___

### <a id="createlistvalidator" name="createlistvalidator"></a> createListValidator

▸ **createListValidator**(`source`): [`DefaultDataValidator`](../classes/GC.Spread.Sheets.DataValidation.DefaultDataValidator.md)

基于列表创建验证器。

**`static`**

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
| `source` | `string` | 列表值。 |

#### Returns

[`DefaultDataValidator`](../classes/GC.Spread.Sheets.DataValidation.DefaultDataValidator.md)

验证器。

___

### <a id="createnumbervalidator" name="createnumbervalidator"></a> createNumberValidator

▸ **createNumberValidator**(`typeOperator`, `v1`, `v2?`, `isIntegerValue?`): [`DefaultDataValidator`](../classes/GC.Spread.Sheets.DataValidation.DefaultDataValidator.md)

基于数字创建验证器。

**`static`**

**`example`**
```
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createNumberValidator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.between, 5, 20, true);
dv.showInputMessage(true);
dv.inputMessage("Value must be between 5 and 20.");
dv.inputTitle("tip");
activeSheet.setDataValidator(1, 1, 1,1,dv,GC.Spread.Sheets.SheetArea.viewport);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `typeOperator` | [`ComparisonOperators`](../enums/GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.md) | 比较运算符类型。该属性的可能值由 GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators 定义。 |
| `v1` | `Object` | 第一个对象。 |
| `v2?` | `Object` | - |
| `isIntegerValue?` | `boolean` | - |

#### Returns

[`DefaultDataValidator`](../classes/GC.Spread.Sheets.DataValidation.DefaultDataValidator.md)

验证器。

___

### <a id="createtextlengthvalidator" name="createtextlengthvalidator"></a> createTextLengthValidator

▸ **createTextLengthValidator**(`typeOperator`, `v1`, `v2?`): [`DefaultDataValidator`](../classes/GC.Spread.Sheets.DataValidation.DefaultDataValidator.md)

基于文本长度创建验证器。

**`static`**

**`example`**
```
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createTextLengthValidator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.greaterThan, 4);
dv.showInputMessage(true);
dv.inputMessage("Number of characters must be greater than 4.");
dv.inputTitle("tip");
activeSheet.setDataValidator(1, 1, 1, 1, dv, GC.Spread.Sheets.SheetArea.viewport);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `typeOperator` | [`ComparisonOperators`](../enums/GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.md) | 比较运算符类型。该属性的可能值由 GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators 定义。 |
| `v1` | `Object` | 第一个对象。 |
| `v2?` | `Object` | - |

#### Returns

[`DefaultDataValidator`](../classes/GC.Spread.Sheets.DataValidation.DefaultDataValidator.md)

验证器。

___

### <a id="createtimevalidator" name="createtimevalidator"></a> createTimeValidator

▸ **createTimeValidator**(`typeOperator`, `v1`, `v2?`): [`DefaultDataValidator`](../classes/GC.Spread.Sheets.DataValidation.DefaultDataValidator.md)

基于时间创建验证器。

**`static`**

**`example`**
```
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createTimeValidator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.between, '9:08:09', '19:08:09');
dv.showInputMessage(true);
dv.inputMessage("Enter a time between 9:08:09 and 19:08:09.");
dv.inputTitle("Tip");
sheet.setDataValidator(1, 1, dv);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `typeOperator` | [`ComparisonOperators`](../enums/GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.md) | 比较运算符类型。该属性的可能值由 GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators 定义。 |
| `v1` | `Object` | 第一个对象。 |
| `v2?` | `Object` | - |

#### Returns

[`DefaultDataValidator`](../classes/GC.Spread.Sheets.DataValidation.DefaultDataValidator.md)

验证器。
