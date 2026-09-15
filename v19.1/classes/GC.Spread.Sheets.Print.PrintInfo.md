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

• **new PrintInfo**(`sheet?`)

表示打印工作表时使用的信息。

**`example`**
```javascript
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.bestFitColumns(true);
printInfo.orientation(GC.Spread.Sheets.Print.PrintPageOrientation.landscape);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheet?` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 指定的工作表 |

## Methods

### <a id="bestfitcolumns" name="bestfitcolumns"></a> bestFitColumns

▸ **bestFitColumns**(`value?`): `any`

获取或设置是否调整列宽以适应打印时最长的文本宽度。

**`example`**
```javascript
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.bestFitColumns(true);
printInfo.orientation(GC.Spread.Sheets.Print.PrintPageOrientation.landscape);
printInfo.pageHeaderFooter({
    normal: {
        footer: {
            center: "SpreadJS"
        }
    }
});
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否调整列宽以适应打印时最长的文本宽度。 |

#### Returns

`any`

如果未设置值，返回是否调整列宽以适应打印时最长的文本宽度；否则返回打印设置信息。

___

### <a id="bestfitrows" name="bestfitrows"></a> bestFitRows

▸ **bestFitRows**(`value?`): `any`

获取或设置是否调整行高以适应打印时最高的文本高度。

**`example`**
```javascript
activeSheet.getCell(0,0).wordWrap(true);
activeSheet.getCell(0,0).value("The quick brown fox jumps over the lazy dog.");
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.bestFitRows(true);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否调整行高以适应打印时最高的文本高度。 |

#### Returns

`any`

如果未设置值，返回是否调整行高以适应打印时最高的文本高度；否则返回打印设置信息。

___

### <a id="blackandwhite" name="blackandwhite"></a> blackAndWhite

▸ **blackAndWhite**(`value?`): `any`

获取或设置是否以黑白方式打印。

**`example`**
```javascript
activeSheet.getRange(0, 0, 5, 5).backColor("red");
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.blackAndWhite(true);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否以黑白方式打印。 |

#### Returns

`any`

如果未设置值，返回是否以黑白方式打印；否则返回打印设置信息。

___

### <a id="centering" name="centering"></a> centering

▸ **centering**(`value?`): `any`

获取或设置打印页面的居中方式。

**`example`**
```javascript
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.columnStart(0);
printInfo.columnEnd(2);
printInfo.centering(GC.Spread.Sheets.Print.PrintCentering.horizontal);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`PrintCentering`](../enums/GC.Spread.Sheets.Print.PrintCentering.md) | 打印页面的居中方式。 |

#### Returns

`any`

如果未设置值，返回打印页面的居中方式；否则返回打印设置信息。

___

### <a id="columnend" name="columnend"></a> columnEnd

▸ **columnEnd**(`value?`): `any`

获取或设置打印单元格范围时的最后一列。

**`example`**
```javascript
var data = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["5", "Washington", "1972/8/8","80", "171"],
];
activeSheet.setArray(0, 0, data);
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.columnStart(0);
printInfo.columnEnd(2);
printInfo.centering(GC.Spread.Sheets.Print.PrintCentering.horizontal);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 打印单元格范围时的最后一列。 |

#### Returns

`any`

如果未设置值，返回打印单元格范围时的最后一列；否则返回打印设置信息。

___

### <a id="columnstart" name="columnstart"></a> columnStart

▸ **columnStart**(`value?`): `any`

获取或设置打印单元格范围时的第一列。

**`example`**
```javascript
var data = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["5", "Washington", "1972/8/8","80", "171"],
];
activeSheet.setArray(0, 0, data);
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.columnStart(2);
printInfo.columnEnd(4);
printInfo.centering(GC.Spread.Sheets.Print.PrintCentering.horizontal);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 打印单元格范围时的第一列。 |

#### Returns

`any`

如果未设置值，返回打印单元格范围时的第一列；否则返回打印设置信息。

___

### <a id="differentfirstpage" name="differentfirstpage"></a> differentFirstPage

