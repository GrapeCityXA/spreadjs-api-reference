# Enumeration: ImeMode

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).ImeMode

定义IME模式来控制输入法编辑器(IME)的状态

**`代码示例`**
```
//本例使用imeMode方法
activeSheet.getRange(-1, 2, -1, 1).imeMode(GC.Spread.Sheets.ImeMode.auto);
```

## Table of contents

### Enumeration members

- [active](GC.Spread.Sheets.ImeMode.md#active)
- [auto](GC.Spread.Sheets.ImeMode.md#auto)
- [disabled](GC.Spread.Sheets.ImeMode.md#disabled)
- [inactive](GC.Spread.Sheets.ImeMode.md#inactive)

## Enumeration members

### <a id="active" name="active"></a> active

• **active** = `2`

所有字符都通过IME输入用户仍然可以停用输入法

___

### <a id="auto" name="auto"></a> auto

• **auto** = `1`

对当前的输入法编辑器状态未做任何更改

___

### <a id="disabled" name="disabled"></a> disabled

• **disabled** = `0`

输入法编辑器已禁用，用户可能无法激活

___

### <a id="inactive" name="inactive"></a> inactive

• **inactive** = `4`

所有输入的字符都没有输入法用户仍然可以激活IME
