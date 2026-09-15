# Enumeration: DataValidationResult

[Sheets](../modules/GC.Spread.Sheets.md).[DataValidation](../modules/GC.Spread.Sheets.DataValidation.md).DataValidationResult

表示数据验证结果。

**`example`**
```javascript
// 本示例使用了 DataValidationResult 枚举类型。
spread.options.highlightInvalidData = true;
// 当公式条件返回 true 时，该公式验证器判定为有效。
var dv = GC.Spread.Sheets.DataValidation.createFormulaValidator("A1&gt;0");
dv.showInputMessage(true);
dv.inputMessage("Enter a value greater than 0 in A1.");
dv.inputTitle("Tip");
dv.showErrorMessage(true);
dv.errorMessage("Incorrect Value");
var activeSheet = spread.getActiveSheet();
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

## Table of contents

### Enumeration members

- [discard](GC.Spread.Sheets.DataValidation.DataValidationResult.md#discard)
- [forceApply](GC.Spread.Sheets.DataValidation.DataValidationResult.md#forceapply)
- [retry](GC.Spread.Sheets.DataValidation.DataValidationResult.md#retry)

## Enumeration members

### <a id="discard" name="discard"></a> discard

• **discard** = `1`

表示对于验证错误，丢弃值且不将其应用到单元格。

___

### <a id="forceapply" name="forceapply"></a> forceApply

• **forceApply** = `0`

表示对于验证错误，强制将值应用到单元格。

___

### <a id="retry" name="retry"></a> retry

• **retry** = `2`

表示对于验证错误，多次尝试将值应用到单元格。
