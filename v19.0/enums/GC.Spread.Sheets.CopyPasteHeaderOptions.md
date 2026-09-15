# Enumeration: CopyPasteHeaderOptions

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).CopyPasteHeaderOptions

指定复制或粘贴数据时包含哪些表头。

**`example`**
```
//此示例允许复制和粘贴表头。
spread.options.copyPasteHeaderOptions = GC.Spread.Sheets.CopyPasteHeaderOptions.allHeaders;
activeSheet.setRowCount(2,GC.Spread.Sheets.SheetArea.colHeader);
activeSheet.setColumnCount(2,GC.Spread.Sheets.SheetArea.rowHeader);
activeSheet.setValue(0, 2,"Column",GC.Spread.Sheets.SheetArea.colHeader);
activeSheet.setValue(1, 0,"Row",GC.Spread.Sheets.SheetArea.rowHeader);
```

## Table of contents

### Enumeration members

- [allHeaders](GC.Spread.Sheets.CopyPasteHeaderOptions.md#allheaders)
- [columnHeaders](GC.Spread.Sheets.CopyPasteHeaderOptions.md#columnheaders)
- [noHeaders](GC.Spread.Sheets.CopyPasteHeaderOptions.md#noheaders)
- [rowHeaders](GC.Spread.Sheets.CopyPasteHeaderOptions.md#rowheaders)

## Enumeration members

### <a id="allheaders" name="allheaders"></a> allHeaders

• **allHeaders** = `3`

复制数据时包含选定的表头；粘贴数据时覆盖选定的表头。

___

### <a id="columnheaders" name="columnheaders"></a> columnHeaders

• **columnHeaders** = `2`

复制数据时包含选定的列表头；粘贴数据时覆盖选定的列表头。

___

### <a id="noheaders" name="noheaders"></a> noHeaders

• **noHeaders** = `0`

复制数据时不包含列和行表头；粘贴数据时不覆盖选定的列或行表头。

___

### <a id="rowheaders" name="rowheaders"></a> rowHeaders

• **rowHeaders** = `1`

复制数据时包含选定的行表头；粘贴数据时覆盖选定的行表头。
