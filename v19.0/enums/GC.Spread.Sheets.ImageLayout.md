# Enumeration: ImageLayout

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).ImageLayout

定义背景图片的布局方式。

**`example`**
```
var rowImage = "./css/images/quarter1.png";
sheet.getCell(1, -1).backgroundImage(rowImage);
sheet.getCell(1, -1).backgroundImageLayout(GC.Spread.Sheets.ImageLayout.center);
```

## Table of contents

### Enumeration members

- [center](GC.Spread.Sheets.ImageLayout.md#center)
- [none](GC.Spread.Sheets.ImageLayout.md#none)
- [stretch](GC.Spread.Sheets.ImageLayout.md#stretch)
- [zoom](GC.Spread.Sheets.ImageLayout.md#zoom)

## Enumeration members

### <a id="center" name="center"></a> center

• **center** = `1`

指定背景图片在区域中心显示。

___

### <a id="none" name="none"></a> none

• **none** = `3`

指定背景图片在区域左上角以原始大小显示。

___

### <a id="stretch" name="stretch"></a> stretch

• **stretch** = `0`

指定背景图片填充整个区域。

___

### <a id="zoom" name="zoom"></a> zoom

• **zoom** = `2`

指定背景图片在区域中保持原始宽高比显示。
