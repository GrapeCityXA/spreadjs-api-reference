# Enumeration: RowColumnStates

[GC](../modules/GC.md).[Data](../modules/GC.Data.md).RowColumnStates

指定行和列状态的类型。

## Table of contents

### Enumeration members

- [active](GC.Data.RowColumnStates.md#active)
- [dirty](GC.Data.RowColumnStates.md#dirty)
- [hover](GC.Data.RowColumnStates.md#hover)
- [inserted](GC.Data.RowColumnStates.md#inserted)
- [pin](GC.Data.RowColumnStates.md#pin)
- [primaryKey](GC.Data.RowColumnStates.md#primarykey)
- [readonly](GC.Data.RowColumnStates.md#readonly)
- [required](GC.Data.RowColumnStates.md#required)
- [selected](GC.Data.RowColumnStates.md#selected)
- [updated](GC.Data.RowColumnStates.md#updated)

## Enumeration members

### <a id="active" name="active"></a> active

• **active** = `16`

当行或列处于焦点状态时，其状态包含 "active" 状态。

___

### <a id="dirty" name="dirty"></a> dirty

• **dirty** = `64`

当单元格值发生更改时，该单元格所在的行和列状态包含 "dirty" 状态。

___

### <a id="hover" name="hover"></a> hover

• **hover** = `1`

当鼠标悬停在行或列上时，其状态包含 "hover" 状态。

___

### <a id="inserted" name="inserted"></a> inserted

• **inserted** = `128`

当插入一行时，其状态包含 "inserted" 状态。此状态仅适用于行。

___

### <a id="pin" name="pin"></a> pin

• **pin** = `1024`

当固定行/列时，其状态包含"pin"（固定）状态。

___

### <a id="primarykey" name="primarykey"></a> primaryKey

• **primaryKey** = `2048`

当列包含主键时，其状态包含"primaryKey"（主键）状态。此状态仅适用于列。

___

### <a id="readonly" name="readonly"></a> readonly

• **readonly** = `4`

当列被锁定时，其状态包含"readonly"（只读）状态。此状态仅适用于列。

___

### <a id="required" name="required"></a> required

• **required** = `4096`

当列值为必填时，其状态包含"required"（必填）状态。此状态仅适用于列。

___

### <a id="selected" name="selected"></a> selected

• **selected** = `32`

当单元格位于选区范围内时，该单元格所在的行和列状态包含 "selected" 状态。

___

### <a id="updated" name="updated"></a> updated

• **updated** = `256`

当更新行时，其状态包含"updated"（已更新）状态。此状态仅适用于行。
