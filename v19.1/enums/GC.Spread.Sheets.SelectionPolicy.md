# Enumeration: SelectionPolicy

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).SelectionPolicy

指定用户如何选择控件中的项目。

**`example`**
```javascript
//此示例设置选择策略。
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

允许用户选择单个项目和项目范围，包括多个范围。

___

### <a id="range" name="range"></a> range

• **range** = `1`

允许用户选择单个项目和项目范围，但不能选择多个范围。

___

### <a id="single" name="single"></a> single

• **single** = `0`

允许用户只能选择单个项目。
