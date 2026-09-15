# Enumeration: DivergeDirection

[Sheets](../modules/GC.Spread.Sheets.md).[CellTypes](../modules/GC.Spread.Sheets.CellTypes.md).DivergeDirection

指定对角单元格类型的发散方向。

**`readonly`**

**`example`**
```
//This example uses the EditorValueType enumeration.
var diagonalCellType = new GC.Spread.Sheets.CellTypes.Diagonal();
diagonalCellType.divergeDirection(GC.Spread.Sheets.CellTypes.DivergeDirection.topLeftToBottomRight)
activeSheet.getCell(2, 2).cellType(diagonalCellType);
```

## Table of contents

### Enumeration members

- [bottomLeftToTopRight](GC.Spread.Sheets.CellTypes.DivergeDirection.md#bottomlefttotopright)
- [topLeftToBottomRight](GC.Spread.Sheets.CellTypes.DivergeDirection.md#toplefttobottomright)

## Enumeration members

### <a id="bottomlefttotopright" name="bottomlefttotopright"></a> bottomLeftToTopRight

• **bottomLeftToTopRight** = `1`

表示从左下角向右上角发散。

___

### <a id="toplefttobottomright" name="toplefttobottomright"></a> topLeftToBottomRight

• **topLeftToBottomRight** = `0`

表示从左上角向右下角发散。
