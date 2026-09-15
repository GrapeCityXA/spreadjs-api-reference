# Enumeration: CalculationMode

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).CalculationMode

指定工作簿的重算行为

**`example`**
```
spread.options.CalculationMode = GC.Spread.Sheets.CalculationMode.manual;
```

## Table of contents

### Enumeration members

- [auto](GC.Spread.Sheets.CalculationMode.md#auto)
- [manual](GC.Spread.Sheets.CalculationMode.md#manual)

## Enumeration members

### <a id="auto" name="auto"></a> auto

• **auto** = `0`

默认的重新计算行为，会在相关数据发生更改时每次计算公式

___

### <a id="manual" name="manual"></a> manual

• **manual** = `1`

仅当用户请求它们时才发生计算
