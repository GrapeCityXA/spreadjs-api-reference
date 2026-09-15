# Enumeration: SearchOrder

[Sheets](../modules/GC.Spread.Sheets.md).[Search](../modules/GC.Spread.Sheets.Search.md).SearchOrder

搜索方向的类型

**`代码示例`**
```
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

- [nOrder](GC.Spread.Sheets.Search.SearchOrder.md#norder)
- [zOrder](GC.Spread.Sheets.Search.SearchOrder.md#zorder)

## Enumeration members

### <a id="norder" name="norder"></a> nOrder

• **nOrder** = `1`

确定是否按行,列坐标进行搜索

___

### <a id="zorder" name="zorder"></a> zOrder

• **zOrder** = `0`

确定是否按列,行坐标进行搜索
