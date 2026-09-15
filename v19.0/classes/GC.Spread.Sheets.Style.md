# Class: Style

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).Style

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Style.md#constructor)

### Properties

- [allowEditInCell](GC.Spread.Sheets.Style.md#alloweditincell)
- [applyAlignment](GC.Spread.Sheets.Style.md#applyalignment)
- [applyBorder](GC.Spread.Sheets.Style.md#applyborder)
- [applyFill](GC.Spread.Sheets.Style.md#applyfill)
- [applyFont](GC.Spread.Sheets.Style.md#applyfont)
- [applyNumberFormat](GC.Spread.Sheets.Style.md#applynumberformat)
- [applyProtection](GC.Spread.Sheets.Style.md#applyprotection)
- [backColor](GC.Spread.Sheets.Style.md#backcolor)
- [backgroundImage](GC.Spread.Sheets.Style.md#backgroundimage)
- [backgroundImageLayout](GC.Spread.Sheets.Style.md#backgroundimagelayout)
- [borderBottom](GC.Spread.Sheets.Style.md#borderbottom)
- [borderLeft](GC.Spread.Sheets.Style.md#borderleft)
- [borderRight](GC.Spread.Sheets.Style.md#borderright)
- [borderTop](GC.Spread.Sheets.Style.md#bordertop)
- [cellButtons](GC.Spread.Sheets.Style.md#cellbuttons)
- [cellPadding](GC.Spread.Sheets.Style.md#cellpadding)
- [cellType](GC.Spread.Sheets.Style.md#celltype)
- [decoration](GC.Spread.Sheets.Style.md#decoration)
- [diagonalDown](GC.Spread.Sheets.Style.md#diagonaldown)
- [diagonalUp](GC.Spread.Sheets.Style.md#diagonalup)
- [dropDowns](GC.Spread.Sheets.Style.md#dropdowns)
- [font](GC.Spread.Sheets.Style.md#font)
- [fontFamily](GC.Spread.Sheets.Style.md#fontfamily)
- [fontSize](GC.Spread.Sheets.Style.md#fontsize)
- [fontStyle](GC.Spread.Sheets.Style.md#fontstyle)
- [fontWeight](GC.Spread.Sheets.Style.md#fontweight)
- [foreColor](GC.Spread.Sheets.Style.md#forecolor)
- [formatter](GC.Spread.Sheets.Style.md#formatter)
- [hAlign](GC.Spread.Sheets.Style.md#halign)
- [hidden](GC.Spread.Sheets.Style.md#hidden)
- [imeMode](GC.Spread.Sheets.Style.md#imemode)
- [isVerticalText](GC.Spread.Sheets.Style.md#isverticaltext)
- [labelOptions](GC.Spread.Sheets.Style.md#labeloptions)
- [locked](GC.Spread.Sheets.Style.md#locked)
- [mask](GC.Spread.Sheets.Style.md#mask)
- [name](GC.Spread.Sheets.Style.md#name)
- [parentName](GC.Spread.Sheets.Style.md#parentname)
- [showEllipsis](GC.Spread.Sheets.Style.md#showellipsis)
- [shrinkToFit](GC.Spread.Sheets.Style.md#shrinktofit)
- [tabStop](GC.Spread.Sheets.Style.md#tabstop)
- [textDecoration](GC.Spread.Sheets.Style.md#textdecoration)
- [textDirection](GC.Spread.Sheets.Style.md#textdirection)
- [textIndent](GC.Spread.Sheets.Style.md#textindent)
- [textOrientation](GC.Spread.Sheets.Style.md#textorientation)
- [themeFont](GC.Spread.Sheets.Style.md#themefont)
- [vAlign](GC.Spread.Sheets.Style.md#valign)
- [watermark](GC.Spread.Sheets.Style.md#watermark)
- [wordWrap](GC.Spread.Sheets.Style.md#wordwrap)

### Methods

- [clone](GC.Spread.Sheets.Style.md#clone)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Style**(`backColor?`, `foreColor?`, `hAlign?`, `vAlign?`, `font?`, `themeFont?`, `formatter?`, `borderLeft?`, `borderTop?`, `borderRight?`, `borderBottom?`, `locked?`, `textIndent?`, `wordWrap?`, `showEllipsis?`, `shrinkToFit?`, `backgroundImage?`, `cellType?`, `backgroundImageLayout?`, `tabStop?`, `textDecoration?`, `imeMode?`, `name?`, `parentName?`, `watermark?`, `cellPadding?`, `labelOptions?`, `quotePrefix?`, `diagonalDown?`, `diagonalUp?`, `isVerticalText?`, `cellButtons?`, `dropdown?`, `textOrientation?`, `decoration?`, `mask?`, `fontStyle?`, `fontWeight?`, `fontSize?`, `fontFamily?`, `hidden?`, `textDirection?`)

表示单元格、行和列的样式。

**`example`**
```
//此示例使用带规则的样式。
activeSheet.setArray(0,0,[1,2,3,4,5,6,7,8,9,10]);
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
style.foreColor = "black";
var cell = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
cell.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.cellValueRule);
cell.operator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.greaterThan);
cell.value1(5);
cell.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 1)]);
cell.style(style);
activeSheet.conditionalFormats.addRule(cell);
var style1 = new GC.Spread.Sheets.Style();
style1.foreColor = "red";
var top = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
top.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.top10Rule);
top.type(GC.Spread.Sheets.ConditionalFormatting.Top10ConditionType.top);
top.rank(3);
top.style(style1);
top.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 1)]);
top.stopIfTrue(true);
activeSheet.conditionalFormats.addRule(top);
```

**`example`**
```
//此示例创建并设置样式参数。
sheet.setValue(0,0, 1,3);
sheet.setValue(1,0, 50,3);
sheet.setValue(2,0, 100,3);
sheet.setValue(3,0, 2,3);
sheet.setValue(4,0, 60,3);
sheet.setValue(5,0, 90,3);
sheet.setValue(6,0, 3,3);
sheet.setValue(7,0, 40,3);
sheet.setValue(8,0, 70,3);
sheet.setValue(9,0, 5,3);
sheet.setValue(10,0, 35,3);
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
style.borderLeft =new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderTop = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderRight = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderBottom =  new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
sheet.conditionalFormats.addAverageRule(GC.Spread.Sheets.ConditionalFormatting.AverageConditionType.above, style, [new GC.Spread.Sheets.Range(0, 0, 10, 3)]);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `backColor?` | `string` \| [`IGradientFill`](../interfaces/GC.Spread.Sheets.IGradientFill.md) \| [`IGradientPathFill`](../interfaces/GC.Spread.Sheets.IGradientPathFill.md) \| [`IPatternFill`](../interfaces/GC.Spread.Sheets.IPatternFill.md) |
| `foreColor?` | `string` |
| `hAlign?` | [`HorizontalAlign`](../enums/GC.Spread.Sheets.HorizontalAlign.md) |
| `vAlign?` | [`VerticalAlign`](../enums/GC.Spread.Sheets.VerticalAlign.md) |
| `font?` | `string` |
| `themeFont?` | `string` |
| `formatter?` | `string` \| [`GeneralFormatter`](GC.Spread.Formatter.GeneralFormatter.md) |
| `borderLeft?` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) |
| `borderTop?` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) |
| `borderRight?` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) |
| `borderBottom?` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) |
| `locked?` | `boolean` |
| `textIndent?` | `number` |
| `wordWrap?` | `boolean` |
| `showEllipsis?` | `boolean` |
| `shrinkToFit?` | `boolean` |
| `backgroundImage?` | `string` |
| `cellType?` | [`Base`](GC.Spread.Sheets.CellTypes.Base.md) |
| `backgroundImageLayout?` | [`ImageLayout`](../enums/GC.Spread.Sheets.ImageLayout.md) |
| `tabStop?` | `boolean` |
| `textDecoration?` | [`TextDecorationType`](../enums/GC.Spread.Sheets.TextDecorationType.md) |
| `imeMode?` | [`ImeMode`](../enums/GC.Spread.Sheets.ImeMode.md) |
| `name?` | `string` |
| `parentName?` | `string` |
| `watermark?` | `string` |
| `cellPadding?` | `string` |
| `labelOptions?` | [`ILabelOptions`](../interfaces/GC.Spread.Sheets.ILabelOptions.md) |
| `quotePrefix?` | `boolean` |
| `diagonalDown?` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) |
| `diagonalUp?` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) |
| `isVerticalText?` | `boolean` |
| `cellButtons?` | [`ICellButton`](../interfaces/GC.Spread.Sheets.ICellButton.md)[] |
| `dropdown?` | [`IDropdown`](../interfaces/GC.Spread.Sheets.IDropdown.md)[] |
| `textOrientation?` | `number` |
| `decoration?` | [`TextDecorationType`](../enums/GC.Spread.Sheets.TextDecorationType.md) |
| `mask?` | [`IMaskType`](../interfaces/GC.Spread.Sheets.IMaskType.md) |
| `fontStyle?` | `string` |
| `fontWeight?` | `string` |
| `fontSize?` | `string` |
| `fontFamily?` | `string` |
| `hidden?` | `boolean` |
| `textDirection?` | [`TextDirectionType`](../enums/GC.Spread.Sheets.TextDirectionType.md) |

## Properties

### <a id="alloweditincell" name="alloweditincell"></a> allowEditInCell

• **allowEditInCell**: `undefined` \| `boolean`

指示单元格是否可以进入编辑模式进行编辑。

**`example`**
```
//此示例设置allowEditInCell属性。
var style = activeSheet.getStyle(1,1,GC.Spread.Sheets.SheetArea.viewport);
style.allowEditInCell = false;
```

___

### <a id="applyalignment" name="applyalignment"></a> applyAlignment

• **applyAlignment**: `boolean`

仅适用于命名样式，布尔值指示是否应用对齐格式。

**`example`**
```
//此示例为命名样式设置applyAlignment属性。
var style = new GC.Spread.Sheets.Style();
style.name = 'test';
style.applyAlignment = false;
spread.addNamedStyle(style);
```

___

### <a id="applyborder" name="applyborder"></a> applyBorder

• **applyBorder**: `boolean`

仅适用于命名样式，布尔值指示是否应用边框格式。

**`example`**
```
//此示例为命名样式设置applyBorder属性。
var style = new GC.Spread.Sheets.Style();
style.name = 'test';
style.applyBorder = false;
spread.addNamedStyle(style);
```

___

### <a id="applyfill" name="applyfill"></a> applyFill

• **applyFill**: `boolean`

仅适用于命名样式，布尔值指示是否应用填充格式。

**`example`**
```
//此示例为命名样式设置applyFill属性。
var style = new GC.Spread.Sheets.Style();
style.name = 'test';
style.applyFill = false;
spread.addNamedStyle(style);
```

___

### <a id="applyfont" name="applyfont"></a> applyFont

• **applyFont**: `boolean`

仅适用于命名样式，布尔值指示是否应用字体格式。

**`example`**
```
//此示例为命名样式设置applyFont属性。
var style = new GC.Spread.Sheets.Style();
style.name = 'test';
style.applyFont = false;
spread.addNamedStyle(style);
```

___

### <a id="applynumberformat" name="applynumberformat"></a> applyNumberFormat

• **applyNumberFormat**: `boolean`

仅适用于命名样式，布尔值指示是否应用数字格式。

**`example`**
```
//此示例为命名样式设置applyNumberFormat属性。
var style = new GC.Spread.Sheets.Style();
style.name = 'test';
style.applyNumberFormat = false;
spread.addNamedStyle(style);
```

___

### <a id="applyprotection" name="applyprotection"></a> applyProtection

• **applyProtection**: `boolean`

仅适用于命名样式，布尔值指示是否应用保护格式。

**`example`**
```
//此示例为命名样式设置applyProtection属性。
var style = new GC.Spread.Sheets.Style();
style.name = 'test';
style.applyProtection = false;
spread.addNamedStyle(style);
```

___

### <a id="backcolor" name="backcolor"></a> backColor

• **backColor**: `undefined` \| `string` \| [`IGradientFill`](../interfaces/GC.Spread.Sheets.IGradientFill.md) \| [`IGradientPathFill`](../interfaces/GC.Spread.Sheets.IGradientPathFill.md) \| [`IPatternFill`](../interfaces/GC.Spread.Sheets.IPatternFill.md)

指示背景颜色。

**`example`**
```
//此示例设置样式backColor属性。
activeSheet.setArray(0,0,[1,2,3,4,5,6,7,8,9,10]);
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
style.foreColor = "black";
var cell = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
cell.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.cellValueRule);
cell.operator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.greaterThan);
cell.value1(5);
cell.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 1)]);
cell.style(style);
activeSheet.conditionalFormats.addRule(cell);
var style1 = new GC.Spread.Sheets.Style();
style1.foreColor = "red";
var top = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
top.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.top10Rule);
top.type(GC.Spread.Sheets.ConditionalFormatting.Top10ConditionType.top);
top.rank(3);
top.style(style1);
top.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 1)]);
top.stopIfTrue(true);
activeSheet.conditionalFormats.addRule(top);
```

___

### <a id="backgroundimage" name="backgroundimage"></a> backgroundImage

• **backgroundImage**: `undefined` \| `string`

指示背景图片。

**`example`**
```
//此示例设置backgroundImage属性。
var style = new GC.Spread.Sheets.Style();
style.backColor = "lightgreen";
style.backgroundImage = "./css/images/quarter1.png";
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
```

___

### <a id="backgroundimagelayout" name="backgroundimagelayout"></a> backgroundImageLayout

• **backgroundImageLayout**: `undefined` \| [`ImageLayout`](../enums/GC.Spread.Sheets.ImageLayout.md)

指示背景图片布局。

**`example`**
```
//此示例设置backgroundImageLayout属性。
var style = new GC.Spread.Sheets.Style();
style.backColor = "lightgreen";
style.backgroundImage = "./css/images/quarter1.png";
style.backgroundImageLayout  = GC.Spread.Sheets.ImageLayout.center;
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
```

___

### <a id="borderbottom" name="borderbottom"></a> borderBottom

• **borderBottom**: `undefined` \| [`LineBorder`](GC.Spread.Sheets.LineBorder.md)

指示底部边框线。

**`example`**
```
//此示例创建边框。
var cellType = new GC.Spread.Sheets.CellTypes.Button();
cellType.buttonBackColor("#FFFF00");
cellType.text("this is a button");
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
style.borderLeft =new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderTop = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderRight = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderBottom = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.cellType = cellType
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
```

___

### <a id="borderleft" name="borderleft"></a> borderLeft

• **borderLeft**: `undefined` \| [`LineBorder`](GC.Spread.Sheets.LineBorder.md)

指示左侧边框线。

**`example`**
```
//此示例创建边框。
var cellType = new GC.Spread.Sheets.CellTypes.Button();
cellType.buttonBackColor("#FFFF00");
cellType.text("this is a button");
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
style.borderLeft =new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderTop = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderRight = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderBottom = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.cellType = cellType
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
```

___

### <a id="borderright" name="borderright"></a> borderRight

• **borderRight**: `undefined` \| [`LineBorder`](GC.Spread.Sheets.LineBorder.md)

指示右侧边框线。

**`example`**
```
//此示例创建边框。
var cellType = new GC.Spread.Sheets.CellTypes.Button();
cellType.buttonBackColor("#FFFF00");
cellType.text("this is a button");
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
style.borderLeft =new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderTop = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderRight = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderBottom = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.cellType = cellType
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
```

___

### <a id="bordertop" name="bordertop"></a> borderTop

• **borderTop**: `undefined` \| [`LineBorder`](GC.Spread.Sheets.LineBorder.md)

指示顶部边框线。

**`example`**
```
//此示例创建边框。
var cellType = new GC.Spread.Sheets.CellTypes.Button();
cellType.buttonBackColor("#FFFF00");
cellType.text("this is a button");
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
style.borderLeft =new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderTop = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderRight = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderBottom = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.cellType = cellType
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
```

___

### <a id="cellbuttons" name="cellbuttons"></a> cellButtons

• **cellButtons**: `undefined` \| [`ICellButton`](../interfaces/GC.Spread.Sheets.ICellButton.md)[]

指示单元格的按钮。

**`property`** {string} [caption] - 指定按钮显示的文本

**`property`** {GC.Spread.Sheets.CaptionAlignment} [captionAlign] - 指定图像和标题的位置

**`property`** {GC.Spread.Sheets.ButtonPosition} [position] - 指定按钮在单元格中的位置

**`property`** {boolean} [enabled] - 指定单元格按钮是否响应用户操作，默认值为true

**`property`** {boolean} [useButtonStyle] - 指定单元格按钮是否为按钮样式，默认值为false

**`property`** {number} [width] - 指定按钮的宽度。如果设置为null或undefined，按钮宽度将根据标题和图像大小自动调整

**`property`** {GC.Spread.Sheets.ButtonVisibility} [visibility] - 指定按钮的可见性：始终可见、选中时可见、编辑时可见，默认值为始终可见

**`property`** {string | function} [command] - 点击按钮时，允许用户执行spread命令或执行回调函数

**`property`** {GC.Spread.Sheets.ButtonImageType} [imageType] - 指定按钮的类型（按钮中显示的图像类型）。为cellButton提供一些预定义类型，custom允许指定图标

**`property`** {string} [imageSrc] - 当imageType为custom时，可以通过imageSrc指定图像（base64）

**`property`** {GC.Spread.Sheets.IImageSize} [imageSize] - 指定图像的大小，默认值为16px

**`property`** {string} [hoverBackColor] - 指定按钮可见且启用时单元格按钮的悬停背景色

**`property`** {string} [buttonBackColor] - 指定按钮启用时单元格按钮的背景色

**`example`**
```
buttonConfig1 = {
    caption: "left",
    enabled: true,
    buttonBackColor: "#174EA6",
    visibility:GC.Spread.Sheets.ButtonVisibility.always,
};
buttonConfig2 = {
    caption: "left",
    enabled: true,
    hoverBackColor: "#3390FF",
    visibility:GC.Spread.Sheets.ButtonVisibility.onSelected,
};
buttonConfig3 = {
    caption: "Cut",
    imageType: GC.Spread.Sheets.ButtonImageType.custom,
    useButtonStyle: true,
    imageSrc:"data:image/svg+xml;base64,PD94bWwgdmVyc2lvb...", //这不是完整的base64字符串
};
//创建样式
var style = new GC.Spread.Sheets.Style();
style.cellButtons=[
     buttonConfig1,
     buttonConfig2,
     buttonConfig3
];
sheet.setStyle(0, 0, style);
```

___

### <a id="cellpadding" name="cellpadding"></a> cellPadding

• **cellPadding**: `undefined` \| `string`

指示单元格内边距。

**`example`**
```
//此示例设置水印的单元格内边距。
var type = new GC.Spread.Sheets.Style();
type.watermark = "User name";
type.cellPadding = "20";
type.labelOptions = {alignment:GC.Spread.Sheets.LabelAlignment.topLeft, visibility: GC.Spread.Sheets.LabelVisibility.visible};
activeSheet.setStyle(0, 1, type);
activeSheet.getRange(0, -1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).height(60);
activeSheet.getRange(-1, 1, -1, 1).width(150);
var combo = new GC.Spread.Sheets.CellTypes.ComboBox();
combo.items([{ text: "Oranges", value: "11k" }, { text: "Apples", value: "15k" }, { text: "Grape", value: "100k" }]);
combo.editorValueType(GC.Spread.Sheets.CellTypes.EditorValueType.text);
activeSheet.setCellType(2, 1, combo, GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(2, 1, GC.Spread.Sheets.SheetArea.viewport).watermark("ComboBox Cell Type").cellPadding('10 10 20 10');
activeSheet.getCell(2, 1, GC.Spread.Sheets.SheetArea.viewport).labelOptions({alignment: GC.Spread.Sheets.LabelAlignment.bottomCenter, foreColor: 'yellowgreen', font: 'bold 15px Arial'});
activeSheet.getRange(2, -1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).height(60);
```

___

### <a id="celltype" name="celltype"></a> cellType

• **cellType**: `undefined` \| [`Base`](GC.Spread.Sheets.CellTypes.Base.md)

指示单元格类型。

**`example`**
```
//此示例创建样式并将其应用于单元格。
var cellType = new GC.Spread.Sheets.CellTypes.Button();
cellType.buttonBackColor("#FFFF00");
cellType.text("this is a button");
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
style.borderLeft =new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderTop = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderRight = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderBottom = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.cellType = cellType
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
```

___

### <a id="decoration" name="decoration"></a> decoration

• **decoration**: [`IDecoration`](../interfaces/GC.Spread.Sheets.IDecoration.md)

定义单元格装饰器以更好地表示单元格。

**`example`**
```
//此示例设置Style的decoration属性。
var style = new GC.Spread.Sheets.Style();
style.decoration = {
    cornerFold: {
       size: 6,
       position: GC.Spread.Sheets.CornerPosition.leftTop,
       color: "red"
    },
    icons: [
         {
             src: './icon.png',
             width: 12,
             height: 12,
             position: GC.Spread.Sheets.IconPosition.left,
         }
    ]
}
```

___

### <a id="diagonaldown" name="diagonaldown"></a> diagonalDown

• **diagonalDown**: `undefined` \| [`LineBorder`](GC.Spread.Sheets.LineBorder.md)

指示对角线向下边框线。

**`example`**
```
activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).diagonalDown(new GC.Spread.Sheets.LineBorder("blue", GC.Spread.Sheets.LineStyle.mediumDashed));
```

___

### <a id="diagonalup" name="diagonalup"></a> diagonalUp

• **diagonalUp**: `undefined` \| [`LineBorder`](GC.Spread.Sheets.LineBorder.md)

指示对角线向上边框线。

**`example`**
```
activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).diagonalUp(new GC.Spread.Sheets.LineBorder("blue", GC.Spread.Sheets.LineStyle.mediumDashed));
```

___

### <a id="dropdowns" name="dropdowns"></a> dropDowns

• **dropDowns**: `undefined` \| [`IDropdown`](../interfaces/GC.Spread.Sheets.IDropdown.md)[]

指示单元格的下拉类型。

**`example`**
```
leftButtonConfig1 = {
    caption: "left",
    enabled: true,
    isLeft: true,
    visibility:GC.Spread.Sheets.ButtonVisibility.always,
    command: "opendropdown"
}
//创建样式
var style = new GC.Spread.Sheets.Style();
style.cellButtons=[
     leftButtonConfig1
];
style.dropDowns= [{ type: "colorPicker" }];
sheet.setStyle(0, 0, style);
```

___

### <a id="font" name="font"></a> font

• **font**: `undefined` \| `string`

指示字体。

**`example`**
```
//此示例设置font属性。
var style = new GC.Spread.Sheets.Style();
style.font = "8pt Arial";
style.hAlign = GC.Spread.Sheets.HorizontalAlign.center;
style.vAlign = GC.Spread.Sheets.VerticalAlign.center;
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(1,1).value("B2");
```

___

### <a id="fontfamily" name="fontfamily"></a> fontFamily

• **fontFamily**: `undefined` \| `string`

指示字体系列。

**`example`**
```
//此示例设置fontFamily属性。
var style = new GC.Spread.Sheets.Style();
style.fontFamily = "Arial";
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(1,1).value("B2");
```

___

### <a id="fontsize" name="fontsize"></a> fontSize

• **fontSize**: `undefined` \| `string`

指示字体大小。

**`example`**
```
//此示例设置fontSize属性。
var style = new GC.Spread.Sheets.Style();
style.fontSize = "22px";
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(1,1).value("B2");
```

___

### <a id="fontstyle" name="fontstyle"></a> fontStyle

• **fontStyle**: `undefined` \| `string`

指示字体样式。

**`example`**
```
//此示例设置fontStyle属性。
var style = new GC.Spread.Sheets.Style();
style.fontStyle = "italic";
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(1,1).value("B2");
```

___

### <a id="fontweight" name="fontweight"></a> fontWeight

• **fontWeight**: `undefined` \| `string`

指示字体粗细。

**`example`**
```
//此示例设置fontWeight属性。
var style = new GC.Spread.Sheets.Style();
style.fontWeight = "bold";
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(1,1).value("B2");
```

___

### <a id="forecolor" name="forecolor"></a> foreColor

• **foreColor**: `undefined` \| `string`

指示前景色。

**`example`**
```
//此示例设置foreColor属性。
activeSheet.setArray(0,0,[1,2,3,4,5,6,7,8,9,10]);
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
style.foreColor = "black";
var cell = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
cell.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.cellValueRule);
cell.operator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.greaterThan);
cell.value1(5);
cell.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 1)]);
cell.style(style);
activeSheet.conditionalFormats.addRule(cell);
var style1 = new GC.Spread.Sheets.Style();
style1.foreColor = "red";
var top = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
top.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.top10Rule);
top.type(GC.Spread.Sheets.ConditionalFormatting.Top10ConditionType.top);
top.rank(3);
top.style(style1);
top.ranges([new GC.Spread.Sheets.Range(0, 0, 10, 1)]);
top.stopIfTrue(true);
activeSheet.conditionalFormats.addRule(top);
```

___

### <a id="formatter" name="formatter"></a> formatter

• **formatter**: `undefined` \| `string` \| [`GeneralFormatter`](GC.Spread.Formatter.GeneralFormatter.md)

指示格式化程序。

**`example`**
```
//此示例使用formatter属性。
var style = new GC.Spread.Sheets.Style();
style.formatter = "0.000%";
style.themeFont = "Body";
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(1,1).value("11");
```

___

### <a id="halign" name="halign"></a> hAlign

• **hAlign**: `undefined` \| [`HorizontalAlign`](../enums/GC.Spread.Sheets.HorizontalAlign.md)

指示水平对齐。

**`example`**
```
//此示例设置hAlign属性。
var style = new GC.Spread.Sheets.Style();
style.font = "8pt Arial";
style.hAlign = GC.Spread.Sheets.HorizontalAlign.center;
style.vAlign = GC.Spread.Sheets.VerticalAlign.center;
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(1,1).value("B2");
```

___

### <a id="hidden" name="hidden"></a> hidden

• **hidden**: `undefined` \| `boolean`

指示单元格公式是否在受保护的工作表中可见。

**`example`**
```
//此示例隐藏单个单元格。
activeSheet.options.isProtected = true;
activeSheet.setValue(1, 1, "=SUM(1,2)");
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
style.borderLeft =new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderTop = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderRight = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderBottom = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.hidden = true;
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
```

___

### <a id="imemode" name="imemode"></a> imeMode

• **imeMode**: `undefined` \| [`ImeMode`](../enums/GC.Spread.Sheets.ImeMode.md)

指示输入法编辑器（IME）模式。

**`deprecated`** 此属性当前仅在Internet Explorer中有效。

**`example`**
```
//此示例设置IME模式。
var style = new GC.Spread.Sheets.Style();
style.imeMode = GC.Spread.Sheets.ImeMode.auto;
activeSheet.setStyle(0, 0, style);
```

___

### <a id="isverticaltext" name="isverticaltext"></a> isVerticalText

• **isVerticalText**: `undefined` \| `boolean`

指示是否设置文本垂直。

**`example`**
```
//此示例使用rotate属性。
var style = new GC.Spread.Sheets.Style();
style.isVerticalText = true;
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
```

___

### <a id="labeloptions" name="labeloptions"></a> labelOptions

• **labelOptions**: `undefined` \| [`ILabelOptions`](../interfaces/GC.Spread.Sheets.ILabelOptions.md)

指示单元格标签选项。

**`property`** {GC.Spread.Sheets.LabelAlignment} [alignment] - 单元格标签位置。

**`property`** {GC.Spread.Sheets.LabelVisibility} [visibility] - 单元格标签可见性。

**`property`** {string} [font] - 单元格标签字体。

**`property`** {string} [foreColor] - 单元格标签前景色。

**`property`** {string} [margin] - 单元格标签边距。

**`example`**
```
//此示例设置水印的单元格标签选项。
var type = new GC.Spread.Sheets.Style();
type.watermark = "User name";
type.cellPadding = "20";
type.labelOptions = {alignment:GC.Spread.Sheets.LabelAlignment.topLeft, visibility: GC.Spread.Sheets.LabelVisibility.visible};
activeSheet.setStyle(0, 1, type);
activeSheet.getRange(0, -1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).height(60);
activeSheet.getRange(-1, 1, -1, 1).width(150);
var combo = new GC.Spread.Sheets.CellTypes.ComboBox();
combo.items([{ text: "Oranges", value: "11k" }, { text: "Apples", value: "15k" }, { text: "Grape", value: "100k" }]);
combo.editorValueType(GC.Spread.Sheets.CellTypes.EditorValueType.text);
activeSheet.setCellType(2, 1, combo, GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(2, 1, GC.Spread.Sheets.SheetArea.viewport).watermark("ComboBox Cell Type").cellPadding('10 10 20 10');
activeSheet.getCell(2, 1, GC.Spread.Sheets.SheetArea.viewport).labelOptions({alignment: GC.Spread.Sheets.LabelAlignment.bottomCenter, foreColor: 'yellowgreen', font: 'bold 15px Arial'});
activeSheet.getRange(2, -1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).height(60);
```

___

### <a id="locked" name="locked"></a> locked

• **locked**: `undefined` \| `boolean`

指示单元格是否被标记为锁定，无法编辑。

**`example`**
```
//此示例解锁单个单元格。
activeSheet.options.isProtected = true;
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
style.borderLeft =new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderTop = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderRight = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderBottom = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.locked = false;
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
```

___

### <a id="mask" name="mask"></a> mask

• **mask**: `undefined` \| [`IMaskType`](../interfaces/GC.Spread.Sheets.IMaskType.md)

指示输入掩码。

**`example`**
```
// 此示例使用mask属性。
var style = new GC.Spread.Sheets.Style();
style.mask = {
    pattern: '000-00000',
    excludeLiteral: true,
    placeholder: '#'
};
activeSheet.setStyle(1, 1, style, GC.Spread.Sheets.SheetArea.viewport);
```

___

### <a id="name" name="name"></a> name

• **name**: `undefined` \| `string`

指示名称。

**`example`**
```
//此示例设置样式名称。
var namedStyle = new GC.Spread.Sheets.Style();
namedStyle.name = "style1";
namedStyle.backColor = "green";
activeSheet.addNamedStyle(namedStyle);
activeSheet.setStyleName(1, 1, "style1"); // cell(1,1)'s backColor is green.
var namedStyle1 = new GC.Spread.Sheets.Style();
namedStyle1.name = "style2";
namedStyle1.parentName = "style1";
namedStyle1.foreColor = "red";    // the namedStyle's foreColor is red.
activeSheet.addNamedStyle(namedStyle1);
activeSheet.setStyleName(2, 1, "style2");
```

___

### <a id="parentname" name="parentname"></a> parentName

• **parentName**: `undefined` \| `string`

指示父样式名称。

**`example`**
```
//此示例设置父样式名称。
var namedStyle = new GC.Spread.Sheets.Style();
namedStyle.name = "style1";
namedStyle.backColor = "green";
activeSheet.addNamedStyle(namedStyle);
activeSheet.setStyleName(1, 1, "style1"); // cell(1,1)'s backColor is green.
var namedStyle1 = new GC.Spread.Sheets.Style();
namedStyle1.name = "style2";
namedStyle1.parentName = "style1";
namedStyle1.foreColor = "red";    // the namedStyle's foreColor is red.
activeSheet.addNamedStyle(namedStyle1);
activeSheet.setStyleName(2, 1, "style2");
```

___

### <a id="showellipsis" name="showellipsis"></a> showEllipsis

• **showEllipsis**: `undefined` \| `boolean`

控制文本超出边界时是否显示省略号。

**`example`**
```
//此示例设置showEllipsis属性。
var style = new GC.Spread.Sheets.Style();
style.showEllipsis = true;
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(1,1).text("TestTestTestTest");
```

___

### <a id="shrinktofit" name="shrinktofit"></a> shrinkToFit

• **shrinkToFit**: `undefined` \| `boolean`

指示是否缩小以适应。

**`example`**
```
//此示例设置shrinkToFit属性。
var style = new GC.Spread.Sheets.Style();
style.shrinkToFit = true;
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(1,1).text("Shrink To Fit");
```

___

### <a id="tabstop" name="tabstop"></a> tabStop

• **tabStop**: `undefined` \| `boolean`

指示用户是否可以使用Tab键将焦点设置到单元格。

**`example`**
```
//此示例设置tabStop属性。
var style = new GC.Spread.Sheets.Style();
style.tabStop = false;
style.backColor = "lightgreen";
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
```

___

### <a id="textdecoration" name="textdecoration"></a> textDecoration

• **textDecoration**: `undefined` \| [`TextDecorationType`](../enums/GC.Spread.Sheets.TextDecorationType.md)

表示添加到文本中的装饰。

**`example`**
```
//此示例使用textDecoration属性。
activeSheet.getCell(0, 0).textDecoration(GC.Spread.Sheets.TextDecorationType.underline);
activeSheet.getRange(1, -1, 1, -1).textDecoration(GC.Spread.Sheets.TextDecorationType.overline | GC.Spread.Sheets.TextDecorationType.underline);
activeSheet.getRange(-1, 1, -1, 1).textDecoration(GC.Spread.Sheets.TextDecorationType.overline | GC.Spread.Sheets.TextDecorationType.lineThrough | GC.Spread.Sheets.TextDecorationType.underline);
var style = new GC.Spread.Sheets.Style();
style.textDecoration = GC.Spread.Sheets.TextDecorationType.overline | GC.Spread.Sheets.TextDecorationType.underline;
activeSheet.setStyle(1, 1, style, GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(0, 0).value("Test");
activeSheet.getCell(1, 0).value("Test");
activeSheet.getCell(0, 1).value("Test");
```

___

### <a id="textdirection" name="textdirection"></a> textDirection

• **textDirection**: `undefined` \| [`TextDirectionType`](../enums/GC.Spread.Sheets.TextDirectionType.md)

定义单元格的文本方向，以更好地表示单元格。

**`example`**
```
//此示例设置Style的textDirection属性。
var style = new GC.Spread.Sheets.Style();
style.textDirection = GC.Spread.Sheets.TextDirectionType.rightToLeft;
```

___

### <a id="textindent" name="textindent"></a> textIndent

• **textIndent**: `undefined` \| `number`

指示单元格中文本缩进量，一个整数值，其中每个增量代表8像素。

**`example`**
```
//此示例设置textIndent属性。
var style = new GC.Spread.Sheets.Style();
style.textIndent = 3;
// 使用Alt+Enter输入多行
style.wordWrap = true;
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(1,1).text("Test");
```

___

### <a id="textorientation" name="textorientation"></a> textOrientation

• **textOrientation**: `undefined` \| `number`

指示单元格中文本旋转角度。

**`example`**
```
//此示例设置textOrientation属性。
var style = new GC.Spread.Sheets.Style();
style.textOrientation = 66;
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(1,1).text("TestTestTestTest");
```

___

### <a id="themefont" name="themefont"></a> themeFont

• **themeFont**: `undefined` \| `string`

指示字体主题。

**`example`**
```
//此示例使用themeFont属性。
var style = new GC.Spread.Sheets.Style();
style.formatter = "0.000%";
style.themeFont = "Body";
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(1,1).value("11");
```

___

### <a id="valign" name="valign"></a> vAlign

• **vAlign**: `undefined` \| [`VerticalAlign`](../enums/GC.Spread.Sheets.VerticalAlign.md)

指示垂直对齐。

**`example`**
```
//此示例设置vAlign属性。
var style = new GC.Spread.Sheets.Style();
style.font = "8pt Arial";
style.hAlign = GC.Spread.Sheets.HorizontalAlign.center;
style.vAlign = GC.Spread.Sheets.VerticalAlign.center;
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(1,1).value("B2");
```

___

### <a id="watermark" name="watermark"></a> watermark

• **watermark**: `undefined` \| `string`

指示水印内容。

**`example`**
```
//以下示例将水印添加到单元格、列和行。
var type = new GC.Spread.Sheets.Style();
type.watermark = "User name";
sheet.setStyle(0, 1, type);
var type = new GC.Spread.Sheets.Style();
type.watermark = "Password";
sheet.setStyle(1, 1, type);
```

**`example`**
```
var type = new GC.Spread.Sheets.Style();
type.watermark = "The watermark.";
activeSheet.setStyle(-1, 1, type);
activeSheet.setStyle(1, -1, type);
activeSheet.setStyle(2, 2, type);
```

___

### <a id="wordwrap" name="wordwrap"></a> wordWrap

• **wordWrap**: `undefined` \| `boolean`

指示是否换行。

**`example`**
```
//此示例设置wordWrap属性。
var style = new GC.Spread.Sheets.Style();
style.textIndent = 3;
// 使用Alt+Enter输入多行
style.wordWrap = true;
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(1,1).text("Test");
```

## Methods

### <a id="clone" name="clone"></a> clone

▸ **clone**(): [`Style`](GC.Spread.Sheets.Style.md)

克隆当前样式。

#### Returns

[`Style`](GC.Spread.Sheets.Style.md)

克隆的样式。
