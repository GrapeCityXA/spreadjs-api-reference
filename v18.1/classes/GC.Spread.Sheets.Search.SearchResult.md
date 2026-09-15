# Class: SearchResult

[Sheets](../modules/GC.Spread.Sheets.md).[Search](../modules/GC.Spread.Sheets.Search.md).SearchResult

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Search.SearchResult.md#constructor)

### Properties

- [foundColumnIndex](GC.Spread.Sheets.Search.SearchResult.md#foundcolumnindex)
- [foundRowIndex](GC.Spread.Sheets.Search.SearchResult.md#foundrowindex)
- [foundSheetIndex](GC.Spread.Sheets.Search.SearchResult.md#foundsheetindex)
- [foundString](GC.Spread.Sheets.Search.SearchResult.md#foundstring)
- [searchFoundFlag](GC.Spread.Sheets.Search.SearchResult.md#searchfoundflag)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new SearchResult**()

定义搜索结果。

## Properties

### <a id="foundcolumnindex" name="foundcolumnindex"></a> foundColumnIndex

• **foundColumnIndex**: `number`

找到匹配的列索引。

**`example`**
```
// 此示例获取 foundColumnIndex 属性。
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

### <a id="foundrowindex" name="foundrowindex"></a> foundRowIndex

• **foundRowIndex**: `number`

找到匹配的行索引。

**`example`**
```
// 此示例获取 foundColumnIndex 属性。
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

### <a id="foundsheetindex" name="foundsheetindex"></a> foundSheetIndex

• **foundSheetIndex**: `number`

找到匹配的页签索引。

**`example`**
```
// 此示例获取 foundColumnIndex 属性。
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

### <a id="foundstring" name="foundstring"></a> foundString

• **foundString**: `Object`

找到的字符串。

**`example`**
```
// 此示例获取 foundColumnIndex 属性。
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

### <a id="searchfoundflag" name="searchfoundflag"></a> searchFoundFlag

• **searchFoundFlag**: [`SearchFoundFlags`](../enums/GC.Spread.Sheets.Search.SearchFoundFlags.md)

指定匹配的内容。

**`example`**
```
// 此示例获取 foundColumnIndex 属性。
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
