# Enumeration: TextDecorationType

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).TextDecorationType

文本样式的类型

**`代码示例`**
``` javascript
//本例使用TextDecorationType枚举
activeSheet.getCell(0, 0).textDecoration(GC.Spread.Sheets.TextDecorationType.underline);
activeSheet.getRange(1, -1, 1, -1).textDecoration(GC.Spread.Sheets.TextDecorationType.overline | GC.Spread.Sheets.TextDecorationType.underline);
activeSheet.getRange(-1, 1, -1, 1).textDecoration(GC.Spread.Sheets.TextDecorationType.overline | GC.Spread.Sheets.TextDecorationType.lineThrough | GC.Spread.Sheets.TextDecorationType.underline);
var style = new GC.Spread.Sheets.Style();
style.textDecoration = GC.Spread.Sheets.TextDecorationType.overline | GC.Spread.Sheets.TextDecorationType.underline;
activeSheet.setStyle(1, 1, style, GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(0, 0).value("Test");
activeSheet.getCell(1, 0).value("Test");
activeSheet.getCell(0, 1).value("Test");
```

## Table of contents

### Enumeration members

- [doubleUnderline](GC.Spread.Sheets.TextDecorationType.md#doubleunderline)
- [lineThrough](GC.Spread.Sheets.TextDecorationType.md#linethrough)
- [none](GC.Spread.Sheets.TextDecorationType.md#none)
- [overline](GC.Spread.Sheets.TextDecorationType.md#overline)
- [underline](GC.Spread.Sheets.TextDecorationType.md#underline)

## Enumeration members

### <a id="doubleunderline" name="doubleunderline"></a> doubleUnderline

• **doubleUnderline** = `8`

在文本显示双行线

___

### <a id="linethrough" name="linethrough"></a> lineThrough

• **lineThrough** = `2`

显示横穿文本线

___

### <a id="none" name="none"></a> none

• **none** = `0`

正常文本

___

### <a id="overline" name="overline"></a> overline

• **overline** = `4`

在文本上方线

___

### <a id="underline" name="underline"></a> underline

• **underline** = `1`

在文本显示下划线
