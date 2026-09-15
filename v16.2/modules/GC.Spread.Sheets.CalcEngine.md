# Namespace: CalcEngine

[Spread](GC.Spread.md).[Sheets](GC.Spread.Sheets.md).CalcEngine

## Table of contents

### Enumerations

- [RangeReferenceRelative](../enums/GC.Spread.Sheets.CalcEngine.RangeReferenceRelative.md)

### Functions

- [evaluateFormula](GC.Spread.Sheets.CalcEngine.md#evaluateformula)
- [expressionToFormula](GC.Spread.Sheets.CalcEngine.md#expressiontoformula)
- [formulaToExpression](GC.Spread.Sheets.CalcEngine.md#formulatoexpression)
- [formulaToRanges](GC.Spread.Sheets.CalcEngine.md#formulatoranges)
- [goalSeek](GC.Spread.Sheets.CalcEngine.md#goalseek)
- [rangeToFormula](GC.Spread.Sheets.CalcEngine.md#rangetoformula)
- [rangesToFormula](GC.Spread.Sheets.CalcEngine.md#rangestoformula)

## Functions

### <a id="evaluateformula" name="evaluateformula"></a> evaluateFormula

▸ **evaluateFormula**(`context`, `formula`, `baseRow?`, `baseColumn?`, `useR1C1?`): `any`

计算指定的公式

**`代码示例`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById('ss'), { sheetCount: 1 });
sheet = spread.getSheet(0);
sheet.setValue(0, 0, 1);
sheet.setValue(1, 0, 2);
// 使用EvaluateFormula()方法来计算公式,而无需在表单的单元格中设置公式
var result = GC.Spread.Sheets.CalcEngine.evaluateFormula(sheet, "SUM(A1:A2)", 0, 0);
console.log("SUM(A1:A2) = " + result);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context` | `Object` | 上下文;通常,您应该使用活跃表单对象 |
| `formula` | `string` | 公式字符串 |
| `baseRow?` | `number` | - |
| `baseColumn?` | `number` | - |
| `useR1C1?` | `boolean` | - |

#### Returns

`any`

The evaluated formula result.

___

### <a id="expressiontoformula" name="expressiontoformula"></a> expressionToFormula

▸ **expressionToFormula**(`context`, `expression`, `baseRow?`, `baseColumn?`, `useR1C1?`): `string`

将指定的表达式树解析为公式字符串

**`代码示例`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById('ss'), { sheetCount: 1 });
sheet = spread.getSheet(0);
sheet.setValue(0, 0, 1);
sheet.setValue(0, 1, 2);
sheet.setValue(0, 2, 3);
sheet.addCustomName("customName1", "=12", 0, 0);
sheet.addCustomName("customName2", "Average(20,45)", 0, 0);
sheet.addCustomName("customName3", "=$A$1:$C$1");
sheet.setFormula(1, 0, "customName1");
sheet.setFormula(1, 1, "customName2");
sheet.setFormula(1, 2, "sum(customName3)");
var cname = sheet.getCustomName("customName2");
if (cname instanceof GC.Spread.Sheets.NameInfo) {
    // 获取CustomName
    var name = cname.getName();
    // 获取Expression
    var expression = cname.getExpression();
    // 获取Expression字符串
    var expStr = GC.Spread.Sheets.CalcEngine.expressionToFormula(sheet, expression, 0, 0);
    console.log("Name: " + name + " ; Expression: " + expStr);
}
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context` | `Object` | 上下文; 通常,您应该使用活跃表单对象 |
| `expression` | [`Expression`](../classes/GC.Spread.CalcEngine.Expression.md) | 表达式树 |
| `baseRow?` | `number` | - |
| `baseColumn?` | `number` | - |
| `useR1C1?` | `boolean` | - |

#### Returns

`string`

公式字符串

___

### <a id="formulatoexpression" name="formulatoexpression"></a> formulaToExpression

▸ **formulaToExpression**(`context`, `formula`, `baseRow?`, `baseColumn?`, `useR1C1?`): [`Expression`](../classes/GC.Spread.CalcEngine.Expression.md)

将指定的公式解析为表达式树

**`代码示例`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById('ss'), { sheetCount: 1 });
sheet = spread.getSheet(0);
sheet.setValue(0, 0, 1);
sheet.setValue(0, 1, 2);
sheet.setValue(0, 2, 3);
sheet.getCell(4, 4).formula("=SUM(A1:C1)");
var formula = sheet.getFormula(4, 4);
var expression = GC.Spread.Sheets.CalcEngine.formulaToExpression(sheet, formula, 0, 0);
console.log("Function Name is: " + expression.functionName);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context` | `Object` | 上下文; 通常,您应该使用活跃表单对象 |
| `formula` | `string` | 公式字符串 |
| `baseRow?` | `number` | - |
| `baseColumn?` | `number` | - |
| `useR1C1?` | `boolean` | - |

#### Returns

[`Expression`](../classes/GC.Spread.CalcEngine.Expression.md)

表达式树

___

### <a id="formulatoranges" name="formulatoranges"></a> formulaToRanges

▸ **formulaToRanges**(`sheet`, `formula`, `baseRow?`, `baseCol?`): `Object`[]

将公式字符串转换为指定的单元格区域

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheet` | [`Worksheet`](../classes/GC.Spread.Sheets.Worksheet.md) | 基表 |
| `formula` | `string` | 公式 |
| `baseRow?` | `number` | 公式的基行索引 |
| `baseCol?` | `number` | 公式的基列索引 |

#### Returns

`Object`[]

引用公式字符串的单元格区域

___

### <a id="goalseek" name="goalseek"></a> goalSeek

▸ **goalSeek**(`changingSheet`, `changingRow`, `changingColumn`, `formulaSheet`, `formulaRow`, `formulaColumn`, `desiredResult`): `boolean`

为一个生成所需公式的单元格查找值会影响另一个单元格

**`代码示例`**
```
// 本示例显示了如何使用目标搜索
// 贷款金额为10000,期限为18个月,每月支付600,计算达到目标贷款所需的利率
sheet.setValue(0, 1, 10000); // Loan Amount
sheet.setValue(1, 1, 18); // 月数
sheet.setFormatter(2, 1, "0%"); // 利率
sheet.setFormatter(3, 1, "0.00");
sheet.setFormula(3, 1, "PMT(B3/12,B2,B1)"); // 支付
GC.Spread.Sheets.CalcEngine.goalSeek(sheet, 2, 1, sheet, 3, 1, -600); // 结果在B3是10％
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `changingSheet` | [`Worksheet`](../classes/GC.Spread.Sheets.Worksheet.md) | 包含要调整单元格的表单 |
| `changingRow` | `number` | 包含要调整的值的单元格的行索引 |
| `changingColumn` | `number` | 包含要调整的值的单元格的列索引 |
| `formulaSheet` | [`Worksheet`](../classes/GC.Spread.Sheets.Worksheet.md) | 包含要解析的公式的表单 |
| `formulaRow` | `number` | 包含要解析的公式的单元格的行索引 |
| `formulaColumn` | `number` | 包含要解析的公式的单元格的列索引 |
| `desiredResult` | `number` | 所需的公式结果 |

#### Returns

`boolean`

是否有方案

___

### <a id="rangetoformula" name="rangetoformula"></a> rangeToFormula

▸ **rangeToFormula**(`range`, `baseRow?`, `baseCol?`, `rangeReferenceRelative?`, `useR1C1?`): `string`

将指定的单元格区域转换为公式字符串

**`代码示例`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById('ss'), { sheetCount: 1 });
sheet = spread.getSheet(0);
// 设值
sheet.setValue(0, 0, 1, 3);
sheet.setValue(1, 0, 50, 3);
sheet.setValue(2, 0, 100, 3);
sheet.setValue(3, 0, 2, 3);
sheet.setValue(4, 0, 60, 3);
sheet.setValue(5, 0, 90, 3);
sheet.clearSelection();
// 添加selection
sheet.addSelection(2, 0, 3, 1);
var range = sheet.getSelections();
// 获取range字符串
var rangeStr = GC.Spread.Sheets.CalcEngine.rangeToFormula(range[0]);
// 使用选定区域创建公式
var formula = "Sum(" + rangeStr + ")";
// 在表单的单元格中设置公式
sheet.setFormula(5, 5, formula, GC.Spread.Sheets.SheetArea.viewport);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](../classes/GC.Spread.Sheets.Range.md) | 表单中的单元格区域 |
| `baseRow?` | `number` | - |
| `baseCol?` | `number` | - |
| `rangeReferenceRelative?` | [`RangeReferenceRelative`](../enums/GC.Spread.Sheets.CalcEngine.RangeReferenceRelative.md) | - |
| `useR1C1?` | `boolean` | - |

#### Returns

`string`

引用指定单元格区域的公式字符串

___

### <a id="rangestoformula" name="rangestoformula"></a> rangesToFormula

▸ **rangesToFormula**(`ranges`, `baseRow?`, `baseCol?`, `rangeReferenceRelative?`, `useR1C1?`): `string`

将指定的单元格区域转换为公式字符串

**`代码示例`**
```
spread = new GC.Spread.Sheets.Workbook(document.getElementById('ss'), { sheetCount: 1 });
sheet = spread.getSheet(0);
// 设定值
sheet.setValue(0, 0, 1, 3);
sheet.setValue(1, 0, 50, 3);
sheet.setValue(2, 0, 100, 3);
sheet.setValue(3, 0, 2, 3);
sheet.setValue(4, 0, 60, 3);
sheet.setValue(5, 0, 90, 3);
sheet.setValue(6, 0, 3, 3);
sheet.setValue(7, 0, 40, 3);
sheet.clearSelection();
// 添加selections
sheet.addSelection(0, 0, 3, 1);
sheet.addSelection(5, 0, 2, 1);
var ranges = sheet.getSelections();
// 获取ranges字符串
var rangesStr = GC.Spread.Sheets.CalcEngine.rangesToFormula(ranges);
// 使用选定区域创建公式
var formula = "Sum(" + rangesStr + ")";
// 在表单的单元格中设置公式
sheet.setFormula(5, 5, formula, GC.Spread.Sheets.SheetArea.viewport);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ranges` | [`Range`](../classes/GC.Spread.Sheets.Range.md)[] | 表单中的单元格区域 |
| `baseRow?` | `number` | - |
| `baseCol?` | `number` | - |
| `rangeReferenceRelative?` | [`RangeReferenceRelative`](../enums/GC.Spread.Sheets.CalcEngine.RangeReferenceRelative.md) | - |
| `useR1C1?` | `boolean` | - |

#### Returns

`string`

引用指定单元格区域的公式字符串
