# Enumeration: SearchFlags

[Sheets](../modules/GC.Spread.Sheets.md).[Search](../modules/GC.Spread.Sheets.Search.md).SearchFlags

指定搜索标志的类型。

**`example`**
```
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

- [blockRange](GC.Spread.Sheets.Search.SearchFlags.md#blockrange)
- [exactMatch](GC.Spread.Sheets.Search.SearchFlags.md#exactmatch)
- [ignoreCase](GC.Spread.Sheets.Search.SearchFlags.md#ignorecase)
- [none](GC.Spread.Sheets.Search.SearchFlags.md#none)
- [useWildCards](GC.Spread.Sheets.Search.SearchFlags.md#usewildcards)

## Enumeration members

### <a id="blockrange" name="blockrange"></a> blockRange

• **blockRange** = `8`

确定是否在单元格范围内搜索。

___

### <a id="exactmatch" name="exactmatch"></a> exactMatch

• **exactMatch** = `2`

确定搜索是否仅考虑完全匹配。

___

### <a id="ignorecase" name="ignorecase"></a> ignoreCase

• **ignoreCase** = `1`

确定搜索是否考虑搜索字符串中字母的大小写。

___

### <a id="none" name="none"></a> none

• **none** = `0`

指定无搜索标志。

___

### <a id="usewildcards" name="usewildcards"></a> useWildCards

• **useWildCards** = `4`

确定搜索是否考虑搜索字符串中的通配符字符（*，？）。
