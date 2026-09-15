# Enumeration: ImeMode

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).ImeMode

定义输入法编辑器(IME)的状态控制模式。

**`deprecated`** 此枚举目前仅在Internet Explorer中有效。

**`example`**
```javascript
//此示例使用imeMode方法。
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

所有字符都通过输入法输入。用户仍可以停用输入法。

___

### <a id="auto" name="auto"></a> auto

• **auto** = `1`

不改变当前输入法编辑器的状态。

___

### <a id="disabled" name="disabled"></a> disabled

• **disabled** = `0`

输入法编辑器被禁用，用户无法激活。

___

### <a id="inactive" name="inactive"></a> inactive

• **inactive** = `4`

所有字符都不使用输入法输入。用户仍可以激活输入法。
