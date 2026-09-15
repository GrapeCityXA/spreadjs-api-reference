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

定义一个全局自定义函数，该函数可在公式中使用。
全局自定义函数可以从任何电子表格中调用。

**`example`**
```javascript
class FactorialFunction extends GC.Spread.CalcEngine.Functions.Function {
    constructor () {
        super('FACTORIAL', 1, 1, {
            description: "用于计算斐波那契数的函数。",
            parameters: [{ name: 'n' }]
        });
    }
    evaluate (n) {
        var fib = [0, 1];
        for (var i = 2; i <= n; i++) {
          fib[i] = fib[i - 1] + fib[i - 2];
        }
        return fib[n];
    }
}
GC.Spread.CalcEngine.Functions.defineGlobalCustomFunction("FACTORIAL", new FactorialFunction());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 函数名称。 |
| `fn` | [`Function`](../classes/GC.Spread.CalcEngine.Functions.Function.md) | 要添加的函数。 |

#### Returns

[`Function`](../classes/GC.Spread.CalcEngine.Functions.Function.md)

被添加的函数。

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
