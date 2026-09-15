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

单元格、行和列的样式

**`代码示例`**
``` javascript
//本示例使用了带有规则的样式
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

**`代码示例`**
``` javascript
//本示例为样式创建和设置参数
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

指示该单元格是否可以进入编辑模式进行编辑。

**`example`**
```
//This example sets the allowEditInCell property.
var style = activeSheet.getStyle(1,1,GC.Spread.Sheets.SheetArea.viewport);
style.allowEditInCell = false;
```

___

### <a id="applyalignment" name="applyalignment"></a> applyAlignment

• **applyAlignment**: `boolean`

只对namedStyle起作用，布尔值表示是否应用对齐方式

**`代码示例`**
``` javascript
//本示例为namedStyle设置了applyAlignment属性
var style = new GC.Spread.Sheets.Style();
style.name = 'test';
style.applyAlignment = false;
spread.addNamedStyle(style);
```

___

### <a id="applyborder" name="applyborder"></a> applyBorder

• **applyBorder**: `boolean`

只对namedStyle起作用，布尔值表示是否应用边框格式

**`代码示例`**
``` javascript
//本示例为namedStyle设置了applyBorder属性
var style = new GC.Spread.Sheets.Style();
style.name = 'test';
style.applyBorder = false;
spread.addNamedStyle(style);
```

___

### <a id="applyfill" name="applyfill"></a> applyFill

• **applyFill**: `boolean`

只对namedStyle起作用，布尔值表示是否应用了填充格式化

**`代码示例`**
``` javascript
//本示例为namedStyle设置applyFill属性
var style = new GC.Spread.Sheets.Style();
style.name = 'test';
style.applyFill = false;
spread.addNamedStyle(style);
```

___

### <a id="applyfont" name="applyfont"></a> applyFont

• **applyFont**: `boolean`

只对namedStyle起作用，布尔值表示是否应用了字体格式化

**`代码示例`**
``` javascript
//本示例为namedStyle设置applyFont属性
var style = new GC.Spread.Sheets.Style();
style.name = 'test';
style.applyFont = false;
spread.addNamedStyle(style);
```

___

### <a id="applynumberformat" name="applynumberformat"></a> applyNumberFormat

• **applyNumberFormat**: `boolean`

只对namedStyle起作用，布尔值表示是否应用数字格式化

**`代码示例`**
``` javascript
//本示例为namedStyle设置applyNumberFormat属性
var style = new GC.Spread.Sheets.Style();
style.name = 'test';
style.applyNumberFormat = false;
spread.addNamedStyle(style);
```

___

### <a id="applyprotection" name="applyprotection"></a> applyProtection

• **applyProtection**: `boolean`

只对namedStyle起作用，布尔值表示是否应用保护格式

**`代码示例`**
``` javascript
//本示例为namedStyle设置applyProtection属性
var style = new GC.Spread.Sheets.Style();
style.name = 'test';
style.applyProtection = false;
spread.addNamedStyle(style);
```

___

### <a id="backcolor" name="backcolor"></a> backColor

• **backColor**: `undefined` \| `string` \| [`IGradientFill`](../interfaces/GC.Spread.Sheets.IGradientFill.md) \| [`IGradientPathFill`](../interfaces/GC.Spread.Sheets.IGradientPathFill.md) \| [`IPatternFill`](../interfaces/GC.Spread.Sheets.IPatternFill.md)

背景色

**`代码示例`**
``` javascript
//本示例设置了背景颜色属性
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

背景图片

**`代码示例`**
``` javascript
//本示例设置了backgroundImage属性
var style = new GC.Spread.Sheets.Style();
style.backColor = "lightgreen";
style.backgroundImage = "./css/images/quarter1.png";
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
```

___

### <a id="backgroundimagelayout" name="backgroundimagelayout"></a> backgroundImageLayout

• **backgroundImageLayout**: `undefined` \| [`ImageLayout`](../enums/GC.Spread.Sheets.ImageLayout.md)

背景图像布局

**`代码示例`**
``` javascript
//本示例设置了backgroundImageLayout属性
var style = new GC.Spread.Sheets.Style();
style.backColor = "lightgreen";
style.backgroundImage = "./css/images/quarter1.png";
style.backgroundImageLayout  = GC.Spread.Sheets.ImageLayout.center;
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
```

___

### <a id="borderbottom" name="borderbottom"></a> borderBottom

• **borderBottom**: `undefined` \| [`LineBorder`](GC.Spread.Sheets.LineBorder.md)

底部边框线

**`代码示例`**
``` javascript
//本示例创建一个边框
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

