# Enumeration: HighlightPosition

[Sheets](../modules/GC.Spread.Sheets.md).[DataValidation](../modules/GC.Spread.Sheets.DataValidation.md).HighlightPosition

表示数据验证高亮位置。

**`example`**
```javascript
//此示例使用highlightStyle方法。
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

指定在无效数据单元格的左下角显示高亮标记。

___

### <a id="bottomright" name="bottomright"></a> bottomRight

• **bottomRight** = `2`

指定在无效数据单元格的右下角显示高亮标记。

___

### <a id="outsideleft" name="outsideleft"></a> outsideLeft

• **outsideLeft** = `4`

指定在无效数据单元格的左侧显示图标类型的图像。

___

### <a id="outsideright" name="outsideright"></a> outsideRight

• **outsideRight** = `5`

指定在无效数据单元格的右侧显示图标类型的图像。

___

### <a id="topleft" name="topleft"></a> topLeft

• **topLeft** = `0`

指定在无效数据单元格的左上角显示高亮标记。

___

### <a id="topright" name="topright"></a> topRight

• **topRight** = `1`

指定在无效数据单元格的右上角显示高亮标记。
