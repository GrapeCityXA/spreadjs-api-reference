# Enumeration: FillType

[Sheets](../modules/GC.Spread.Sheets.md).[Fill](../modules/GC.Spread.Sheets.Fill.md).FillType

表示填充数据的类型。

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

表示自动填充类型。

___

### <a id="date" name="date"></a> date

• **date** = `3`

表示日期填充类型。

___

### <a id="direction" name="direction"></a> direction

• **direction** = `0`

表示方向填充类型。

___

### <a id="growth" name="growth"></a> growth

• **growth** = `2`

表示增长填充类型。

___

### <a id="linear" name="linear"></a> linear

• **linear** = `1`

表示线性填充类型。
