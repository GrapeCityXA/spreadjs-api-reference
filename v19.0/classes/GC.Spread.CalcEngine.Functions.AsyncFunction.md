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

表示用于定义异步函数的抽象基类。
异步函数通常用于需要服务器请求或其他耗时任务的操作。

**`example`**
```
class WeatherFunction extends GC.Spread.CalcEngine.Functions.AsyncFunction {
    constructor () {
        super('WEATHER', 0, 0, {
            description: "获取天气",
            parameters: []
        });
    }
    evaluate (context) {
        setTimeout(function () { context.setAsyncResult('sunny'); }, 100); // 这里使用setTimeout来模拟服务器调用。
    }
}
spread.addCustomFunction(new WeatherFunction());
spread.getActiveSheet().setFormula(0, 0, '=WEATHER()');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 函数名称。 |
| `minArgs?` | `number` | - |
| `maxArgs?` | `number` | - |
| `description?` | [`IFunctionDescription`](../interfaces/GC.Spread.CalcEngine.Functions.IFunctionDescription.md) | - |

#### Overrides

[Function](GC.Spread.CalcEngine.Functions.Function.md).[constructor](GC.Spread.CalcEngine.Functions.Function.md#constructor)

## Properties

### <a id="maxargs" name="maxargs"></a> maxArgs

• **maxArgs**: `number`

表示函数的最大参数数量。

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[maxArgs](GC.Spread.CalcEngine.Functions.Function.md#maxargs)

___

### <a id="minargs" name="minargs"></a> minArgs

• **minArgs**: `number`

表示函数的最小参数数量。

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[minArgs](GC.Spread.CalcEngine.Functions.Function.md#minargs)

___

### <a id="name" name="name"></a> name

• **name**: `string`

表示函数的名称。

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[name](GC.Spread.CalcEngine.Functions.Function.md#name)

___

### <a id="typename" name="typename"></a> typeName

• **typeName**: `string`

表示用于支持序列化的类型名称字符串。

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[typeName](GC.Spread.CalcEngine.Functions.Function.md#typename)

## Methods

### <a id="acceptsarray" name="acceptsarray"></a> acceptsArray

▸ **acceptsArray**(`argIndex`): `boolean`

确定函数是否接受指定参数的数组值。

**`function`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `argIndex` | `number` | 参数的索引。 |

#### Returns

`boolean`

如果函数接受指定参数的数组值，则为`true`；否则为`false`。

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[acceptsArray](GC.Spread.CalcEngine.Functions.Function.md#acceptsarray)

___

### <a id="acceptserror" name="acceptserror"></a> acceptsError

▸ **acceptsError**(`argIndex`): `boolean`

指示函数是否可以处理错误值。

**`function`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `argIndex` | `number` | 参数的索引。 |

#### Returns

`boolean`

如果函数可以处理指定参数的错误值，则为`true`；否则为`false`。

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[acceptsError](GC.Spread.CalcEngine.Functions.Function.md#acceptserror)

___

### <a id="acceptsmissingargument" name="acceptsmissingargument"></a> acceptsMissingArgument

▸ **acceptsMissingArgument**(`argIndex`): `boolean`

指示Evaluate方法是否可以处理缺失的参数。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `argIndex` | `number` | 参数的索引 |

#### Returns

`boolean`

如果Evaluate方法可以处理缺失的参数，则为`true`；否则为`false`。

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[acceptsMissingArgument](GC.Spread.CalcEngine.Functions.Function.md#acceptsmissingargument)

___

### <a id="acceptsreference" name="acceptsreference"></a> acceptsReference

▸ **acceptsReference**(`argIndex`): `boolean`

确定函数是否接受指定参数的引用值。

**`function`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `argIndex` | `number` | 参数的索引。 |

#### Returns

`boolean`

如果函数接受指定参数的引用值，则为`true`；否则为`false`。

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[acceptsReference](GC.Spread.CalcEngine.Functions.Function.md#acceptsreference)

___

### <a id="defaultvalue" name="defaultvalue"></a> defaultValue

▸ **defaultValue**(): `any`

返回在获取异步结果之前求值函数结果的默认值。

#### Returns

`any`

在获取异步结果之前求值函数结果的默认值。

___

### <a id="description" name="description"></a> description

▸ **description**(): [`IFunctionDescription`](../interfaces/GC.Spread.CalcEngine.Functions.IFunctionDescription.md)

返回函数的描述。

**`function`**

#### Returns

[`IFunctionDescription`](../interfaces/GC.Spread.CalcEngine.Functions.IFunctionDescription.md)

函数的描述。

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[description](GC.Spread.CalcEngine.Functions.Function.md#description)

___

### <a id="evaluate" name="evaluate"></a> evaluate

▸ **evaluate**(...`args`): `any`

返回函数应用于参数的结果。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `...args` | `any` | 函数求值的参数 |

#### Returns

`any`

函数应用于参数的结果。

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[evaluate](GC.Spread.CalcEngine.Functions.Function.md#evaluate)

___

### <a id="evaluateasync" name="evaluateasync"></a> evaluateAsync

▸ **evaluateAsync**(`context`, `args`): `any`

返回函数应用于参数的结果。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context` | [`AsyncEvaluateContext`](GC.Spread.CalcEngine.AsyncEvaluateContext.md) | 求值上下文 |
| `args` | `any` | 函数求值的参数 |

