# Enumeration: ErrorStyle

[Sheets](../modules/GC.Spread.Sheets.md).[DataValidation](../modules/GC.Spread.Sheets.DataValidation.md).ErrorStyle

表示数据验证错误样式。

**`example`**
```javascript
// 本示例使用了 ErrorStyle 枚举类型。
spread.options.highlightInvalidData = true;
var activeSheet = spread.getActiveSheet();
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createListValidator('Fruit,Vegetable,Food');
dv.errorStyle(GC.Spread.Sheets.DataValidation.ErrorStyle.stop);
sheet.setDataValidator(1,1, dv);
```

## Table of contents

### Enumeration members

- [information](GC.Spread.Sheets.DataValidation.ErrorStyle.md#information)
- [stop](GC.Spread.Sheets.DataValidation.ErrorStyle.md#stop)
- [warning](GC.Spread.Sheets.DataValidation.ErrorStyle.md#warning)

## Enumeration members

### <a id="information" name="information"></a> information

• **information** = `2`

指定在错误提示中使用信息图标。

___

### <a id="stop" name="stop"></a> stop

• **stop** = `0`

指定在错误提示中使用停止图标。

___

### <a id="warning" name="warning"></a> warning

• **warning** = `1`

指定在错误提示中使用警告图标。
