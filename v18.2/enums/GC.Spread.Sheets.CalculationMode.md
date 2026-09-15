# Enumeration: CalculationMode

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).CalculationMode

指定工作簿的重新计算行为。

**`example`**
```
spread.options.calculationMode = GC.Spread.Sheets.CalculationMode.manual;
```

## Table of contents

### Enumeration members

- [auto](GC.Spread.Sheets.CalculationMode.md#auto)
- [manual](GC.Spread.Sheets.CalculationMode.md#manual)

## Enumeration members

### <a id="auto" name="auto"></a> auto

• **auto** = `0`

默认的重新计算行为，每当相关数据发生变化时都会计算公式。

___

### <a id="manual" name="manual"></a> manual

• **manual** = `1`

仅在用户请求时进行计算。
