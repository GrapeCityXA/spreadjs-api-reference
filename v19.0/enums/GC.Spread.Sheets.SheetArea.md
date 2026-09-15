# Enumeration: SheetArea

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).SheetArea

指定工作表区域。

**`example`**
```
//创建描述工作表点击区域的日志文本。
// 使用网页浏览器查看控制台日志文本
activeSheet.bind(GC.Spread.Sheets.Events.CellClick, function (sender, args) {
    if(args.sheetArea === GC.Spread.Sheets.SheetArea.colHeader){
        console.log("列标题被点击。");
    }
    if(args.sheetArea === GC.Spread.Sheets.SheetArea.rowHeader){
        console.log("行标题被点击。");
    }
    if(args.sheetArea === GC.Spread.Sheets.SheetArea.corner){
        console.log("角落标题被点击。");
    }
    console.log("点击的列索引: " + args.col);
    console.log("点击的行索引: " + args.row);
});
//绑定事件
activeSheet.bind(GC.Spread.Sheets.Events.CellDoubleClick, function (sender, args) {
    if(args.sheetArea === GC.Spread.Sheets.SheetArea.colHeader){
        console.log("列标题被双击。");
    }
    if(args.sheetArea === GC.Spread.Sheets.SheetArea.rowHeader){
        console.log("行标题被双击。");
    }
    if(args.sheetArea === GC.Spread.Sheets.SheetArea.corner){
        console.log("角落标题被双击。");
    }
    console.log("双击的列索引: " + args.col);
    console.log("双击的行索引: " + args.row);
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

表示列标题。

___

### <a id="corner" name="corner"></a> corner

• **corner** = `0`

表示工作表角落。

___

### <a id="rowheader" name="rowheader"></a> rowHeader

• **rowHeader** = `2`

表示行标题。

___

### <a id="viewport" name="viewport"></a> viewport

• **viewport** = `3`

表示视口。
