# Enumeration: PrintVisibilityType

[Sheets](../modules/GC.Spread.Sheets.md).[Print](../modules/GC.Spread.Sheets.Print.md).PrintVisibilityType

指定区域是否可见。

**`example`**
```javascript
activeSheet.setArray(0, 0, [['Title 1', 'Title 2'], [1, 2], [3, 4]]);
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.showColumnHeader(GC.Spread.Sheets.Print.PrintVisibilityType.hide);
activeSheet.printInfo(printInfo);
spread.print(0);
```

## Table of contents

### Enumeration members

- [hide](GC.Spread.Sheets.Print.PrintVisibilityType.md#hide)
- [inherit](GC.Spread.Sheets.Print.PrintVisibilityType.md#inherit)
- [show](GC.Spread.Sheets.Print.PrintVisibilityType.md#show)
- [showOnce](GC.Spread.Sheets.Print.PrintVisibilityType.md#showonce)

## Enumeration members

### <a id="hide" name="hide"></a> hide

• **hide** = `1`

隐藏区域。

___

### <a id="inherit" name="inherit"></a> inherit

• **inherit** = `0`

继承 Worksheet 类的设置。

___

### <a id="show" name="show"></a> show

• **show** = `2`

在每页显示。

___

### <a id="showonce" name="showonce"></a> showOnce

• **showOnce** = `3`

仅显示一次。
