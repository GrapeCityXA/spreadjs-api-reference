# Interface: IReplyMessage<S, T\>

## Type parameters

| Name |
| :------ |
| `S` |
| `T` |

## Table of contents

### Properties

- [a](IReplyMessage.md#a)
- [create](IReplyMessage.md#create)
- [data](IReplyMessage.md#data)
- [del](IReplyMessage.md#del)
- [error](IReplyMessage.md#error)
- [op](IReplyMessage.md#op)
- [v](IReplyMessage.md#v)

## Properties

### <a id="a" name="a"></a> a

• **a**: `string`

___

### <a id="create" name="create"></a> create

• `Optional` **create**: [`ICreateComponent`](ICreateComponent.md)

___

### <a id="data" name="data"></a> data

• `Optional` **data**: [`ISnapshot`](ISnapshot.md)<`S`\>

___

### <a id="del" name="del"></a> del

• `Optional` **del**: `boolean`

___

### <a id="error" name="error"></a> error

• `Optional` **error**: [`IErrorData`](IErrorData.md)

___

### <a id="op" name="op"></a> op

• `Optional` **op**: `T`

___

### <a id="v" name="v"></a> v

• `Optional` **v**: `number`
