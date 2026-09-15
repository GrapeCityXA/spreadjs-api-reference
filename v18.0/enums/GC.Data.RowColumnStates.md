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

当行或列获得焦点时，其状态包含 active 状态。

___

### <a id="dirty" name="dirty"></a> dirty

• **dirty** = `64`

当单元格值发生变化时，单元格所在的行和列状态包含 dirty 状态。

___

### <a id="hover" name="hover"></a> hover

• **hover** = `1`

当鼠标悬停在行和列上时，其状态包括 hover 状态。

___

### <a id="inserted" name="inserted"></a> inserted

• **inserted** = `128`

当插入行时，其状态包括 inserted 状态。此状态仅支持行。

___

### <a id="pin" name="pin"></a> pin

• **pin** = `1024`

当固定行/列时，其状态包括 pin 状态。

___

### <a id="primarykey" name="primarykey"></a> primaryKey

• **primaryKey** = `2048`

当列具有主键时，其状态包括 primaryKey 状态。此状态仅支持列。

___

### <a id="readonly" name="readonly"></a> readonly

• **readonly** = `4`

当列为只读时，其状态包括 readonly 状态。此状态仅支持列。

___

### <a id="required" name="required"></a> required

• **required** = `4096`

当列的值是必填项时，其状态包含 required 状态。此状态仅支持列。

___

### <a id="selected" name="selected"></a> selected

• **selected** = `32`

当单元格处于选中范围内时，单元格所在的行和列状态包含 selected 状态。

___

### <a id="updated" name="updated"></a> updated

• **updated** = `256`

当更新某一行时，其状态包含 updated 状态。此状态仅支持行。
