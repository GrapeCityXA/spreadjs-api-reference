# Interface: IRequestMessage<T\>

## Type parameters

| Name |
| :------ |
| `T` |

## Table of contents

### Properties

- [a](IRequestMessage.md#a)
- [create](IRequestMessage.md#create)
- [del](IRequestMessage.md#del)
- [error](IRequestMessage.md#error)
- [op](IRequestMessage.md#op)
- [v](IRequestMessage.md#v)

## Properties

### <a id="a" name="a"></a> a

• **a**: [`MessageActions`](../enums/MessageActions.md)

message action

___

### <a id="create" name="create"></a> create

• `Optional` **create**: [`ICreateComponent`](ICreateComponent.md)

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

version
