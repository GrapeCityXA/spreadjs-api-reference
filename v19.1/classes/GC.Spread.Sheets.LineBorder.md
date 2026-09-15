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

表示边框一侧的线条边框。

**`example`**
```javascript
//此示例创建一个边框。
var border = new GC.Spread.Sheets.LineBorder
border.color = "#7FFFD4";
border.style = GC.Spread.Sheets.LineStyle.double;
var cell = activeSheet.getCell(1, 1, GC.Spread.Sheets.SheetArea.viewport);
cell.borderLeft(border);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `color?` | `string` | 表示边框颜色，使用颜色名称（例如"red"）或"#RGB"、"#RRGGBB"、"rgb(R,B,B)"、"rgba(R,G,B,A)"等格式。 |
| `style?` | [`LineStyle`](../enums/GC.Spread.Sheets.LineStyle.md) | 表示边框线条样式。 |

## Properties

### <a id="color" name="color"></a> color

• **color**: `string`

表示边框线条的颜色。使用已知的颜色名称或HEX格式的颜色值。默认值为黑色。

**`example`**
```javascript
//此示例设置color属性。
var border = new GC.Spread.Sheets.LineBorder
border.color = "#7FFFD4";
border.style = GC.Spread.Sheets.LineStyle.double;
var cell = activeSheet.getCell(1, 1, GC.Spread.Sheets.SheetArea.viewport);
cell.borderLeft(border);
```

___

### <a id="style" name="style"></a> style

• **style**: [`LineStyle`](../enums/GC.Spread.Sheets.LineStyle.md)

表示边框线条的样式。默认值为空。

**`example`**
```javascript
//此示例设置style属性。
var border = new GC.Spread.Sheets.LineBorder
border.color = "#7FFFD4";
border.style = GC.Spread.Sheets.LineStyle.double;
var cell = activeSheet.getCell(1, 1, GC.Spread.Sheets.SheetArea.viewport);
cell.borderLeft(border);
```
