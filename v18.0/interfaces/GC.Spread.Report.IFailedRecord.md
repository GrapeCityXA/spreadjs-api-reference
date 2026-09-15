# Interface: IFailedRecord

[Spread](../modules/GC.Spread.md).[Report](../modules/GC.Spread.Report.md).IFailedRecord

## Hierarchy

- [`IRecord`](GC.Spread.Report.IRecord.md)

  ↳ **`IFailedRecord`**

## Table of contents

### Properties

- [entity](GC.Spread.Report.IFailedRecord.md#entity)
- [info](GC.Spread.Report.IFailedRecord.md#info)
- [reason](GC.Spread.Report.IFailedRecord.md#reason)

## Properties

### <a id="entity" name="entity"></a> entity

• **entity**: `Object`

记录键值对象。

#### Index signature

▪ [key: `string`]: [`DataType`](../modules/GC.Spread.Report.md#datatype)

#### Inherited from

[IRecord](GC.Spread.Report.IRecord.md).[entity](GC.Spread.Report.IRecord.md#entity)

___

### <a id="info" name="info"></a> info

• **info**: `Object`

记录信息。

#### Index signature

▪ [key: `string`]: [`IEntityFieldInfo`](GC.Spread.Report.IEntityFieldInfo.md)

#### Inherited from

[IRecord](GC.Spread.Report.IRecord.md).[info](GC.Spread.Report.IRecord.md#info)

___

### <a id="reason" name="reason"></a> reason

• `Optional` **reason**: `string`

原因是DataManager表的submitChanges记录失败的原因。