左侧边框线

**`代码示例`**
``` javascript
//本示例创建一个边框
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

右边框线

**`代码示例`**
``` javascript
//本示例创建一个边框
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

上边框线

**`代码示例`**
``` javascript
//本示例创建一个边框
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

单元格按钮

**`property`** {string} [caption] - 要显示的按钮的文本

**`property`** {GC.Spread.Sheets.CaptionAlignment} [captionAlign] - 图片和标题的位置

**`property`** {GC.Spread.Sheets.ButtonPosition} [position] - 按钮在单元格中的位置

**`property`** {boolean} [enabled] - 单元格按钮是否响应用户操作，默认值为true

**`property`** {boolean} [useButtonStyle] - 是否为按钮样式，默认值为false

**`property`** {number} [width] - 按钮的宽度如果设置为null或undefined,则按钮宽度将根据标题和图像大小自动调整

**`property`** {GC.Spread.Sheets.ButtonVisibility} [visibility] - 按钮可见为 always, onSelected, onEditing, 默认值为always

**`property`** {string | function} [command] - 单击按钮时，允许用户执行排列命令或用户可以执行回调

**`property`** {GC.Spread.Sheets.ButtonImageType} [imageType] - 指定按钮的类型（在按钮中显示的图像类型）。按钮单元格类型提供一些预设类型，允许用户可以选择

**`property`** {string} [imageSrc] - 当图像是自定义时，可以通过imagesRC特定图像（base64）

**`property`** {GC.Spread.Sheets.IImageSize} [imageSize] - 特定图像的大小，默认值为16px

**`property`** {string} [hoverBackColor] - 当按钮可见并启用时，请确定单元按钮的悬停后面色

**`property`** {string} [buttonBackColor] - 启用按钮时，请确定单元按钮的后面色

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
    imageSrc:"data:image/svg+xml;base64,PD94bWwgdmVyc2lvb...", //This is not a complete base64 string
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

单元格填充

**`代码示例`**
``` javascript
//本示例设置水印的单元格填充
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

单元格类型

**`代码示例`**
``` javascript
//本示例创建了一个样式并将其应用于单元格
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

定义一个用于单元格的装饰器

**`代码示例`**
``` javascript
//This example sets the decoration property for Style.
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

对角线下边框线

**`代码示例`**
``` javascript
activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).diagonalDown(new GC.Spread.Sheets.LineBorder("blue", GC.Spread.Sheets.LineStyle.mediumDashed));
```

___

### <a id="diagonalup" name="diagonalup"></a> diagonalUp

• **diagonalUp**: `undefined` \| [`LineBorder`](GC.Spread.Sheets.LineBorder.md)

对角线上的边框线

**`代码示例`**
``` javascript
activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).diagonalUp(new GC.Spread.Sheets.LineBorder("blue", GC.Spread.Sheets.LineStyle.mediumDashed));
```

___

### <a id="dropdowns" name="dropdowns"></a> dropDowns

• **dropDowns**: `undefined` \| [`IDropdown`](../interfaces/GC.Spread.Sheets.IDropdown.md)[]

单元格的下拉类型

**`代码示例`**
``` javascript
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

字体

**`代码示例`**
``` javascript
//本示例设置了字体属性
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

表示字体系列。

**`example`**
```
//This example sets the fontFamily property.
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
//This example sets the fontSize property.
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
//This example sets the fontStyle property.
var style = new GC.Spread.Sheets.Style();
style.fontStyle = "italic";
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(1,1).value("B2");
```

___

### <a id="fontweight" name="fontweight"></a> fontWeight

• **fontWeight**: `undefined` \| `string`

表示字体粗细。

**`example`**
```
//This example sets the fontWeight property.
var style = new GC.Spread.Sheets.Style();
style.fontWeight = "bold";
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(1,1).value("B2");
```

