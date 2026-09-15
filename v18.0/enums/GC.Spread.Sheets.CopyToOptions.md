# Enumeration: CopyToOptions

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).CopyToOptions

复制选项

**`代码示例`**
``` javascript
//本示例使用CopyToOption枚举
activeSheet.getCell(0,0).value("1");
activeSheet.copyTo(0,0,1,1,2,2,GC.Spread.Sheets.CopyToOptions.value);
```

## Table of contents

### Enumeration members

- [all](GC.Spread.Sheets.CopyToOptions.md#all)
- [altText](GC.Spread.Sheets.CopyToOptions.md#alttext)
- [bindingPath](GC.Spread.Sheets.CopyToOptions.md#bindingpath)
- [comment](GC.Spread.Sheets.CopyToOptions.md#comment)
- [conditionalFormat](GC.Spread.Sheets.CopyToOptions.md#conditionalformat)
- [defaultValue](GC.Spread.Sheets.CopyToOptions.md#defaultvalue)
- [formula](GC.Spread.Sheets.CopyToOptions.md#formula)
- [hyperlink](GC.Spread.Sheets.CopyToOptions.md#hyperlink)
- [outline](GC.Spread.Sheets.CopyToOptions.md#outline)
- [span](GC.Spread.Sheets.CopyToOptions.md#span)
- [sparkline](GC.Spread.Sheets.CopyToOptions.md#sparkline)
- [style](GC.Spread.Sheets.CopyToOptions.md#style)
- [tag](GC.Spread.Sheets.CopyToOptions.md#tag)
- [value](GC.Spread.Sheets.CopyToOptions.md#value)

## Enumeration members

### <a id="all" name="all"></a> all

• **all** = `8191`

表示所有类型的数据

___

### <a id="alttext" name="alttext"></a> altText

• **altText** = `4096`

指示数据类型是替代文本

___

### <a id="bindingpath" name="bindingpath"></a> bindingPath

• **bindingPath** = `256`

数据类型是绑定路径

___

### <a id="comment" name="comment"></a> comment

• **comment** = `4`

数据类型为批注

___

### <a id="conditionalformat" name="conditionalformat"></a> conditionalFormat

• **conditionalFormat** = `512`

数据类型为条件格式

___

### <a id="defaultvalue" name="defaultvalue"></a> defaultValue

• **defaultValue** = `2048`

指示数据类型是默认值

___

### <a id="formula" name="formula"></a> formula

• **formula** = `2`

数据类型为公式

___

### <a id="hyperlink" name="hyperlink"></a> hyperlink

• **hyperlink** = `1024`

数据类型为超链接

___

### <a id="outline" name="outline"></a> outline

• **outline** = `8`

复制区域分组

___

### <a id="span" name="span"></a> span

• **span** = `32`

复制单元格合并

___

### <a id="sparkline" name="sparkline"></a> sparkline

• **sparkline** = `16`

数据类型为迷你图

___

### <a id="style" name="style"></a> style

• **style** = `64`

数据类型为样式

___

### <a id="tag" name="tag"></a> tag

• **tag** = `128`

数据类型为标签

___

### <a id="value" name="value"></a> value

• **value** = `1`

数据类型为纯数据
