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

获取或设置 CalcEngine 兼容 Excel 计算模式，默认值为FALSE

当 ExcelCompatibleCalcMode 被禁用时，SpreadJS 将自动将文本转换为数字进行计算

启用 ExcelCompatibleCalcMode，则在直接作为参数或在数组/引用时，会对文本进行不同的处理

例如：A1 的文本值为 "1", 如果禁用，则 SUM(A1,1) 结果为 2，如果启用，结果为 1
