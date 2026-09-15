# Enumeration: StorageType

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).StorageType

存储数据类型

**`代码示例`**
```
//本示例使用StorageType枚举
activeSheet.getCell(0,0).value("A1");
activeSheet.clear(0,0,3,3,GC.Spread.Sheets.SheetArea.viewport,GC.Spread.Sheets.StorageType.data);
```

## Table of contents

### Enumeration members

- [altText](GC.Spread.Sheets.StorageType.md#alttext)
- [axis](GC.Spread.Sheets.StorageType.md#axis)
- [bindingPath](GC.Spread.Sheets.StorageType.md#bindingpath)
- [comment](GC.Spread.Sheets.StorageType.md#comment)
- [data](GC.Spread.Sheets.StorageType.md#data)
- [hyperlink](GC.Spread.Sheets.StorageType.md#hyperlink)
- [sparkline](GC.Spread.Sheets.StorageType.md#sparkline)
- [style](GC.Spread.Sheets.StorageType.md#style)
- [tag](GC.Spread.Sheets.StorageType.md#tag)

## Enumeration members

### <a id="alttext" name="alttext"></a> altText

• **altText** = `512`

 存储数据类型为替代文本

___

### <a id="axis" name="axis"></a> axis

• **axis** = `32`

 存储数据类型为轴信息

___

### <a id="bindingpath" name="bindingpath"></a> bindingPath

• **bindingPath** = `64`

 存储数据类型为数据绑定路径

___

### <a id="comment" name="comment"></a> comment

• **comment** = `4`

 存储数据类型为批注

___

### <a id="data" name="data"></a> data

• **data** = `1`

 存储数据类型为纯值

___

### <a id="hyperlink" name="hyperlink"></a> hyperlink

• **hyperlink** = `256`

 存储数据类型为超链接

___

### <a id="sparkline" name="sparkline"></a> sparkline

• **sparkline** = `16`

 存储数据类型为迷你图

___

### <a id="style" name="style"></a> style

• **style** = `2`

 存储数据类型为样式

___

### <a id="tag" name="tag"></a> tag

• **tag** = `8`

 存储数据类型为标签
