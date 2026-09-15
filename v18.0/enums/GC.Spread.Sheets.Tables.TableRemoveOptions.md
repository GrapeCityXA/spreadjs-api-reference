# Enumeration: TableRemoveOptions

[Sheets](../modules/GC.Spread.Sheets.md).[Tables](../modules/GC.Spread.Sheets.Tables.md).TableRemoveOptions

删除表时保留哪些数据

**`代码示例`**
``` javascript
activeSheet.tables.add("Table1", 0, 0, 3, 3, GC.Spread.Sheets.Tables.TableThemes.dark1);
activeSheet.getCell(0,0).text("Name");
activeSheet.getCell(0,1).text("Value");
activeSheet.getCell(0,2).text("T/F");
activeSheet.getCell(1,0).text("AW");
activeSheet.getCell(1,1).text("5");
activeSheet.getCell(1,2).text("T");
//点击按钮
$("#button1").click(function () {
     var table  = activeSheet.tables.find(0,0);
     activeSheet.tables.remove(table, GC.Spread.Sheets.Tables.TableRemoveOptions.keepData);
});
```

## Table of contents

### Enumeration members

- [keepData](GC.Spread.Sheets.Tables.TableRemoveOptions.md#keepdata)
- [keepStyle](GC.Spread.Sheets.Tables.TableRemoveOptions.md#keepstyle)
- [none](GC.Spread.Sheets.Tables.TableRemoveOptions.md#none)

## Enumeration members

### <a id="keepdata" name="keepdata"></a> keepData

• **keepData** = `1`

 保持数据

___

### <a id="keepstyle" name="keepstyle"></a> keepStyle

• **keepStyle** = `2`

 保持样式

___

### <a id="none" name="none"></a> none

• **none** = `0`

 删除数据和样式
