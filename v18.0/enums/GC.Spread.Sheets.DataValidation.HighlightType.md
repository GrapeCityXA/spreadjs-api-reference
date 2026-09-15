# Enumeration: HighlightType

[Sheets](../modules/GC.Spread.Sheets.md).[DataValidation](../modules/GC.Spread.Sheets.DataValidation.md).HighlightType

指示数据验证的突出显示类型。

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

- [circle](GC.Spread.Sheets.DataValidation.HighlightType.md#circle)
- [dogEar](GC.Spread.Sheets.DataValidation.HighlightType.md#dogear)
- [icon](GC.Spread.Sheets.DataValidation.HighlightType.md#icon)

## Enumeration members

### <a id="circle" name="circle"></a> circle

• **circle** = `0`

在无效数据单元格中使用圆圈

___

### <a id="dogear" name="dogear"></a> dogEar

• **dogEar** = `1`

在无效数据单元格中使用dogEar

___

### <a id="icon" name="icon"></a> icon

• **icon** = `2`

在无效数据单元格中使用图标
