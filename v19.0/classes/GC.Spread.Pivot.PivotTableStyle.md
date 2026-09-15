# Class: PivotTableStyle

[Spread](../modules/GC.Spread.md).[Pivot](../modules/GC.Spread.Pivot.md).PivotTableStyle

## Table of contents

### Constructors

- [constructor](GC.Spread.Pivot.PivotTableStyle.md#constructor)

### Properties

- [backColor](GC.Spread.Pivot.PivotTableStyle.md#backcolor)
- [borderBottom](GC.Spread.Pivot.PivotTableStyle.md#borderbottom)
- [borderHorizontal](GC.Spread.Pivot.PivotTableStyle.md#borderhorizontal)
- [borderLeft](GC.Spread.Pivot.PivotTableStyle.md#borderleft)
- [borderRight](GC.Spread.Pivot.PivotTableStyle.md#borderright)
- [borderTop](GC.Spread.Pivot.PivotTableStyle.md#bordertop)
- [borderVertical](GC.Spread.Pivot.PivotTableStyle.md#bordervertical)
- [font](GC.Spread.Pivot.PivotTableStyle.md#font)
- [fontFamily](GC.Spread.Pivot.PivotTableStyle.md#fontfamily)
- [fontSize](GC.Spread.Pivot.PivotTableStyle.md#fontsize)
- [fontStyle](GC.Spread.Pivot.PivotTableStyle.md#fontstyle)
- [fontWeight](GC.Spread.Pivot.PivotTableStyle.md#fontweight)
- [foreColor](GC.Spread.Pivot.PivotTableStyle.md#forecolor)
- [textDecoration](GC.Spread.Pivot.PivotTableStyle.md#textdecoration)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new PivotTableStyle**(`backColor?`, `foreColor?`, `font?`, `borderLeft?`, `borderTop?`, `borderRight?`, `borderBottom?`, `borderHorizontal?`, `borderVertical?`, `textDecoration?`, `fontStyle?`, `fontWeight?`, `fontSize?`, `fontFamily?`)

表示数据透视表样式。

#### Parameters

| Name | Type |
| :------ | :------ |
| `backColor?` | `string` |
| `foreColor?` | `string` |
| `font?` | `string` |
| `borderLeft?` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) |
| `borderTop?` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) |
| `borderRight?` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) |
| `borderBottom?` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) |
| `borderHorizontal?` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) |
| `borderVertical?` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) |
| `textDecoration?` | [`TextDecorationType`](../enums/GC.Spread.Sheets.TextDecorationType.md) |
| `fontStyle?` | `string` |
| `fontWeight?` | `string` |
| `fontSize?` | `string` |
| `fontFamily?` | `string` |

## Properties

### <a id="backcolor" name="backcolor"></a> backColor

• **backColor**: `string`

指示背景颜色。

___

### <a id="borderbottom" name="borderbottom"></a> borderBottom

• **borderBottom**: [`LineBorder`](GC.Spread.Sheets.LineBorder.md)

指示下边框。

___

### <a id="borderhorizontal" name="borderhorizontal"></a> borderHorizontal

• **borderHorizontal**: [`LineBorder`](GC.Spread.Sheets.LineBorder.md)

指示水平边框。

___

### <a id="borderleft" name="borderleft"></a> borderLeft

• **borderLeft**: [`LineBorder`](GC.Spread.Sheets.LineBorder.md)

指示左边框。

___

### <a id="borderright" name="borderright"></a> borderRight

• **borderRight**: [`LineBorder`](GC.Spread.Sheets.LineBorder.md)

指示右边框。

___

### <a id="bordertop" name="bordertop"></a> borderTop

• **borderTop**: [`LineBorder`](GC.Spread.Sheets.LineBorder.md)

指示上边框。

___

### <a id="bordervertical" name="bordervertical"></a> borderVertical

• **borderVertical**: [`LineBorder`](GC.Spread.Sheets.LineBorder.md)

指示垂直边框。

___

### <a id="font" name="font"></a> font

• **font**: `string`

指示字体。

___

### <a id="fontfamily" name="fontfamily"></a> fontFamily

• **fontFamily**: `string`

指示字体族。

**`example`**
```javascript
// 此示例设置fontFamily属性。
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var wholePivotTableStyle = new GC.Spread.Pivot.PivotTableStyle();
wholePivotTableStyle.fontFamily = "Arial Black";
theme.wholeTableStyle(wholePivotTableStyle);
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme);
```

___

### <a id="fontsize" name="fontsize"></a> fontSize

• **fontSize**: `string`

指示字体大小。

**`example`**
```javascript
// 此示例设置fontSize属性。
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var wholePivotTableStyle = new GC.Spread.Pivot.PivotTableStyle();
wholePivotTableStyle.fontSize = "16px";
theme.wholeTableStyle(wholePivotTableStyle);
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme);
```

___

### <a id="fontstyle" name="fontstyle"></a> fontStyle

• **fontStyle**: `string`

指示字体样式。

**`example`**
```javascript
// 此示例设置fontStyle属性。
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var wholePivotTableStyle = new GC.Spread.Pivot.PivotTableStyle();
wholePivotTableStyle.fontStyle = "italic";
theme.wholeTableStyle(wholePivotTableStyle);
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme);
```

___

### <a id="fontweight" name="fontweight"></a> fontWeight

• **fontWeight**: `string`

指示字体粗细。

**`example`**
```javascript
// 此示例设置fontWeight属性。
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var wholePivotTableStyle = new GC.Spread.Pivot.PivotTableStyle();
wholePivotTableStyle.fontWeight = "bold";
theme.wholeTableStyle(wholePivotTableStyle);
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme);
```

___

### <a id="forecolor" name="forecolor"></a> foreColor

• **foreColor**: `string`

指示前景色。

___

### <a id="textdecoration" name="textdecoration"></a> textDecoration

• **textDecoration**: [`TextDecorationType`](../enums/GC.Spread.Sheets.TextDecorationType.md)

指示文本装饰。
