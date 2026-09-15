# Class: LineBorder

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).LineBorder

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.LineBorder.md#constructor)

### Properties

- [color](GC.Spread.Sheets.LineBorder.md#color)
- [style](GC.Spread.Sheets.LineBorder.md#style)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new LineBorder**(`color?`, `style?`)

边框

**`代码示例`**
```
//本示例创建一个边框
var border = new GC.Spread.Sheets.LineBorder
border.color = "#7FFFD4";
border.style = GC.Spread.Sheets.LineStyle.double;
var cell = activeSheet.getCell(1, 1, GC.Spread.Sheets.SheetArea.viewport);
cell.borderLeft(border);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `color?` | `string` |
| `style?` | [`LineStyle`](../enums/GC.Spread.Sheets.LineStyle.md) |

## Properties

### <a id="color" name="color"></a> color

• **color**: `string`

边框的颜色 使用已知的颜色名称或十六进制样式颜色值 默认值为黑色

**`代码示例`**
```
//本示例设置了颜色属性
var border = new GC.Spread.Sheets.LineBorder
border.color = "#7FFFD4";
border.style = GC.Spread.Sheets.LineStyle.double;
var cell = activeSheet.getCell(1, 1, GC.Spread.Sheets.SheetArea.viewport);
cell.borderLeft(border);
```

___

### <a id="style" name="style"></a> style

• **style**: [`LineStyle`](../enums/GC.Spread.Sheets.LineStyle.md)

边框线的线条样式默认值为空

**`代码示例`**
```
//本示例设置了style属性
var border = new GC.Spread.Sheets.LineBorder
border.color = "#7FFFD4";
border.style = GC.Spread.Sheets.LineStyle.double;
var cell = activeSheet.getCell(1, 1, GC.Spread.Sheets.SheetArea.viewport);
cell.borderLeft(border);
```
