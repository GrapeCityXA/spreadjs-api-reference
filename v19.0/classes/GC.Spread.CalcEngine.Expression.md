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
// 将公式字符串转换为表达式树
const expression = GC.Spread.Sheets.CalcEngine.formulaToExpression(sheet, "=SUM(A1:B2)");
console.log(expression.type); // 返回ExpressionType.function
console.log(expression.functionName); // 返回"SUM"
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `type` | [`ExpressionType`](../enums/GC.Spread.CalcEngine.ExpressionType.md) |

## Properties

### <a id="type" name="type"></a> type

• **type**: [`ExpressionType`](../enums/GC.Spread.CalcEngine.ExpressionType.md)

表示公式解析树中表达式节点的类型。每个表达式节点代表公式中的一个特定元素，例如数字、字符串、引用、函数或运算符。

**`example`**
```
console.log(GC.Spread.Sheets.CalcEngine.formulaToExpression(sheet, "=1").type === GC.Spread.CalcEngine.ExpressionType.number);
```
