# Enumeration: HeaderOptions

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).HeaderOptions

将区域数据导出到HTML时包含哪些头

**`代码示例`**
```
//本示例向您展示了如何使用行头和列头将区域数据导出到HTML
activeSheet.getRange(-1, -1, -1, -1).toHtml(GC.Spread.Sheets.HeaderOptions.allHeaders);
```

## Table of contents

### Enumeration members

- [allHeaders](GC.Spread.Sheets.HeaderOptions.md#allheaders)
- [columnHeaders](GC.Spread.Sheets.HeaderOptions.md#columnheaders)
- [noHeaders](GC.Spread.Sheets.HeaderOptions.md#noheaders)
- [rowHeaders](GC.Spread.Sheets.HeaderOptions.md#rowheaders)

## Enumeration members

### <a id="allheaders" name="allheaders"></a> allHeaders

• **allHeaders** = `3`

当导出区域数据到HTML时,包括选定的头

___

### <a id="columnheaders" name="columnheaders"></a> columnHeaders

• **columnHeaders** = `2`

当导出区域数据到HTML时,包括选定的列头

___

### <a id="noheaders" name="noheaders"></a> noHeaders

• **noHeaders** = `0`

当导出区域数据到HTML时,既不包括列头也不包括行头

___

### <a id="rowheaders" name="rowheaders"></a> rowHeaders

• **rowHeaders** = `1`

当导出区域数据到HTML时,包括选定的行头
