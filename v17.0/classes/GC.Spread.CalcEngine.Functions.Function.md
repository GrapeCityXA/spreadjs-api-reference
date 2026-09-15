# Class: Function

[CalcEngine](../modules/GC.Spread.CalcEngine.md).[Functions](../modules/GC.Spread.CalcEngine.Functions.md).Function

## Hierarchy

- **`Function`**

  ↳ [`AsyncFunction`](GC.Spread.CalcEngine.Functions.AsyncFunction.md)

## Table of contents

### Constructors

- [constructor](GC.Spread.CalcEngine.Functions.Function.md#constructor)

### Properties

- [maxArgs](GC.Spread.CalcEngine.Functions.Function.md#maxargs)
- [minArgs](GC.Spread.CalcEngine.Functions.Function.md#minargs)
- [name](GC.Spread.CalcEngine.Functions.Function.md#name)
- [typeName](GC.Spread.CalcEngine.Functions.Function.md#typename)

### Methods

- [acceptsArray](GC.Spread.CalcEngine.Functions.Function.md#acceptsarray)
- [acceptsError](GC.Spread.CalcEngine.Functions.Function.md#acceptserror)
- [acceptsMissingArgument](GC.Spread.CalcEngine.Functions.Function.md#acceptsmissingargument)
- [acceptsReference](GC.Spread.CalcEngine.Functions.Function.md#acceptsreference)
- [description](GC.Spread.CalcEngine.Functions.Function.md#description)
- [evaluate](GC.Spread.CalcEngine.Functions.Function.md#evaluate)
- [findBranchArgument](GC.Spread.CalcEngine.Functions.Function.md#findbranchargument)
- [findTestArgument](GC.Spread.CalcEngine.Functions.Function.md#findtestargument)
- [isBranch](GC.Spread.CalcEngine.Functions.Function.md#isbranch)
- [isContextSensitive](GC.Spread.CalcEngine.Functions.Function.md#iscontextsensitive)
- [isVolatile](GC.Spread.CalcEngine.Functions.Function.md#isvolatile)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Function**(`name`, `minArgs?`, `maxArgs?`, `functionDescription?`)

用于定义函数的抽象基类

**`example`**
```
class FactorialFunction extends GC.Spread.CalcEngine.Functions.Function {
    constructor () {
        super('FACTORIAL', 1, 1, {
            description: "Function to calculate the Fibonacci number.",
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
spread.addCustomFunction(new FactorialFunction());
spread.getActiveSheet().setFormula(0, 0, '=FACTORIAL(10)');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 函数的名称 |
| `minArgs?` | `number` | 函数的最大参数数量 |
| `maxArgs?` | `number` | 函数的最小参数数量 |
| `functionDescription?` | [`IFunctionDescription`](../interfaces/GC.Spread.CalcEngine.Functions.IFunctionDescription.md) | - |

## Properties

### <a id="maxargs" name="maxargs"></a> maxArgs

• **maxArgs**: `number`

函数的最大参数数量

___

### <a id="minargs" name="minargs"></a> minArgs

• **minArgs**: `number`

函数的最小参数数量

___

### <a id="name" name="name"></a> name

• **name**: `string`

函数的名称

___

### <a id="typename" name="typename"></a> typeName

• **typeName**: `string`

支持序列化的类型名称字符串

## Methods

### <a id="acceptsarray" name="acceptsarray"></a> acceptsArray

▸ **acceptsArray**(`argIndex`): `boolean`

函数是否接收指定参数的数组值

**`function`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `argIndex` | `number` | 参数的索引 |

#### Returns

`boolean`

为`true`时, 函数接收指定参数的数组值；若为`false`则不接收

___

### <a id="acceptserror" name="acceptserror"></a> acceptsError

▸ **acceptsError**(`argIndex`): `boolean`

函数是否可以处理错误值

**`function`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `argIndex` | `number` | 参数的索引 |

#### Returns

`boolean`

为`true`时, 函数可以处理指定参数的错误值；若为 `false`则不可处理

___

### <a id="acceptsmissingargument" name="acceptsmissingargument"></a> acceptsMissingArgument

▸ **acceptsMissingArgument**(`argIndex`): `boolean`

Evaluate方法是否可以处理丢失的参数

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `argIndex` | `number` | 参数的索引 |

#### Returns

`boolean`

为`true`时, Evaluate方法可以处理缺失的参数; 如果为`false`则不可处理

___

### <a id="acceptsreference" name="acceptsreference"></a> acceptsReference

▸ **acceptsReference**(`argIndex`): `boolean`

函数是否接收指定参数的引用值

**`function`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `argIndex` | `number` | 参数的索引 |

#### Returns

`boolean`

为`true`时, 函数接收指定参数的引用值；若为 `false`则不接收

___

### <a id="description" name="description"></a> description

▸ **description**(): [`IFunctionDescription`](../interfaces/GC.Spread.CalcEngine.Functions.IFunctionDescription.md)

返回函数的描述

**`function`**

#### Returns

[`IFunctionDescription`](../interfaces/GC.Spread.CalcEngine.Functions.IFunctionDescription.md)

函数的描述

___

### <a id="evaluate" name="evaluate"></a> evaluate

▸ **evaluate**(...`args`): `any`

返回函数作为参数

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...args` | `any` | 函数求值的参数 |

#### Returns

`any`

应用于参数的函数

___

### <a id="findbranchargument" name="findbranchargument"></a> findBranchArgument

▸ **findBranchArgument**(`test`): `number`

查找分支参数

**`example`**
```
function EqualsFunction() {
    this.name = 'Equals';
    this.maxArgs = 3;
    this.minArgs = 3;
}
EqualsFunction.prototype = new GC.Spread.CalcEngine.Functions.Function();
EqualsFunction.prototype.evaluate = function(logicalTest, valueIfTrue, valueIfFalse) {
    return logicalTest ? valueIfTrue : valueIfFalse;
}
EqualsFunction.prototype.isBranch = function() {
    return true;
}
EqualsFunction.prototype.findTestArgument = function() {
    return 0;
}
EqualsFunction.prototype.findBranchArgument = function(logicalTestResult) {
    if (logicalTestResult === true) {
        return 1;
    }
    return 2;
}
var equalsFunction = new EqualsFunction();
var spread = GC.Spread.Sheets.findControl("ss") || GC.Spread.Sheets.findControl("sampleDiv");
spread.addCustomFunction(equalsFunction);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `test` | `any` | 测试 |

#### Returns

`number`

将作为分支条件的参数的索引

___

### <a id="findtestargument" name="findtestargument"></a> findTestArgument

▸ **findTestArgument**(): `number`

在分支此函数时查找测试参数

**`example`**
```
function EqualsFunction() {
    this.name = 'Equals';
    this.maxArgs = 3;
    this.minArgs = 3;
}
EqualsFunction.prototype = new GC.Spread.CalcEngine.Functions.Function();
EqualsFunction.prototype.evaluate = function(logicalTest, valueIfTrue, valueIfFalse) {
    return logicalTest ? valueIfTrue : valueIfFalse;
}
EqualsFunction.prototype.isBranch = function() {
    return true;
}
EqualsFunction.prototype.findTestArgument = function() {
    return 0;
}
EqualsFunction.prototype.findBranchArgument = function(logicalTestResult) {
    if (logicalTestResult === true) {
        return 1;
    }
    return 2;
}
var equalsFunction = new EqualsFunction();
var spread = GC.Spread.Sheets.findControl("ss") || GC.Spread.Sheets.findControl("sampleDiv");
spread.addCustomFunction(equalsFunction);
```

#### Returns

`number`

将被视为测试条件的参数索引

___

### <a id="isbranch" name="isbranch"></a> isBranch

▸ **isBranch**(): `boolean`

获取表示此函数是否由参数作为条件分支的值

**`example`**
```
function EqualsFunction() {
    this.name = 'Equals';
    this.maxArgs = 3;
    this.minArgs = 3;
}
EqualsFunction.prototype = new GC.Spread.CalcEngine.Functions.Function();
EqualsFunction.prototype.evaluate = function(logicalTest, valueIfTrue, valueIfFalse) {
    return logicalTest ? valueIfTrue : valueIfFalse;
}
EqualsFunction.prototype.isBranch = function() {
    return true;
}
EqualsFunction.prototype.findTestArgument = function() {
    return 0;
}
EqualsFunction.prototype.findBranchArgument = function(logicalTestResult) {
    if (logicalTestResult === true) {
        return 1;
    }
    return 2;
}
var equalsFunction = new EqualsFunction();
var spread = GC.Spread.Sheets.findControl("ss") || GC.Spread.Sheets.findControl("sampleDiv");
spread.addCustomFunction(equalsFunction);
```

#### Returns

`boolean`

为`true` 时，该实例是分支；若 `false`则不是

___

### <a id="iscontextsensitive" name="iscontextsensitive"></a> isContextSensitive

▸ **isContextSensitive**(): `boolean`

确定函数的计算是否依赖于计算的上下文

#### Returns

`boolean`

为`true` 时，函数的计算依赖于上下文；若为 `false`则不依赖

___

### <a id="isvolatile" name="isvolatile"></a> isVolatile

▸ **isVolatile**(): `boolean`

确定函数在计算时是否易失

#### Returns

`boolean`

为`true` 时，则函数是易失的；若为`false`则不是
