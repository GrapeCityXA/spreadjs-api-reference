# Enumeration: HeaderOptions

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).HeaderOptions

指定导出范围数据到HTML时包含哪些表头。

**`example`**
```
//此示例展示如何导出带行表头和列表头的范围数据到HTML。
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

导出范围数据到HTML时包含选定的表头。

___

### <a id="columnheaders" name="columnheaders"></a> columnHeaders

• **columnHeaders** = `2`

导出范围数据到HTML时包含选定的列表头。

___

### <a id="noheaders" name="noheaders"></a> noHeaders

• **noHeaders** = `0`

导出范围数据到HTML时不包含列和行表头。

___

### <a id="rowheaders" name="rowheaders"></a> rowHeaders

• **rowHeaders** = `1`

导出范围数据到HTML时包含选定的行表头。
