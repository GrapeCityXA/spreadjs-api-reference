# Enumeration: CalculationMode

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).CalculationMode

指定工作簿的重新计算行为。

**`example`**
```javascript
spread.options.calculationMode = GC.Spread.Sheets.CalculationMode.manual;
```

## Table of contents

### Enumeration members

- [auto](GC.Spread.Sheets.CalculationMode.md#auto)
- [manual](GC.Spread.Sheets.CalculationMode.md#manual)
- [partial](GC.Spread.Sheets.CalculationMode.md#partial)

## Enumeration members

### <a id="auto" name="auto"></a> auto

• **auto** = `0`

默认的重新计算行为，每当相关数据发生变化时都会计算公式。

___

### <a id="manual" name="manual"></a> manual

• **manual** = `1`

仅在用户请求时进行计算。

___

### <a id="partial" name="partial"></a> partial

• **partial** = `2`

当相关数据发生变化时，计算除 SJS.TABLE 外的所有公式。
