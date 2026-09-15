# Enumeration: ButtonImageType

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).ButtonImageType

指定cellbutton的类型

**`代码示例`**
``` javascript
//本示例设置了cellbutton的类型
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

类型为cancel

___

### <a id="clear" name="clear"></a> clear

• **clear** = `2`

类型为clear

___

### <a id="collapse" name="collapse"></a> collapse

• **collapse** = `17`

类型为collapse

___

### <a id="custom" name="custom"></a> custom

• **custom** = `1`

类型是自定义

___

### <a id="dropdown" name="dropdown"></a> dropdown

• **dropdown** = `5`

类型为dropdown

___

### <a id="ellipsis" name="ellipsis"></a> ellipsis

• **ellipsis** = `6`

类型为ellipsis

___

### <a id="expand" name="expand"></a> expand

• **expand** = `18`

类型为expand

___

### <a id="left" name="left"></a> left

• **left** = `7`

类型为left

___

### <a id="minus" name="minus"></a> minus

• **minus** = `10`

类型为minus

___

### <a id="none" name="none"></a> none

• **none** = `0`

类型为none

___

### <a id="ok" name="ok"></a> ok

• **ok** = `4`

类型为ok

___

### <a id="plus" name="plus"></a> plus

• **plus** = `9`

类型为plus

___

### <a id="redo" name="redo"></a> redo

• **redo** = `12`

类型为redo

___

### <a id="right" name="right"></a> right

• **right** = `8`

类型为right

___

### <a id="search" name="search"></a> search

• **search** = `13`

类型为search

___

### <a id="separator" name="separator"></a> separator

• **separator** = `14`

类型为separator

___

### <a id="spinleft" name="spinleft"></a> spinLeft

• **spinLeft** = `15`

类型为spinLeft

___

### <a id="spinright" name="spinright"></a> spinRight

• **spinRight** = `16`

类型为spinRight

___

### <a id="undo" name="undo"></a> undo

• **undo** = `11`

类型为undo
