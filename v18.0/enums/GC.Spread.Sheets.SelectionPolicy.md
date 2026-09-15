# Enumeration: SelectionPolicy

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).SelectionPolicy

用户如何选择控件中的项

**`代码示例`**
``` javascript
//本示例设置选择策略
activeSheet.selectionUnit(GC.Spread.Sheets.SelectionUnit.row);
activeSheet.selectionPolicy(GC.Spread.Sheets.SelectionPolicy.range);
```

## Table of contents

### Enumeration members

- [multiRange](GC.Spread.Sheets.SelectionPolicy.md#multirange)
- [range](GC.Spread.Sheets.SelectionPolicy.md#range)
- [single](GC.Spread.Sheets.SelectionPolicy.md#single)

## Enumeration members

### <a id="multirange" name="multirange"></a> multiRange

• **multiRange** = `2`

允许用户选择单个项和项区域，包括多个区域

___

### <a id="range" name="range"></a> range

• **range** = `1`

允许用户选择单个项和项区域，但不能选择多个区域

___

### <a id="single" name="single"></a> single

• **single** = `0`

允许用户仅选择单个项
