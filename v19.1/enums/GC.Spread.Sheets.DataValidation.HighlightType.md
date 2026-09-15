# Enumeration: HighlightType

[Sheets](../modules/GC.Spread.Sheets.md).[DataValidation](../modules/GC.Spread.Sheets.DataValidation.md).HighlightType

表示数据验证高亮类型。

**`example`**
```javascript
//此示例使用highlightStyle方法。
sheet.setValue(1, 1, "sss");
var dv = GC.Spread.Sheets.DataValidation.createListValidator('Fruit,Vegetable,Food');
// 自定义无效数据单元格的高亮样式类型、颜色和显示位置
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

指定在无效数据单元格中使用圆形。

___

### <a id="dogear" name="dogear"></a> dogEar

• **dogEar** = `1`

指定在无效数据单元格中使用折角。

___

### <a id="icon" name="icon"></a> icon

• **icon** = `2`

指定在无效数据单元格中使用图标。
