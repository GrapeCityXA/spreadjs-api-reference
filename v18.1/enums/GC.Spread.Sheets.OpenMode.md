# Enumeration: OpenMode

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).OpenMode

打开sjs函数的打开模式。

## Table of contents

### Enumeration members

- [incremental](GC.Spread.Sheets.OpenMode.md#incremental)
- [lazy](GC.Spread.Sheets.OpenMode.md#lazy)
- [normal](GC.Spread.Sheets.OpenMode.md#normal)

## Enumeration members

### <a id="incremental" name="incremental"></a> incremental

• **incremental** = `2`

增量打开模式。打开文件时，UI和UI事件可以直接刷新和响应。

___

### <a id="lazy" name="lazy"></a> lazy

• **lazy** = `1`

延迟打开模式。打开文件时，只有活动工作表会直接加载。其他工作表只有在被使用时才会加载。

___

### <a id="normal" name="normal"></a> normal

• **normal** = `0`

普通打开模式，不使用延迟和增量加载。打开文件时，UI和UI事件可以在特定时间点刷新和响应。
