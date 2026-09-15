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

异步函数的计算上下文

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context` | `any` | 计算上下文 |

## Methods

### <a id="setasyncresult" name="setasyncresult"></a> setAsyncResult

▸ **setAsyncResult**(`value`): `void`

将异步函数的计算结果设置给CalcEngine, CalcEngine使用此值重新计算包含此异步函数和所有依赖单元格的单元格

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 异步函数计算结果 |

#### Returns

`void`
