# Enumeration: RowColumnStates

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).RowColumnStates

指定行和列的状态类型。

## Table of contents

### Enumeration members

- [active](GC.Spread.Sheets.RowColumnStates.md#active)
- [dirty](GC.Spread.Sheets.RowColumnStates.md#dirty)
- [edit](GC.Spread.Sheets.RowColumnStates.md#edit)
- [hover](GC.Spread.Sheets.RowColumnStates.md#hover)
- [inserted](GC.Spread.Sheets.RowColumnStates.md#inserted)
- [invalid](GC.Spread.Sheets.RowColumnStates.md#invalid)
- [invalidFormula](GC.Spread.Sheets.RowColumnStates.md#invalidformula)
- [selected](GC.Spread.Sheets.RowColumnStates.md#selected)

## Enumeration members

### <a id="active" name="active"></a> active

• **active** = `16`

当行或列处于焦点状态时，其状态包括"active"状态。

___

### <a id="dirty" name="dirty"></a> dirty

• **dirty** = `64`

当单元格值发生变化时，其行和列状态包括"dirty"状态。

___

### <a id="edit" name="edit"></a> edit

• **edit** = `8`

当单元格正在编辑时，其行和列状态包括"edit"状态。

___

### <a id="hover" name="hover"></a> hover

• **hover** = `1`

当鼠标悬停在行和列上时，其状态包括"hover"状态。

___

### <a id="inserted" name="inserted"></a> inserted

• **inserted** = `128`

当插入行时，其状态包括"inserted"状态。此状态仅支持行。

___

### <a id="invalid" name="invalid"></a> invalid

• **invalid** = `2`

当数据验证条件评估失败时，其行和列状态包括"invalid"状态。

___

### <a id="invalidformula" name="invalidformula"></a> invalidFormula

• **invalidFormula** = `512`

当单元格值为无效公式字符串时，其单元格状态包括"invalidFormula"状态。

___

### <a id="selected" name="selected"></a> selected

• **selected** = `32`

当单元格处于选择范围时，其行和列状态包括"selected"状态。
