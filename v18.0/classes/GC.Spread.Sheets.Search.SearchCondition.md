# Class: SearchCondition

[Sheets](../modules/GC.Spread.Sheets.md).[Search](../modules/GC.Spread.Sheets.Search.md).SearchCondition

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Search.SearchCondition.md#constructor)

### Properties

- [columnEnd](GC.Spread.Sheets.Search.SearchCondition.md#columnend)
- [columnStart](GC.Spread.Sheets.Search.SearchCondition.md#columnstart)
- [endSheetIndex](GC.Spread.Sheets.Search.SearchCondition.md#endsheetindex)
- [rowEnd](GC.Spread.Sheets.Search.SearchCondition.md#rowend)
- [rowStart](GC.Spread.Sheets.Search.SearchCondition.md#rowstart)
- [searchFlags](GC.Spread.Sheets.Search.SearchCondition.md#searchflags)
- [searchOrder](GC.Spread.Sheets.Search.SearchCondition.md#searchorder)
- [searchString](GC.Spread.Sheets.Search.SearchCondition.md#searchstring)
- [searchTarget](GC.Spread.Sheets.Search.SearchCondition.md#searchtarget)
- [sheetArea](GC.Spread.Sheets.Search.SearchCondition.md#sheetarea)
- [startSheetIndex](GC.Spread.Sheets.Search.SearchCondition.md#startsheetindex)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new SearchCondition**()

定义搜索条件

**`代码示例`**
``` javascript
activeSheet.getCell(5,4).text("testSearch");
var searchCondition = new GC.Spread.Sheets.Search.SearchCondition();
searchCondition.searchString = "testSearch";
searchCondition.startSheetIndex = spread.getActiveSheetIndex();
searchCondition.endSheetIndex = spread.getActiveSheetIndex();
searchCondition.searchOrder = GC.Spread.Sheets.Search.SearchOrder.nOrder;
searchCondition.searchTarget = GC.Spread.Sheets.Search.SearchFoundFlags.cellText;
searchCondition.searchFlags = GC.Spread.Sheets.Search.SearchFlags.ignoreCase| GC.Spread.Sheets.Search.SearchFlags.useWildCards;
var searchresult= spread.search(searchCondition);
var str ="[searchFoundFlag:"+ searchresult.searchFoundFlag+",\r\n foundSheetIndex:"+searchresult.foundSheetIndex+",foundRowIndex:" + searchresult.foundRowIndex+", * foundColumnIndex:"+searchresult.foundColumnIndex+", foundString:"+searchresult.foundString+"]";
alert(str);
```

## Properties

### <a id="columnend" name="columnend"></a> columnEnd

• **columnEnd**: `number`

结束列的索引

**`代码示例`**
``` javascript
//本示例搜索一个单元格块
activeSheet.getCell(0,0).text("testSearch");
activeSheet.getCell(5,4).text("testSearch");
var searchCondition = new GC.Spread.Sheets.Search.SearchCondition();
searchCondition.searchString = "testSearch";
searchCondition.startSheetIndex = spread.getActiveSheetIndex();
searchCondition.endSheetIndex = spread.getActiveSheetIndex();
searchCondition.columnStart = 1;
searchCondition.columnEnd = 10;
searchCondition.rowStart = 1;
searchCondition.rowEnd = 10;
searchCondition.sheetArea = GC.Spread.Sheets.SheetArea.viewport;
searchCondition.searchOrder = GC.Spread.Sheets.Search.SearchOrder.nOrder;
searchCondition.searchTarget = GC.Spread.Sheets.Search.SearchFoundFlags.cellText;
searchCondition.searchFlags = GC.Spread.Sheets.Search.SearchFlags.blockRange;
var searchresult= spread.search(searchCondition);
var str ="[searchFoundFlag:"+ searchresult.searchFoundFlag+",\r\n foundSheetIndex:"+searchresult.foundSheetIndex+",foundRowIndex:" + searchresult.foundRowIndex+", foundColumnIndex:"+searchresult.foundColumnIndex+", foundString:"+searchresult.foundString+"]";
alert(str);
```

___

### <a id="columnstart" name="columnstart"></a> columnStart

• **columnStart**: `number`

开始的列的索引

**`代码示例`**
``` javascript
//本示例搜索一个单元格块
activeSheet.getCell(0,0).text("testSearch");
activeSheet.getCell(5,4).text("testSearch");
var searchCondition = new GC.Spread.Sheets.Search.SearchCondition();
searchCondition.searchString = "testSearch";
searchCondition.startSheetIndex = spread.getActiveSheetIndex();
searchCondition.endSheetIndex = spread.getActiveSheetIndex();
searchCondition.columnStart = 1;
searchCondition.columnEnd = 10;
searchCondition.rowStart = 1;
searchCondition.rowEnd = 10;
searchCondition.sheetArea = GC.Spread.Sheets.SheetArea.viewport;
searchCondition.searchOrder = GC.Spread.Sheets.Search.SearchOrder.nOrder;
searchCondition.searchTarget = GC.Spread.Sheets.Search.SearchFoundFlags.cellText;
searchCondition.searchFlags = GC.Spread.Sheets.Search.SearchFlags.blockRange;
var searchresult= spread.search(searchCondition);
var str ="[searchFoundFlag:"+ searchresult.searchFoundFlag+",\r\n foundSheetIndex:"+searchresult.foundSheetIndex+",foundRowIndex:" + searchresult.foundRowIndex+", foundColumnIndex:"+searchresult.foundColumnIndex+", foundString:"+searchresult.foundString+"]";
alert(str);
```

___

### <a id="endsheetindex" name="endsheetindex"></a> endSheetIndex

• **endSheetIndex**: `number`

结束搜索的工作表的索引

**`代码示例`**
``` javascript
activeSheet.getCell(5,4).text("testSearch");
var searchCondition = new GC.Spread.Sheets.Search.SearchCondition();
searchCondition.searchString = "testSearch";
searchCondition.startSheetIndex = spread.getActiveSheetIndex();
searchCondition.endSheetIndex = spread.getActiveSheetIndex();
searchCondition.searchOrder = GC.Spread.Sheets.Search.SearchOrder.nOrder;
searchCondition.searchTarget = GC.Spread.Sheets.Search.SearchFoundFlags.cellText;
searchCondition.searchFlags = GC.Spread.Sheets.Search.SearchFlags.ignoreCase| GC.Spread.Sheets.Search.SearchFlags.useWildCards;
var searchresult= spread.search(searchCondition);
var str ="[searchFoundFlag:"+ searchresult.searchFoundFlag+",\r\n foundSheetIndex:"+searchresult.foundSheetIndex+",foundRowIndex:" + searchresult.foundRowIndex+", foundColumnIndex:"+searchresult.foundColumnIndex+", foundString:"+searchresult.foundString+"]";
alert(str);
```

___

### <a id="rowend" name="rowend"></a> rowEnd

• **rowEnd**: `number`

结束行的索引

**`代码示例`**
``` javascript
//本示例搜索一个单元格块
activeSheet.getCell(0,0).text("testSearch");
activeSheet.getCell(5,4).text("testSearch");
var searchCondition = new GC.Spread.Sheets.Search.SearchCondition();
searchCondition.searchString = "testSearch";
searchCondition.startSheetIndex = spread.getActiveSheetIndex();
searchCondition.endSheetIndex = spread.getActiveSheetIndex();
searchCondition.columnStart = 1;
searchCondition.columnEnd = 10;
searchCondition.rowStart = 1;
searchCondition.rowEnd = 10;
searchCondition.sheetArea = GC.Spread.Sheets.SheetArea.viewport;
searchCondition.searchOrder = GC.Spread.Sheets.Search.SearchOrder.nOrder;
searchCondition.searchTarget = GC.Spread.Sheets.Search.SearchFoundFlags.cellText;
searchCondition.searchFlags = GC.Spread.Sheets.Search.SearchFlags.blockRange;
var searchresult= spread.search(searchCondition);
var str ="[searchFoundFlag:"+ searchresult.searchFoundFlag+",\r\n foundSheetIndex:"+searchresult.foundSheetIndex+",foundRowIndex:" + searchresult.foundRowIndex+", foundColumnIndex:"+searchresult.foundColumnIndex+", foundString:"+searchresult.foundString+"]";
alert(str);
```

___

### <a id="rowstart" name="rowstart"></a> rowStart

• **rowStart**: `number`

开始行的索引

**`代码示例`**
``` javascript
//本示例搜索一个单元格块
activeSheet.getCell(0,0).text("testSearch");
activeSheet.getCell(5,4).text("testSearch");
var searchCondition = new GC.Spread.Sheets.Search.SearchCondition();
searchCondition.searchString = "testSearch";
searchCondition.startSheetIndex = spread.getActiveSheetIndex();
searchCondition.endSheetIndex = spread.getActiveSheetIndex();
searchCondition.columnStart = 1;
searchCondition.columnEnd = 10;
searchCondition.rowStart = 1;
searchCondition.rowEnd = 10;
searchCondition.sheetArea = GC.Spread.Sheets.SheetArea.viewport;
searchCondition.searchOrder = GC.Spread.Sheets.Search.SearchOrder.nOrder;
searchCondition.searchTarget = GC.Spread.Sheets.Search.SearchFoundFlags.cellText;
searchCondition.searchFlags = GC.Spread.Sheets.Search.SearchFlags.blockRange;
var searchresult= spread.search(searchCondition);
var str ="[searchFoundFlag:"+ searchresult.searchFoundFlag+",\r\n foundSheetIndex:"+searchresult.foundSheetIndex+",foundRowIndex:" + searchresult.foundRowIndex+", foundColumnIndex:"+searchresult.foundColumnIndex+", foundString:"+searchresult.foundString+"]";
alert(str);
```

___

### <a id="searchflags" name="searchflags"></a> searchFlags

• **searchFlags**: [`SearchFlags`](../enums/GC.Spread.Sheets.Search.SearchFlags.md)

搜索选项的枚举

**`代码示例`**
``` javascript
//本示例设置searchFlags属性
activeSheet.getCell(5,4).text("testSearch");
var searchCondition = new GC.Spread.Sheets.Search.SearchCondition();
searchCondition.searchString = "testSearch";
searchCondition.startSheetIndex = spread.getActiveSheetIndex();
searchCondition.endSheetIndex = spread.getActiveSheetIndex();
searchCondition.searchOrder = GC.Spread.Sheets.Search.SearchOrder.nOrder;
searchCondition.searchTarget = GC.Spread.Sheets.Search.SearchFoundFlags.cellText;
searchCondition.searchFlags = GC.Spread.Sheets.Search.SearchFlags.ignoreCase| GC.Spread.Sheets.Search.SearchFlags.useWildCards;
var searchresult= spread.search(searchCondition);
var str ="[searchFoundFlag:"+ searchresult.searchFoundFlag+",\r\n foundSheetIndex:"+searchresult.foundSheetIndex+",foundRowIndex:" + searchresult.foundRowIndex+", foundColumnIndex:"+searchresult.foundColumnIndex+", foundString:"+searchresult.foundString+"]";
alert(str);
```

___

### <a id="searchorder" name="searchorder"></a> searchOrder

• **searchOrder**: [`SearchOrder`](../enums/GC.Spread.Sheets.Search.SearchOrder.md)

该枚举指定按(列，行)或(行，列)的坐标进行搜索

**`代码示例`**
``` javascript
//本示例设置searchFlags属性
activeSheet.getCell(5,4).text("testSearch");
var searchCondition = new GC.Spread.Sheets.Search.SearchCondition();
searchCondition.searchString = "testSearch";
searchCondition.startSheetIndex = spread.getActiveSheetIndex();
searchCondition.endSheetIndex = spread.getActiveSheetIndex();
searchCondition.searchOrder = GC.Spread.Sheets.Search.SearchOrder.nOrder;
searchCondition.searchTarget = GC.Spread.Sheets.Search.SearchFoundFlags.cellText;
searchCondition.searchFlags = GC.Spread.Sheets.Search.SearchFlags.ignoreCase| GC.Spread.Sheets.Search.SearchFlags.useWildCards;
var searchresult= spread.search(searchCondition);
var str ="[searchFoundFlag:"+ searchresult.searchFoundFlag+",\r\n foundSheetIndex:"+searchresult.foundSheetIndex+",foundRowIndex:" + searchresult.foundRowIndex+", foundColumnIndex:"+searchresult.foundColumnIndex+", foundString:"+searchresult.foundString+"]";
alert(str);
```

___

### <a id="searchstring" name="searchstring"></a> searchString

• **searchString**: `string`

要搜索的字符串

**`代码示例`**
``` javascript
//本示例设置searchFlags属性
activeSheet.getCell(5,4).text("testSearch");
var searchCondition = new GC.Spread.Sheets.Search.SearchCondition();
searchCondition.searchString = "testSearch";
searchCondition.startSheetIndex = spread.getActiveSheetIndex();
searchCondition.endSheetIndex = spread.getActiveSheetIndex();
searchCondition.searchOrder = GC.Spread.Sheets.Search.SearchOrder.nOrder;
searchCondition.searchTarget = GC.Spread.Sheets.Search.SearchFoundFlags.cellText;
searchCondition.searchFlags = GC.Spread.Sheets.Search.SearchFlags.ignoreCase| GC.Spread.Sheets.Search.SearchFlags.useWildCards;
var searchresult= spread.search(searchCondition);
var str ="[searchFoundFlag:"+ searchresult.searchFoundFlag+",\r\n foundSheetIndex:"+searchresult.foundSheetIndex+",foundRowIndex:" + searchresult.foundRowIndex+", foundColumnIndex:"+searchresult.foundColumnIndex+", foundString:"+searchresult.foundString+"]";
alert(str);
```

___

### <a id="searchtarget" name="searchtarget"></a> searchTarget

• **searchTarget**: [`SearchFoundFlags`](../enums/GC.Spread.Sheets.Search.SearchFoundFlags.md)

搜索是否包括单元格注释，标签或文本中的内容的枚举

**`代码示例`**
``` javascript
//本示例设置searchFlags属性
activeSheet.getCell(5,4).text("testSearch");
var searchCondition = new GC.Spread.Sheets.Search.SearchCondition();
searchCondition.searchString = "testSearch";
searchCondition.startSheetIndex = spread.getActiveSheetIndex();
searchCondition.endSheetIndex = spread.getActiveSheetIndex();
searchCondition.searchOrder = GC.Spread.Sheets.Search.SearchOrder.nOrder;
searchCondition.searchTarget = GC.Spread.Sheets.Search.SearchFoundFlags.cellText;
searchCondition.searchFlags = GC.Spread.Sheets.Search.SearchFlags.ignoreCase| GC.Spread.Sheets.Search.SearchFlags.useWildCards;
var searchresult= spread.search(searchCondition);
var str ="[searchFoundFlag:"+ searchresult.searchFoundFlag+",\r\n foundSheetIndex:"+searchresult.foundSheetIndex+",foundRowIndex:" + searchresult.foundRowIndex+", foundColumnIndex:"+searchresult.foundColumnIndex+", foundString:"+searchresult.foundString+"]";
alert(str);
```

___

### <a id="sheetarea" name="sheetarea"></a> sheetArea

• **sheetArea**: [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md)

工作表的搜索区域

**`代码示例`**
``` javascript
//本示例搜索一个单元格块
activeSheet.getCell(0,0).text("testSearch");
activeSheet.getCell(5,4).text("testSearch");
var searchCondition = new GC.Spread.Sheets.Search.SearchCondition();
searchCondition.searchString = "testSearch";
searchCondition.startSheetIndex = spread.getActiveSheetIndex();
searchCondition.endSheetIndex = spread.getActiveSheetIndex();
searchCondition.columnStart = 1;
searchCondition.columnEnd = 10;
searchCondition.rowStart = 1;
searchCondition.rowEnd = 10;
searchCondition.sheetArea = GC.Spread.Sheets.SheetArea.viewport;
searchCondition.searchOrder = GC.Spread.Sheets.Search.SearchOrder.nOrder;
searchCondition.searchTarget = GC.Spread.Sheets.Search.SearchFoundFlags.cellText;
searchCondition.searchFlags = GC.Spread.Sheets.Search.SearchFlags.blockRange;
var searchresult= spread.search(searchCondition);
var str ="[searchFoundFlag:"+ searchresult.searchFoundFlag+",\r\n foundSheetIndex:"+searchresult.foundSheetIndex+",foundRowIndex:" + searchresult.foundRowIndex+", foundColumnIndex:"+searchresult.foundColumnIndex+", foundString:"+searchresult.foundString+"]";
alert(str);
```

___

### <a id="startsheetindex" name="startsheetindex"></a> startSheetIndex

• **startSheetIndex**: `number`

要开始搜索的工作表的索引

**`代码示例`**
``` javascript
//本示例搜索一个单元格块
activeSheet.getCell(0,0).text("testSearch");
activeSheet.getCell(5,4).text("testSearch");
var searchCondition = new GC.Spread.Sheets.Search.SearchCondition();
searchCondition.searchString = "testSearch";
searchCondition.startSheetIndex = spread.getActiveSheetIndex();
searchCondition.endSheetIndex = spread.getActiveSheetIndex();
searchCondition.columnStart = 1;
searchCondition.columnEnd = 10;
searchCondition.rowStart = 1;
searchCondition.rowEnd = 10;
searchCondition.sheetArea = GC.Spread.Sheets.SheetArea.viewport;
searchCondition.searchOrder = GC.Spread.Sheets.Search.SearchOrder.nOrder;
searchCondition.searchTarget = GC.Spread.Sheets.Search.SearchFoundFlags.cellText;
searchCondition.searchFlags = GC.Spread.Sheets.Search.SearchFlags.blockRange;
var searchresult= spread.search(searchCondition);
var str ="[searchFoundFlag:"+ searchresult.searchFoundFlag+",\r\n foundSheetIndex:"+searchresult.foundSheetIndex+",foundRowIndex:" + searchresult.foundRowIndex+", foundColumnIndex:"+searchresult.foundColumnIndex+", foundString:"+searchresult.foundString+"]";
alert(str);
```
