# Enumeration: PrintCentering

[Sheets](../modules/GC.Spread.Sheets.md).[Print](../modules/GC.Spread.Sheets.Print.md).PrintCentering

详细说明打印页面的居中类型

**`代码示例`**
``` javascript
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

将打印的布局在页面上水平和垂直居中

___

### <a id="horizontal" name="horizontal"></a> horizontal

• **horizontal** = `1`

将打印的布局在页面上水平居中

___

### <a id="none" name="none"></a> none

• **none** = `0`

不使打印页面居中

___

### <a id="vertical" name="vertical"></a> vertical

• **vertical** = `2`

将打印的布局在页面上垂直居中