▸ **differentFirstPage**(`value?`): `any`

获取或设置是否在第一页打印不同的页眉/页脚文本和格式。

**`example`**
```javascript
activeSheet.setArray(0, 0, new Array(60).fill(["sample text"]));
var printInfo = activeSheet.printInfo();
printInfo.differentFirstPage(true);
printInfo.pageHeaderFooter({
     first: {
         header: {
             left: "It is &A.",
             center: "&SThis is text.",
             right: "&BHeader"
         }
     }
});
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否在第一页打印不同的页眉/页脚文本和格式。 |

#### Returns

`any`

如果未设置值，返回是否在第一页打印不同的页眉/页脚文本和格式；否则返回打印设置信息。

___

### <a id="differentoddandevenpages" name="differentoddandevenpages"></a> differentOddAndEvenPages

▸ **differentOddAndEvenPages**(`value?`): `any`

获取或设置是否在奇偶页打印不同的页眉/页脚文本和格式。

**`example`**
```javascript
activeSheet.setArray(0, 0, new Array(60).fill(["sample text"]));
var printInfo = activeSheet.printInfo();
printInfo.differentOddAndEvenPages(true);
printInfo.pageHeaderFooter({
     odd: {
         header: {
             left: "odd page",
             center: "page number: &P",
             right: "&BHeader"
         }
     },
     even: {
         header: {
             left: "even page",
             center: "page number: &P",
             right: "&BHeader"
         }
     }
});
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否在奇偶页打印不同的页眉/页脚文本和格式。 |

#### Returns

`any`

如果未设置值，返回是否在奇偶页打印不同的页眉/页脚文本和格式；否则返回打印设置信息。

___

### <a id="firstpagenumber" name="firstpagenumber"></a> firstPageNumber

▸ **firstPageNumber**(`value?`): `any`

获取或设置在偶数页打印的页码。

**`example`**
```javascript
activeSheet.setArray(0, 0, new Array(60).fill(["sample text"]));
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.firstPageNumber(5);
printInfo.pageHeaderFooter({
    normal: {
        header: {
            left: "page number: &N"
        }
    }
});
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 在偶数页打印的页码。 |

#### Returns

`any`

如果未设置值，返回在偶数页打印的页码；否则返回打印设置信息。

___

### <a id="fitpagestall" name="fitpagestall"></a> fitPagesTall

▸ **fitPagesTall**(`value?`): `any`

获取或设置优化打印时要检查的垂直页数。

**`example`**
```javascript
activeSheet.setArray(0, 0, new Array(60).fill(["sample text"]));
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.fitPagesTall(1);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 优化打印时要检查的垂直页数。 |

#### Returns

`any`

如果未设置值，返回要检查的垂直页数；否则返回打印设置信息。

___

### <a id="fitpageswide" name="fitpageswide"></a> fitPagesWide

▸ **fitPagesWide**(`value?`): `any`

获取或设置优化打印时要检查的水平页数。

**`example`**
```javascript
activeSheet.setArray(0, 0, [new Array(16).fill("A")]);
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.fitPagesWide(1);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 优化打印时要检查的水平页数。 |

#### Returns

`any`

如果未设置值，返回要检查的水平页数；否则返回打印设置信息。

___

### <a id="margin" name="margin"></a> margin

▸ **margin**(`value?`): `any`

获取或设置打印边距，以英寸的百分之一为单位。

**`example`**
```javascript
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

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`PrintMargins`](../interfaces/GC.Spread.Sheets.Print.PrintMargins.md) | 打印边距。 |

#### Returns

`any`

如果未设置值，返回打印边距；否则返回打印设置信息。

___

### <a id="orientation" name="orientation"></a> orientation

▸ **orientation**(`value?`): `any`

获取或设置打印时使用的页面方向。

