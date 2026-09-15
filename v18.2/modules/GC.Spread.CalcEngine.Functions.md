# Namespace: Functions

[Spread](GC.Spread.md).[CalcEngine](GC.Spread.CalcEngine.md).Functions

## Table of contents

### Enumerations

- [AsyncFunctionEvaluateMode](../enums/GC.Spread.CalcEngine.Functions.AsyncFunctionEvaluateMode.md)

### Classes

- [AsyncFunction](../classes/GC.Spread.CalcEngine.Functions.AsyncFunction.md)
- [Function](../classes/GC.Spread.CalcEngine.Functions.Function.md)

### Interfaces

- [IFunctionDescription](../interfaces/GC.Spread.CalcEngine.Functions.IFunctionDescription.md)
- [IParameterDescription](../interfaces/GC.Spread.CalcEngine.Functions.IParameterDescription.md)

### Functions

- [defineGlobalCustomFunction](GC.Spread.CalcEngine.Functions.md#defineglobalcustomfunction)
- [findGlobalFunction](GC.Spread.CalcEngine.Functions.md#findglobalfunction)
- [removeGlobalFunction](GC.Spread.CalcEngine.Functions.md#removeglobalfunction)

## Functions

### <a id="defineglobalcustomfunction" name="defineglobalcustomfunction"></a> defineGlobalCustomFunction

▸ **defineGlobalCustomFunction**(`name`, `fn`): [`Function`](../classes/GC.Spread.CalcEngine.Functions.Function.md)

定义全局自定义函数。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 函数名称。 |
| `fn` | [`Function`](../classes/GC.Spread.CalcEngine.Functions.Function.md) | 要添加的函数。 |

#### Returns

[`Function`](../classes/GC.Spread.CalcEngine.Functions.Function.md)

___

### <a id="findglobalfunction" name="findglobalfunction"></a> findGlobalFunction

▸ **findGlobalFunction**(`name?`): `any`

获取所有全局函数或由名称指定的一个全局函数。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name?` | `string` | 函数名称。 |

#### Returns

`any`

如果名称为空，返回所有全局函数，否则返回指定名称的函数。

___

### <a id="removeglobalfunction" name="removeglobalfunction"></a> removeGlobalFunction

▸ **removeGlobalFunction**(`name?`): `void`

如果名称为空，则删除所有全局函数，否则删除指定名称的函数。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name?` | `string` | 函数名称。 |

#### Returns

`void`
