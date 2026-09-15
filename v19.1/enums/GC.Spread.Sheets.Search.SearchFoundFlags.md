# Enumeration: SearchFoundFlags

[Sheets](../modules/GC.Spread.Sheets.md).[Search](../modules/GC.Spread.Sheets.Search.md).SearchFoundFlags

指定搜索字符串的查找位置。

**`example`**
```javascript
//此示例使用 SearchFlags 枚举。
activeSheet.getCell(2,3).value("testSearch");
var searchCondition = new GC.Spread.Sheets.Search.SearchCondition();
searchCondition.searchString = "testSearch";
searchCondition.startSheetIndex = spread.getActiveSheetIndex();
searchCondition.endSheetIndex = spread.getActiveSheetIndex();
searchCondition.searchOrder = GC.Spread.Sheets.Search.SearchOrder.nOrder;
searchCondition.searchTarget = GC.Spread.Sheets.Search.SearchFoundFlags.cellText;
searchCondition.searchFlags = GC.Spread.Sheets.Search.SearchFlags.ignoreCase| GC.Spread.Sheets.Search.SearchFlags.useWildCards;
var searchresult= activeSheet.search(searchCondition);
var str ="[searchFoundFlag:"+ searchresult.searchFoundFlag+",\r\n foundSheetIndex:"+searchresult.foundSheetIndex+",foundRowIndex:" +
searchresult.foundRowIndex+", foundColumnIndex:"+searchresult.foundColumnIndex+", foundString:"+searchresult.foundSheetIndex+"]";
alert(str);
```

## Table of contents

### Enumeration members

- [cellComment](GC.Spread.Sheets.Search.SearchFoundFlags.md#cellcomment)
- [cellFormula](GC.Spread.Sheets.Search.SearchFoundFlags.md#cellformula)
- [cellTag](GC.Spread.Sheets.Search.SearchFoundFlags.md#celltag)
- [cellText](GC.Spread.Sheets.Search.SearchFoundFlags.md#celltext)
- [cellThreadedComment](GC.Spread.Sheets.Search.SearchFoundFlags.md#cellthreadedcomment)
- [none](GC.Spread.Sheets.Search.SearchFoundFlags.md#none)

## Enumeration members

### <a id="cellcomment" name="cellcomment"></a> cellComment

• **cellComment** = `16`

表示在单元格注释中找到字符串。

___

### <a id="cellformula" name="cellformula"></a> cellFormula

• **cellFormula** = `8`

表示在单元格公式中找到字符串。

___

### <a id="celltag" name="celltag"></a> cellTag

• **cellTag** = `4`

表示在单元格标签中找到字符串。

___

### <a id="celltext" name="celltext"></a> cellText

• **cellText** = `1`

表示在单元格文本中找到字符串。

___

### <a id="cellthreadedcomment" name="cellthreadedcomment"></a> cellThreadedComment

• **cellThreadedComment** = `32`

表示在单元格评论中找到字符串。

___

### <a id="none" name="none"></a> none

• **none** = `0`

表示未找到字符串。
