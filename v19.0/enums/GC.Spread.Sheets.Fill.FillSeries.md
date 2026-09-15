# Enumeration: FillSeries

[Sheets](../modules/GC.Spread.Sheets.md).[Fill](../modules/GC.Spread.Sheets.Fill.md).FillSeries

表示拖拽填充的系列类型。

**`example`**
```
//此示例自动填充工作表中的某个区域。
activeSheet.setValue(0, 0, 5);
var start = new GC.Spread.Sheets.Range(0, 0, 1, 1);
var r3 = new GC.Spread.Sheets.Range(0, 0, 4, 1);
activeSheet.fillAuto(start,r3, {fillType:GC.Spread.Sheets.Fill.FillType.auto, series:GC.Spread.Sheets.Fill.FillSeries.column, fillDirection:GC.Spread.Sheets.Fill.FillDirection.down});
```

## Table of contents

### Enumeration members

- [column](GC.Spread.Sheets.Fill.FillSeries.md#column)
- [row](GC.Spread.Sheets.Fill.FillSeries.md#row)

## Enumeration members

### <a id="column" name="column"></a> column

• **column** = `0`

填充列数据。

___

### <a id="row" name="row"></a> row

• **row** = `1`

填充行数据。