**`example`**
```javascript
activeSheet.setArray(0, 0, [['Title 1', 'Title 2'], [1, 2], [3, 4]]);
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
// 指定打印时的页面方向。
printInfo.orientation(GC.Spread.Sheets.Print.PrintPageOrientation.landscape);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`PrintPageOrientation`](../enums/GC.Spread.Sheets.Print.PrintPageOrientation.md) | 打印时使用的页面方向。 |

#### Returns

`any`

如果未设置值，返回打印时使用的页面方向；否则返回打印设置信息。

___

### <a id="pageheaderfooter" name="pageheaderfooter"></a> pageHeaderFooter

▸ **pageHeaderFooter**(`value?`): `any`

获取或设置打印页面上自定义页眉/页脚的文本和格式选项。

**`example`**
```javascript
activeSheet.setArray(0, 0, new Array(60).fill(["sample text"]));
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.pageHeaderFooter({
     normal: {
         header: {
             left: "It is &T.",
             center: "&SThis is text.",
             right: "&BHeader"
         }
     }
});
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`IPageCustomHeaderFooterOptions`](../interfaces/GC.Spread.Sheets.Print.IPageCustomHeaderFooterOptions.md) | 打印页面上自定义页眉/页脚的文本和格式选项。 |

#### Returns

`any`

如果未设置值，返回打印页面上自定义页眉/页脚的文本和格式选项；否则返回打印设置信息。

___

### <a id="pageorder" name="pageorder"></a> pageOrder

▸ **pageOrder**(`value?`): `any`

获取或设置打印页面的顺序。

**`example`**
```javascript
activeSheet.setRowCount(200);
activeSheet.setColumnCount(20);
activeSheet.setArray(0, 0, Array.from({ length: 200 }, (_, i) => [i]));
activeSheet.setArray(0, 0, [Array.from({ length: 20 }, (_, i) => i)]);
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.pageOrder(GC.Spread.Sheets.Print.PrintPageOrder.auto);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`PrintPageOrder`](../enums/GC.Spread.Sheets.Print.PrintPageOrder.md) | 打印页面的顺序。 |

#### Returns

`any`

如果未设置值，返回指定打印页面顺序的值；否则返回打印设置信息。

___

### <a id="pagerange" name="pagerange"></a> pageRange

▸ **pageRange**(`value?`): `any`

获取或设置打印的页面范围。

**`example`**
```javascript
activeSheet.setRowCount(200);
activeSheet.setArray(0, 0, Array.from({ length: 200 }, (_, i) => [i]));
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.pageRange("1-3");
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 从文档开头计数的页码或页面范围，用逗号分隔。例如，输入"1,3,5-12"。 |

#### Returns

`any`

如果未设置值，返回提供页码或页面范围的字符串；否则返回打印设置信息。

___

### <a id="papersize" name="papersize"></a> paperSize

▸ **paperSize**(`value?`): `any`

获取或设置打印的纸张尺寸。

**`example`**
```javascript
activeSheet.setArray(0, 0, new Array(20).fill(["sample text"]));
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.paperSize(new GC.Spread.Sheets.Print.PaperSize(300, 300));
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`PaperSize`](GC.Spread.Sheets.Print.PaperSize.md) | 打印的纸张尺寸。 |

#### Returns

`any`

如果未设置值，返回打印的纸张尺寸；否则返回打印设置信息。

___

### <a id="qualityfactor" name="qualityfactor"></a> qualityFactor

▸ **qualityFactor**(`value?`): `any`

获取或设置打印的质量因子。

**`example`**
```javascript
activeSheet.setArray(0, 0, new Array(20).fill(["sample text"]));
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.qualityFactor(6);
activeSheet.printInfo(printInfo);
spread.print();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 打印的质量因子是1到8之间的正整数。质量因子越大，打印质量越好。当质量因子较大时，会影响打印效率。 |

#### Returns

`any`

如果未设置值，返回打印的质量因子；否则返回打印设置信息。

___

### <a id="repeatcolumnend" name="repeatcolumnend"></a> repeatColumnEnd

▸ **repeatColumnEnd**(`value?`): `any`

获取或设置要在每页左侧重复打印的列范围的最后一列。

