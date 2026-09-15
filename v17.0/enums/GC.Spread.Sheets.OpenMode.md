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

增量加载模式。打开文件时, 可以直接刷新和响应 UI 和 UI 事件

___

### <a id="lazy" name="lazy"></a> lazy

• **lazy** = `1`

按需加载模式。打开文件时, 只会直接加载活动表单。其他表单只有在使用时才会加载

___

### <a id="normal" name="normal"></a> normal

• **normal** = `0`

正常模式
