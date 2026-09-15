# Interface: ISubmitSnapshotContext<T\>

## Type parameters

| Name |
| :------ |
| `T` |

## Hierarchy

- [`IContext`](IContext.md)

  ↳ **`ISubmitSnapshotContext`**

## Table of contents

### Properties

- [connection](ISubmitSnapshotContext.md#connection)
- [op](ISubmitSnapshotContext.md#op)
- [options](ISubmitSnapshotContext.md#options)
- [trigger](ISubmitSnapshotContext.md#trigger)

## Properties

### <a id="connection" name="connection"></a> connection

• `Optional` **connection**: `Connection`

#### Inherited from

[IContext](IContext.md).[connection](IContext.md#connection)

___

### <a id="op" name="op"></a> op

• `Optional` **op**: [`IOp`](IOp.md)<`T`\>

___

### <a id="options" name="options"></a> options

• `Optional` **options**: [`ICustomOptions`](ICustomOptions.md)

#### Inherited from

[IContext](IContext.md).[options](IContext.md#options)

___

### <a id="trigger" name="trigger"></a> trigger

• `Optional` **trigger**: [`SubmitSnapshotTrigger`](../enums/SubmitSnapshotTrigger.md)
