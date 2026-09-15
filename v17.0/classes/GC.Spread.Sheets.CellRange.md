# Class: CellRange

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).CellRange

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.CellRange.md#constructor)

### Properties

- [col](GC.Spread.Sheets.CellRange.md#col)
- [colCount](GC.Spread.Sheets.CellRange.md#colcount)
- [row](GC.Spread.Sheets.CellRange.md#row)
- [rowCount](GC.Spread.Sheets.CellRange.md#rowcount)
- [sheet](GC.Spread.Sheets.CellRange.md#sheet)
- [sheetArea](GC.Spread.Sheets.CellRange.md#sheetarea)

### Methods

- [altText](GC.Spread.Sheets.CellRange.md#alttext)
- [backColor](GC.Spread.Sheets.CellRange.md#backcolor)
- [backgroundImage](GC.Spread.Sheets.CellRange.md#backgroundimage)
- [backgroundImageLayout](GC.Spread.Sheets.CellRange.md#backgroundimagelayout)
- [bindingPath](GC.Spread.Sheets.CellRange.md#bindingpath)
- [borderBottom](GC.Spread.Sheets.CellRange.md#borderbottom)
- [borderLeft](GC.Spread.Sheets.CellRange.md#borderleft)
- [borderRight](GC.Spread.Sheets.CellRange.md#borderright)
- [borderTop](GC.Spread.Sheets.CellRange.md#bordertop)
- [cellButtons](GC.Spread.Sheets.CellRange.md#cellbuttons)
- [cellPadding](GC.Spread.Sheets.CellRange.md#cellpadding)
- [cellType](GC.Spread.Sheets.CellRange.md#celltype)
- [clear](GC.Spread.Sheets.CellRange.md#clear)
- [comment](GC.Spread.Sheets.CellRange.md#comment)
- [defaultValue](GC.Spread.Sheets.CellRange.md#defaultvalue)
- [diagonalDown](GC.Spread.Sheets.CellRange.md#diagonaldown)
- [diagonalUp](GC.Spread.Sheets.CellRange.md#diagonalup)
- [dropDowns](GC.Spread.Sheets.CellRange.md#dropdowns)
- [font](GC.Spread.Sheets.CellRange.md#font)
- [fontFamily](GC.Spread.Sheets.CellRange.md#fontfamily)
- [fontSize](GC.Spread.Sheets.CellRange.md#fontsize)
- [fontStyle](GC.Spread.Sheets.CellRange.md#fontstyle)
- [fontWeight](GC.Spread.Sheets.CellRange.md#fontweight)
- [foreColor](GC.Spread.Sheets.CellRange.md#forecolor)
- [formatter](GC.Spread.Sheets.CellRange.md#formatter)
- [formula](GC.Spread.Sheets.CellRange.md#formula)
- [hAlign](GC.Spread.Sheets.CellRange.md#halign)
- [height](GC.Spread.Sheets.CellRange.md#height)
- [imeMode](GC.Spread.Sheets.CellRange.md#imemode)
- [isVerticalText](GC.Spread.Sheets.CellRange.md#isverticaltext)
- [labelOptions](GC.Spread.Sheets.CellRange.md#labeloptions)
- [locked](GC.Spread.Sheets.CellRange.md#locked)
- [mask](GC.Spread.Sheets.CellRange.md#mask)
- [quotePrefix](GC.Spread.Sheets.CellRange.md#quoteprefix)
- [resizable](GC.Spread.Sheets.CellRange.md#resizable)
- [setBorder](GC.Spread.Sheets.CellRange.md#setborder)
- [setStyle](GC.Spread.Sheets.CellRange.md#setstyle)
- [setStyleName](GC.Spread.Sheets.CellRange.md#setstylename)
- [showEllipsis](GC.Spread.Sheets.CellRange.md#showellipsis)
- [shrinkToFit](GC.Spread.Sheets.CellRange.md#shrinktofit)
- [tabStop](GC.Spread.Sheets.CellRange.md#tabstop)
- [tag](GC.Spread.Sheets.CellRange.md#tag)
- [text](GC.Spread.Sheets.CellRange.md#text)
- [textDecoration](GC.Spread.Sheets.CellRange.md#textdecoration)
- [textIndent](GC.Spread.Sheets.CellRange.md#textindent)
- [textOrientation](GC.Spread.Sheets.CellRange.md#textorientation)
- [themeFont](GC.Spread.Sheets.CellRange.md#themefont)
- [toHtml](GC.Spread.Sheets.CellRange.md#tohtml)
- [vAlign](GC.Spread.Sheets.CellRange.md#valign)
- [validator](GC.Spread.Sheets.CellRange.md#validator)
- [value](GC.Spread.Sheets.CellRange.md#value)
- [visible](GC.Spread.Sheets.CellRange.md#visible)
- [watermark](GC.Spread.Sheets.CellRange.md#watermark)
- [width](GC.Spread.Sheets.CellRange.md#width)
- [wordWrap](GC.Spread.Sheets.CellRange.md#wordwrap)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new CellRange**(`sheet`, `row`, `col`, `rowCount?`, `colCount?`, `sheetArea?`)

表单中的单元格区域

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheet` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 包含此单元格区域的表单 |
| `row` | `number` | 单元格的行索引 |
| `col` | `number` | 单元格的列索引 |
| `rowCount?` | `number` | - |
| `colCount?` | `number` | - |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

## Properties

### <a id="col" name="col"></a> col

• **col**: `number`

获取起始列索引

___

### <a id="colcount" name="colcount"></a> colCount

• **colCount**: `number`

获取列数

___

### <a id="row" name="row"></a> row

• **row**: `number`

获取起始行索引

___

### <a id="rowcount" name="rowcount"></a> rowCount

• **rowCount**: `number`

获取行数

___

### <a id="sheet" name="sheet"></a> sheet

• **sheet**: [`Worksheet`](GC.Spread.Sheets.Worksheet.md)

获取包含此单元格区域的表单

___

### <a id="sheetarea" name="sheetarea"></a> sheetArea

• **sheetArea**: [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md)

获取包含此单元格区域的区域

## Methods

### <a id="alttext" name="alttext"></a> altText

▸ **altText**(`value?`): `any`

获取或设置屏幕阅读器的单元格的替代文本

**`example`**
```
var SpreadIcon = {
    FolderOpen: '\ue685',
    InfoFilled: '\ue718',
    Library: '\ue69d',
    NotebookFilled: '\uD800\uDC0F',
    Browse: '\ue626'
};
activeSheet.getCell(1, 1).value(SpreadIcon.FolderOpen).altText("Folder Open Icon");

// Besides plain text, the alternative text could also contain placeholder {value} or {formatted}, which represents cell value or cell formatted value.
// For example, if the cell value is 1000, and the alt text is "Sales amount is {value}", the final accessible content should be "Sales amount is 1000".
activeSheet.getCell(1, 1).value(1000).altText("Sales amount is {value}");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `any` | 单元格的替代文本 |

#### Returns

`any`

如果未设置值，则返回单元格的替代文本；否则，返回单元格

___

### <a id="backcolor" name="backcolor"></a> backColor

▸ **backColor**(`value?`): `any`

获取或设置单元格的背景颜色，如"red"、"#FFFF00"、"rgb(255,0,0)"、"Accent 5"等

**`代码示例`**
```
activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).backColor("pink");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` \| [`IGradientFill`](../interfaces/GC.Spread.Sheets.IGradientFill.md) \| [`IGradientPathFill`](../interfaces/GC.Spread.Sheets.IGradientPathFill.md) \| [`IPatternFill`](../interfaces/GC.Spread.Sheets.IPatternFill.md) |

#### Returns

`any`

如果没有设置值，返回单元格背景颜色；否则，返回单元格

___

### <a id="backgroundimage" name="backgroundimage"></a> backgroundImage

▸ **backgroundImage**(`value?`): `any`

获取或设置单元格的背景图像

**`代码示例`**
```
activeSheet.getCell(1,1).backgroundImage("images/example.jpg");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果没有设置值，返回单元格背景图像；否则，返回单元格

___

### <a id="backgroundimagelayout" name="backgroundimagelayout"></a> backgroundImageLayout

▸ **backgroundImageLayout**(`value?`): `any`

获取或设置单元格的背景图像布局

**`代码示例`**
```
var layout = GC.Spread.Sheets.ImageLayout.stretch;
activeSheet.getRange(-1, 1, -1, 1, GC.Spread.Sheets.SheetArea.viewport).backgroundImageLayout(layout);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`ImageLayout`](../enums/GC.Spread.Sheets.ImageLayout.md) |

#### Returns

`any`

如果没有设置值，返回单元格背景图像布局；否则，返回单元格

___

### <a id="bindingpath" name="bindingpath"></a> bindingPath

▸ **bindingPath**(`path?`): `any`

获取或设置单元格绑定的绑定路径

**`代码示例`**
```
//本示例使用了bindingPath方法
var test = {name: "John"};
activeSheet.getCell(0,0).bindingPath( "name");
activeSheet.setDataSource(new GC.Spread.Sheets.Bindings.CellBindingSource(test));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `path?` | `string` | 单元格绑定的绑定路径 |

#### Returns

`any`

如果没有设置值，返回单元格绑定的绑定路径；否则，返回表单

___

### <a id="borderbottom" name="borderbottom"></a> borderBottom

▸ **borderBottom**(`value?`): `any`

获取或设置单元格的底边框

**`代码示例`**
```
activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).borderBottom(new GC.Spread.Sheets.LineBorder("blue", GC.Spread.Sheets.LineStyle.mediumDashed));
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) |

#### Returns

`any`

如果没有设置值，返回单元格底部边框线；否则，返回单元格

___

### <a id="borderleft" name="borderleft"></a> borderLeft

▸ **borderLeft**(`value?`): `any`

获取或设置单元格的左边框

**`代码示例`**
```
activeSheet.getRange(2, -1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).borderLeft(new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.mediumDashed));
```

**`代码示例`**
```
activeSheet.getCell(1,1).borderLeft(new GC.Spread.Sheets.LineBorder("red", GC.Spread.Sheets.LineStyle.double));
```

**`代码示例`**
```
activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).borderLeft(new GC.Spread.Sheets.LineBorder("blue", GC.Spread.Sheets.LineStyle.mediumDashed));
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) |

#### Returns

`any`

如果没有设置值，返回单元格的左边框；否则，返回单元格

___

### <a id="borderright" name="borderright"></a> borderRight

▸ **borderRight**(`value?`): `any`

获取或设置单元格的右边框

**`代码示例`**
```
activeSheet.getRange(2, -1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).borderRight(new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.mediumDashed));
```

**`代码示例`**
```
activeSheet.getCell(1,1).borderRight(new GC.Spread.Sheets.LineBorder("red", GC.Spread.Sheets.LineStyle.double));
```

**`代码示例`**
```
activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).borderRight(new GC.Spread.Sheets.LineBorder("blue", GC.Spread.Sheets.LineStyle.mediumDashed));
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) |

#### Returns

`any`

如果没有设置值，返回单元格的右边框线；否则，返回单元格

___

### <a id="bordertop" name="bordertop"></a> borderTop

▸ **borderTop**(`value?`): `any`

获取或设置单元格的顶部边框

**`代码示例`**
```
activeSheet.getRange(2, -1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).borderTop(new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.mediumDashed));
```

**`代码示例`**
```
activeSheet.getCell(1,1).borderTop(new GC.Spread.Sheets.LineBorder("red", GC.Spread.Sheets.LineStyle.double));
```

**`代码示例`**
```
activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).borderTop(new GC.Spread.Sheets.LineBorder("blue", GC.Spread.Sheets.LineStyle.mediumDashed));
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) |

#### Returns

`any`

如果没有设置值，返回单元格顶部边框线；否则，返回单元格

___

### <a id="cellbuttons" name="cellbuttons"></a> cellButtons

▸ **cellButtons**(`value?`): `any`

获取或设置单元格的单元格按钮

**`代码示例`**
```
activeSheet.getRange(2,-1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).cellButtons([caption:"Text"]]);
```

**`代码示例`**
```
var cellButtons = activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).cellButtons();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`ICellButton`](../interfaces/GC.Spread.Sheets.ICellButton.md)[] | 单元格按钮 |

#### Returns

`any`

如果没有设置值，返回单元格按钮；否则，返回单元格

___

### <a id="cellpadding" name="cellpadding"></a> cellPadding

▸ **cellPadding**(`value?`): `any`

获取或设置单元格填充

**`代码示例`**
```
// 本示例在水印周围添加单元格填充
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

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果没有设置值，返回单元格填充值；否则，返回单元格

___

### <a id="celltype" name="celltype"></a> cellType

▸ **cellType**(`value?`): `any`

获取或设置单元格的单元格类型

**`代码示例`**
```
activeSheet.getRange(-1, 1, -1, 1, GC.Spread.Sheets.SheetArea.viewport).cellType(new GC.Spread.Sheets.CellTypes.CheckBox());
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`Base`](GC.Spread.Sheets.CellTypes.Base.md) |

#### Returns

`any`

如果没有设置值，返回单元格类型；否则，返回单元格

___

### <a id="clear" name="clear"></a> clear

▸ **clear**(`type`): `void`

清除指定区域

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | [`StorageType`](../enums/GC.Spread.Sheets.StorageType.md) | 清除类型 |

#### Returns

`void`

___

### <a id="comment" name="comment"></a> comment

▸ **comment**(`value?`): `any`

获取或设置单元格的批注

**`代码示例`**
```
// 本示例创建了一个单元格批注
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("yellow");
comment.foreColor("green");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
activeSheet.getCell(5,5).comment(comment);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`Comment`](GC.Spread.Sheets.Comments.Comment.md) | 在单元格中设置的批注 |

#### Returns

`any`

如果没有设置值，返回单元格中的批注；否则，返回单元格区域

___

### <a id="defaultvalue" name="defaultvalue"></a> defaultValue

▸ **defaultValue**(`value?`): `any`

获取或设置单元格的默认值

**`example`**
```
activeSheet.getCell(1,1).defaultValue(10);
activeSheet.getCell(1,3).defaultValue("=LastYear+1000");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `any` |

#### Returns

`any`

如果没有设置值，则返回单元格默认值；否则，返回单元格

___

### <a id="diagonaldown" name="diagonaldown"></a> diagonalDown

▸ **diagonalDown**(`value?`): `any`

获取或设置单元格的对角线向下

**`代码示例`**
```
activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).diagonalDown(new GC.Spread.Sheets.LineBorder("blue", GC.Spread.Sheets.LineStyle.mediumDashed));
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) |

#### Returns

`any`

如果没有设置值，返回单元格对角线向下的线；否则，返回单元格

___

### <a id="diagonalup" name="diagonalup"></a> diagonalUp

▸ **diagonalUp**(`value?`): `any`

获取或设置单元格的对角线向上

**`代码示例`**
```
activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).diagonalUp(new GC.Spread.Sheets.LineBorder("blue", GC.Spread.Sheets.LineStyle.mediumDashed));
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) |

#### Returns

`any`

如果没有设置值，返回单元格对角线向上行；否则，返回单元格

___

### <a id="dropdowns" name="dropdowns"></a> dropDowns

▸ **dropDowns**(`value?`): `any`

获取或设置单元格的下拉列表

**`代码示例`**
```
activeSheet.getRange(2,-1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).dropDowns([caption:"Text"]]);
```

**`代码示例`**
```
var dropDowns = activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).dropDowns();
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`IDropdown`](../interfaces/GC.Spread.Sheets.IDropdown.md)[] |

#### Returns

`any`

如果没有设置值，返回单元格的下拉列表；否则，返回单元格

___

### <a id="font" name="font"></a> font

▸ **font**(`value?`): `any`

获取或设置单元格的字体，例如"normal normal normal 20px/normal Arial"

**`代码示例`**
```
activeSheet.getRange(2, -1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).font("12pt Arial");
```

**`代码示例`**
```
activeSheet.getCell(1,1).font("8pt Arial");
```

**`代码示例`**
```
activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).font("12pt Arial");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果没有设置值，返回单元格的字体；否则，返回单元格

___

### <a id="fontfamily" name="fontfamily"></a> fontFamily

▸ **fontFamily**(`value?`): `any`

获取或设置单元格的字体族，例如“Arial”。

**`example`**
```
activeSheet.getRange(2, -1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).fontFamily("Arial");
```

**`example`**
```
activeSheet.getCell(1,1).fontFamily("Arial");
```

**`example`**
```
activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).fontFamily("Arial");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置值，则返回单元格的字体族；否则，返回单元格。

___

### <a id="fontsize" name="fontsize"></a> fontSize

▸ **fontSize**(`value?`): `any`

Gets or sets the fontSize for the cell, such as "16px".

**`example`**
```
activeSheet.getRange(2, -1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).fontSize("16px");
```

**`example`**
```
activeSheet.getCell(1,1).fontSize("16px");
```

**`example`**
```
activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).fontSize("16px");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置值，返回单元格的字体大小；否则，返回单元格。

___

### <a id="fontstyle" name="fontstyle"></a> fontStyle

▸ **fontStyle**(`value?`): `any`

Gets or sets the fontStyle for the cell, such as "italic".

**`example`**
```
activeSheet.getRange(2, -1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).fontStyle("italic");
```

**`example`**
```
activeSheet.getCell(1,1).fontStyle("italic");
```

**`example`**
```
activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).fontStyle("italic");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置值，则返回单元格的字体样式；否则，返回单元格。

___

### <a id="fontweight" name="fontweight"></a> fontWeight

▸ **fontWeight**(`value?`): `any`

Gets or sets the fontWeight for the cell, such as "bold".

**`example`**
```
activeSheet.getRange(2, -1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).fontWeight("bold");
```

**`example`**
```
activeSheet.getCell(1,1).fontWeight("bold");
```

**`example`**
```
activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).fontWeight("bold");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置值，则返回单元格的字重设置；否则，返回单元格。

___

### <a id="forecolor" name="forecolor"></a> foreColor

▸ **foreColor**(`value?`): `any`

获取或设置单元格中的文本颜色，如"red"、"#FFFF00"、"rgb(255,0,0)"、"Accent 5"等

**`代码示例`**
```
activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).foreColor("blue");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果没有设置值，返回单元格前景色；否则，返回单元格

___

### <a id="formatter" name="formatter"></a> formatter

▸ **formatter**(`value?`): `any`

获取或设置单元格的格式化

**`代码示例`**
```
activeSheet.getCell(1,1).formatter("0.000%");
```

**`代码示例`**
```
activeSheet.getCell(1, -1).formatter("0.000%");
activeSheet.getCell(1,0).value("2");
```

**`代码示例`**
```
activeSheet.getCell(-1, 0).formatter("0.000%");
activeSheet.getCell(0,0).value("2");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` \| [`GeneralFormatter`](GC.Spread.Formatter.GeneralFormatter.md) |

#### Returns

`any`

如果没有设置值，返回单元格格式化字符串或对象；否则，返回单元格

___

### <a id="formula" name="formula"></a> formula

▸ **formula**(`value?`): `any`

获取或设置单元格的公式

**`代码示例`**
```
activeSheet.getCell(0,2).formula("DATEDIF(DATE(2003,1,1),DATE(2016,1,1),\"Y\")");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果没有设置值，返回单元格公式；否则，返回单元格

___

### <a id="halign" name="halign"></a> hAlign

▸ **hAlign**(`value?`): `any`

获取或设置单元格内容的水平对齐方式

**`代码示例`**
```
activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).hAlign(GC.Spread.Sheets.HorizontalAlign.right);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`HorizontalAlign`](../enums/GC.Spread.Sheets.HorizontalAlign.md) |

#### Returns

`any`

如果没有设置值，则返回单元格内容的水平对齐；否则，返回单元格

___

### <a id="height" name="height"></a> height

▸ **height**(`value?`): `any`

获取或设置行的高度(以像素为单位)

**`代码示例`**
```
activeSheet.getRange(0, -1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).height(90);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值，返回行高；否则，返回行

___

### <a id="imemode" name="imemode"></a> imeMode

▸ **imeMode**(`value?`): `any`

获取或设置单元格的imeMode

**`代码示例`**
```
activeSheet.getCell(0, 0).imeMode(GC.Spread.Sheets.ImeMode.disabled);
//or
var style = new GC.Spread.Sheets.Style();
style.imeMode = GC.Spread.Sheets.ImeMode.disabled;
activeSheet.setStyle(0, 0, style);
```

**`代码示例`**
```
activeSheet.getRange(2, -1, 1, -1).imeMode(GC.Spread.Sheets.ImeMode.active);
```

**`代码示例`**
```
activeSheet.getRange(-1, 2, -1, 1).imeMode(GC.Spread.Sheets.ImeMode.auto);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`ImeMode`](../enums/GC.Spread.Sheets.ImeMode.md) |

#### Returns

`any`

如果没有设置值，返回单元格imeMode;否则，返回单元格

___

### <a id="isverticaltext" name="isverticaltext"></a> isVerticalText

▸ **isVerticalText**(`value?`): `any`

获取或设置单元格的文本是否垂直

**`代码示例`**
```
activeSheet.getRange(2,-1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).isVerticalText(false);
activeSheet.setText(2,0,"This is a test");
```

**`代码示例`**
```
activeSheet.getCell(1,1).isVerticalText(true);
```

**`代码示例`**
```
activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).isVerticalText(true);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值，则返回单元格的文本是否垂直； 否则，返回单元格

___

### <a id="labeloptions" name="labeloptions"></a> labelOptions

▸ **labelOptions**(`value?`): `any`

获取或设置单元格标签选项

**`代码示例`**
```
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

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`ILabelOptions`](../interfaces/GC.Spread.Sheets.ILabelOptions.md) |

#### Returns

`any`

如果未设置值，则返回单元格标签选项的值；否则，返回单元格

___

### <a id="locked" name="locked"></a> locked

▸ **locked**(`value?`): `any`

获取或设置单元格是否锁定当表单受到保护时，无法编辑锁定的单元格

**`代码示例`**
```
activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).locked(true);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值，返回单元格是否被锁定；否则，返回单元格

___

### <a id="mask" name="mask"></a> mask

▸ **mask**(`value?`): `any`

获取或设置单元格的掩码。

**`example`**
```
//This example sets mask of the cell.
var style = new GC.Spread.Sheets.Style();
var pattern = "[a0_]{8}";
style.pattern = pattern;
activeSheet.setStyle(0, 1, style);
activeSheet.getCell(0, 1, GC.Spread.Sheets.SheetArea.viewport).mask({ pattern: pattern});
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`IMaskType`](../interfaces/GC.Spread.Sheets.IMaskType.md) |

#### Returns

`any`

If no value is set, returns the value of the cell mask; otherwise, returns the cell.

___

### <a id="quoteprefix" name="quoteprefix"></a> quotePrefix

▸ **quotePrefix**(`value?`): `any`

获取或设置单元格的引号前缀

**`代码示例`**
```
activeSheet.getCell(1,1).quotePrefix(true);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值，返回引号前缀的内容；否则，返回单元格

___

### <a id="resizable" name="resizable"></a> resizable

▸ **resizable**(`value?`): `any`

获取或设置用户是否可以调整行或列的大小

**`代码示例`**
```
activeSheet.getRange(-1, 3, -1, 1. GC.Spread.Sheets.SheetArea.viewport).resizable(true);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值，返回用户是否可以调整行大小；否则，返回行或列

___

### <a id="setborder" name="setborder"></a> setBorder

▸ **setBorder**(`border`, `option`): `void`

设置区域的边框

**`代码示例`**
```
//本示例创建了边框
sheet.getCell(1, 1).borderTop(new GC.Spread.Sheets.LineBorder("#F0F8FF",GC.Spread.Sheets.LineStyle.double));
sheet.getCell(1, 1).borderLeft(new GC.Spread.Sheets.LineBorder("#F0F8FF",GC.Spread.Sheets.LineStyle.hair));
sheet.getCell(1, 1).borderRight(new GC.Spread.Sheets.LineBorder("#FAEBD7",GC.Spread.Sheets.LineStyle.dashDot));
sheet.getCell(1, 1).borderBottom(new GC.Spread.Sheets.LineBorder("#00FFFF",GC.Spread.Sheets.LineStyle.medium));
sheet.getRange(-1, 5, -1, 1, GC.Spread.Sheets.SheetArea.viewport).borderTop(new GC.Spread.Sheets.LineBorder("#F0FFFF",GC.Spread.Sheets.LineStyle.medium));
sheet.getRange(-1, 5, -1, 1, GC.Spread.Sheets.SheetArea.viewport).borderLeft(new GC.Spread.Sheets.LineBorder("#F5F5DC",GC.Spread.Sheets.LineStyle.medium));
sheet.getRange(-1, 5, -1, 1, GC.Spread.Sheets.SheetArea.viewport).borderRight(new GC.Spread.Sheets.LineBorder("#FF02FF", GC.Spread.Sheets.LineStyle.dashDot));
sheet.getRange(-1, 5, -1, 1, GC.Spread.Sheets.SheetArea.viewport).borderBottom (new GC.Spread.Sheets.LineBorder("#FFE4C4",GC.Spread.Sheets.LineStyle.thin));
sheet.getRange(2, 2, 2, 2, GC.Spread.Sheets.SheetArea.viewport).setBorder(new GC.Spread.Sheets.LineBorder("#8A2BE2",GC.Spread.Sheets.LineStyle.thick), { all:true });
sheet.getRange(5, -1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).borderTop( new GC.Spread.Sheets.LineBorder("#A52A2A",GC.Spread.Sheets.LineStyle.mediumDashed));
sheet.getRange(5, -1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).borderLeft( new GC.Spread.Sheets.LineBorder("#FF02FF",GC.Spread.Sheets.LineStyle.medium));
sheet.getRange(5, -1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).borderRight(new GC.Spread.Sheets.LineBorder("#5F9EA0", GC.Spread.Sheets.LineStyle.dashDot));
sheet.getRange(5, -1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).borderBottom(new GC.Spread.Sheets.LineBorder("#6495ED",GC.Spread.Sheets.LineStyle.dotted));
sheet.getRange(5, -1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).diagonalUp(new GC.Spread.Sheets.LineBorder("#FF02FF",GC.Spread.Sheets.LineStyle.dotted));
sheet.getRange(5, -1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).diagonalDown(new GC.Spread.Sheets.LineBorder("#6495ED",GC.Spread.Sheets.LineStyle.medium));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `border` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) | 边框线 |
| `option` | [`ISetBorderOptions`](../interfaces/GC.Spread.Sheets.ISetBorderOptions.md) | 确定选项对象包含要设置的单元格区域的哪一部分 {all:true, left:true, top:true, right:true, bottom:true, diagonalUp:true, diagonalDown:true, outline:true,inside:true, innerHorizontal:true, innerVertical:true} |

#### Returns

`void`

___

### <a id="setstyle" name="setstyle"></a> setStyle

▸ **setStyle**(`value`): `void`

设置单元格的样式

**`代码示例`**
```
let style = new GC.Spread.Sheets.Style();
style.formatter = "#,##0.00";
sheet.getRange("E5:F10").setStyle(style);
sheet.getRange(0,0,4,4).setStyle(style);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | [`Style`](GC.Spread.Sheets.Style.md) | 样式 |

#### Returns

`void`

___

### <a id="setstylename" name="setstylename"></a> setStyleName

▸ **setStyleName**(`value`): `void`

设置单元格的命名样式

**`代码示例`**
```
let style = new GC.Spread.Sheets.Style();
style.name = "bold_style";
style.font = "bold 12px sans-serif";
sheet.addNamedStyle(style);
sheet.getRange("A1:D3").setStyleName("bold_style");
sheet.getRange(5,5,10,10).setStyleName("bold_style");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `string` | 样式名称 |

#### Returns

`void`

___

### <a id="showellipsis" name="showellipsis"></a> showEllipsis

▸ **showEllipsis**(`value?`): `any`

获取或设置单元格省略符属性

**`代码示例`**
```
activeSheet.getRange(2,-1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).showEllipsis(false);
activeSheet.setText(2,0,"This is a test");
```

**`代码示例`**
```
activeSheet.getCell(1,1).showEllipsis(true);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置值，则返回单元格省略符属性

___

### <a id="shrinktofit" name="shrinktofit"></a> shrinkToFit

▸ **shrinkToFit**(`value?`): `any`

获取或设置单元格是否缩小文本以适应单元格大小

**`代码示例`**
```
activeSheet.getRange(2,-1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).shrinkToFit(false);
activeSheet.setText(2,0,"This is a test");
```

**`代码示例`**
```
activeSheet.getCell(1,1).shrinkToFit(true);
```

**`代码示例`**
```
activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).shrinkToFit(true);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置值，则返回单元格是否缩小文本以适应；否则，返回单元格

___

### <a id="tabstop" name="tabstop"></a> tabStop

▸ **tabStop**(`value?`): `any`

获取或设置一个值，该值指示用户是否可以使用Tab键设置单元格的焦点

**`代码示例`**
```
activeSheet.getCell(1,1).tabStop(false);
activeSheet.getRange(1, -1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).tabStop(false);
activeSheet.getRange(-1, 1, -1, 1, GC.Spread.Sheets.SheetArea.viewport).tabStop(false);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值，返回用户是否可以使用Tab键设置单元格的焦点；否则，返回单元格

___

### <a id="tag" name="tag"></a> tag

▸ **tag**(`value?`): `any`

获取或设置单元格的标签

**`代码示例`**
```
activeSheet.getCell(1,1).tag("cell tag");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `any` |

#### Returns

`any`

如果没有设置值，返回标签值；否则，返回单元格

___

### <a id="text" name="text"></a> text

▸ **text**(`value?`): `any`

获取或设置单元格的格式化文本

**`代码示例`**
```
activeSheet.getCell(1,1).text("cell object");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果没有设置值，返回单元格文本；否则，返回单元格

___

### <a id="textdecoration" name="textdecoration"></a> textDecoration

▸ **textDecoration**(`value?`): `any`

获取或设置添加到单元格文本的修饰的类型

**`代码示例`**
```
activeSheet.getRange(1, -1, 1, -1).textDecoration(GC.Spread.Sheets.TextDecorationType.overline | GC.Spread.Sheets.TextDecorationType.underline);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`TextDecorationType`](../enums/GC.Spread.Sheets.TextDecorationType.md) |

#### Returns

`any`

如果没有设置值，返回修饰的类型；否则，返回单元格

___

### <a id="textindent" name="textindent"></a> textIndent

▸ **textIndent**(`value?`): `any`

获取或设置单元格的文本缩进

**`代码示例`**
```
activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).textIndent(1);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值，返回单元格文本缩进；否则，返回单元格

___

### <a id="textorientation" name="textorientation"></a> textOrientation

▸ **textOrientation**(`value?`): `any`

获取或设置单元格的文本旋转角度

**`代码示例`**
```
activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).textOrientation(66);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值，返回单元格文本的旋转角度；否则，返回单元格

___

### <a id="themefont" name="themefont"></a> themeFont

▸ **themeFont**(`value?`): `any`

获取或设置单元格的主题字体

**`代码示例`**
```
activeSheet.getCell(-1, 0).themeFont("Body");
activeSheet.getCell(0,0).value("Test");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果没有设置值，返回单元格的主题字体；否则，返回单元格

___

### <a id="tohtml" name="tohtml"></a> toHtml

▸ **toHtml**(`headerOptions?`, `includeStyle?`): `string`

从指定区域获取HTML内容

**`代码示例`**
```
activeSheet.getRange(0, 0, 10, 10).toHtml();
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `headerOptions?` | [`HeaderOptions`](../enums/GC.Spread.Sheets.HeaderOptions.md) |
| `includeStyle?` | `boolean` |

#### Returns

`string`

包含单元格文本、单元格合并和单元格样式的HTML内容

___

### <a id="valign" name="valign"></a> vAlign

▸ **vAlign**(`value?`): `any`

获取或设置单元格内容的垂直对齐方式

**`代码示例`**
```
activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).vAlign(GC.Spread.Sheets.VerticalAlign.top);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`VerticalAlign`](../enums/GC.Spread.Sheets.VerticalAlign.md) |

#### Returns

`any`

如果没有设置值，则返回单元格内容的垂直对齐方式；否则，返回单元格

___

### <a id="validator" name="validator"></a> validator

▸ **validator**(`value?`): `any`

获取或设置单元格的数据验证

**`代码示例`**
```
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createDateValidator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.between, new Date(2012, 11, 31), new Date(2013, 11, 31));
dv.showInputMessage(true);
dv.inputMessage("Enter a date between 12/31/2012 and 12/31/2013.");
dv.inputTitle("Tip");
activeSheet.getCell(0,0).validator(dv);
```

**`代码示例`**
```
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createDateValidator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.between, new Date(2012, 11, 31), new Date(2013, 11, 31));
dv.showInputMessage(true);
dv.inputMessage("Enter a date between 12/31/2012 and 12/31/2013.");
dv.inputTitle("Tip");
activeSheet.getCell(1, -1).validator(dv);
```

**`代码示例`**
```
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createListValidator("1,2,3");
dv.showInputMessage(true);
dv.inputMessage("Value must be 1,2 or 3");
dv.inputTitle("tip");
activeSheet.setDataValidator(-1,0,dv);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`DefaultDataValidator`](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md) | 单元格数据验证 |

#### Returns

`any`

如果没有设置值，返回单元格数据验证；否则，返回单元格

___

### <a id="value" name="value"></a> value

▸ **value**(`value?`): `any`

获取或设置单元格的未格式化值

**`代码示例`**
```
activeSheet.getCell(1,1).value(10);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `any` |

#### Returns

`any`

如果没有设置值，返回单元格值；否则，返回单元格

___

### <a id="visible" name="visible"></a> visible

▸ **visible**(`value?`): `any`

获取或设置是否显示行或列

**`代码示例`**
```
activeSheet.getCell(-1, 0).visible(false);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值，返回行或列的可见值；否则，返回行或列

___

### <a id="watermark" name="watermark"></a> watermark

▸ **watermark**(`value?`): `any`

获取或设置单元格水印的内容

**`代码示例`**
```
activeSheet.getCell(1,1).watermark("lightgreen");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果没有设置值，返回水印的内容；否则，返回单元格

___

### <a id="width" name="width"></a> width

▸ **width**(`value?`): `any`

获取或设置列的宽度(以像素为单位)

**`代码示例`**
```
activeSheet.getCell(-1, 0).width(20);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果没有设置值，返回列宽度；否则，返回列

___

### <a id="wordwrap" name="wordwrap"></a> wordWrap

▸ **wordWrap**(`value?`): `any`

获取或设置单元格是否允许文本换行

**`代码示例`**
```
activeSheet.getRange(-1, 3, -1, 1, GC.Spread.Sheets.SheetArea.viewport).wordWrap(true);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值，返回单元格是否允许文本换行；否则，返回单元格
