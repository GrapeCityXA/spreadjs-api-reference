# Enumeration: OpenMode

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).OpenMode

SpreadJS 加载 JSON 的模式

## Table of contents

### Enumeration members

- [incremental](GC.Spread.Sheets.OpenMode.md#incremental)
- [lazy](GC.Spread.Sheets.OpenMode.md#lazy)
- [normal](GC.Spread.Sheets.OpenMode.md#normal)

## Enumeration members

### <a id="incremental" name="incremental"></a> incremental

• **incremental** = `2`

分阶段加载内容，保持界面可响应用户操作。
___

### <a id="lazy" name="lazy"></a> lazy

• **lazy** = `1`

按需加载当前使用的工作表，切换工作表时动态加载所需的内容。

___

### <a id="normal" name="normal"></a> normal

• **normal** = `0`

一次性加载全部内容，适合小型文件。
