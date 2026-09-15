# Enumeration: AsyncFunctionEvaluateMode

[CalcEngine](../modules/GC.Spread.CalcEngine.md).[Functions](../modules/GC.Spread.CalcEngine.Functions.md).AsyncFunctionEvaluateMode

异步函数求值模式

## Table of contents

### Enumeration members

- [calculateOnce](GC.Spread.CalcEngine.Functions.AsyncFunctionEvaluateMode.md#calculateonce)
- [onInterval](GC.Spread.CalcEngine.Functions.AsyncFunctionEvaluateMode.md#oninterval)
- [onRecalculation](GC.Spread.CalcEngine.Functions.AsyncFunctionEvaluateMode.md#onrecalculation)

## Enumeration members

### <a id="calculateonce" name="calculateonce"></a> calculateOnce

• **calculateOnce** = `1`

枚举值为1,异步函数只计算一次

___

### <a id="oninterval" name="oninterval"></a> onInterval

• **onInterval** = `2`

枚举值为2,异步函数根据间隔进行计算

___

### <a id="onrecalculation" name="onrecalculation"></a> onRecalculation

• **onRecalculation** = `0`

枚举值为0,异步函数计算已更改的、引用的单元格
