# Enumeration: SheetArea

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).SheetArea

工作表区域

**`代码示例`**
``` javascript
//创建描述单击工作表中哪个区域的日志
// 使用浏览器查看控制台日志
activeSheet.bind(GC.Spread.Sheets.Events.CellClick, function (sender, args) {
    if(args.sheetArea === GC.Spread.Sheets.SheetArea.colHeader){
        console.log("The column header was clicked.");
    }
    if(args.sheetArea === GC.Spread.Sheets.SheetArea.rowHeader){
        console.log("The row header was clicked.");
    }
    if(args.sheetArea === GC.Spread.Sheets.SheetArea.corner){
        console.log("The corner header was clicked.");
    }
    console.log("Clicked column index: " + args.col);
    console.log("Clicked row index: " + args.row);
});
//绑定事件
activeSheet.bind(GC.Spread.Sheets.Events.CellDoubleClick, function (sender, args) {
    if(args.sheetArea === GC.Spread.Sheets.SheetArea.colHeader){
        console.log("The column header was double clicked.");
    }
    if(args.sheetArea === GC.Spread.Sheets.SheetArea.rowHeader){
        console.log("The row header was double clicked.");
    }
    if(args.sheetArea === GC.Spread.Sheets.SheetArea.corner){
        console.log("The corner header was double clicked.");
    }
    console.log("Double clicked column index: " + args.col);
    console.log("Double clicked row index: " + args.row);
});
```

## Table of contents

### Enumeration members

- [colHeader](GC.Spread.Sheets.SheetArea.md#colheader)
- [corner](GC.Spread.Sheets.SheetArea.md#corner)
- [rowHeader](GC.Spread.Sheets.SheetArea.md#rowheader)
- [viewport](GC.Spread.Sheets.SheetArea.md#viewport)

## Enumeration members

### <a id="colheader" name="colheader"></a> colHeader

• **colHeader** = `1`

列头

___

### <a id="corner" name="corner"></a> corner

• **corner** = `0`

表角

___

### <a id="rowheader" name="rowheader"></a> rowHeader

• **rowHeader** = `2`

行头

___

### <a id="viewport" name="viewport"></a> viewport

• **viewport** = `3`

视图区域
