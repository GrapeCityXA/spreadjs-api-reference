# Enumeration: FillDirection

[Sheets](../modules/GC.Spread.Sheets.md).[Fill](../modules/GC.Spread.Sheets.Fill.md).FillDirection

拖拽填充方向的类型

**`代码示例`**
```
var start = new GC.Spread.Sheets.Range(0, 2, 1, 1);
activeSheet.setValue(0, 2, 5);
var r3 = new GC.Spread.Sheets.Range(0, 2, 4, 1);
activeSheet.fillAuto(start, r3, {fillType: GC.Spread.Sheets.Fill.FillType.auto, fillDirection:GC.Spread.Sheets.Fill.FillDirection.down, series: GC.Spread.Sheets.Fill.FillSeries.column});
```

## Table of contents

### Enumeration members

- [down](GC.Spread.Sheets.Fill.FillDirection.md#down)
- [left](GC.Spread.Sheets.Fill.FillDirection.md#left)
- [right](GC.Spread.Sheets.Fill.FillDirection.md#right)
- [up](GC.Spread.Sheets.Fill.FillDirection.md#up)

## Enumeration members

### <a id="down" name="down"></a> down

• **down** = `3`

  从上到下填充

___

### <a id="left" name="left"></a> left

• **left** = `0`

 从右到左填充

___

### <a id="right" name="right"></a> right

• **right** = `1`

 从左到右填充

___

### <a id="up" name="up"></a> up

• **up** = `2`

 从下到上填充
