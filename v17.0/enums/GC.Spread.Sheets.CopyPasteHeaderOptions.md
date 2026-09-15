# Enumeration: CopyPasteHeaderOptions

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).CopyPasteHeaderOptions

指定数据复制或粘贴时包含哪些头部

**`代码示例`**
```
//本示例允许复制和粘贴头部
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

在数据复制时，包括选定的标题；在粘贴数据时，覆盖选定的标题

___

### <a id="columnheaders" name="columnheaders"></a> columnHeaders

• **columnHeaders** = `2`

在复制数据时包括选定的列头；在粘贴数据时，覆盖选定的列头

___

### <a id="noheaders" name="noheaders"></a> noHeaders

• **noHeaders** = `0`

复制数据时，不包括列标头或行标头；在粘贴数据时，不会覆盖选定的列或行标题

___

### <a id="rowheaders" name="rowheaders"></a> rowHeaders

• **rowHeaders** = `1`

在数据复制时，包含选定的行头；数据粘贴时，粘贴时覆盖选定的行头
