# Class: AsyncEvaluateContext

[Spread](../modules/GC.Spread.md).[CalcEngine](../modules/GC.Spread.CalcEngine.md).AsyncEvaluateContext

## Table of contents

### Constructors

- [constructor](GC.Spread.CalcEngine.AsyncEvaluateContext.md#constructor)

### Methods

- [setAsyncResult](GC.Spread.CalcEngine.AsyncEvaluateContext.md#setasyncresult)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new AsyncEvaluateContext**(`context`)

表示异步函数的求值上下文。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context` | `any` | 通用求值上下文。 |

## Methods

### <a id="setasyncresult" name="setasyncresult"></a> setAsyncResult

▸ **setAsyncResult**(`value`): `void`

将异步函数求值结果设置到CalcEngine，CalcEngine使用此值重新计算包含此异步函数的单元格和所有依赖单元格。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 异步函数求值结果。 |

#### Returns

`void`
