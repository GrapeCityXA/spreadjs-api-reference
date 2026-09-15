# Class: AsyncFunction

[CalcEngine](../modules/GC.Spread.CalcEngine.md).[Functions](../modules/GC.Spread.CalcEngine.Functions.md).AsyncFunction

## Hierarchy

- [`Function`](GC.Spread.CalcEngine.Functions.Function.md)

  ↳ **`AsyncFunction`**

## Table of contents

### Constructors

- [constructor](GC.Spread.CalcEngine.Functions.AsyncFunction.md#constructor)

### Properties

- [maxArgs](GC.Spread.CalcEngine.Functions.AsyncFunction.md#maxargs)
- [minArgs](GC.Spread.CalcEngine.Functions.AsyncFunction.md#minargs)
- [name](GC.Spread.CalcEngine.Functions.AsyncFunction.md#name)
- [typeName](GC.Spread.CalcEngine.Functions.AsyncFunction.md#typename)

### Methods

- [acceptsArray](GC.Spread.CalcEngine.Functions.AsyncFunction.md#acceptsarray)
- [acceptsError](GC.Spread.CalcEngine.Functions.AsyncFunction.md#acceptserror)
- [acceptsMissingArgument](GC.Spread.CalcEngine.Functions.AsyncFunction.md#acceptsmissingargument)
- [acceptsReference](GC.Spread.CalcEngine.Functions.AsyncFunction.md#acceptsreference)
- [defaultValue](GC.Spread.CalcEngine.Functions.AsyncFunction.md#defaultvalue)
- [description](GC.Spread.CalcEngine.Functions.AsyncFunction.md#description)
- [evaluate](GC.Spread.CalcEngine.Functions.AsyncFunction.md#evaluate)
- [evaluateAsync](GC.Spread.CalcEngine.Functions.AsyncFunction.md#evaluateasync)
- [evaluateMode](GC.Spread.CalcEngine.Functions.AsyncFunction.md#evaluatemode)
- [findBranchArgument](GC.Spread.CalcEngine.Functions.AsyncFunction.md#findbranchargument)
- [findTestArgument](GC.Spread.CalcEngine.Functions.AsyncFunction.md#findtestargument)
- [interval](GC.Spread.CalcEngine.Functions.AsyncFunction.md#interval)
- [isBranch](GC.Spread.CalcEngine.Functions.AsyncFunction.md#isbranch)
- [isContextSensitive](GC.Spread.CalcEngine.Functions.AsyncFunction.md#iscontextsensitive)
- [isVolatile](GC.Spread.CalcEngine.Functions.AsyncFunction.md#isvolatile)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new AsyncFunction**(`name`, `minArgs?`, `maxArgs?`, `description?`)

表示用于定义异步函数的抽象基类

**`代码示例`**
```
class WeatherFunction extends GC.Spread.CalcEngine.Functions.AsyncFunction {
    constructor () {
        super('WEATHER', 0, 0, {
            description: "Get Weather",
            parameters: []
        });
    }
    evaluate (context) {
        setTimeout(function () { context.setAsyncResult('sunny'); }, 100);
    }
}
spread.addCustomFunction(new WeatherFunction());
spread.getActiveSheet().setFormula(0, 0, '=WEATHER()');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 函数的名称 |
| `minArgs?` | `number` | 函数的最小参数数目 |
| `maxArgs?` | `number` | 函数的最大参数数目 |
| `description?` | [`IFunctionDescription`](../interfaces/GC.Spread.CalcEngine.Functions.IFunctionDescription.md) | 函数的描述 |

#### Overrides

[Function](GC.Spread.CalcEngine.Functions.Function.md).[constructor](GC.Spread.CalcEngine.Functions.Function.md#constructor)

## Properties

### <a id="maxargs" name="maxargs"></a> maxArgs

• **maxArgs**: `number`

函数的最大参数数量

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[maxArgs](GC.Spread.CalcEngine.Functions.Function.md#maxargs)

___

### <a id="minargs" name="minargs"></a> minArgs

• **minArgs**: `number`

函数的最小参数数量

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[minArgs](GC.Spread.CalcEngine.Functions.Function.md#minargs)

___

### <a id="name" name="name"></a> name

• **name**: `string`

函数的名称

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[name](GC.Spread.CalcEngine.Functions.Function.md#name)

___

### <a id="typename" name="typename"></a> typeName

• **typeName**: `string`

支持序列化的类型名称字符串

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[typeName](GC.Spread.CalcEngine.Functions.Function.md#typename)

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

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[acceptsArray](GC.Spread.CalcEngine.Functions.Function.md#acceptsarray)

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

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[acceptsError](GC.Spread.CalcEngine.Functions.Function.md#acceptserror)

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

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[acceptsMissingArgument](GC.Spread.CalcEngine.Functions.Function.md#acceptsmissingargument)

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

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[acceptsReference](GC.Spread.CalcEngine.Functions.Function.md#acceptsreference)

___

### <a id="defaultvalue" name="defaultvalue"></a> defaultValue

▸ **defaultValue**(): `any`

在获取异步结果之前，返回已计算函数结果的默认值

#### Returns

`any`

获取异步结果之前计算的函数结果的默认值

___

### <a id="description" name="description"></a> description

▸ **description**(): [`IFunctionDescription`](../interfaces/GC.Spread.CalcEngine.Functions.IFunctionDescription.md)

返回函数的描述

**`function`**

#### Returns

[`IFunctionDescription`](../interfaces/GC.Spread.CalcEngine.Functions.IFunctionDescription.md)

函数的描述

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[description](GC.Spread.CalcEngine.Functions.Function.md#description)

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

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[evaluate](GC.Spread.CalcEngine.Functions.Function.md#evaluate)

___

### <a id="evaluateasync" name="evaluateasync"></a> evaluateAsync

▸ **evaluateAsync**(`context`, `args`): `any`

返回函数作为参数

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context` | [`AsyncEvaluateContext`](GC.Spread.CalcEngine.AsyncEvaluateContext.md) | 计算上下文 |
| `args` | `any` | 函数求值的参数 |

#### Returns

`any`

应用于参数的函数

___

### <a id="evaluatemode" name="evaluatemode"></a> evaluateMode

▸ **evaluateMode**(): [`AsyncFunctionEvaluateMode`](../enums/GC.Spread.CalcEngine.Functions.AsyncFunctionEvaluateMode.md)

设置如何重新计算公式

#### Returns

[`AsyncFunctionEvaluateMode`](../enums/GC.Spread.CalcEngine.Functions.AsyncFunctionEvaluateMode.md)

计算模式

___

### <a id="findbranchargument" name="findbranchargument"></a> findBranchArgument

▸ **findBranchArgument**(`test`): `number`

查找分支参数

**`代码示例`**
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

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[findBranchArgument](GC.Spread.CalcEngine.Functions.Function.md#findbranchargument)

___

### <a id="findtestargument" name="findtestargument"></a> findTestArgument

▸ **findTestArgument**(): `number`

在分支此函数时查找测试参数

**`代码示例`**
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

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[findTestArgument](GC.Spread.CalcEngine.Functions.Function.md#findtestargument)

___

### <a id="interval" name="interval"></a> interval

▸ **interval**(): `number`

返回时间间隔

#### Returns

`number`

以毫秒为单位的间隔

___

### <a id="isbranch" name="isbranch"></a> isBranch

▸ **isBranch**(): `boolean`

获取表示此函数是否由参数作为条件分支的值

**`代码示例`**
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

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[isBranch](GC.Spread.CalcEngine.Functions.Function.md#isbranch)

___

### <a id="iscontextsensitive" name="iscontextsensitive"></a> isContextSensitive

▸ **isContextSensitive**(): `boolean`

确定函数的计算是否依赖于计算的上下文

#### Returns

`boolean`

为`true` 时，函数的计算依赖于上下文；若为 `false`则不依赖

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[isContextSensitive](GC.Spread.CalcEngine.Functions.Function.md#iscontextsensitive)

___

### <a id="isvolatile" name="isvolatile"></a> isVolatile

▸ **isVolatile**(): `boolean`

确定函数在计算时是否易失

#### Returns

`boolean`

为`true` 时，则函数是易失的；若为`false`则不是

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[isVolatile](GC.Spread.CalcEngine.Functions.Function.md#isvolatile)
