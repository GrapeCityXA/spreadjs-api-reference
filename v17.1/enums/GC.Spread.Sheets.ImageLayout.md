# Enumeration: ImageLayout

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).ImageLayout

定义背景图像布局

**`代码示例`**
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

背景图像显示在区域的中心

___

### <a id="none" name="none"></a> none

• **none** = `3`

背景图像以其原始大小显示在区域的左上角

___

### <a id="stretch" name="stretch"></a> stretch

• **stretch** = `0`

背景图像填充该区域

___

### <a id="zoom" name="zoom"></a> zoom

• **zoom** = `2`

背景图像以其原始高宽比显示在区域中
