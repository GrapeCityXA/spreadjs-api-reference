# Enumeration: PrintPageOrder

[Sheets](../modules/GC.Spread.Sheets.md).[Print](../modules/GC.Spread.Sheets.Print.md).PrintPageOrder

页面的打印顺序

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.pageOrder(GC.Spread.Sheets.Print.PrintPageOrder.auto);
activeSheet.printInfo(printInfo);
spread.print(0);
```

## Table of contents

### Enumeration members

- [auto](GC.Spread.Sheets.Print.PrintPageOrder.md#auto)
- [downThenOver](GC.Spread.Sheets.Print.PrintPageOrder.md#downthenover)
- [overThenDown](GC.Spread.Sheets.Print.PrintPageOrder.md#overthendown)

## Enumeration members

### <a id="auto" name="auto"></a> auto

• **auto** = `0`

自动确定打印页面的最佳顺序

___

### <a id="downthenover" name="downthenover"></a> downThenOver

• **downThenOver** = `1`

向下打印页面，然后跨页面打印

___

### <a id="overthendown" name="overthendown"></a> overThenDown

• **overThenDown** = `2`

依次打印页面
