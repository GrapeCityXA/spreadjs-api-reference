# Class: Expression

[Spread](../modules/GC.Spread.md).[CalcEngine](../modules/GC.Spread.CalcEngine.md).Expression

## Table of contents

### Constructors

- [constructor](GC.Spread.CalcEngine.Expression.md#constructor)

### Properties

- [type](GC.Spread.CalcEngine.Expression.md#type)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Expression**(`type`)

表达树节点的抽象基类
**`代码示例`**
``` javascript
// the below code will return a Expression
GC.Spread.Sheets.CalcEngine.formulaToExpression(sheet, "=1");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `type` | [`ExpressionType`](../enums/GC.Spread.CalcEngine.ExpressionType.md) |

## Properties

### <a id="type" name="type"></a> type

• **type**: [`ExpressionType`](../enums/GC.Spread.CalcEngine.ExpressionType.md)

表达式类型
**`代码示例`**
``` javascript
console.log(GC.Spread.Sheets.CalcEngine.formulaToExpression(sheet, "=1").type === GC.Spread.CalcEngine.ExpressionType.number);
```
