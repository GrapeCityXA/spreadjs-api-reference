# Enumeration: ButtonVisibility

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).ButtonVisibility

指定单元格按钮的可见性。

**`example`**
```
//此示例设置单元格按钮的可见性。
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

表示单元格按钮始终可见。

___

### <a id="onediting" name="onediting"></a> onEditing

• **onEditing** = `2`

表示单元格按钮在单元格进入编辑状态时可见。

___

### <a id="onselected" name="onselected"></a> onSelected

• **onSelected** = `1`

表示单元格按钮在单元格激活时可见。