**`example`**
```javascript
activeSheet.setArray(0, 0, [['Title 1', 'Title 2']]);
activeSheet.setArray(0, 2, [Array.from({ length: 18 }, (_, i) => i)]);
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.repeatColumnStart(0);
printInfo.repeatColumnEnd(1);
activeSheet.printInfo(printInfo);
spread.print(); // "Title 1" 和 "Title 2" 将在每页重复打印。
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 要在每页左侧重复打印的列范围的最后一列。 |

#### Returns

`any`

如果未设置值，返回要在每页左侧重复打印的列范围的最后一列；否则返回打印设置信息。

___

### <a id="repeatcolumnstart" name="repeatcolumnstart"></a> repeatColumnStart

▸ **repeatColumnStart**(`value?`): `any`

获取或设置要在每页左侧重复打印的列范围的第一列。

**`example`**
```javascript
activeSheet.setArray(0, 0, [['Title 1', 'Title 2']]);
activeSheet.setArray(0, 2, [Array.from({ length: 18 }, (_, i) => i)]);
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.repeatColumnStart(0);
printInfo.repeatColumnEnd(1);
activeSheet.printInfo(printInfo);
spread.print(); // "Title 1" 和 "Title 2" 将在每页重复打印。
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 要在每页左侧重复打印的列范围的第一列。 |

#### Returns

`any`

如果未设置值，返回要在每页左侧重复打印的列范围的第一列；否则返回打印设置信息。

___

### <a id="repeatrowend" name="repeatrowend"></a> repeatRowEnd

▸ **repeatRowEnd**(`value?`): `any`

获取或设置要在每页顶部重复打印的行范围的最后一行。

**`example`**
```javascript
activeSheet.setArray(0, 0, [['Title 1'], ['Title 2']]);
activeSheet.setArray(2, 0, Array.from({ length: 60 }, (_, i) => [i]));
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.repeatRowStart(0);
printInfo.repeatRowEnd(1);
activeSheet.printInfo(printInfo);
spread.print(); // "Title 1" 和 "Title 2" 将在每页重复打印。
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 要在每页顶部重复打印的行范围的最后一行。 |

#### Returns

`any`

如果未设置值，返回要在每页顶部重复打印的行范围的最后一行；否则返回打印设置信息。

___

### <a id="repeatrowstart" name="repeatrowstart"></a> repeatRowStart

▸ **repeatRowStart**(`value?`): `any`

获取或设置要在每页顶部打印的重复行范围的第一行。

**`example`**
```javascript
activeSheet.setArray(0, 0, [['Title 1'], ['Title 2']]);
activeSheet.setArray(2, 0, Array.from({ length: 60 }, (_, i) => [i]));
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.repeatRowStart(0);
printInfo.repeatRowEnd(1);
activeSheet.printInfo(printInfo);
spread.print(); // "Title 1" and "Title 2" will be printed repeatedly on each page.
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 要在每页顶部打印的重复行范围的第一行。 |

#### Returns

`any`

如果未设置值，则返回要在每页顶部打印的重复行范围的第一行；否则返回打印设置信息。

___

### <a id="rowend" name="rowend"></a> rowEnd

▸ **rowEnd**(`value?`): `any`

获取或设置打印单元格范围时的最后一行。

**`example`**
```javascript
activeSheet.setColumnCount(3);
activeSheet.setArray(0, 0, new Array(60).fill(["sample text"]));
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.rowStart(0);
printInfo.rowEnd(2);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 打印单元格范围时的最后一行。 |

#### Returns

`any`

如果未设置值，返回打印单元格范围时的最后一行；否则返回打印设置信息。

___

### <a id="rowstart" name="rowstart"></a> rowStart

▸ **rowStart**(`value?`): `any`

获取或设置打印单元格范围时的第一行。

**`example`**
```javascript
activeSheet.setColumnCount(3);
activeSheet.setArray(0, 0, new Array(60).fill(["sample text"]));
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.rowStart(0);
printInfo.rowEnd(2);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 打印单元格范围时的第一行。 |

