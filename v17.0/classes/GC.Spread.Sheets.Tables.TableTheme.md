# Class: TableTheme

[Sheets](../modules/GC.Spread.Sheets.md).[Tables](../modules/GC.Spread.Sheets.Tables.md).TableTheme

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Tables.TableTheme.md#constructor)

### Methods

- [firstColumnStripSize](GC.Spread.Sheets.Tables.TableTheme.md#firstcolumnstripsize)
- [firstColumnStripStyle](GC.Spread.Sheets.Tables.TableTheme.md#firstcolumnstripstyle)
- [firstFooterCellStyle](GC.Spread.Sheets.Tables.TableTheme.md#firstfootercellstyle)
- [firstHeaderCellStyle](GC.Spread.Sheets.Tables.TableTheme.md#firstheadercellstyle)
- [firstRowStripSize](GC.Spread.Sheets.Tables.TableTheme.md#firstrowstripsize)
- [firstRowStripStyle](GC.Spread.Sheets.Tables.TableTheme.md#firstrowstripstyle)
- [footerRowStyle](GC.Spread.Sheets.Tables.TableTheme.md#footerrowstyle)
- [headerRowStyle](GC.Spread.Sheets.Tables.TableTheme.md#headerrowstyle)
- [highlightFirstColumnStyle](GC.Spread.Sheets.Tables.TableTheme.md#highlightfirstcolumnstyle)
- [highlightLastColumnStyle](GC.Spread.Sheets.Tables.TableTheme.md#highlightlastcolumnstyle)
- [lastFooterCellStyle](GC.Spread.Sheets.Tables.TableTheme.md#lastfootercellstyle)
- [lastHeaderCellStyle](GC.Spread.Sheets.Tables.TableTheme.md#lastheadercellstyle)
- [name](GC.Spread.Sheets.Tables.TableTheme.md#name)
- [secondColumnStripSize](GC.Spread.Sheets.Tables.TableTheme.md#secondcolumnstripsize)
- [secondColumnStripStyle](GC.Spread.Sheets.Tables.TableTheme.md#secondcolumnstripstyle)
- [secondRowStripSize](GC.Spread.Sheets.Tables.TableTheme.md#secondrowstripsize)
- [secondRowStripStyle](GC.Spread.Sheets.Tables.TableTheme.md#secondrowstripstyle)
- [wholeTableStyle](GC.Spread.Sheets.Tables.TableTheme.md#wholetablestyle)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new TableTheme**()

表格样式设置

**`代码示例`**
```
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
    new GC.Spread.Sheets.LineBorder("blue", GC.Spread.Sheets.LineStyle.thick));
tableStyle.headerRowStyle(tableStyleInfo);
var table = activeSheet.tables.add("table1", 1, 1, 5, 5, tableStyle);
```

## Methods

### <a id="firstcolumnstripsize" name="firstcolumnstripsize"></a> firstColumnStripSize

▸ **firstColumnStripSize**(`value?`): `any`

获取或设置第一个交替列的大小

**`代码示例`**
```
//本示例创建了一个表
var tableStyle = new GC.Spread.Sheets.Tables.TableTheme();
var thinBorder = new GC.Spread.Sheets.LineBorder("black", GC.Spread.Sheets.LineStyle.dotted);
tableStyle.wholeTableStyle(new GC.Spread.Sheets.Tables.TableStyle("aliceblue", "green", "bold 10pt arial", thinBorder, thinBorder, thinBorder, thinBorder, thinBorder, thinBorder));
//style
var tStyleInfo = new GC.Spread.Sheets.Tables.TableStyle();
tStyleInfo.backColor = "green";
tStyleInfo.foreColor = "red";
tStyleInfo.borderBottom = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.borderLeft = new GC.Spread.Sheets.LineBorder("yellow", GC.Spread.Sheets.LineStyle.medium);
tStyleInfo.borderTop = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.borderRight = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.font = "bold 11pt arial";
tableStyle.firstColumnStripSize(2);
tableStyle.firstColumnStripStyle(tStyleInfo);
var sTable = activeSheet.tables.add("Custom", 1, 1, 10, 5, tableStyle);
sTable.bandColumns(true);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置任何值，则返回第一交替列的大小；否则，返回表格主题

___

### <a id="firstcolumnstripstyle" name="firstcolumnstripstyle"></a> firstColumnStripStyle

▸ **firstColumnStripStyle**(`value?`): `any`

获取或设置第一个交替列的样式

**`代码示例`**
```
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
tableStyle.firstColumnStripSize(2);
tableStyle.firstColumnStripStyle(tStyleInfo);
var sTable = activeSheet.tables.add("Custom", 1, 1, 10, 5, tableStyle);
sTable.bandColumns(true);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`TableStyle`](GC.Spread.Sheets.Tables.TableStyle.md) |

#### Returns

`any`

如果未设置任何值，则返回第一个交替列的样式；否则，返回表格主题

___

### <a id="firstfootercellstyle" name="firstfootercellstyle"></a> firstFooterCellStyle

▸ **firstFooterCellStyle**(`value?`): `any`

获取或设置第一个页脚单元格的样式

**`代码示例`**
```
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
tableStyle.firstFooterCellStyle(tStyleInfo);
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, tableStyle);
sTable.showFooter(true);
//set footer value
sTable.setColumnValue(0, "Total");
sTable.highlightFirstColumn(true);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`TableStyle`](GC.Spread.Sheets.Tables.TableStyle.md) |

#### Returns

`any`

如果未设置任何值，则返回第一个页脚单元格的样式；否则，返回表格主题

___

### <a id="firstheadercellstyle" name="firstheadercellstyle"></a> firstHeaderCellStyle

▸ **firstHeaderCellStyle**(`value?`): `any`

获取或设置第一个页眉单元格的样式

**`代码示例`**
```
var tableStyle = new GC.Spread.Sheets.TableStyle();
var thinBorder = new GC.Spread.Sheets.LineBorder("black", GC.Spread.Sheets.LineStyle.dotted);
tableStyle.wholeTableStyle(new GC.Spread.Sheets.TableStyleInfo("aliceblue", "green", "bold 10pt arial", thinBorder, thinBorder, thinBorder, thinBorder, thinBorder, thinBorder));
var tStyleInfo = new GC.Spread.Sheets.TableStyleInfo();
tStyleInfo.backColor = "green";
tStyleInfo.foreColor = "red";
tStyleInfo.borderBottom = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.borderLeft = new GC.Spread.Sheets.LineBorder("yellow", GC.Spread.Sheets.LineStyle.medium);
tStyleInfo.borderTop = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.borderRight = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.font = "bold 11pt arial";
tableStyle.firstHeaderCellStyle(tStyleInfo);
var sTable = activeSheet.addTable("table1", 1, 1, 10, 5, tableStyle);
sTable.highlightFirstColumn(true);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`TableStyle`](GC.Spread.Sheets.Tables.TableStyle.md) |

#### Returns

`any`

如果未设置任何值，则返回第一个页眉单元格的样式；否则，返回表格主题

___

### <a id="firstrowstripsize" name="firstrowstripsize"></a> firstRowStripSize

▸ **firstRowStripSize**(`value?`): `any`

获取或设置第一个交替行的大小

**`代码示例`**
```
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
tableStyle.firstRowStripSize(2);
tableStyle.firstRowStripStyle(tStyleInfo);
activeSheet.tables.add("Custom", 1, 1, 10, 5, tableStyle);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置任何值，则返回第一交替行的大小；否则，返回表格主题

___

### <a id="firstrowstripstyle" name="firstrowstripstyle"></a> firstRowStripStyle

▸ **firstRowStripStyle**(`value?`): `any`

获取或设置第一个交替行样式

**`代码示例`**
```
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
tableStyle.firstRowStripSize(2);
tableStyle.firstRowStripStyle(tStyleInfo);
activeSheet.tables.add("Custom", 1, 1, 10, 5, tableStyle);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`TableStyle`](GC.Spread.Sheets.Tables.TableStyle.md) |

#### Returns

`any`

如果未设置任何值，则返回第一个交替行样式；否则，返回表格主题

___

### <a id="footerrowstyle" name="footerrowstyle"></a> footerRowStyle

▸ **footerRowStyle**(`value?`): `any`

获取或设置页脚区域的默认样式

**`代码示例`**
```
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
tableStyle.footerRowStyle(tStyleInfo);
var sTable = activeSheet.tables.add("Custom", 1, 1, 10, 5, tableStyle);
sTable.showFooter(true);
//设置页脚值
sTable.setColumnValue(0, "Total");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`TableStyle`](GC.Spread.Sheets.Tables.TableStyle.md) |

#### Returns

`any`

如果未设置任何值，则返回页脚区域的默认样式 否则，返回表格主题

___

### <a id="headerrowstyle" name="headerrowstyle"></a> headerRowStyle

▸ **headerRowStyle**(`value?`): `any`

获取或设置页眉区域的默认样式

**`代码示例`**
```
var tableStyle = new GC.Spread.Sheets.Tables.TableTheme();
tableStyle.wholeTableStyle(new GC.Spread.Sheets.Tables.TableStyle("aliceblue"));
var tableStyleInfo = new GC.Spread.Sheets.Tables.TableStyle(
    "black",
    "white",
    "bold 11pt arial",
    new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin),
    new GC.Spread.Sheets.LineBorder("red", GC.Spread.Sheets.LineStyle.thick),
    new GC.Spread.Sheets.LineBorder("yellow", GC.Spread.Sheets.LineStyle.thin),
    new GC.Spread.Sheets.LineBorder("blue", GC.Spread.Sheets.LineStyle.thick));
tableStyle.headerRowStyle(tableStyleInfo);
var table = activeSheet.tables.add("table1", 1, 1, 5, 5, tableStyle);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`TableStyle`](GC.Spread.Sheets.Tables.TableStyle.md) |

#### Returns

`any`

如果未设置任何值，则返回页眉区域的默认样式；否则，返回表格主题

___

### <a id="highlightfirstcolumnstyle" name="highlightfirstcolumnstyle"></a> highlightFirstColumnStyle

▸ **highlightFirstColumnStyle**(`value?`): `any`

获取或设置第一列的样式

**`代码示例`**
```
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
tableStyle.highlightFirstColumnStyle(tStyleInfo);
var sTable = activeSheet.tables.add("Custom", 1, 1, 10, 5, tableStyle);
sTable.highlightFirstColumn(true);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`TableStyle`](GC.Spread.Sheets.Tables.TableStyle.md) |

#### Returns

`any`

如果未设置任何值，则返回第一列的样式 否则，返回表格主题

___

### <a id="highlightlastcolumnstyle" name="highlightlastcolumnstyle"></a> highlightLastColumnStyle

▸ **highlightLastColumnStyle**(`value?`): `any`

获取或设置最后一列的样式

**`代码示例`**
```
var tableStyle = new GC.Spread.Sheets.Tables.TableTheme();
var thinBorder = new GC.Spread.Sheets.LineBorder("black", GC.Spread.Sheets.LineStyle.dotted);
tableStyle.wholeTableStyle(new GC.Spread.Sheets.Tables.TableStyle("aliceblue", "green", "bold 10pt arial", thinBorder, thinBorder, thinBorder, thinBorder, thinBorder, thinBorder));
//style
var tStyleInfo = new GC.Spread.Sheets.Tables.TableStyle();
tStyleInfo.backColor = "green";
tStyleInfo.foreColor = "red";
tStyleInfo.borderBottom = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.borderLeft = new GC.Spread.Sheets.LineBorder("yellow", GC.Spread.Sheets.LineStyle.medium);
tStyleInfo.borderTop = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.borderRight = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.font = "bold 11pt arial";
tableStyle.highlightLastColumnStyle(tStyleInfo);
var sTable = activeSheet.tables.add("Custom", 1, 1, 10, 5, tableStyle);
sTable.highlightLastColumn(true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`TableStyle`](GC.Spread.Sheets.Tables.TableStyle.md) | 最后一列的样式 |

#### Returns

`any`

如果未设置任何值，则返回最后一列的样式 否则，返回表格主题

___

### <a id="lastfootercellstyle" name="lastfootercellstyle"></a> lastFooterCellStyle

▸ **lastFooterCellStyle**(`value?`): `any`

获取或设置最后一个页脚单元格的样式

**`代码示例`**
```
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
tableStyle.lastFooterCellStyle(tStyleInfo);
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, tableStyle);
sTable.showFooter(true);
//set footer formula
sTable.setColumnFormula(4, "SUM(F3:F11)");
sTable.highlightLastColumn(true);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`TableStyle`](GC.Spread.Sheets.Tables.TableStyle.md) |

#### Returns

`any`

如果未设置任何值，则返回最后一个页脚单元格的样式；否则，返回表格主题

___

### <a id="lastheadercellstyle" name="lastheadercellstyle"></a> lastHeaderCellStyle

▸ **lastHeaderCellStyle**(`value?`): `any`

获取或设置最后一个页眉单元格的样式

**`代码示例`**
```
var tableStyle = new GC.Spread.Sheets.TableStyle();
var thinBorder = new GC.Spread.Sheets.LineBorder("black", GC.Spread.Sheets.LineStyle.dotted);
tableStyle.wholeTableStyle(new GC.Spread.Sheets.TableStyleInfo("aliceblue", "green", "bold 10pt arial", thinBorder, thinBorder, thinBorder, thinBorder, thinBorder, thinBorder));
var tStyleInfo = new GC.Spread.Sheets.TableStyleInfo();
tStyleInfo.backColor = "green";
tStyleInfo.foreColor = "red";
tStyleInfo.borderBottom = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.borderLeft = new GC.Spread.Sheets.LineBorder("yellow", GC.Spread.Sheets.LineStyle.medium);
tStyleInfo.borderTop = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.borderRight = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.font = "bold 11pt arial";
tableStyle.lastHeaderCellStyle(tStyleInfo);
var sTable = activeSheet.addTable("table1", 1, 1, 10, 5, tableStyle);
sTable.highlightLastColumn(true);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`TableStyle`](GC.Spread.Sheets.Tables.TableStyle.md) |

#### Returns

`any`

如果未设置任何值，则返回最后一个标题单元格的样式；否则，返回表格主题

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置样式的名称

**`代码示例`**
```
var tableStyle = new GC.Spread.Sheets.TableStyle();
var thinBorder = new GC.Spread.Sheets.LineBorder("black", GC.Spread.Sheets.LineStyle.dotted);
tableStyle.wholeTableStyle(new GC.Spread.Sheets.TableStyleInfo("aliceblue", "green", "bold 10pt arial", thinBorder, thinBorder, thinBorder, thinBorder, thinBorder, thinBorder));
var tStyleInfo = new GC.Spread.Sheets.TableStyleInfo();
tStyleInfo.backColor = "green";
tStyleInfo.foreColor = "red";
tStyleInfo.borderBottom = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.borderLeft = new GC.Spread.Sheets.LineBorder("yellow", GC.Spread.Sheets.LineStyle.medium);
tStyleInfo.borderTop = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.borderRight = new GC.Spread.Sheets.LineBorder("green", GC.Spread.Sheets.LineStyle.thin);
tStyleInfo.font = "bold 11pt arial";
tableStyle.name("tstyle");
tableStyle.firstColumnStripSize(2);
tableStyle.firstColumnStripStyle(tStyleInfo);
var sTable = activeSheet.addTable("Custom", 1, 1, 10, 5, tableStyle);
sTable.bandColumns(true);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置值，则返回样式的名称；否则，返回表主题

___

### <a id="secondcolumnstripsize" name="secondcolumnstripsize"></a> secondColumnStripSize

▸ **secondColumnStripSize**(`value?`): `any`

获取或设置第二个交替列的大小

**`代码示例`**
```
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
tableStyle.secondColumnStripSize(2);
tableStyle.secondColumnStripStyle(tStyleInfo);
var sTable = activeSheet.tables.add("Custom", 1, 1, 10, 5, tableStyle);
sTable.bandColumns(true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 第二个交替列的大小 |

#### Returns

`any`

如果未设置任何值，则返回第二个交替列的大小；否则，返回表格主题

___

### <a id="secondcolumnstripstyle" name="secondcolumnstripstyle"></a> secondColumnStripStyle

▸ **secondColumnStripStyle**(`value?`): `any`

获取或设置第二个交替列的样式

**`代码示例`**
```
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
tableStyle.secondColumnStripSize(2);
tableStyle.secondColumnStripStyle(tStyleInfo);
var sTable = activeSheet.tables.add("Custom", 1, 1, 10, 5, tableStyle);
sTable.bandColumns(true);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`TableStyle`](GC.Spread.Sheets.Tables.TableStyle.md) |

#### Returns

`any`

如果未设置任何值，则返回第二个交替列的样式；否则，返回表格主题

___

### <a id="secondrowstripsize" name="secondrowstripsize"></a> secondRowStripSize

▸ **secondRowStripSize**(`value?`): `any`

获取或设置第二个交替行的大小

**`代码示例`**
```
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
tableStyle.secondRowStripSize(2);
tableStyle.secondRowStripStyle(tStyleInfo);
activeSheet.tables.add("Custom", 1, 1, 10, 5, tableStyle);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置任何值，则返回第二个交替行的大小；否则，返回表格主题

___

### <a id="secondrowstripstyle" name="secondrowstripstyle"></a> secondRowStripStyle

▸ **secondRowStripStyle**(`value?`): `any`

获取或设置第二个交替行样式

**`代码示例`**
```
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
tableStyle.secondRowStripSize(2);
tableStyle.secondRowStripStyle(tStyleInfo);
activeSheet.tables.add("Custom", 1, 1, 10, 5, tableStyle);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`TableStyle`](GC.Spread.Sheets.Tables.TableStyle.md) |

#### Returns

`any`

如果未设置任何值，则返回第二个交替的行样式；否则，返回表格主题

___

### <a id="wholetablestyle" name="wholetablestyle"></a> wholeTableStyle

▸ **wholeTableStyle**(`value?`): `any`

获取或设置数据区域的默认样式

**`代码示例`**
```
var tableStyle = new GC.Spread.Sheets.Tables.TableTheme();
var thinBorder = new GC.Spread.Sheets.LineBorder("black", GC.Spread.Sheets.LineStyle.dotted);
tableStyle.wholeTableStyle(new GC.Spread.Sheets.Tables.TableStyle("aliceblue", "green", "bold 10pt arial", thinBorder, thinBorder, thinBorder, thinBorder, thinBorder, thinBorder));
var table = activeSheet.tables.add("table1", 1, 1, 5, 5, tableStyle);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`TableStyle`](GC.Spread.Sheets.Tables.TableStyle.md) |

#### Returns

`any`

如果未设置任何值，则返回数据区域的默认样式 否则，返回表格主题
