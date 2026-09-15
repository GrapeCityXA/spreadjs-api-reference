# Enumeration: CopyToOptions

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).CopyToOptions

指定复制选项。

**`example`**
```javascript
//此示例使用CopyToOption枚举。
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

• **all** = `32767`

表示所有数据类型。

___

### <a id="alttext" name="alttext"></a> altText

• **altText** = `4096`

表示数据类型为替代文本。

___

### <a id="bindingpath" name="bindingpath"></a> bindingPath

• **bindingPath** = `256`

表示数据类型为绑定路径。

___

### <a id="comment" name="comment"></a> comment

• **comment** = `4`

表示数据类型为注释。

___

### <a id="conditionalformat" name="conditionalformat"></a> conditionalFormat

• **conditionalFormat** = `512`

表示数据类型为条件格式。

___

### <a id="defaultvalue" name="defaultvalue"></a> defaultValue

• **defaultValue** = `2048`

表示数据类型为默认值。

___

### <a id="formula" name="formula"></a> formula

• **formula** = `2`

表示数据类型为公式。

___

### <a id="hyperlink" name="hyperlink"></a> hyperlink

• **hyperlink** = `1024`

表示数据类型为超链接。

___

### <a id="outline" name="outline"></a> outline

• **outline** = `8`

表示复制范围组。

___

### <a id="span" name="span"></a> span

• **span** = `32`

表示复制跨度。

___

### <a id="sparkline" name="sparkline"></a> sparkline

• **sparkline** = `16`

表示数据类型为迷你图。

___

### <a id="style" name="style"></a> style

• **style** = `64`

表示数据类型为样式。

___

### <a id="tag" name="tag"></a> tag

• **tag** = `128`

表示数据类型为标签。

___

### <a id="value" name="value"></a> value

• **value** = `1`

表示数据类型为纯数据。