#### Returns

`any`

函数应用于参数的结果。

___

### <a id="evaluatemode" name="evaluatemode"></a> evaluateMode

▸ **evaluateMode**(): [`AsyncFunctionEvaluateMode`](../enums/GC.Spread.CalcEngine.Functions.AsyncFunctionEvaluateMode.md)

决定如何重新计算公式。

#### Returns

[`AsyncFunctionEvaluateMode`](../enums/GC.Spread.CalcEngine.Functions.AsyncFunctionEvaluateMode.md)

求值模式。

___

### <a id="findbranchargument" name="findbranchargument"></a> findBranchArgument

▸ **findBranchArgument**(`test`): `number`

查找分支参数。

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
| `test` | `any` | 测试条件。 |

#### Returns

`number`

表示将被视为分支条件的参数的索引。

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[findBranchArgument](GC.Spread.CalcEngine.Functions.Function.md#findbranchargument)

___

### <a id="findtestargument" name="findtestargument"></a> findTestArgument

▸ **findTestArgument**(): `number`

当此函数有分支时查找测试参数。

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

表示将被视为测试条件的参数的索引。

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[findTestArgument](GC.Spread.CalcEngine.Functions.Function.md#findtestargument)

___

### <a id="interval" name="interval"></a> interval

▸ **interval**(): `number`

返回时间间隔。

#### Returns

`number`

以毫秒为单位的时间间隔。

___

### <a id="isbranch" name="isbranch"></a> isBranch

▸ **isBranch**(): `boolean`

获取一个值，该值指示此函数是否按条件参数进行分支。
与findBranchArgument和findTestArgument配合使用。

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

如果此实例有分支，则为`true`；否则为`false`。

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[isBranch](GC.Spread.CalcEngine.Functions.Function.md#isbranch)

___

### <a id="iscontextsensitive" name="iscontextsensitive"></a> isContextSensitive

▸ **isContextSensitive**(): `boolean`

确定函数的求值是否依赖于求值发生的上下文。

**`example`**
```javascript
class ContextFunction extends GC.Spread.CalcEngine.Functions.Function {
    constructor () {
        super('CONTEXT', 0, 0);
    }
    isContextSensitive () {
        return true;
    }
    evaluate (context) {
        return context.row + "/" + context.column;
    }
}
spread.addCustomFunction(new ContextFunction());
spread.getActiveSheet().setFormula(0, 0, '=CONTEXT()');
```

#### Returns

`boolean`

如果函数的求值依赖于上下文，则为`true`；否则为`false`。

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[isContextSensitive](GC.Spread.CalcEngine.Functions.Function.md#iscontextsensitive)

___

### <a id="isvolatile" name="isvolatile"></a> isVolatile

▸ **isVolatile**(): `boolean`

确定函数在求值过程中是否易变。
易变性函数会在工作簿中的任何单元格发生更改时重新计算。

**`example`**
```javascript
class RandColorFunction extends GC.Spread.CalcEngine.Functions.Function {
    constructor () {
        super('RANDCOLOR', 0, 0);
    }
    isVolatile () {
        return true;
    }
    evaluate () {
        return "#" + Math.floor(Math.random() * 16777215).toString(16);
    }
}
spread.addCustomFunction(new RandColorFunction());
spread.getActiveSheet().setFormula(0, 0, '=RANDCOLOR()');
```

#### Returns

`boolean`

如果函数易变，则为`true`；否则为`false`。

#### Inherited from

[Function](GC.Spread.CalcEngine.Functions.Function.md).[isVolatile](GC.Spread.CalcEngine.Functions.Function.md#isvolatile)
