# Enumeration: HighlightPosition

[Sheets](../modules/GC.Spread.Sheets.md).[DataValidation](../modules/GC.Spread.Sheets.DataValidation.md).HighlightPosition

数据验证高亮显示位置

**`example`**
```
//This example uses the highlightStyle method.
sheet.setValue(1, 1, "sss");
var dv = GC.Spread.Sheets.DataValidation.createListValidator('Fruit,Vegetable,Food');
dv.highlightStyle({
   type:GC.Spread.Sheets.DataValidation.HighlightType.dogEar,
   color:'blue',
   position:GC.Spread.Sheets.DataValidation.HighlightPosition.topLeft
});
sheet.setDataValidator(1,1, dv);
spread.options.highlightInvalidData = true;
```

## Table of contents

### Enumeration members

- [bottomLeft](GC.Spread.Sheets.DataValidation.HighlightPosition.md#bottomleft)
- [bottomRight](GC.Spread.Sheets.DataValidation.HighlightPosition.md#bottomright)
- [outsideLeft](GC.Spread.Sheets.DataValidation.HighlightPosition.md#outsideleft)
- [outsideRight](GC.Spread.Sheets.DataValidation.HighlightPosition.md#outsideright)
- [topLeft](GC.Spread.Sheets.DataValidation.HighlightPosition.md#topleft)
- [topRight](GC.Spread.Sheets.DataValidation.HighlightPosition.md#topright)

## Enumeration members

### <a id="bottomleft" name="bottomleft"></a> bottomLeft

• **bottomLeft** = `3`

在无效数据单元的左下方指定高亮显示标志

___

### <a id="bottomright" name="bottomright"></a> bottomRight

• **bottomRight** = `2`

在无效数据单元的右下角指定高亮显示标志

___

### <a id="outsideleft" name="outsideleft"></a> outsideLeft

• **outsideLeft** = `4`

在无效数据单元格左侧的图标类型的图像

___

### <a id="outsideright" name="outsideright"></a> outsideRight

• **outsideRight** = `5`

在无效数据单元格右侧的图标类型的图像

___

### <a id="topleft" name="topleft"></a> topLeft

• **topLeft** = `0`

在无效数据单元的左上方指定高亮显示标志

___

### <a id="topright" name="topright"></a> topRight

• **topRight** = `1`

在无效数据单元的右上角指定高亮显示标志
