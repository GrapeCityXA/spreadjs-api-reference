# Enumeration: HorizontalPosition

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).HorizontalPosition

单元格或列的水平位置

**`代码示例`**
```
//本示例使用了HorizontalPosition枚举
activeSheet.setActiveCell(10,5);
activeSheet.showCell(10, 5, GC.Spread.Sheets.VerticalPosition.top, GC.Spread.Sheets.HorizontalPosition.center);
```

## Table of contents

### Enumeration members

- [center](GC.Spread.Sheets.HorizontalPosition.md#center)
- [left](GC.Spread.Sheets.HorizontalPosition.md#left)
- [nearest](GC.Spread.Sheets.HorizontalPosition.md#nearest)
- [right](GC.Spread.Sheets.HorizontalPosition.md#right)

## Enumeration members

### <a id="center" name="center"></a> center

• **center** = `1`

 将单元格或列放置在中心

___

### <a id="left" name="left"></a> left

• **left** = `0`

 将单元格或列定位到左侧

___

### <a id="nearest" name="nearest"></a> nearest

• **nearest** = `3`

 将单元格或列定位到最近的边缘

___

### <a id="right" name="right"></a> right

• **right** = `2`

 将单元格或列定位到右侧
