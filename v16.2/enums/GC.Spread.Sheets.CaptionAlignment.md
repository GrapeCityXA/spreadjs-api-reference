# Enumeration: CaptionAlignment

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).CaptionAlignment

标题的位置

**`代码示例`**
```
//本示例设置了标题的位置
//创建配置
leftButtonConfig1 = {
    caption: "left",
    enabled: true,
    position: GC.Spread.Sheets.ButtonPosition.right,
    captionAlign:GC.Spread.Sheets.CaptionAlignment.right,
};
rightButtonConfig1 = {
    caption: "left",
    enabled: true,
    position: GC.Spread.Sheets.ButtonPosition.left,
    captionAlign:GC.Spread.Sheets.CaptionAlignment.left,
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

- [left](GC.Spread.Sheets.CaptionAlignment.md#left)
- [right](GC.Spread.Sheets.CaptionAlignment.md#right)

## Enumeration members

### <a id="left" name="left"></a> left

• **left** = `0`

标题在按钮的左边

___

### <a id="right" name="right"></a> right

• **right** = `1`

标题在按钮的右边
