# Enumeration: CalculationType

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).CalculationType

指定计算时的类型

## Table of contents

### Enumeration members

- [all](GC.Spread.Sheets.CalculationType.md#all)
- [minimal](GC.Spread.Sheets.CalculationType.md#minimal)
- [rebuild](GC.Spread.Sheets.CalculationType.md#rebuild)
- [regular](GC.Spread.Sheets.CalculationType.md#regular)

## Enumeration members

### <a id="all" name="all"></a> all

• **all** = `0`

默认的计算类型，会将范围内的单元格标记为需要计算的脏数据

___

### <a id="minimal" name="minimal"></a> minimal

• **minimal** = `2`

除当前单元格，不会更多标记其他单元格为脏数据

___

### <a id="rebuild" name="rebuild"></a> rebuild

• **rebuild** = `1`

这将重建范围内的所有公式模型，然后将它们标记为需要计算的脏数据。

___

### <a id="regular" name="regular"></a> regular

• **regular** = `3`

将把易变单元格（volatile）和循环引用单元格（circular）标记为需要计算的脏数据。
