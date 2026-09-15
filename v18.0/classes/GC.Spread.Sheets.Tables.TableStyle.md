# Class: TableStyle

[Sheets](../modules/GC.Spread.Sheets.md).[Tables](../modules/GC.Spread.Sheets.Tables.md).TableStyle

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Tables.TableStyle.md#constructor)

### Properties

- [backColor](GC.Spread.Sheets.Tables.TableStyle.md#backcolor)
- [borderBottom](GC.Spread.Sheets.Tables.TableStyle.md#borderbottom)
- [borderHorizontal](GC.Spread.Sheets.Tables.TableStyle.md#borderhorizontal)
- [borderLeft](GC.Spread.Sheets.Tables.TableStyle.md#borderleft)
- [borderRight](GC.Spread.Sheets.Tables.TableStyle.md#borderright)
- [borderTop](GC.Spread.Sheets.Tables.TableStyle.md#bordertop)
- [borderVertical](GC.Spread.Sheets.Tables.TableStyle.md#bordervertical)
- [font](GC.Spread.Sheets.Tables.TableStyle.md#font)
- [fontFamily](GC.Spread.Sheets.Tables.TableStyle.md#fontfamily)
- [fontSize](GC.Spread.Sheets.Tables.TableStyle.md#fontsize)
- [fontStyle](GC.Spread.Sheets.Tables.TableStyle.md#fontstyle)
- [fontWeight](GC.Spread.Sheets.Tables.TableStyle.md#fontweight)
- [foreColor](GC.Spread.Sheets.Tables.TableStyle.md#forecolor)
- [textDecoration](GC.Spread.Sheets.Tables.TableStyle.md#textdecoration)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new TableStyle**(`backColor?`, `foreColor?`, `font?`, `borderLeft?`, `borderTop?`, `borderRight?`, `borderBottom?`, `borderHorizontal?`, `borderVertical?`, `textDecoration?`, `fontStyle?`, `fontWeight?`, `fontSize?`, `fontFamily?`)

表格样式信息

**`代码示例`**
``` javascript
//本示例创建了一个表
var tableStyle = new GC.Spread.Sheets.Tables.TableTheme();
var thinBorder = new GC.Spread.Sheets.LineBorder("black", GC.Spread.Sheets.LineStyle.dotted);
tableStyle.wholeTableStyle(new GC.Spread.Sheets.Tables.TableStyle("aliceblue", "green", "bold 10pt arial", thinBorder, thinBorder, thinBorder, thinBorder, thinBorder, thinBorder));
var tableStyleInfo = new GC.Spread.Sheets.Tables.TableStyle(
    "black",
    "white",
    "bold 11pt arial",
    new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin),
    new GC.Spread.Sheets.LineBorder("red", GC.Spread.Sheets.LineStyle.thick),
    new GC.Spread.Sheets.LineBorder("yellow", GC.Spread.Sheets.LineStyle.thin),
    new GC.Spread.Sheets.LineBorder("blue", GC.Spread.Sheets.LineStyle.thick),
    new GC.Spread.Sheets.LineBorder("pink", GC.Spread.Sheets.LineStyle.thin),
    new GC.Spread.Sheets.LineBorder("black", GC.Spread.Sheets.LineStyle.thick),
    GC.Spread.Sheets.TextDecorationType.overline | GC.Spread.Sheets.TextDecorationType.underline);
tableStyle.headerRowStyle(tableStyleInfo);
var table = activeSheet.tables.add("table1", 1, 1, 5, 5, tableStyle);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `backColor?` | `string` \| [`IGradientFill`](../interfaces/GC.Spread.Sheets.IGradientFill.md) \| [`IGradientPathFill`](../interfaces/GC.Spread.Sheets.IGradientPathFill.md) \| [`IPatternFill`](../interfaces/GC.Spread.Sheets.IPatternFill.md) | 表格背景色 |
| `foreColor?` | `string` | 表格前景色 |
| `font?` | `string` | 字体 |
| `borderLeft?` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) | 表格的左边框线 |
| `borderTop?` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) | 表格的上边框线 |
| `borderRight?` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) | 表格的右边框线 |
| `borderBottom?` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) | 表格的下边框线 |
| `borderHorizontal?` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) | 表格的水平边框线 |
| `borderVertical?` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) | 表格的垂直边框线 |
| `textDecoration?` | [`TextDecorationType`](../enums/GC.Spread.Sheets.TextDecorationType.md) | 表格的文本修饰 |
| `fontStyle?` | `string` |
| `fontWeight?` | `string` |
| `fontSize?` | `string` |
| `fontFamily?` | `string` |

## Properties

### <a id="backcolor" name="backcolor"></a> backColor

• **backColor**: `string` \| [`IGradientFill`](../interfaces/GC.Spread.Sheets.IGradientFill.md) \| [`IGradientPathFill`](../interfaces/GC.Spread.Sheets.IGradientPathFill.md) \| [`IPatternFill`](../interfaces/GC.Spread.Sheets.IPatternFill.md)

背景色

**`代码示例`**
``` javascript
//本示例创建了一个表
var tableStyle = new GC.Spread.Sheets.Tables.TableTheme();
var thinBorder = new GC.Spread.Sheets.LineBorder("black", GC.Spread.Sheets.LineStyle.dotted);
tableStyle.wholeTableStyle(new GC.Spread.Sheets.Tables.TableStyle("aliceblue", "green", "bold 10pt arial", thinBorder, thinBorder, thinBorder, thinBorder, thinBorder, thinBorder));
var tStyleInfo = new GC.Spread.Sheets.Tables.TableStyle();
tStyleInfo.backColor = "green";
tStyleInfo.foreColor = "red";
tStyleInfo.borderBottom = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.borderLeft = new GC.Spread.Sheets.LineBorder("yellow", GC.Spread.Sheets.LineStyle.medium);
tStyleInfo.borderTop = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.borderRight = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.font = "bold 11pt arial";
tableStyle.headerRowStyle(tStyleInfo);
var table = activeSheet.tables.add("table1", 1, 1, 5, 5, tableStyle);
```

___

### <a id="borderbottom" name="borderbottom"></a> borderBottom

• **borderBottom**: [`LineBorder`](GC.Spread.Sheets.LineBorder.md)

表格的下边框线

**`代码示例`**
``` javascript
//本示例创建了一个表
var tableStyle = new GC.Spread.Sheets.Tables.TableTheme();
var thinBorder = new GC.Spread.Sheets.LineBorder("black", GC.Spread.Sheets.LineStyle.dotted);
tableStyle.wholeTableStyle(new GC.Spread.Sheets.Tables.TableStyle("aliceblue", "green", "bold 10pt arial", thinBorder, thinBorder, thinBorder, thinBorder, thinBorder, thinBorder));
var tStyleInfo = new GC.Spread.Sheets.Tables.TableStyle();
tStyleInfo.backColor = "green";
tStyleInfo.foreColor = "red";
tStyleInfo.borderBottom = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.borderLeft = new GC.Spread.Sheets.LineBorder("yellow", GC.Spread.Sheets.LineStyle.medium);
tStyleInfo.borderTop = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.borderRight = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.font = "bold 11pt arial";
tableStyle.headerRowStyle(tStyleInfo);
var table = activeSheet.tables.add("table1", 1, 1, 5, 5, tableStyle);
```

___

### <a id="borderhorizontal" name="borderhorizontal"></a> borderHorizontal

• **borderHorizontal**: [`LineBorder`](GC.Spread.Sheets.LineBorder.md)

Indicates the horizontal border line of the table.

**`代码示例`**
``` javascript
//本示例设置borderHorizontal属性
var tableStyle = new GC.Spread.Sheets.Tables.TableTheme();
var thinBorder = new GC.Spread.Sheets.LineBorder("black", GC.Spread.Sheets.LineStyle.dotted);
tableStyle.wholeTableStyle(new GC.Spread.Sheets.Tables.TableStyle("aliceblue", "green", "bold 10pt arial", thinBorder, thinBorder, thinBorder, thinBorder, thinBorder, thinBorder));
var tStyleInfo = new GC.Spread.Sheets.Tables.TableStyle();
tStyleInfo.backColor = "green";
tStyleInfo.foreColor = "red";
tStyleInfo.borderHorizontal = new GC.Spread.Sheets.LineBorder("red", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.borderVertical = new GC.Spread.Sheets.LineBorder("blue", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.font = "bold 11pt arial";
tableStyle.firstRowStripStyle(tStyleInfo);
var table = activeSheet.tables.add("table1", 1, 1, 5, 5, tableStyle);
```

___

### <a id="borderleft" name="borderleft"></a> borderLeft

• **borderLeft**: [`LineBorder`](GC.Spread.Sheets.LineBorder.md)

表格的水平边框线

**`代码示例`**
``` javascript
//本示例创建了一个表
var tableStyle = new GC.Spread.Sheets.Tables.TableTheme();
var thinBorder = new GC.Spread.Sheets.LineBorder("black", GC.Spread.Sheets.LineStyle.dotted);
tableStyle.wholeTableStyle(new GC.Spread.Sheets.Tables.TableStyle("aliceblue", "green", "bold 10pt arial", thinBorder, thinBorder, thinBorder, thinBorder, thinBorder, thinBorder));
var tStyleInfo = new GC.Spread.Sheets.Tables.TableStyle();
tStyleInfo.backColor = "green";
tStyleInfo.foreColor = "red";
tStyleInfo.borderBottom = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.borderLeft = new GC.Spread.Sheets.LineBorder("yellow", GC.Spread.Sheets.LineStyle.medium);
tStyleInfo.borderTop = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.borderRight = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.font = "bold 11pt arial";
tableStyle.headerRowStyle(tStyleInfo);
var table = activeSheet.tables.add("table1", 1, 1, 5, 5, tableStyle);
```

___

### <a id="borderright" name="borderright"></a> borderRight

• **borderRight**: [`LineBorder`](GC.Spread.Sheets.LineBorder.md)

表格的右边框线

**`代码示例`**
``` javascript
//本示例创建了一个表
var tableStyle = new GC.Spread.Sheets.Tables.TableTheme();
var thinBorder = new GC.Spread.Sheets.LineBorder("black", GC.Spread.Sheets.LineStyle.dotted);
tableStyle.wholeTableStyle(new GC.Spread.Sheets.Tables.TableStyle("aliceblue", "green", "bold 10pt arial", thinBorder, thinBorder, thinBorder, thinBorder, thinBorder, thinBorder));
var tStyleInfo = new GC.Spread.Sheets.Tables.TableStyle();
tStyleInfo.backColor = "green";
tStyleInfo.foreColor = "red";
tStyleInfo.borderBottom = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.borderLeft = new GC.Spread.Sheets.LineBorder("yellow", GC.Spread.Sheets.LineStyle.medium);
tStyleInfo.borderTop = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.borderRight = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.font = "bold 11pt arial";
tableStyle.headerRowStyle(tStyleInfo);
var table = activeSheet.tables.add("table1", 1, 1, 5, 5, tableStyle);
```

___

### <a id="bordertop" name="bordertop"></a> borderTop

• **borderTop**: [`LineBorder`](GC.Spread.Sheets.LineBorder.md)

表格的上边框线

**`代码示例`**
``` javascript
//本示例创建了一个表
var tableStyle = new GC.Spread.Sheets.Tables.TableTheme();
var thinBorder = new GC.Spread.Sheets.LineBorder("black", GC.Spread.Sheets.LineStyle.dotted);
tableStyle.wholeTableStyle(new GC.Spread.Sheets.Tables.TableStyle("aliceblue", "green", "bold 10pt arial", thinBorder, thinBorder, thinBorder, thinBorder, thinBorder, thinBorder));
var tStyleInfo = new GC.Spread.Sheets.Tables.TableStyle();
tStyleInfo.backColor = "green";
tStyleInfo.foreColor = "red";
tStyleInfo.borderBottom = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.borderLeft = new GC.Spread.Sheets.LineBorder("yellow", GC.Spread.Sheets.LineStyle.medium);
tStyleInfo.borderTop = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.borderRight = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.font = "bold 11pt arial";
tableStyle.headerRowStyle(tStyleInfo);
var table = activeSheet.tables.add("table1", 1, 1, 5, 5, tableStyle);
```

___

### <a id="bordervertical" name="bordervertical"></a> borderVertical

• **borderVertical**: [`LineBorder`](GC.Spread.Sheets.LineBorder.md)

表格的垂直边框线

**`代码示例`**
``` javascript
//本示例设置borderHorizontal属性
var tableStyle = new GC.Spread.Sheets.Tables.TableTheme();
var thinBorder = new GC.Spread.Sheets.LineBorder("black", GC.Spread.Sheets.LineStyle.dotted);
tableStyle.wholeTableStyle(new GC.Spread.Sheets.Tables.TableStyle("aliceblue", "green", "bold 10pt arial", thinBorder, thinBorder, thinBorder, thinBorder, thinBorder, thinBorder));
var tStyleInfo = new GC.Spread.Sheets.Tables.TableStyle();
tStyleInfo.backColor = "green";
tStyleInfo.foreColor = "red";
tStyleInfo.borderHorizontal = new GC.Spread.Sheets.LineBorder("red", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.borderVertical = new GC.Spread.Sheets.LineBorder("blue", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.font = "bold 11pt arial";
tableStyle.firstRowStripStyle(tStyleInfo);
var table = activeSheet.tables.add("table1", 1, 1, 5, 5, tableStyle);
```

___

### <a id="font" name="font"></a> font

• **font**: `string`

字体

**`代码示例`**
``` javascript
//本示例创建了一个表
var tableStyle = new GC.Spread.Sheets.Tables.TableTheme();
var thinBorder = new GC.Spread.Sheets.LineBorder("black", GC.Spread.Sheets.LineStyle.dotted);
tableStyle.wholeTableStyle(new GC.Spread.Sheets.Tables.TableStyle("aliceblue", "green", "bold 10pt arial", thinBorder, thinBorder, thinBorder, thinBorder, thinBorder, thinBorder));
var tStyleInfo = new GC.Spread.Sheets.Tables.TableStyle();
tStyleInfo.backColor = "green";
tStyleInfo.foreColor = "red";
tStyleInfo.borderBottom = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.borderLeft = new GC.Spread.Sheets.LineBorder("yellow", GC.Spread.Sheets.LineStyle.medium);
tStyleInfo.borderTop = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.borderRight = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.font = "bold 11pt arial";
tableStyle.headerRowStyle(tStyleInfo);
var table = activeSheet.tables.add("table1", 1, 1, 5, 5, tableStyle);
```

___

### <a id="fontfamily" name="fontfamily"></a> fontFamily

• **fontFamily**: `string`

Indicates the font family.

**`example`**
```
//This example sets the fontFamily property.
var spread = new GC.Spread.Sheets.Workbook(document.getElementById('ss'));
var activeSheet = spread.getActiveSheet();
var tableStyle = new GC.Spread.Sheets.Tables.TableTheme();
var wholeTableStyle = new GC.Spread.Sheets.Tables.TableStyle();
wholeTableStyle.fontFamily = "Arial Black";
tableStyle.wholeTableStyle(wholeTableStyle);
var table = activeSheet.tables.add("table1", 1, 1, 5, 5, tableStyle);
```

___

### <a id="fontsize" name="fontsize"></a> fontSize

• **fontSize**: `string`

Indicates the font size.

**`example`**
```
//This example sets the fontSize property.
var spread = new GC.Spread.Sheets.Workbook(document.getElementById('ss'));
var activeSheet = spread.getActiveSheet();
var tableStyle = new GC.Spread.Sheets.Tables.TableTheme();
var wholeTableStyle = new GC.Spread.Sheets.Tables.TableStyle();
wholeTableStyle.fontSize = "16px";
tableStyle.wholeTableStyle(wholeTableStyle);
var table = activeSheet.tables.add("table1", 1, 1, 5, 5, tableStyle);
```

___

### <a id="fontstyle" name="fontstyle"></a> fontStyle

• **fontStyle**: `string`

Indicates the font style.

**`example`**
```
//This example sets the fontStyle property.
var spread = new GC.Spread.Sheets.Workbook(document.getElementById('ss'));
var activeSheet = spread.getActiveSheet();
var tableStyle = new GC.Spread.Sheets.Tables.TableTheme();
var wholeTableStyle = new GC.Spread.Sheets.Tables.TableStyle();
wholeTableStyle.fontStyle = "italic";
tableStyle.wholeTableStyle(wholeTableStyle);
var table = activeSheet.tables.add("table1", 1, 1, 5, 5, tableStyle);
```

___

### <a id="fontweight" name="fontweight"></a> fontWeight

• **fontWeight**: `string`

Indicates the font weight.

**`example`**
```
//This example sets the fontWeight property.
var spread = new GC.Spread.Sheets.Workbook(document.getElementById('ss'));
var activeSheet = spread.getActiveSheet();
var tableStyle = new GC.Spread.Sheets.Tables.TableTheme();
var wholeTableStyle = new GC.Spread.Sheets.Tables.TableStyle();
wholeTableStyle.fontWeight = "bold";
tableStyle.wholeTableStyle(wholeTableStyle);
var table = activeSheet.tables.add("table1", 1, 1, 5, 5, tableStyle);
```

___

### <a id="forecolor" name="forecolor"></a> foreColor

• **foreColor**: `string`

前景色

**`代码示例`**
``` javascript
//本示例设置borderHorizontal属性
var tableStyle = new GC.Spread.Sheets.Tables.TableTheme();
var thinBorder = new GC.Spread.Sheets.LineBorder("black", GC.Spread.Sheets.LineStyle.dotted);
tableStyle.wholeTableStyle(new GC.Spread.Sheets.Tables.TableStyle("aliceblue", "green", "bold 10pt arial", thinBorder, thinBorder, thinBorder, thinBorder, thinBorder, thinBorder));
var tStyleInfo = new GC.Spread.Sheets.Tables.TableStyle();
tStyleInfo.backColor = "green";
tStyleInfo.foreColor = "red";
tStyleInfo.borderHorizontal = new GC.Spread.Sheets.LineBorder("red", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.borderVertical = new GC.Spread.Sheets.LineBorder("blue", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.font = "bold 11pt arial";
tableStyle.firstRowStripStyle(tStyleInfo);
var table = activeSheet.tables.add("table1", 1, 1, 5, 5, tableStyle);
```

___

### <a id="textdecoration" name="textdecoration"></a> textDecoration

• **textDecoration**: [`TextDecorationType`](../enums/GC.Spread.Sheets.TextDecorationType.md)

文本修饰
**`example`**
```
//This example sets the textDecoration property.
var tableStyle = new GC.Spread.Sheets.Tables.TableTheme();
var thinBorder = new GC.Spread.Sheets.LineBorder("black", GC.Spread.Sheets.LineStyle.dotted);
tableStyle.wholeTableStyle(new GC.Spread.Sheets.Tables.TableStyle("aliceblue", "green", "bold 10pt arial", thinBorder, thinBorder, thinBorder, thinBorder, thinBorder, thinBorder));
var tStyleInfo = new GC.Spread.Sheets.Tables.TableStyle();
tStyleInfo.backColor = "green";
tStyleInfo.foreColor = "red";
tStyleInfo.font = "bold 11pt arial";
tStyleInfo.textDecoration = GC.Spread.Sheets.TextDecorationType.doubleUnderline;
tableStyle.firstRowStripStyle(tStyleInfo);
var table = activeSheet.tables.add("table1", 1, 1, 5, 5, tableStyle);
```
