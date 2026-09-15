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

提供表示表达式树节点的类的基类。这是一个抽象类。

**`example`**
```
// 下面的代码将返回一个Expression
GC.Spread.Sheets.CalcEngine.formulaToExpression(sheet, "=1");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `type` | [`ExpressionType`](../enums/GC.Spread.CalcEngine.ExpressionType.md) |

## Properties

### <a id="type" name="type"></a> type

• **type**: [`ExpressionType`](../enums/GC.Spread.CalcEngine.ExpressionType.md)

表示表达式类型

**`example`**
```
console.log(GC.Spread.Sheets.CalcEngine.formulaToExpression(sheet, "=1").type === GC.Spread.CalcEngine.ExpressionType.number);
```
