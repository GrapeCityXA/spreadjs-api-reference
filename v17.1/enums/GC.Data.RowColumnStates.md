# Enumeration: RowColumnStates

[GC](../modules/GC.md).[Data](../modules/GC.Data.md).RowColumnStates

行和列的状态类型

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

当行或列获取焦点，它表示 "active" 状态

___

### <a id="dirty" name="dirty"></a> dirty

• **dirty** = `64`

当单元格的值发生改变，单元格所在行或列的状态代表 "dirty"

___

### <a id="hover" name="hover"></a> hover

• **hover** = `1`

当鼠标悬停在行和列上时，其状态包括"hover"状态

___

### <a id="inserted" name="inserted"></a> inserted

• **inserted** = `128`

插入行时，其状态包括"inserted"状态。此状态仅支持行

___

### <a id="pin" name="pin"></a> pin

• **pin** = `1024`

当固定行/列时，其状态包括"pin"状态

___

### <a id="primarykey" name="primarykey"></a> primaryKey

• **primaryKey** = `2048`

当列具有主键时，其状态包括"primaryKey"状态。该状态仅适用于列

___

### <a id="readonly" name="readonly"></a> readonly

• **readonly** = `4`

当列锁定时，其状态包括"readonly"状态。此状态仅支持列

___

### <a id="required" name="required"></a> required

• **required** = `4096`

当需要列的值时，其状态包括"required"状态。该状态仅适用于列

___

### <a id="selected" name="selected"></a> selected

• **selected** = `32`

当单元格处于选择范围时，单元格行和列状态包括"selected"状态

___

### <a id="updated" name="updated"></a> updated

• **updated** = `256`

更新行时，其状态包括"updated"状态。此状态仅支持行
