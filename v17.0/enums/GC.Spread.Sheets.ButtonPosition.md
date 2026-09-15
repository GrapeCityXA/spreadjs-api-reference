# Enumeration: ButtonPosition

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).ButtonPosition

指定cellbutton的位置

**`代码示例`**
```
//本示例设置了cellbutton的位置
//创建配置
leftButtonConfig1 = {
    caption: "left",
    enabled: true,
    position: GC.Spread.Sheets.ButtonPosition.right,
    visibility:GC.Spread.Sheets.ButtonVisibility.always,
};
rightButtonConfig1 = {
    caption: "left",
    enabled: true,
    position: GC.Spread.Sheets.ButtonPosition.left,
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

- [left](GC.Spread.Sheets.ButtonPosition.md#left)
- [right](GC.Spread.Sheets.ButtonPosition.md#right)

## Enumeration members

### <a id="left" name="left"></a> left

• **left** = `0`

cellbutton位于单元格的左侧

___

### <a id="right" name="right"></a> right

• **right** = `1`

cellbutton位于单元格的右侧
