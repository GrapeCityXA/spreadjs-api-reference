# Enumeration: SelectionUnit

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).SelectionUnit

指定用户或应用程序可以选择的最小单位。

**`example`**
```javascript
//此示例设置单位类型。
activeSheet.selectionUnit(GC.Spread.Sheets.SelectionUnit.row);
activeSheet.selectionPolicy(GC.Spread.Sheets.SelectionPolicy.range);
```

## Table of contents

### Enumeration members

- [cell](GC.Spread.Sheets.SelectionUnit.md#cell)
- [column](GC.Spread.Sheets.SelectionUnit.md#column)
- [row](GC.Spread.Sheets.SelectionUnit.md#row)

## Enumeration members

### <a id="cell" name="cell"></a> cell

• **cell** = `0`

表示可以选择的最小单位是单元格。

___

### <a id="column" name="column"></a> column

• **column** = `2`

表示可以选择的最小单位是列。

___

### <a id="row" name="row"></a> row

• **row** = `1`

表示可以选择的最小单位是行。
