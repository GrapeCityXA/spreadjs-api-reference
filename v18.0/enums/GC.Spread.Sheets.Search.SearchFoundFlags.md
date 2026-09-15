# Enumeration: SearchFoundFlags

[Sheets](../modules/GC.Spread.Sheets.md).[Search](../modules/GC.Spread.Sheets.Search.md).SearchFoundFlags

在何处找到搜索字符串

**`代码示例`**
``` javascript
//本示例使用SearchFlags枚举
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
- [none](GC.Spread.Sheets.Search.SearchFoundFlags.md#none)

## Enumeration members

### <a id="cellcomment" name="cellcomment"></a> cellComment

• **cellComment** = `16`

表示该字符串在单元格批注中找到。

___

### <a id="cellformula" name="cellformula"></a> cellFormula

• **cellFormula** = `8`

在单元格公式中找到该字符串

___

### <a id="celltag" name="celltag"></a> cellTag

• **cellTag** = `4`

在单元格标签中找到了字符串

___

### <a id="celltext" name="celltext"></a> cellText

• **cellText** = `1`

在单元格文本中找到该字符串

___

### <a id="none" name="none"></a> none

• **none** = `0`

找不到字符串
