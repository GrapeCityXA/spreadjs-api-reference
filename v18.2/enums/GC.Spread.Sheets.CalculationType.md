# Enumeration: CalculationType

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).CalculationType

指定计算函数的计算类型。

## Table of contents

### Enumeration members

- [all](GC.Spread.Sheets.CalculationType.md#all)
- [minimal](GC.Spread.Sheets.CalculationType.md#minimal)
- [rebuild](GC.Spread.Sheets.CalculationType.md#rebuild)
- [regular](GC.Spread.Sheets.CalculationType.md#regular)

## Enumeration members

### <a id="all" name="all"></a> all

• **all** = `0`

默认的计算类型，将范围内的单元格标记为需要计算。

___

### <a id="minimal" name="minimal"></a> minimal

• **minimal** = `2`

保持当前的计算脏状态，并且不会标记易变单元格和循环引用单元格。

___

### <a id="rebuild" name="rebuild"></a> rebuild

• **rebuild** = `1`

这将重建范围内的所有公式模型，然后将它们标记为需要计算。

___

### <a id="regular" name="regular"></a> regular

• **regular** = `3`

保持当前的计算脏状态，并将易变单元格和循环引用单元格标记为需要计算。
