# Enumeration: ButtonImageType

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).ButtonImageType

指定单元格按钮的类型。

**`example`**
```
//此示例设置单元格按钮的类型。
//创建配置
leftButtonConfig1 = {
    caption: "left",
    enabled: true,
    isLeft: true,
    imageType:GC.Spread.Sheets.ButtonImageType.left,
};
rightButtonConfig1 = {
    caption: "left",
    enabled: true,
    isLeft: false,
    imageType:GC.Spread.Sheets.ButtonImageType.right,
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

- [cancel](GC.Spread.Sheets.ButtonImageType.md#cancel)
- [clear](GC.Spread.Sheets.ButtonImageType.md#clear)
- [collapse](GC.Spread.Sheets.ButtonImageType.md#collapse)
- [custom](GC.Spread.Sheets.ButtonImageType.md#custom)
- [dropdown](GC.Spread.Sheets.ButtonImageType.md#dropdown)
- [ellipsis](GC.Spread.Sheets.ButtonImageType.md#ellipsis)
- [expand](GC.Spread.Sheets.ButtonImageType.md#expand)
- [left](GC.Spread.Sheets.ButtonImageType.md#left)
- [minus](GC.Spread.Sheets.ButtonImageType.md#minus)
- [none](GC.Spread.Sheets.ButtonImageType.md#none)
- [ok](GC.Spread.Sheets.ButtonImageType.md#ok)
- [plus](GC.Spread.Sheets.ButtonImageType.md#plus)
- [redo](GC.Spread.Sheets.ButtonImageType.md#redo)
- [right](GC.Spread.Sheets.ButtonImageType.md#right)
- [search](GC.Spread.Sheets.ButtonImageType.md#search)
- [separator](GC.Spread.Sheets.ButtonImageType.md#separator)
- [spinLeft](GC.Spread.Sheets.ButtonImageType.md#spinleft)
- [spinRight](GC.Spread.Sheets.ButtonImageType.md#spinright)
- [undo](GC.Spread.Sheets.ButtonImageType.md#undo)

## Enumeration members

### <a id="cancel" name="cancel"></a> cancel

• **cancel** = `3`

表示单元格按钮类型为取消。

___

### <a id="clear" name="clear"></a> clear

• **clear** = `2`

表示单元格按钮类型为清除。

___

### <a id="collapse" name="collapse"></a> collapse

• **collapse** = `17`

表示单元格按钮类型为折叠。

___

### <a id="custom" name="custom"></a> custom

• **custom** = `1`

表示单元格按钮类型为自定义。

___

### <a id="dropdown" name="dropdown"></a> dropdown

• **dropdown** = `5`

表示单元格按钮类型为下拉。

___

### <a id="ellipsis" name="ellipsis"></a> ellipsis

• **ellipsis** = `6`

表示单元格按钮类型为省略号。

___

### <a id="expand" name="expand"></a> expand

• **expand** = `18`

表示单元格按钮类型为展开。

___

### <a id="left" name="left"></a> left

• **left** = `7`

表示单元格按钮类型为左。

___

### <a id="minus" name="minus"></a> minus

• **minus** = `10`

表示单元格按钮类型为减号。

___

### <a id="none" name="none"></a> none

• **none** = `0`

表示单元格按钮图像类型为无。

___

### <a id="ok" name="ok"></a> ok

• **ok** = `4`

表示单元格按钮类型为确定。

___

### <a id="plus" name="plus"></a> plus

• **plus** = `9`

表示单元格按钮类型为加号。

___

### <a id="redo" name="redo"></a> redo

• **redo** = `12`

表示单元格按钮类型为重做。

___

### <a id="right" name="right"></a> right

• **right** = `8`

表示单元格按钮类型为右。

___

### <a id="search" name="search"></a> search

• **search** = `13`

表示单元格按钮类型为搜索。

___

### <a id="separator" name="separator"></a> separator

• **separator** = `14`

表示单元格按钮类型为分隔符。

___

### <a id="spinleft" name="spinleft"></a> spinLeft

• **spinLeft** = `15`

表示单元格按钮类型为向左旋转。

___

### <a id="spinright" name="spinright"></a> spinRight

• **spinRight** = `16`

表示单元格按钮类型为向右旋转。

___

### <a id="undo" name="undo"></a> undo

• **undo** = `11`

表示单元格按钮类型为撤销。
