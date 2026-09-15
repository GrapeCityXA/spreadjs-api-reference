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

定义搜索条件。

**`example`**
```javascript
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

结束搜索的列索引。

**`example`**
```javascript
//此示例搜索一个单元格区域。
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

开始搜索的列索引。

**`example`**
```javascript
//此示例搜索一个单元格区域。
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

结束搜索的页签索引。

**`example`**
```javascript
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

结束搜索的行索引。

**`example`**
```javascript
// 此示例搜索一个单元格区域。
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

开始搜索的行索引。

**`example`**
```javascript
// 此示例搜索一个单元格区域。
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

指定搜索选项的枚举。

**`example`**
```javascript
//此示例设置 searchFlags 属性。
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

指定搜索是否按列、行坐标进行。

**`example`**
```javascript
//此示例设置 searchOrder 属性。
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

指定搜索的字符串。

**`example`**
```javascript
//此示例设置 searchString 属性。
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

指定搜索是否包括单元格注释、标签或文本。

**`example`**
```javascript
//此示例设置 searchTarget 属性。
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

指定搜索的区域。

**`example`**
```javascript
// 此示例搜索一个单元格区域。
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

开始搜索的页签索引。

**`example`**
```javascript
// 此示例搜索一个单元格区域。
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
