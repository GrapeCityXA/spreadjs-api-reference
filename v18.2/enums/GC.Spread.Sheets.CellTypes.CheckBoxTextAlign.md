# Enumeration: CheckBoxTextAlign

[Sheets](../modules/GC.Spread.Sheets.md).[CellTypes](../modules/GC.Spread.Sheets.CellTypes.md).CheckBoxTextAlign

指定复选框单元格的文本对齐方式。

**`example`**
```
//此示例创建一个复选框单元格。
var cellType1 = new GC.Spread.Sheets.CellTypes.CheckBox();
cellType1.caption("caption");
cellType1.textTrue("true");
cellType1.textFalse("false");
cellType1.textIndeterminate("indeterminate");
cellType1.textAlign(GC.Spread.Sheets.CellTypes.CheckBoxTextAlign.bottom);
cellType1.isThreeState(true);
cellType1.boxSize(20);
activeSheet.getCell(1, 1).cellType(cellType1);
```

## Table of contents

### Enumeration members

- [bottom](GC.Spread.Sheets.CellTypes.CheckBoxTextAlign.md#bottom)
- [inside](GC.Spread.Sheets.CellTypes.CheckBoxTextAlign.md#inside)
- [left](GC.Spread.Sheets.CellTypes.CheckBoxTextAlign.md#left)
- [right](GC.Spread.Sheets.CellTypes.CheckBoxTextAlign.md#right)
- [top](GC.Spread.Sheets.CellTypes.CheckBoxTextAlign.md#top)

## Enumeration members

### <a id="bottom" name="bottom"></a> bottom

• **bottom** = `1`

指定文本位于复选框下方。

___

### <a id="inside" name="inside"></a> inside

• **inside** = `4`

指定文本位于切换按钮内部。

___

### <a id="left" name="left"></a> left

• **left** = `2`

指定文本位于复选框左侧。

___

### <a id="right" name="right"></a> right

• **right** = `3`

指定文本位于复选框右侧。

___

### <a id="top" name="top"></a> top

• **top** = `0`

指定文本位于复选框上方。
