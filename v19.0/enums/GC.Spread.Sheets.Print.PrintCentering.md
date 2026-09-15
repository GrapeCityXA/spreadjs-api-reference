# Enumeration: PrintCentering

[Sheets](../modules/GC.Spread.Sheets.md).[Print](../modules/GC.Spread.Sheets.Print.md).PrintCentering

指定打印页面的居中类型。

**`example`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.columnStart(0);
printInfo.columnEnd(2);
printInfo.centering(GC.Spread.Sheets.Print.PrintCentering.horizontal);
activeSheet.printInfo(printInfo);
spread.print(0);
```

## Table of contents

### Enumeration members

- [both](GC.Spread.Sheets.Print.PrintCentering.md#both)
- [horizontal](GC.Spread.Sheets.Print.PrintCentering.md#horizontal)
- [none](GC.Spread.Sheets.Print.PrintCentering.md#none)
- [vertical](GC.Spread.Sheets.Print.PrintCentering.md#vertical)

## Enumeration members

### <a id="both" name="both"></a> both

• **both** = `3`

在页面上水平和垂直居中打印布局。

___

### <a id="horizontal" name="horizontal"></a> horizontal

• **horizontal** = `1`

在页面上水平居中打印布局。

___

### <a id="none" name="none"></a> none

• **none** = `0`

不进行任何居中。

___

### <a id="vertical" name="vertical"></a> vertical

• **vertical** = `2`

在页面上垂直居中打印布局。
