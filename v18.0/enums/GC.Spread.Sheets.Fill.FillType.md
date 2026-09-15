# Enumeration: FillType

[Sheets](../modules/GC.Spread.Sheets.md).[Fill](../modules/GC.Spread.Sheets.Fill.md).FillType

填充数据的类型
**`example`**
```
start = new GC.Spread.Sheets.Range(0, 2, 1, 1);
var r3 = new GC.Spread.Sheets.Range(0, 2, 4, 1);
activeSheet.fillAuto(start, r3, {
    fillType: GC.Spread.Sheets.Fill.FillType.auto,
    series: GC.Spread.Sheets.Fill.FillSeries.column,
});
```

## Table of contents

### Enumeration members

- [auto](GC.Spread.Sheets.Fill.FillType.md#auto)
- [date](GC.Spread.Sheets.Fill.FillType.md#date)
- [direction](GC.Spread.Sheets.Fill.FillType.md#direction)
- [growth](GC.Spread.Sheets.Fill.FillType.md#growth)
- [linear](GC.Spread.Sheets.Fill.FillType.md#linear)

## Enumeration members

### <a id="auto" name="auto"></a> auto

• **auto** = `4`

自动填充类型

___

### <a id="date" name="date"></a> date

• **date** = `3`

日期填充类型

___

### <a id="direction" name="direction"></a> direction

• **direction** = `0`

方向填充类型

___

### <a id="growth" name="growth"></a> growth

• **growth** = `2`

增长填充类型

___

### <a id="linear" name="linear"></a> linear

• **linear** = `1`

线性填充类型
