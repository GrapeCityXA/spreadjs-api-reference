# Namespace: CalcEngine

[GC](GC.md).[Spread](GC.Spread.md).CalcEngine

## Table of contents

### Namespaces

- [Functions](GC.Spread.CalcEngine.Functions.md)
- [LanguagePackages](GC.Spread.CalcEngine.LanguagePackages.md)

### Enumerations

- [ExpressionType](../enums/GC.Spread.CalcEngine.ExpressionType.md)

### Classes

- [AsyncEvaluateContext](../classes/GC.Spread.CalcEngine.AsyncEvaluateContext.md)
- [CalcArray](../classes/GC.Spread.CalcEngine.CalcArray.md)
- [CalcError](../classes/GC.Spread.CalcEngine.CalcError.md)
- [Expression](../classes/GC.Spread.CalcEngine.Expression.md)

### Variables

- [ExcelCompatibleCalcMode](GC.Spread.CalcEngine.md#excelcompatiblecalcmode)

## Variables

### <a id="excelcompatiblecalcmode" name="excelcompatiblecalcmode"></a> ExcelCompatibleCalcMode

• **ExcelCompatibleCalcMode**: `boolean`

获取或设置CalcEngine的Excel兼容模式。默认值为false.
当ExcelCompatibleCalcMode禁用时，SpreadJS会自动将文本转换为数字进行计算。
当ExcelCompatibleCalcMode启用时，当文本作为参数直接提供或在数组/引用中时，会以不同方式处理。
例如，A1是文本值"1"，如果禁用则SUM(A1, 1)将为2，如果启用则为1。

**`example`**
```
GC.Spread.CalcEngine.ExcelCompatibleCalcMode = true;
```
