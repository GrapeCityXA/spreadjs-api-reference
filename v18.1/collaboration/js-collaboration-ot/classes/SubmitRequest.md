# Class: SubmitRequest<S, T\>

## Type parameters

| Name |
| :------ |
| `S` |
| `T` |

## Table of contents

### Constructors

- [constructor](SubmitRequest.md#constructor)

### Properties

- [context](SubmitRequest.md#context)
- [doc](SubmitRequest.md#doc)
- [document](SubmitRequest.md#document)
- [extra](SubmitRequest.md#extra)
- [id](SubmitRequest.md#id)
- [maxRetries](SubmitRequest.md#maxretries)
- [op](SubmitRequest.md#op)
- [ops](SubmitRequest.md#ops)
- [retries](SubmitRequest.md#retries)
- [start](SubmitRequest.md#start)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new SubmitRequest**<`S`, `T`\>()

#### Type parameters

| Name |
| :------ |
| `S` |
| `T` |

## Properties

### <a id="context" name="context"></a> context

• **context**: [`IContext`](../interfaces/IContext.md)

___

### <a id="doc" name="doc"></a> doc

• **doc**: [`DocumentServices`](DocumentServices.md)<`S`, `T`\>

___

### <a id="document" name="document"></a> document

• **document**: ``null`` \| [`IDocument`](../interfaces/IDocument.md)

___

### <a id="extra" name="extra"></a> extra

• **extra**: `unknown`

___

### <a id="id" name="id"></a> id

• **id**: `string`

___

### <a id="maxretries" name="maxretries"></a> maxRetries

• `Optional` **maxRetries**: `number`

___

### <a id="op" name="op"></a> op

• **op**: [`IOp`](../interfaces/IOp.md)<`T`\>

___

### <a id="ops" name="ops"></a> ops

• **ops**: [`IOp`](../interfaces/IOp.md)<`T`\>[]

___

### <a id="retries" name="retries"></a> retries

• **retries**: `number`

___

### <a id="start" name="start"></a> start

• **start**: `number`
