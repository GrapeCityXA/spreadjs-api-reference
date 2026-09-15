# Enumeration: TextDecorationType

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).TextDecorationType

定义文本装饰类型。

**`example`**
```javascript
//此示例使用TextDecorationType枚举。
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

- [accountingUnderline](GC.Spread.Sheets.TextDecorationType.md#accountingunderline)
- [doubleAccountingUnderline](GC.Spread.Sheets.TextDecorationType.md#doubleaccountingunderline)
- [doubleUnderline](GC.Spread.Sheets.TextDecorationType.md#doubleunderline)
- [lineThrough](GC.Spread.Sheets.TextDecorationType.md#linethrough)
- [none](GC.Spread.Sheets.TextDecorationType.md#none)
- [overline](GC.Spread.Sheets.TextDecorationType.md#overline)
- [underline](GC.Spread.Sheets.TextDecorationType.md#underline)

## Enumeration members

### <a id="accountingunderline" name="accountingunderline"></a> accountingUnderline

• **accountingUnderline** = `16`

指定在文本下方显示单会计下划线。

___

### <a id="doubleaccountingunderline" name="doubleaccountingunderline"></a> doubleAccountingUnderline

• **doubleAccountingUnderline** = `32`

指定在文本下方显示双会计下划线。

___

### <a id="doubleunderline" name="doubleunderline"></a> doubleUnderline

• **doubleUnderline** = `8`

指定在文本下方显示双线条。

___

### <a id="linethrough" name="linethrough"></a> lineThrough

• **lineThrough** = `2`

指定在文本中间显示线条。

___

### <a id="none" name="none"></a> none

• **none** = `0`

指定普通文本。

___

### <a id="overline" name="overline"></a> overline

• **overline** = `4`

指定在文本上方显示线条。

___

### <a id="underline" name="underline"></a> underline

• **underline** = `1`

指定在文本下方显示线条。
