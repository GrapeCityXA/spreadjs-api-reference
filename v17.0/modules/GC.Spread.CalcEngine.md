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

获取或设置CalcEngine的Excel兼容模式。默认值为FALSE
当禁用ExcelCompatibleCalcMode时，SpreadJS将自动将文本转换为数字进行计算
当启用ExcelCompatibleCalcMode时，在直接提供或作为数组/引用提供参数时，会以不同方式对待文本
例如，如果A1是文本值"1"，则如果禁用，则SUM(A1, 1)将为2，启用时将为1


**`example`**
```
GC.Spread.CalcEngine.ExcelCompatibleCalcMode = true;
```
