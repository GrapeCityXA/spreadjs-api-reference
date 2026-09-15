# Enumeration: VerticalPosition

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).VerticalPosition

指定单元格或行在组件中的垂直位置。

**`example`**
```
//此示例使用VerticalPosition枚举。
activeSheet.setActiveCell(10,5);
activeSheet.showCell(10, 5, GC.Spread.Sheets.VerticalPosition.top, GC.Spread.Sheets.HorizontalPosition.center);
```

## Table of contents

### Enumeration members

- [bottom](GC.Spread.Sheets.VerticalPosition.md#bottom)
- [center](GC.Spread.Sheets.VerticalPosition.md#center)
- [nearest](GC.Spread.Sheets.VerticalPosition.md#nearest)
- [top](GC.Spread.Sheets.VerticalPosition.md#top)

## Enumeration members

### <a id="bottom" name="bottom"></a> bottom

• **bottom** = `2`

将单元格或行定位在底部。

___

### <a id="center" name="center"></a> center

• **center** = `1`

将单元格或行定位在中间。

___

### <a id="nearest" name="nearest"></a> nearest

• **nearest** = `3`

将单元格或行定位在最近的边缘。

___

### <a id="top" name="top"></a> top

• **top** = `0`

将单元格或行定位在顶部。
