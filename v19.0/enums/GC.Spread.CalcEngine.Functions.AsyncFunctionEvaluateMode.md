# Enumeration: AsyncFunctionEvaluateMode

[CalcEngine](../modules/GC.Spread.CalcEngine.md).[Functions](../modules/GC.Spread.CalcEngine.Functions.md).AsyncFunctionEvaluateMode

表示异步函数求值模式。

## Table of contents

### Enumeration members

- [calculateOnce](GC.Spread.CalcEngine.Functions.AsyncFunctionEvaluateMode.md#calculateonce)
- [onInterval](GC.Spread.CalcEngine.Functions.AsyncFunctionEvaluateMode.md#oninterval)
- [onRecalculation](GC.Spread.CalcEngine.Functions.AsyncFunctionEvaluateMode.md#onrecalculation)

## Enumeration members

### <a id="calculateonce" name="calculateonce"></a> calculateOnce

• **calculateOnce** = `1`

枚举值为1，指定异步函数只求值一次。

___

### <a id="oninterval" name="oninterval"></a> onInterval

• **onInterval** = `2`

枚举值为2，指定异步函数基于时间间隔求值。

___

### <a id="onrecalculation" name="onrecalculation"></a> onRecalculation

• **onRecalculation** = `0`

枚举值为0，指定异步函数在引用的单元格发生变化时求值。
