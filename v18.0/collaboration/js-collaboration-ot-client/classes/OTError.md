# Class: OTError

## Hierarchy

- `Error`

  ↳ **`OTError`**

## Table of contents

### Constructors

- [constructor](OTError.md#constructor)

### Properties

- [data](OTError.md#data)
- [idToError](OTError.md#idtoerror)
- [message](OTError.md#message)
- [name](OTError.md#name)
- [stack](OTError.md#stack)
- [CODES](OTError.md#codes)
- [prepareStackTrace](OTError.md#preparestacktrace)
- [stackTraceLimit](OTError.md#stacktracelimit)

### Methods

- [captureStackTrace](OTError.md#capturestacktrace)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new OTError**(`message?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `message?` | `string` |

#### Inherited from

Error.constructor

## Properties

### <a id="data" name="data"></a> data

• `Optional` **data**: `unknown`

___

### <a id="idtoerror" name="idtoerror"></a> idToError

• `Optional` **idToError**: ``null`` \| [`IIdToError`](../interfaces/IIdToError.md)

___

### <a id="message" name="message"></a> message

• **message**: `string`

#### Inherited from

Error.message

___

### <a id="name" name="name"></a> name

• **name**: `string`

#### Overrides

Error.name

___

### <a id="stack" name="stack"></a> stack

• `Optional` **stack**: `string`

#### Inherited from

Error.stack

___

### <a id="codes" name="codes"></a> CODES

▪ `Static` **CODES**: `Record`<`string`, `string`\>

___

### <a id="preparestacktrace" name="preparestacktrace"></a> prepareStackTrace

▪ `Static` `Optional` **prepareStackTrace**: (`err`: `Error`, `stackTraces`: `CallSite`[]) => `any`

#### Type declaration

▸ (`err`, `stackTraces`): `any`

用于格式化堆栈跟踪的可选重写项

**`see`** https://v8.dev/docs/stack-trace-api#customizing-stack-traces

##### Parameters

| Name | Type |
| :------ | :------ |
| `err` | `Error` |
| `stackTraces` | `CallSite`[] |

##### Returns

`any`

#### Inherited from

Error.prepareStackTrace

___

### <a id="stacktracelimit" name="stacktracelimit"></a> stackTraceLimit

▪ `Static` **stackTraceLimit**: `number`

#### Inherited from

Error.stackTraceLimit

## Methods

### <a id="capturestacktrace" name="capturestacktrace"></a> captureStackTrace

▸ `Static` **captureStackTrace**(`targetObject`, `constructorOpt?`): `void`

Create .stack property on a target object

#### Parameters

| Name | Type |
| :------ | :------ |
| `targetObject` | `object` |
| `constructorOpt?` | `Function` |

#### Returns

`void`

#### Inherited from

Error.captureStackTrace
