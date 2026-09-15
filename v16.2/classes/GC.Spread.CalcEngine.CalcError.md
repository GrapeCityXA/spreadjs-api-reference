# Class: CalcError

[Spread](../modules/GC.Spread.md).[CalcEngine](../modules/GC.Spread.CalcEngine.md).CalcError

## Table of contents

### Constructors

- [constructor](GC.Spread.CalcEngine.CalcError.md#constructor)

### Methods

- [toString](GC.Spread.CalcEngine.CalcError.md#tostring)
- [parse](GC.Spread.CalcEngine.CalcError.md#parse)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new CalcError**(`error`)

代表计算错误

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `error` | `string` | 关于错误的描述 |

## Methods

### <a id="tostring" name="tostring"></a> toString

▸ **toString**(): `string`

返回此实例的字符串

#### Returns

`string`

错误字符串

___

### <a id="parse" name="parse"></a> parse

▸ `Static` **parse**(`value`): [`CalcError`](GC.Spread.CalcEngine.CalcError.md)

从字符串解析指定的错误

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` | 错误字符串 |

#### Returns

[`CalcError`](GC.Spread.CalcEngine.CalcError.md)

计算错误
