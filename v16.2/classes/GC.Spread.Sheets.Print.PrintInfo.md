# Class: PrintInfo

[Sheets](../modules/GC.Spread.Sheets.md).[Print](../modules/GC.Spread.Sheets.Print.md).PrintInfo

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Print.PrintInfo.md#constructor)

### Methods

- [bestFitColumns](GC.Spread.Sheets.Print.PrintInfo.md#bestfitcolumns)
- [bestFitRows](GC.Spread.Sheets.Print.PrintInfo.md#bestfitrows)
- [blackAndWhite](GC.Spread.Sheets.Print.PrintInfo.md#blackandwhite)
- [centering](GC.Spread.Sheets.Print.PrintInfo.md#centering)
- [columnEnd](GC.Spread.Sheets.Print.PrintInfo.md#columnend)
- [columnStart](GC.Spread.Sheets.Print.PrintInfo.md#columnstart)
- [differentFirstPage](GC.Spread.Sheets.Print.PrintInfo.md#differentfirstpage)
- [differentOddAndEvenPages](GC.Spread.Sheets.Print.PrintInfo.md#differentoddandevenpages)
- [firstPageNumber](GC.Spread.Sheets.Print.PrintInfo.md#firstpagenumber)
- [fitPagesTall](GC.Spread.Sheets.Print.PrintInfo.md#fitpagestall)
- [fitPagesWide](GC.Spread.Sheets.Print.PrintInfo.md#fitpageswide)
- [margin](GC.Spread.Sheets.Print.PrintInfo.md#margin)
- [orientation](GC.Spread.Sheets.Print.PrintInfo.md#orientation)
- [pageHeaderFooter](GC.Spread.Sheets.Print.PrintInfo.md#pageheaderfooter)
- [pageOrder](GC.Spread.Sheets.Print.PrintInfo.md#pageorder)
- [pageRange](GC.Spread.Sheets.Print.PrintInfo.md#pagerange)
- [paperSize](GC.Spread.Sheets.Print.PrintInfo.md#papersize)
- [qualityFactor](GC.Spread.Sheets.Print.PrintInfo.md#qualityfactor)
- [repeatColumnEnd](GC.Spread.Sheets.Print.PrintInfo.md#repeatcolumnend)
- [repeatColumnStart](GC.Spread.Sheets.Print.PrintInfo.md#repeatcolumnstart)
- [repeatRowEnd](GC.Spread.Sheets.Print.PrintInfo.md#repeatrowend)
- [repeatRowStart](GC.Spread.Sheets.Print.PrintInfo.md#repeatrowstart)
- [rowEnd](GC.Spread.Sheets.Print.PrintInfo.md#rowend)
- [rowStart](GC.Spread.Sheets.Print.PrintInfo.md#rowstart)
- [showBorder](GC.Spread.Sheets.Print.PrintInfo.md#showborder)
- [showColumnHeader](GC.Spread.Sheets.Print.PrintInfo.md#showcolumnheader)
- [showGridLine](GC.Spread.Sheets.Print.PrintInfo.md#showgridline)
- [showRowHeader](GC.Spread.Sheets.Print.PrintInfo.md#showrowheader)
- [useMax](GC.Spread.Sheets.Print.PrintInfo.md#usemax)
- [watermark](GC.Spread.Sheets.Print.PrintInfo.md#watermark)
- [zoomFactor](GC.Spread.Sheets.Print.PrintInfo.md#zoomfactor)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new PrintInfo**()

表单的打印信息

## Methods

### <a id="bestfitcolumns" name="bestfitcolumns"></a> bestFitColumns

▸ **bestFitColumns**(`value?`): `any`

获取或设置是否将列宽调整为适合打印的最长文本宽度

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.bestFitColumns(true);
printInfo.orientation(GC.Spread.Sheets.Print.PrintPageOrientation.landscape);
printInfo.pageHeaderFooter({
     normal: {
         footer: {
             center: "GrapeCity"
         }
     }
});
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置任何值,则返回是否将列宽调整为适合打印的最长文本宽度;否则,返回打印设置信息

___

### <a id="bestfitrows" name="bestfitrows"></a> bestFitRows

▸ **bestFitRows**(`value?`): `any`

获取或设置是否调整行高以适合要打印的最高文本高度

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.bestFitRows(true);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置任何值,则返回是否将行高调整为适合打印的最高文本高度;否则,返回打印设置信息

___

### <a id="blackandwhite" name="blackandwhite"></a> blackAndWhite

▸ **blackAndWhite**(`value?`): `any`

获取或设置是否以黑白打印

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.blackAndWhite(true);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置任何值,则返回是否以黑白打印;否则,返回打印设置信息

___

### <a id="centering" name="centering"></a> centering

▸ **centering**(`value?`): `any`

获取或设置打印页面居中的方式

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.columnStart(0);
printInfo.columnEnd(2);
printInfo.centering(GC.Spread.Sheets.Print.PrintCentering.horizontal);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`PrintCentering`](../enums/GC.Spread.Sheets.Print.PrintCentering.md) |

#### Returns

`any`

如果未设置任何值,则返回打印页面的居中方式;否则,返回打印设置信息

___

### <a id="columnend" name="columnend"></a> columnEnd

▸ **columnEnd**(`value?`): `any`

获取或设置在打印单元格区域时要打印的最后一列

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.columnStart(0);
printInfo.columnEnd(2);
printInfo.centering(GC.Spread.Sheets.Print.PrintCentering.horizontal);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置任何值,则在打印单元格区域时返回要打印的最后一列;否则,返回打印设置信息

___

### <a id="columnstart" name="columnstart"></a> columnStart

▸ **columnStart**(`value?`): `any`

获取或设置打印单元格区域时要打印的第一列

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.columnStart(0);
printInfo.columnEnd(2);
printInfo.centering(GC.Spread.Sheets.Print.PrintCentering.horizontal);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置任何值,则在打印单元格区域时返回要打印的第一列;否则,返回打印设置信息

___

### <a id="differentfirstpage" name="differentfirstpage"></a> differentFirstPage

▸ **differentFirstPage**(`value?`): `any`

获取或设置是否在第一页打印页眉/页脚的不同文本和格式

**`代码示例`**
```
var printInfo = activeSheet.printInfo();
printInfo.differentFirstPage(true);
printInfo.pageHeaderFooter({
     first: {
         header: {
             left: "It is &amp;T.",
             center: "&amp;SThis is text.",
             right: "&amp;BHeader"
         }
     }
});
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值,返回是否在第一页打印不同的文本和格式的页眉/页脚;否则,返回打印设置信息

___

### <a id="differentoddandevenpages" name="differentoddandevenpages"></a> differentOddAndEvenPages

▸ **differentOddAndEvenPages**(`value?`): `any`

获取或设置是否在奇数页和偶数页上打印不同的页眉/页脚文本和格式

**`代码示例`**
```
var printInfo = activeSheet.printInfo();
printInfo.differentOddAndEvenPages(true);
printInfo.pageHeaderFooter({
     odd: {
         header: {
             left: "It is &amp;T.",
             center: "&amp;SThis is text.",
             right: "&amp;BHeader"
         }
     },
     even: {
         header: {
             left: "It is &amp;T.",
             center: "&amp;SThis is text.",
             right: "&amp;BHeader"
         }
     }
});
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果没有设置值,则返回是否在奇数页和偶数页上打印不同的页眉/页脚文本和格式;否则,返回打印设置信息

___

### <a id="firstpagenumber" name="firstpagenumber"></a> firstPageNumber

▸ **firstPageNumber**(`value?`): `any`

获取或设置要在第一页上打印的页码

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.firstPageNumber(1);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置任何值,则返回要打印在第一页上的页码;否则,返回打印设置信息

___

### <a id="fitpagestall" name="fitpagestall"></a> fitPagesTall

▸ **fitPagesTall**(`value?`): `any`

获取或设置优化打印时要检查的垂直页面数

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.fitPagesTall(1);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置任何值,则返回要检查的垂直页面数;否则,返回打印设置信息

___

### <a id="fitpageswide" name="fitpageswide"></a> fitPagesWide

▸ **fitPagesWide**(`value?`): `any`

获取或设置优化打印时要检查的水平页面数

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.fitPagesWide(1);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置任何值,则返回要检查的水平页面数;否则,返回打印设置信息

___

### <a id="margin" name="margin"></a> margin

▸ **margin**(`value?`): `any`

获取或设置打印页边距,以百分之一英寸为单位

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.pageHeaderFooter({
     normal: {
         header: {
             left: "Header Left",
             right: "Header Right"
         },
         footer: {
             left: "Footer Left",
             center: "Footer Center",
             right: "Footer Right"
         }
     }
});
printInfo.margin({top:75, bottom:75, left:20, right:20, header:10, footer:20});
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`PrintMargins`](../interfaces/GC.Spread.Sheets.Print.PrintMargins.md) |

#### Returns

`any`

如果未设置任何值,则返回打印页边距;否则,返回打印设置信息

___

### <a id="orientation" name="orientation"></a> orientation

▸ **orientation**(`value?`): `any`

获取或设置用于打印的页面方向

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.bestFitColumns(true);
printInfo.orientation(GC.Spread.Sheets.Print.PrintPageOrientation.landscape);
printInfo.pageHeaderFooter({
     normal: {
         footer: {
             center: "GrapeCity"
         }
     }
});
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`PrintPageOrientation`](../enums/GC.Spread.Sheets.Print.PrintPageOrientation.md) |

#### Returns

`any`

如果未设置任何值,则返回用于打印的页面方向 否则,返回打印设置信息

___

### <a id="pageheaderfooter" name="pageheaderfooter"></a> pageHeaderFooter

▸ **pageHeaderFooter**(`value?`): `any`

获取或设置在页面上自定义打印页眉/页脚的文本和格式选项

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.pageHeaderFooter({
     normal: {
         header: {
             left: "It is &amp;T.",
             center: "&amp;SThis is text.",
             right: "&amp;BHeader"
         }
     }
});
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`IPageCustomHeaderFooterOptions`](../interfaces/GC.Spread.Sheets.Print.IPageCustomHeaderFooterOptions.md) |

#### Returns

`any`

如果没有设置值,返回在页面上打印自定义页眉/页脚的文本和格式的选项;否则,返回打印设置信息

___

### <a id="pageorder" name="pageorder"></a> pageOrder

▸ **pageOrder**(`value?`): `any`

获取或设置页面打印顺序

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.pageOrder(GC.Spread.Sheets.Print.PrintPageOrder.auto);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`PrintPageOrder`](../enums/GC.Spread.Sheets.Print.PrintPageOrder.md) |

#### Returns

`any`

如果未设置任何值,则返回一个指定页面的打印顺序的值 否则,返回打印设置信息

___

### <a id="pagerange" name="pagerange"></a> pageRange

▸ **pageRange**(`value?`): `any`

获取或设置要打印的页面区域

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.pageRange("1-3");
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置任何值,则返回提供页码或页码区域的字符串;否则,返回打印设置信息

___

### <a id="papersize" name="papersize"></a> paperSize

▸ **paperSize**(`value?`): `any`

获取或设置要打印的纸张尺寸

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.pageHeaderFooter({
     normal: {
         header: {
             left: "Header Left"
         }
     }
});
printInfo.paperSize(new GC.Spread.Sheets.Print.PaperSize(300, 300));
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`PaperSize`](GC.Spread.Sheets.Print.PaperSize.md) |

#### Returns

`any`

___

### <a id="qualityfactor" name="qualityfactor"></a> qualityFactor

▸ **qualityFactor**(`value?`): `any`

获取或设置打印的质量因子

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.pageHeaderFooter({
     normal: {
         header: {
             left: "Header Left"
         }
     }
});
printInfo.qualityFactor(6);
activeSheet.printInfo(printInfo);
spread.print();
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置任何值,则返回打印的质量因子;否则,返回打印设置信息

___

### <a id="repeatcolumnend" name="repeatcolumnend"></a> repeatColumnEnd

▸ **repeatColumnEnd**(`value?`): `any`

获取或设置要在每页左侧打印的列区域的最后一列

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.pageHeaderFooter({
     normal: {
         header: {
             left: "Header Left"
         }
     }
});
printInfo.repeatColumnStart(0);
printInfo.repeatColumnEnd(2);
printInfo.repeatRowStart(0);
printInfo.repeatRowEnd(2);
activeSheet.printInfo(printInfo);
spread.print();
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置任何值,则返回要在每页左侧打印的列区域的最后一列;否则,返回打印设置信息

___

### <a id="repeatcolumnstart" name="repeatcolumnstart"></a> repeatColumnStart

▸ **repeatColumnStart**(`value?`): `any`

获取或设置要在每页左侧打印的列区域的第一列

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.pageHeaderFooter({
     normal: {
         header: {
             left: "Header Left"
         }
     }
});
printInfo.repeatColumnStart(0);
printInfo.repeatColumnEnd(2);
printInfo.repeatRowStart(0);
printInfo.repeatRowEnd(2);
activeSheet.printInfo(printInfo);
spread.print();
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置任何值,则返回要在每页左侧打印的列区域的第一列;否则,返回打印设置信息

___

### <a id="repeatrowend" name="repeatrowend"></a> repeatRowEnd

▸ **repeatRowEnd**(`value?`): `any`

获取或设置要打印在每页顶部的行区域的最后一行

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.pageHeaderFooter({
     normal: {
         header: {
             left: "Header Left"
         }
     }
});
printInfo.repeatColumnStart(0);
printInfo.repeatColumnEnd(2);
printInfo.repeatRowStart(0);
printInfo.repeatRowEnd(2);
activeSheet.printInfo(printInfo);
spread.print();
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置任何值,则返回要打印在每页顶部的行区域的最后一行;否则,返回打印设置信息

___

### <a id="repeatrowstart" name="repeatrowstart"></a> repeatRowStart

▸ **repeatRowStart**(`value?`): `any`

获取或设置要打印在每页顶部的行区域的第一行

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.pageHeaderFooter({
     normal: {
         header: {
             left: "Header Left"
         }
     }
});
printInfo.repeatColumnStart(0);
printInfo.repeatColumnEnd(2);
printInfo.repeatRowStart(0);
printInfo.repeatRowEnd(2);
activeSheet.printInfo(printInfo);
spread.print();
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置任何值,则返回要在每页顶部打印的行区域的第一行;否则,返回打印设置信息

___

### <a id="rowend" name="rowend"></a> rowEnd

▸ **rowEnd**(`value?`): `any`

获取或设置在打印单元格区域时要打印的最后一行

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.pageHeaderFooter({
     normal: {
         header: {
             left: "Header Left"
         }
     }
});
printInfo.rowStart(0);
printInfo.rowEnd(2);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置任何值,则在打印单元格区域时返回要打印的最后一行;否则,返回打印设置信息

___

### <a id="rowstart" name="rowstart"></a> rowStart

▸ **rowStart**(`value?`): `any`

获取或设置在打印单元格区域时要打印的第一行

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.pageHeaderFooter({
     normal: {
         header: {
             left: "Header Left"
         }
     }
});
printInfo.rowStart(0);
printInfo.rowEnd(2);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置任何值,则在打印单元格区域时返回要打印的第一行;否则,返回打印设置信息

___

### <a id="showborder" name="showborder"></a> showBorder

▸ **showBorder**(`value?`): `any`

获取或设置是否在整个控件周围打印分组列边框

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.showBorder(false);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置任何值,则返回是否在整个控件周围打印分组列边框;否则,返回打印设置信息

___

### <a id="showcolumnheader" name="showcolumnheader"></a> showColumnHeader

▸ **showColumnHeader**(`value?`): `any`

获取或设置是否打印列标题

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.showColumnHeader(GC.Spread.Sheets.Print.PrintVisibilityType.hide);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`PrintVisibilityType`](../enums/GC.Spread.Sheets.Print.PrintVisibilityType.md) |

#### Returns

`any`

如果未设置任何值,则返回是否打印列标题 否则,返回打印设置信息

___

### <a id="showgridline" name="showgridline"></a> showGridLine

▸ **showGridLine**(`value?`): `any`

获取或设置是否打印网格线

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.showGridLine(false);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置任何值,则返回是否打印网格线 否则,返回打印设置信息

___

### <a id="showrowheader" name="showrowheader"></a> showRowHeader

▸ **showRowHeader**(`value?`): `any`

获取或设置是否打印行标题

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.showRowHeader(GC.Spread.Sheets.Print.PrintVisibilityType.hide);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`PrintVisibilityType`](../enums/GC.Spread.Sheets.Print.PrintVisibilityType.md) |

#### Returns

`any`

如果未设置任何值,则返回是否打印行标题 否则,返回打印设置信息

___

### <a id="usemax" name="usemax"></a> useMax

▸ **useMax**(`value?`): `any`

获取或设置是否仅打印包含数据的行和列

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.useMax(true);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置任何值,则返回是否仅打印包含数据的行和列;否则,返回打印设置信息

___

### <a id="watermark" name="watermark"></a> watermark

▸ **watermark**(`value?`): [`IWatermarkItem`](../interfaces/GC.Spread.Sheets.Print.IWatermarkItem.md)

获取或设置所有水印

**`代码示例`**
```
// 本示例说明如何设置水印
var printInfo = activeSheet.printInfo();
printInfo.watermark([{x:0, y:0, width:100, height:100, imageSrc:".image/watermark.jpg", page:"all"}]);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`IWatermarkItem`](../interfaces/GC.Spread.Sheets.Print.IWatermarkItem.md)[] |

#### Returns

[`IWatermarkItem`](../interfaces/GC.Spread.Sheets.Print.IWatermarkItem.md)

水印项

___

### <a id="zoomfactor" name="zoomfactor"></a> zoomFactor

▸ **zoomFactor**(`value?`): `any`

获取或设置用于打印的缩放系数

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.zoomFactor(2);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

If no value is set, returns a value that specifies the amount to enlarge or reduce the printed worksheet; otherwise, returns the print setting information.