#### Returns

`any`

如果未设置值，返回打印单元格范围时的第一行；否则返回打印设置信息。

___

### <a id="showborder" name="showborder"></a> showBorder

▸ **showBorder**(`value?`): `any`

获取或设置是否打印整个控件的外边框。

**`example`**
```javascript
activeSheet.setArray(0, 0, [['Title 1', 'Title 2'], [1, 2], [3, 4]]);
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.showBorder(false);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否打印整个控件的外边框。 |

#### Returns

`any`

如果未设置值，返回是否打印整个控件的外边框；否则返回打印设置信息。

___

### <a id="showcolumnheader" name="showcolumnheader"></a> showColumnHeader

▸ **showColumnHeader**(`value?`): `any`

获取或设置是否打印列标题。

**`example`**
```javascript
activeSheet.setArray(0, 0, [['Title 1', 'Title 2'], [1, 2], [3, 4]]);
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.showColumnHeader(GC.Spread.Sheets.Print.PrintVisibilityType.hide);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`PrintVisibilityType`](../enums/GC.Spread.Sheets.Print.PrintVisibilityType.md) | 是否打印列标题。 |

#### Returns

`any`

如果未设置值，返回是否打印列标题；否则返回打印设置信息。

___

### <a id="showgridline" name="showgridline"></a> showGridLine

▸ **showGridLine**(`value?`): `any`

获取或设置是否打印网格线。

**`example`**
```javascript
activeSheet.setArray(0, 0, [['Title 1', 'Title 2'], [1, 2], [3, 4]]);
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.showGridLine(true);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否打印网格线。 |

#### Returns

`any`

如果未设置值，返回是否打印网格线；否则返回打印设置信息。

___

### <a id="showrowheader" name="showrowheader"></a> showRowHeader

▸ **showRowHeader**(`value?`): `any`

获取或设置是否打印行标题。

**`example`**
```javascript
activeSheet.setArray(0, 0, [['Title 1', 'Title 2'], [1, 2], [3, 4]]);
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.showRowHeader(GC.Spread.Sheets.Print.PrintVisibilityType.hide);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`PrintVisibilityType`](../enums/GC.Spread.Sheets.Print.PrintVisibilityType.md) | 是否打印行标题。 |

#### Returns

`any`

如果未设置值，返回是否打印行标题；否则返回打印设置信息。

___

### <a id="usemax" name="usemax"></a> useMax

▸ **useMax**(`value?`): `any`

获取或设置是否仅打印包含数据的行和列。

**`example`**
```javascript
var activeSheet = spread.getActiveSheet();
activeSheet.setArray(0, 0, [['Title 1', 'Title 2'], [1, 2], [3, 4]]);
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.useMax(true);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否仅打印包含数据的行和列。 |

#### Returns

`any`

如果未设置值，返回是否仅打印包含数据的行和列；否则返回打印设置信息。

___

### <a id="watermark" name="watermark"></a> watermark

▸ **watermark**(`value?`): `any`

获取或设置所有水印。

**`example`**
```javascript
// 此示例展示如何设置水印。
var printInfo = activeSheet.printInfo();
printInfo.watermark([{x:0, y:0, width:100, height:100, imageSrc:".image/watermark.jpg", page:"all"}]);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`IWatermarkItem`](../interfaces/GC.Spread.Sheets.Print.IWatermarkItem.md)[] | 水印项。 |

#### Returns

`any`

水印项。

___

### <a id="zoomfactor" name="zoomfactor"></a> zoomFactor

▸ **zoomFactor**(`value?`): `any`

获取或设置用于打印的缩放因子。

**`example`**
```javascript
activeSheet.setArray(0, 0, [['Title 1', 'Title 2'], [1, 2], [3, 4]]);
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.zoomFactor(2);
activeSheet.printInfo(printInfo);
spread.print(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 用于打印的缩放因子。 |

#### Returns

`any`

如果未设置值，返回指定放大或缩小打印工作表的数值；否则返回打印设置信息。
