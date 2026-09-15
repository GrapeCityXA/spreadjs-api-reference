# Enumeration: PrintPageOrientation

[Sheets](../modules/GC.Spread.Sheets.md).[Print](../modules/GC.Spread.Sheets.Print.md).PrintPageOrientation

用于打印的页面方向

**`代码示例`**
```
activeSheet.setArray(0, 0, [['Title 1', 'Title 2'], [1, 2], [3, 4]]);
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
// Specify the page orientation for printing.
printInfo.orientation(GC.Spread.Sheets.Print.PrintPageOrientation.landscape);
activeSheet.printInfo(printInfo);
spread.print(0);
```

## Table of contents

### Enumeration members

- [landscape](GC.Spread.Sheets.Print.PrintPageOrientation.md#landscape)
- [portrait](GC.Spread.Sheets.Print.PrintPageOrientation.md#portrait)

## Enumeration members

### <a id="landscape" name="landscape"></a> landscape

• **landscape** = `2`

横向打印

___

### <a id="portrait" name="portrait"></a> portrait

• **portrait** = `1`

纵向打印
