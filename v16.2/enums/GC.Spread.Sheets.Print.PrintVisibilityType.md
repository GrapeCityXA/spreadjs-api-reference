# Enumeration: PrintVisibilityType

[Sheets](../modules/GC.Spread.Sheets.md).[Print](../modules/GC.Spread.Sheets.Print.md).PrintVisibilityType

该区域是否可见

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.showColumnHeader(GC.Spread.Sheets.Print.PrintVisibilityType.hide);
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

隐藏该区域

___

### <a id="inherit" name="inherit"></a> inherit

• **inherit** = `0`

从Worksheet类继承设置

___

### <a id="show" name="show"></a> show

• **show** = `2`

在每个页面中显示

___

### <a id="showonce" name="showonce"></a> showOnce

• **showOnce** = `3`

显示一次 (在第一页)
