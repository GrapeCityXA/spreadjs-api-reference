# Enumeration: ButtonVisibility

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).ButtonVisibility

单元格按钮是否可见

**`代码示例`**
``` javascript
//本示例设置了单元格按钮的可见性
//创建配置
leftButtonConfig1 = {
    caption: "left",
    enabled: true,
    isLeft: true,
    visibility:GC.Spread.Sheets.ButtonVisibility.always,
};
rightButtonConfig1 = {
    caption: "left",
    enabled: true,
    isLeft: false,
    visibility:GC.Spread.Sheets.ButtonVisibility.onSelected,
};
//创建样式
var style = new GC.Spread.Sheets.Style();
style.cellButtons=[
     leftButtonConfig1,
     rightButtonConfig1
];
sheet.setStyle(0, 0, style);
```

## Table of contents

### Enumeration members

- [always](GC.Spread.Sheets.ButtonVisibility.md#always)
- [onEditing](GC.Spread.Sheets.ButtonVisibility.md#onediting)
- [onSelected](GC.Spread.Sheets.ButtonVisibility.md#onselected)

## Enumeration members

### <a id="always" name="always"></a> always

• **always** = `0`

总是显示

___

### <a id="onediting" name="onediting"></a> onEditing

• **onEditing** = `2`

单元格输入编辑时单元格按钮可见

___

### <a id="onselected" name="onselected"></a> onSelected

• **onSelected** = `1`

单元格处于活动状态时单元格按钮可见