___

### <a id="forecolor" name="forecolor"></a> foreColor

• **foreColor**: `undefined` \| `string`

前景色

**`代码示例`**
``` javascript
//本示例设置了foreColor属性
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

格式化

**`代码示例`**
``` javascript
//格式化示例
var style = new GC.Spread.Sheets.Style();
style.formatter = "0.000%";
style.themeFont = "Body";
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(1,1).value("11");
```

___

### <a id="halign" name="halign"></a> hAlign

• **hAlign**: `undefined` \| [`HorizontalAlign`](../enums/GC.Spread.Sheets.HorizontalAlign.md)

水平对齐

**`代码示例`**
``` javascript
//本示例设置hAlign属性
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

指示当工作表受保护时单元格公式是否可见。

**`example`**
```
//This example hidden a single cell.
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

输入法编辑器(IME)模式

**`代码示例`**
``` javascript
//本示例设置了IME模式
var style = new GC.Spread.Sheets.Style();
style.imeMode = GC.Spread.Sheets.ImeMode.auto;
activeSheet.setStyle(0, 0, style);
```

___

### <a id="isverticaltext" name="isverticaltext"></a> isVerticalText

• **isVerticalText**: `undefined` \| `boolean`

是否将文本垂直设置

**`代码示例`**
``` javascript
//本示例使用了rotate属性
var style = new GC.Spread.Sheets.Style();
style.isVerticalText = true;
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
```

___

### <a id="labeloptions" name="labeloptions"></a> labelOptions

• **labelOptions**: `undefined` \| [`ILabelOptions`](../interfaces/GC.Spread.Sheets.ILabelOptions.md)

单元格标签选项

**`property`** {GC.Spread.Sheets.LabelAlignment} [alignment] - 单元格标签位置

**`property`** {GC.Spread.Sheets.LabelVisibility} [visibility] - 单元格标签可见性

**`property`** {string} [font] - 单元格标签字体

**`property`** {string} [foreColor] - 单元格标签前颜色

**`property`** {string} [margin] - 单元格标签边距

**`代码示例`**
``` javascript
//本示例为水印设置标签选项
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

单元格是否标签为锁定而不进行编辑

**`代码示例`**
``` javascript
//本示例解锁单个单元格
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

表示输入掩码。

**`example`**
```
// This example uses the mask property.
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

名称

**`代码示例`**
``` javascript
//本示例设置样式名
var namedStyle = new GC.Spread.Sheets.Style();
namedStyle.name = "style1";
namedStyle.backColor = "green";
activeSheet.addNamedStyle(namedStyle);
activeSheet.setStyleName(1, 1, "style1"); // 单元格(1,1)背景色为绿色
var namedStyle1 = new GC.Spread.Sheets.Style();
namedStyle1.name = "style2";
namedStyle1.parentName = "style1";
namedStyle1.foreColor = "red";    // namedStyle的前景色为红色
activeSheet.addNamedStyle(namedStyle1);
activeSheet.setStyleName(2, 1, "style2");
```

___

### <a id="parentname" name="parentname"></a> parentName

• **parentName**: `undefined` \| `string`

父样式的名称

**`代码示例`**
``` javascript
//本示例设置父名称
var namedStyle = new GC.Spread.Sheets.Style();
namedStyle.name = "style1";
namedStyle.backColor = "green";
activeSheet.addNamedStyle(namedStyle);
activeSheet.setStyleName(1, 1, "style1"); // 单元格(1,1)背景色为绿色
var namedStyle1 = new GC.Spread.Sheets.Style();
namedStyle1.name = "style2";
namedStyle1.parentName = "style1";
namedStyle1.foreColor = "red";    // namedStyle的前景色为红色
activeSheet.addNamedStyle(namedStyle1);
activeSheet.setStyleName(2, 1, "style2");
```

___

### <a id="showellipsis" name="showellipsis"></a> showEllipsis

• **showEllipsis**: `undefined` \| `boolean`

控制文本越界是否显示省略号

**`代码示例`**
``` javascript
//本示例设置showEllipsis属性
var style = new GC.Spread.Sheets.Style();
style.showEllipsis = true;
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(1,1).text("TestTestTestTest");
```

___

### <a id="shrinktofit" name="shrinktofit"></a> shrinkToFit

• **shrinkToFit**: `undefined` \| `boolean`

是否缩小以适应

**`代码示例`**
``` javascript
//本示例设置shrinkToFit属性
var style = new GC.Spread.Sheets.Style();
style.shrinkToFit = true;
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(1,1).text("Shrink To Fit");
```

___

### <a id="tabstop" name="tabstop"></a> tabStop

• **tabStop**: `undefined` \| `boolean`

用户是否可以使用Tab键设置单元格的焦点

**`代码示例`**
``` javascript
//本示例设置了tabStop属性
var style = new GC.Spread.Sheets.Style();
style.tabStop = false;
style.backColor = "lightgreen";
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
```

___

### <a id="textdecoration" name="textdecoration"></a> textDecoration

• **textDecoration**: `undefined` \| [`TextDecorationType`](../enums/GC.Spread.Sheets.TextDecorationType.md)

添加到文本的样式

**`代码示例`**
``` javascript
//本示例使用了textDecoration属性
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

定义单元格的文本方向以更好地表示单元格。

**`example`**
```
//This example sets the text direction property for Style.
var style = new GC.Spread.Sheets.Style();
style.textDirection = GC.Spread.Sheets.TextDirectionType.rightToLeft;
```

___

### <a id="textindent" name="textindent"></a> textIndent

• **textIndent**: `undefined` \| `number`

单元格中文本的缩进单位数，为整数值，增量1表示8像素

**`代码示例`**
``` javascript
//本示例设置了textIndent属性
var style = new GC.Spread.Sheets.Style();
style.textIndent = 3;
// 用Alt+Enter键输入多行
style.wordWrap = true;
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(1,1).text("Test");
```

___

### <a id="textorientation" name="textorientation"></a> textOrientation

• **textOrientation**: `undefined` \| `number`

单元格的文本旋转角度

**`代码示例`**
``` javascript
//本示例设置了textOrientation属性
var style = new GC.Spread.Sheets.Style();
style.textOrientation = 66;
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(1,1).text("TestTestTestTest");
```

___

### <a id="themefont" name="themefont"></a> themeFont

• **themeFont**: `undefined` \| `string`

字体主题

**`代码示例`**
``` javascript
//本示例使用了themeFont属性
var style = new GC.Spread.Sheets.Style();
style.formatter = "0.000%";
style.themeFont = "Body";
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(1,1).value("11");
```

___

### <a id="valign" name="valign"></a> vAlign

• **vAlign**: `undefined` \| [`VerticalAlign`](../enums/GC.Spread.Sheets.VerticalAlign.md)

垂直对齐

**`代码示例`**
``` javascript
//本示例设置vAlign属性
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

水印内容

**`代码示例`**
``` javascript
//下面的示例向单元格、列和行添加水印
var type = new GC.Spread.Sheets.Style();
type.watermark = "User name";
sheet.setStyle(0, 1, type);
var type = new GC.Spread.Sheets.Style();
type.watermark = "Password";
sheet.setStyle(1, 1, type);
```

**`代码示例`**
``` javascript
var type = new GC.Spread.Sheets.Style();
type.watermark = "The watermark.";
activeSheet.setStyle(-1, 1, type);
activeSheet.setStyle(1, -1, type);
activeSheet.setStyle(2, 2, type);
```

___

### <a id="wordwrap" name="wordwrap"></a> wordWrap

• **wordWrap**: `undefined` \| `boolean`

是否换行文本

**`代码示例`**
``` javascript
//本示例设置了wordWrap属性
var style = new GC.Spread.Sheets.Style();
style.textIndent = 3;
// 用Alt+Enter键输入多行
style.wordWrap = true;
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
activeSheet.getCell(1,1).text("Test");
```

## Methods

### <a id="clone" name="clone"></a> clone

▸ **clone**(): [`Style`](GC.Spread.Sheets.Style.md)

克隆当前的样式

#### Returns

[`Style`](GC.Spread.Sheets.Style.md)

克隆的样式
