# Class: Events

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).Events

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Events.md#constructor)

### Events

- [ActiveSheetChanged](GC.Spread.Sheets.Events.md#activesheetchanged)
- [ActiveSheetChanging](GC.Spread.Sheets.Events.md#activesheetchanging)
- [BeforePrint](GC.Spread.Sheets.Events.md#beforeprint)
- [ButtonClicked](GC.Spread.Sheets.Events.md#buttonclicked)
- [CalculationProgress](GC.Spread.Sheets.Events.md#calculationprogress)
- [CellChanged](GC.Spread.Sheets.Events.md#cellchanged)
- [CellClick](GC.Spread.Sheets.Events.md#cellclick)
- [CellDoubleClick](GC.Spread.Sheets.Events.md#celldoubleclick)
- [ClipboardChanged](GC.Spread.Sheets.Events.md#clipboardchanged)
- [ClipboardChanging](GC.Spread.Sheets.Events.md#clipboardchanging)
- [ClipboardPasted](GC.Spread.Sheets.Events.md#clipboardpasted)
- [ClipboardPasting](GC.Spread.Sheets.Events.md#clipboardpasting)
- [ColumnChanged](GC.Spread.Sheets.Events.md#columnchanged)
- [ColumnChanging](GC.Spread.Sheets.Events.md#columnchanging)
- [ColumnWidthChanged](GC.Spread.Sheets.Events.md#columnwidthchanged)
- [ColumnWidthChanging](GC.Spread.Sheets.Events.md#columnwidthchanging)
- [CommentChanged](GC.Spread.Sheets.Events.md#commentchanged)
- [CommentRemoved](GC.Spread.Sheets.Events.md#commentremoved)
- [CommentRemoving](GC.Spread.Sheets.Events.md#commentremoving)
- [DragDropBlock](GC.Spread.Sheets.Events.md#dragdropblock)
- [DragDropBlockCompleted](GC.Spread.Sheets.Events.md#dragdropblockcompleted)
- [DragFillBlock](GC.Spread.Sheets.Events.md#dragfillblock)
- [DragFillBlockCompleted](GC.Spread.Sheets.Events.md#dragfillblockcompleted)
- [DragMerged](GC.Spread.Sheets.Events.md#dragmerged)
- [DragMerging](GC.Spread.Sheets.Events.md#dragmerging)
- [EditChange](GC.Spread.Sheets.Events.md#editchange)
- [EditEnded](GC.Spread.Sheets.Events.md#editended)
- [EditEnding](GC.Spread.Sheets.Events.md#editending)
- [EditStarting](GC.Spread.Sheets.Events.md#editstarting)
- [EditorStatusChanged](GC.Spread.Sheets.Events.md#editorstatuschanged)
- [EnterCell](GC.Spread.Sheets.Events.md#entercell)
- [FloatingObjectChanged](GC.Spread.Sheets.Events.md#floatingobjectchanged)
- [FloatingObjectLoaded](GC.Spread.Sheets.Events.md#floatingobjectloaded)
- [FloatingObjectRemoved](GC.Spread.Sheets.Events.md#floatingobjectremoved)
- [FloatingObjectRemoving](GC.Spread.Sheets.Events.md#floatingobjectremoving)
- [FloatingObjectSelectionChanged](GC.Spread.Sheets.Events.md#floatingobjectselectionchanged)
- [FormControlButtonClicked](GC.Spread.Sheets.Events.md#formcontrolbuttonclicked)
- [FormControlValueChanged](GC.Spread.Sheets.Events.md#formcontrolvaluechanged)
- [InvalidOperation](GC.Spread.Sheets.Events.md#invalidoperation)
- [LeaveCell](GC.Spread.Sheets.Events.md#leavecell)
- [LeftColumnChanged](GC.Spread.Sheets.Events.md#leftcolumnchanged)
- [OutlineColumnCheckStatusChanged](GC.Spread.Sheets.Events.md#outlinecolumncheckstatuschanged)
- [PictureChanged](GC.Spread.Sheets.Events.md#picturechanged)
- [PictureSelectionChanged](GC.Spread.Sheets.Events.md#pictureselectionchanged)
- [PivotTableChanged](GC.Spread.Sheets.Events.md#pivottablechanged)
- [RangeChanged](GC.Spread.Sheets.Events.md#rangechanged)
- [RangeFilterCleared](GC.Spread.Sheets.Events.md#rangefiltercleared)
- [RangeFilterClearing](GC.Spread.Sheets.Events.md#rangefilterclearing)
- [RangeFiltered](GC.Spread.Sheets.Events.md#rangefiltered)
- [RangeFiltering](GC.Spread.Sheets.Events.md#rangefiltering)
- [RangeGroupStateChanged](GC.Spread.Sheets.Events.md#rangegroupstatechanged)
- [RangeGroupStateChanging](GC.Spread.Sheets.Events.md#rangegroupstatechanging)
- [RangeSorted](GC.Spread.Sheets.Events.md#rangesorted)
- [RangeSorting](GC.Spread.Sheets.Events.md#rangesorting)
- [ReportSheetDataChanged](GC.Spread.Sheets.Events.md#reportsheetdatachanged)
- [ReportSheetDataChanging](GC.Spread.Sheets.Events.md#reportsheetdatachanging)
- [ReportSheetRecordsSubmitted](GC.Spread.Sheets.Events.md#reportsheetrecordssubmitted)
- [ReportSheetRecordsSubmitting](GC.Spread.Sheets.Events.md#reportsheetrecordssubmitting)
- [RowChanged](GC.Spread.Sheets.Events.md#rowchanged)
- [RowChanging](GC.Spread.Sheets.Events.md#rowchanging)
- [RowHeightChanged](GC.Spread.Sheets.Events.md#rowheightchanged)
- [RowHeightChanging](GC.Spread.Sheets.Events.md#rowheightchanging)
- [RowOperation](GC.Spread.Sheets.Events.md#rowoperation)
- [SelectionChanged](GC.Spread.Sheets.Events.md#selectionchanged)
- [SelectionChanging](GC.Spread.Sheets.Events.md#selectionchanging)
- [ShapeChanged](GC.Spread.Sheets.Events.md#shapechanged)
- [ShapeRemoved](GC.Spread.Sheets.Events.md#shaperemoved)
- [ShapeRemoving](GC.Spread.Sheets.Events.md#shaperemoving)
- [ShapeSelectionChanged](GC.Spread.Sheets.Events.md#shapeselectionchanged)
- [SheetChanged](GC.Spread.Sheets.Events.md#sheetchanged)
- [SheetChanging](GC.Spread.Sheets.Events.md#sheetchanging)
- [SheetMoved](GC.Spread.Sheets.Events.md#sheetmoved)
- [SheetMoving](GC.Spread.Sheets.Events.md#sheetmoving)
- [SheetNameChanged](GC.Spread.Sheets.Events.md#sheetnamechanged)
- [SheetNameChanging](GC.Spread.Sheets.Events.md#sheetnamechanging)
- [SheetTabClick](GC.Spread.Sheets.Events.md#sheettabclick)
- [SheetTabDoubleClick](GC.Spread.Sheets.Events.md#sheettabdoubleclick)
- [SlicerChanged](GC.Spread.Sheets.Events.md#slicerchanged)
- [SparklineChanged](GC.Spread.Sheets.Events.md#sparklinechanged)
- [TableColumnsChanged](GC.Spread.Sheets.Events.md#tablecolumnschanged)
- [TableFilterCleared](GC.Spread.Sheets.Events.md#tablefiltercleared)
- [TableFilterClearing](GC.Spread.Sheets.Events.md#tablefilterclearing)
- [TableFiltered](GC.Spread.Sheets.Events.md#tablefiltered)
- [TableFiltering](GC.Spread.Sheets.Events.md#tablefiltering)
- [TableResized](GC.Spread.Sheets.Events.md#tableresized)
- [TableResizing](GC.Spread.Sheets.Events.md#tableresizing)
- [TableRowsChanged](GC.Spread.Sheets.Events.md#tablerowschanged)
- [TopRowChanged](GC.Spread.Sheets.Events.md#toprowchanged)
- [TouchToolStripOpening](GC.Spread.Sheets.Events.md#touchtoolstripopening)
- [UserFormulaEntered](GC.Spread.Sheets.Events.md#userformulaentered)
- [ValidationError](GC.Spread.Sheets.Events.md#validationerror)
- [ValueChanged](GC.Spread.Sheets.Events.md#valuechanged)
- [ViewZoomed](GC.Spread.Sheets.Events.md#viewzoomed)
- [ViewZooming](GC.Spread.Sheets.Events.md#viewzooming)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Events**()

定义SpreadJS支持的事件

## Events

### <a id="activesheetchanged" name="activesheetchanged"></a> ActiveSheetChanged

• `Static` **ActiveSheetChanged**: `string`

当用户更改活动表单时触发

**`name`** GC.Spread.Sheets.Workbook#ActiveSheetChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `oldSheet` 旧表

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `newSheet` 新表

**`代码示例`**
```
//本示例为ActiveSheetChanged事件创建日志
// 使用IE查看控制台日志
spread.bind(GC.Spread.Sheets.Events.ActiveSheetChanged, function (sender, args) {
    console.log("Active sheet has been switched.");
});
```

___

### <a id="activesheetchanging" name="activesheetchanging"></a> ActiveSheetChanging

• `Static` **ActiveSheetChanging**: `string`

当用户更改活动表单时触发

**`name`** GC.Spread.Sheets.Workbook#ActiveSheetChanging

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `oldSheet` 旧表

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `newSheet` 新表

**`param`** *boolean* `cancel` 是否应取消操作

**`代码示例`**
```
//本示例停止活动表单的更改
spread.bind(GC.Spread.Sheets.Events.ActiveSheetChanging, function (sender, args) {
    //取消表单切换
    args.cancel = true;
});
```

___

### <a id="beforeprint" name="beforeprint"></a> BeforePrint

• `Static` **BeforePrint**: `string`

在打印之前

**`name`** GC.Spread.Sheets.Workbook#BeforePrint

**`param`** *Object* `iframe` 打印 Dom

**`param`** *boolean* `cancel` 是否取消打印

**`代码示例`**
```
//本示例使用BeforePrint
window.onload = function(){
     var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
     spread.bind(GC.Spread.Sheets.Events.BeforePrint, function (e, data) {
         alert(data.iframe + '\n' + 'cancel: ' + data.cancel);
     });
}
```

___

### <a id="buttonclicked" name="buttonclicked"></a> ButtonClicked

• `Static` **ButtonClicked**: `string`

当用户单击单元格中的按钮，复选框或超链接时触发

**`name`** GC.Spread.Sheets.Workbook#ButtonClicked

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `row` 单元格的行索引

**`param`** *number* `col` 单元格的列索引

**`param`** *[GC.Spread.Sheets.SheetArea](../enums/GC.Spread.Sheets.SheetArea.md)* `sheetArea` 包含单元格的表单区域

**`代码示例`**
```
//本示例创建一个按钮单元格
var cellType = new GC.Spread.Sheets.CellTypes.Button();
cellType.buttonBackColor("#FFFF00");
cellType.text("this is a button");
activeSheet.setCellType(1,1,cellType);
//bind
spread.bind(GC.Spread.Sheets.Events.ButtonClicked, function (e, args) {
    var sheet = args.sheet, row = args.row, col = args.col;
    var cellType = activeSheet.getCellType(row, col);
    if (cellType instanceof GC.Spread.Sheets.CellTypes.Button) {
        alert("Button Clicked");
    }
});
```

___

### <a id="calculationprogress" name="calculationprogress"></a> CalculationProgress

• `Static` **CalculationProgress**: `string`

使用增量计算进行计算时发生。

**`name`** GC.Spread.Sheets.Workbook#CalculationProgress

**`param`** *number* `totalCells` 计算单元格总数。

**`param`** *number* `pendingCells` 需要计算单元格计数。

**`param`** *number* `iterate` 迭代计算的次数已完成，仅在迭代计算时可用。

**`example`**
```
//This example uses the CalculationProgress event, to log the calculation progress.
spread.options.incrementalCalculation = true;
spread.bind(GC.Spread.Sheets.Events.CalculationProgress, function (e, info) {
     var msg = "Calculate ";
     if (info.pendingCells === 0) {
         msg += "finished";
     } else if (info.iterate >= 0) {
         msg += info.pendingCells + " cells in iterative calculation round " + info.iterate;
     } else {
         msg += (info.totalCells - info.pendingCells) + "/" + info.totalCells + "cells";
     }
     console.log(msg)
});
```

___

### <a id="cellchanged" name="cellchanged"></a> CellChanged

• `Static` **CellChanged**: `string`

在此表单中对单元格进行更改时可能会发生，可能需要重绘该单元格

**`name`** GC.Spread.Sheets.Worksheet#CellChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `row` 单元格的行索引

**`param`** *number* `col` 单元格的列索引

**`param`** *[GC.Spread.Sheets.SheetArea](../enums/GC.Spread.Sheets.SheetArea.md)* `sheetArea` 单元格的表单区域

**`param`** *string* `propertyName` 已更改的单元格属性的名称

**`param`** *boolean* `isUndo` 此事件是否来自撤消操作

**`代码示例`**
```
//本示例使用CellChanged事件
activeSheet.bind(GC.Spread.Sheets.Events.CellChanged, function (e, info) {
    if(info.sheetArea === GC.Spread.Sheets.SheetArea.viewport){
        alert("Cell index (" + info.row + "," + info.col + ")");
    }
});
```

___

### <a id="cellclick" name="cellclick"></a> CellClick

• `Static` **CellClick**: `string`

当用户在单元格中按下鼠标左键时触发

**`name`** GC.Spread.Sheets.Worksheet#CellClick

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.SheetArea](../enums/GC.Spread.Sheets.SheetArea.md)* `sheetArea` 单击的单元格所在的表单区域

**`param`** *number* `row` 单击的单元格的行索引

**`param`** *number* `col` 单击的单元格的列索引

**`代码示例`**
```
//本示例使用CellClick事件
// Use web browser to see the console log text
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
//bind
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
})
```

___

### <a id="celldoubleclick" name="celldoubleclick"></a> CellDoubleClick

• `Static` **CellDoubleClick**: `string`

当用户在单元格中两次按下鼠标左键(双击)时触发

**`name`** GC.Spread.Sheets.Worksheet#CellDoubleClick

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.SheetArea](../enums/GC.Spread.Sheets.SheetArea.md)* `sheetArea` 单击的单元格所在的表单区域

**`param`** *number* `row` 单击的单元格的行索引

**`param`** *number* `col` 单击的单元格的列索引

**`代码示例`**
```
//本示例使用CellDoubleClick事件
// Use web browser to see the console log text
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
//bind
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

___

### <a id="clipboardchanged" name="clipboardchanged"></a> ClipboardChanged

• `Static` **ClipboardChanged**: `string`

Spread.Sheets的剪贴板更改时触发

**`name`** GC.Spread.Sheets.Worksheet#ClipboardChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *Object* `copyData` 已设置到剪贴板中的数据

**`param`** *string* `copyData.text` 剪贴板的文本字符串

**`param`** *string* `copyData.html` 剪贴板的html字符串

**`param`** *Array* `objects` 复制的浮动对象，它包含图片，自定义浮动对象，切片器，图表和形状

**`代码示例`**
```
//本示例使用ClipboardChanged事件
spread.bind(GC.Spread.Sheets.Events.ClipboardChanged, function (sender, args) {
    console.log("ClipboardChanged.", args);
});
```

___

### <a id="clipboardchanging" name="clipboardchanging"></a> ClipboardChanging

• `Static` **ClipboardChanging**: `string`

在剪贴板由于操作而更改时触发

**`name`** GC.Spread.Sheets.Worksheet#ClipboardChanging

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *Object* `copyData` 设置在剪贴板中的数据

**`param`** *string* `copyData.text` 剪贴板的文本字符串

**`param`** *string* `copyData.html` 剪贴板的html字符串

**`param`** *{@link GC.Spread.Sheets.Range[]}* `ranges` 当前剪切或复制操作的源工作表的源范围。

**`param`** *{@link GC.Spread.Sheet.ClipboardActionType}* `action` 表示当前操作的类型。

**`param`** *Array* `objects` 顶部浮动对象，它包含图片，自定义浮动对象，切片器，图表和形状

**`param`** *boolean* `cancel` 是否应取消操作

**`代码示例`**
```
//本示例使用ClipboardChanging事件
spread.bind(GC.Spread.Sheets.Events.ClipboardChanging, function (sender, args) {
    console.log("ClipboardChanging", args);
});
```

___

### <a id="clipboardpasted" name="clipboardpasted"></a> ClipboardPasted

• `Static` **ClipboardPasted**: `string`

当用户从剪贴板粘贴时触发

**`name`** GC.Spread.Sheets.Worksheet#ClipboardPasted

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.Range](GC.Spread.Sheets.Range.md)* `cellRange` 粘贴的区域

**`param`** *[GC.Spread.Sheets.ClipboardPasteOptions](../enums/GC.Spread.Sheets.ClipboardPasteOptions.md)* `pasteOption` 粘贴选项，表示从剪贴板粘贴哪些数据:值，格式或公式

**`param`** *Object* `pasteData` 剪贴板中的数据将粘贴到表单中

**`param`** *string* `pasteData.text` 剪贴板的文本字符串

**`param`** *string* `pasteData.html` 剪贴板的html字符串

**`param`** *string* `pasteData.image` 剪贴板的图像src字符串

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `fromSheet` 数据区域的源表

**`param`** *[GC.Spread.Sheets.Range](GC.Spread.Sheets.Range.md)* `[fromRange]` 复制或剪切区域时粘贴的源区域

**`param`** *{@link GC.Spread.Sheet.ClipboardActionType}* `action` 指示当前操作的类型。

**`param`** *Array* `objects` 粘贴的浮动元素，它包含图片、自定义浮动对象、切片器、图表和形状

**`param`** *[GC.Spread.Sheets.InsertShiftCell](../enums/GC.Spread.Sheets.InsertShiftCell.md)* `[shiftCells]` shift选项, 如果没有, 则返回undefined

**`代码示例`**
```
//本示例使用ClipboardPasted事件
spread.bind(GC.Spread.Sheets.Events.ClipboardPasted, function (sender, args) {
    console.log("ClipboardPasted", args);
});
```

___

### <a id="clipboardpasting" name="clipboardpasting"></a> ClipboardPasting

• `Static` **ClipboardPasting**: `string`

当用户从剪贴板粘贴时触发

**`name`** GC.Spread.Sheets.Worksheet#ClipboardPasting

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.Range](GC.Spread.Sheets.Range.md)* `cellRange` 粘贴区域

**`param`** *[GC.Spread.Sheets.ClipboardPasteOptions](../enums/GC.Spread.Sheets.ClipboardPasteOptions.md)* `pasteOption` 粘贴选项，表示从剪贴板粘贴哪些数据:值，格式或公式

**`param`** *Object* `pasteData` 剪贴板中的数据将粘贴到表单中

**`param`** *string* `pasteData.text` 剪贴板的文本字符串

**`param`** *string* `pasteData.html` 剪贴板的html字符串

**`param`** *string* `pasteData.image` 剪贴板的图像src字符串

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `fromSheet` 数据区域的源表

**`param`** *[GC.Spread.Sheets.Range](GC.Spread.Sheets.Range.md)* `[fromRange]` 复制或剪切区域时粘贴的源区域

**`param`** *{@link GC.Spread.Sheet.ClipboardActionType}* `action` 指示当前操作的类型。

**`param`** *Array* `objects` 粘贴的浮动元素，它包含图片、自定义浮动对象、切片器、图表和形状

**`param`** *boolean* `cancel` 是否应取消操作

**`param`** *[GC.Spread.Sheets.InsertShiftCell](../enums/GC.Spread.Sheets.InsertShiftCell.md)* `[shiftCells]` shift选项, 如果没有, 则返回undefined

**`代码示例`**
```
//本示例使用ClipboardPasting事件
spread.bind(GC.Spread.Sheets.Events.ClipboardPasting, function (sender, args) {
    console.log("ClipboardPasting", args);
});
```

___

### <a id="columnchanged" name="columnchanged"></a> ColumnChanged

• `Static` **ColumnChanged**: `string`

当对此表单中的列或列区域进行更改，可能需要重新绘制该列或列区域时触发

**`name`** GC.Spread.Sheets.Worksheet#ColumnChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `col` 列索引

**`param`** *[GC.Spread.Sheets.SheetArea](../enums/GC.Spread.Sheets.SheetArea.md)* `sheetArea` 表单区域

**`param`** *string* `propertyName` 已更改的列属性的名称

**`param`** *boolean* `isUndo` 此事件是否来自撤消操作

**`代码示例`**
```
//本示例使用了ColumnChanged事件
activeSheet.bind(GC.Spread.Sheets.Events.ColumnChanged, function (e, info) {
    if(info.sheetArea === GC.Spread.Sheets.SheetArea.viewport){
        alert("Index (" + info.col + ")");
    }
});
```

___

### <a id="columnchanging" name="columnchanging"></a> ColumnChanging

• `Static` **ColumnChanging**: `string`

在对本表单中的列或列区域进行更改之前发生，可能需要重新绘制该列或列区域

**`name`** GC.Spread.Sheets.Worksheet#ColumnChanging

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `col` 列索引

**`param`** *[GC.Spread.Sheets.SheetArea](../enums/GC.Spread.Sheets.SheetArea.md)* `sheetArea` 表单区域

**`param`** *string* `propertyName` 已更改的列属性的名称

**`代码示例`**
```
//本示例使用了ColumnChanging事件
activeSheet.bind(GC.Spread.Sheets.Events.ColumnChanging, function (e, info) {
    if(info.sheetArea === GC.Spread.Sheets.SheetArea.viewport){
        alert("Index (" + info.col + ")");
    }
});
```

___

### <a id="columnwidthchanged" name="columnwidthchanged"></a> ColumnWidthChanged

• `Static` **ColumnWidthChanged**: `string`

当列宽度发生更改时触发

**`name`** GC.Spread.Sheets.Worksheet#ColumnWidthChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *Array* `colList` 宽度改变的列的列表

**`param`** *boolean* `header` 列是否为行标题列

**`代码示例`**
```
//本示例使用了ColumnWidthChanged事件
activeSheet.bind(GC.Spread.Sheets.Events.ColumnWidthChanged, function (e, info) {
        alert("Column (" + info.colList + ")");
});
```

___

### <a id="columnwidthchanging" name="columnwidthchanging"></a> ColumnWidthChanging

• `Static` **ColumnWidthChanging**: `string`

当列宽度改变时触发

**`name`** GC.Spread.Sheets.Worksheet#ColumnWidthChanging

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *Array* `colList` 宽度改变的列的列表

**`param`** *boolean* `header` 列是否为行标题列

**`param`** *boolean* `cancel` 是否应取消操作

**`代码示例`**
```
//本示例使用了columnwidthchange事件
activeSheet.bind(GC.Spread.Sheets.Events.ColumnWidthChanging, function (e, info) {
        alert("Column (" + info.colList + ")");
});
```

___

### <a id="commentchanged" name="commentchanged"></a> CommentChanged

• `Static` **CommentChanged**: `string`

当批注更改时触发

**`name`** GC.Spread.Sheets.Worksheet#CommentChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.Comments.Comment](GC.Spread.Sheets.Comments.Comment.md)* `comment` 触发事件的批注

**`param`** *string* `propertyName` 已更改的批注属性的名称

**`代码示例`**
```
//本示例使用CommentChanged事件
activeSheet.bind(GC.Spread.Sheets.Events.CommentChanged, function (e, info) {
    alert("changed");
});
```

___

### <a id="commentremoved" name="commentremoved"></a> CommentRemoved

• `Static` **CommentRemoved**: `string`

当用户删除批注时触发

**`name`** GC.Spread.Sheets.Worksheet#CommentRemoved

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.Comments.Comment](GC.Spread.Sheets.Comments.Comment.md)* `comment` 该批注已被删除

**`代码示例`**
```
//本示例使用commentremove事件
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("orange");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
activeSheet.getCell(5,5).comment(comment);
activeSheet.bind(GC.Spread.Sheets.Events.CommentRemoved, function (e, info) {
       console.log("sheet name: " + info.sheetName);
});
```

___

### <a id="commentremoving" name="commentremoving"></a> CommentRemoving

• `Static` **CommentRemoving**: `string`

当用户删除任何批注时触发

**`name`** GC.Spread.Sheets.Worksheet#CommentRemoving

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.Comments.Comment](GC.Spread.Sheets.Comments.Comment.md)* `comment` 该批注已被删除

**`param`** *boolean* `cancel` 是否应取消操作

**`代码示例`**
```
//本示例阻止批注被删除
var comment = new GC.Spread.Sheets.Comments.Comment();
comment.text("new comment!");
comment.backColor("orange");
comment.displayMode(GC.Spread.Sheets.Comments.DisplayMode.alwaysShown);
activeSheet.getCell(5,5).comment(comment);
activeSheet.bind(GC.Spread.Sheets.Events.CommentRemoving, function (e, info) {
      info.cancel = true;
});
```

___

### <a id="dragdropblock" name="dragdropblock"></a> DragDropBlock

• `Static` **DragDropBlock**: `string`

当用户拖放单元格区域时触发

**`name`** GC.Spread.Sheets.Worksheet#DragDropBlock

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `fromRow` 源区域(正在拖动的区域)的左上角单元格的行索引

**`param`** *number* `fromCol` 源区域(正在拖动的区域)的左上角单元格的列索引

**`param`** *number* `toRow` 目标区域(删除所选内容的位置)的左上角单元格的行索引

**`param`** *number* `toCol` 目标区域(在其中删除所选内容)的右下单元格的列索引

**`param`** *number* `rowCount` 正在拖动的单元格区域的行数

**`param`** *number* `colCount` 正在拖动的单元格区域的列数

**`param`** *boolean* `copy` 源区域是否被复制

**`param`** *boolean* `insert` 是否插入源区域

**`param`** *[GC.Spread.Sheets.CopyToOptions](../enums/GC.Spread.Sheets.CopyToOptions.md)* `copyOption` 拖放操作的复制选项值

**`param`** *boolean* `cancel` 是否应取消操作

**`代码示例`**
```
//本示例为DragDropBlock事件创建了日志
// Use web browser to see the console log text
var activeSheet = spread.getActiveSheet();
activeSheet.bind(GC.Spread.Sheets.Events.DragDropBlock, function (e, args) {
        console.log("From Column:" + args.fromCol);
        console.log("From Row:" + args.fromRow);
        console.log("To Column:" + args.toCol);
        console.log("To Row:" + args.toRow);
    });
```

___

### <a id="dragdropblockcompleted" name="dragdropblockcompleted"></a> DragDropBlockCompleted

• `Static` **DragDropBlockCompleted**: `string`

当用户完成对单元格区域的拖放时触发

**`name`** GC.Spread.Sheets.Worksheet#DragDropBlockCompleted

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `fromRow` 源区域(正在拖动的区域)的左上角单元格的行索引

**`param`** *number* `fromCol` 源区域(正在拖动的区域)的左上角单元格的列索引

**`param`** *number* `toRow` 目标区域(删除所选内容的位置)的左上角单元格的行索引

**`param`** *number* `toCol` 目标区域(在其中删除所选内容)的右下单元格的列索引

**`param`** *number* `rowCount` 正在拖动的单元格区域的行数

**`param`** *number* `colCount` 正在拖动的单元格区域的列数

**`param`** *boolean* `copy` 源区域是否被复制

**`param`** *boolean* `insert` 是否插入源区域

**`param`** *[GC.Spread.Sheets.CopyToOptions](../enums/GC.Spread.Sheets.CopyToOptions.md)* `copyOption` 拖放操作的复制选项值

**`代码示例`**
```
//本示例使用了DragDropBlockCompleted事件
activeSheet.bind(GC.Spread.Sheets.Events.DragDropBlockCompleted, function (e, args) {
        alert("From Column (" + args.fromCol + ")");
});
```

___

### <a id="dragfillblock" name="dragfillblock"></a> DragFillBlock

• `Static` **DragFillBlock**: `string`

当用户拖动以填充单元格区域时触发

**`name`** GC.Spread.Sheets.Worksheet#DragFillBlock

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.Range](GC.Spread.Sheets.Range.md)* `fillRange` 填充操作使用的区域

**`param`** *[GC.Spread.Sheets.Fill.AutoFillType](../enums/GC.Spread.Sheets.Fill.AutoFillType.md)* `autoFillType` 用于填充操作的AutoFillType值

**`param`** *[GC.Spread.Sheets.Fill.FillDirection](../enums/GC.Spread.Sheets.Fill.FillDirection.md)* `fillDirection` 填充的方向

**`param`** *boolean* `cancel` 是否应取消操作

**`代码示例`**
```
//本示例使用了DragFillBlock事件
activeSheet.bind(GC.Spread.Sheets.Events.DragFillBlock, function (e, info) {
        alert("Direction (" + info.fillDirection + ")");
});
```

___

### <a id="dragfillblockcompleted" name="dragfillblockcompleted"></a> DragFillBlockCompleted

• `Static` **DragFillBlockCompleted**: `string`

当用户完成拖动以填充单元格区域时触发

**`name`** GC.Spread.Sheets.Worksheet#DragFillBlockCompleted

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.Range](GC.Spread.Sheets.Range.md)* `fillRange` 填充操作使用的区域

**`param`** *[GC.Spread.Sheets.Fill.AutoFillType](../enums/GC.Spread.Sheets.Fill.AutoFillType.md)* `autoFillType` 用于填充操作的AutoFillType值

**`param`** *[GC.Spread.Sheets.Fill.FillDirection](../enums/GC.Spread.Sheets.Fill.FillDirection.md)* `fillDirection` 填充的方向

**`代码示例`**
```
//本示例使用了DragFillBlockCompleted事件
activeSheet.bind(GC.Spread.Sheets.Events.DragFillBlockCompleted, function (e, info) {
        alert("Type (" + info.autoFillType + ")");
});
```

___

### <a id="dragmerged" name="dragmerged"></a> DragMerged

• `Static` **DragMerged**: `string`

在用户拖动合并单元格后发生

**`name`** GC.Spread.Sheets.Worksheet#DragMerged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.Range](GC.Spread.Sheets.Range.md)* `mergeRange` 将要合并的区域

**`代码示例`**
```
//本示例返回行索引
// 按Ctrl键合并
$(document).keydown(function (e) {
     if (e.keyCode === 17) {
        spread.options.allowUserDragMerge = true;
     }
});
$(document).keyup(function (e) {
     if (e.keyCode === 17) {
        spread.options.allowUserDragMerge = false;
     }
});
activeSheet.bind(GC.Spread.Sheets.Events.DragMerging, function (e, data) {
     var mergeRange = data.mergeRange;
     alert(mergeRange.row);
});
activeSheet.bind(GC.Spread.Sheets.Events.DragMerged, function (e, data) {
     var mergeRange = data.mergeRange;
     alert(mergeRange.row);
});
```

___

### <a id="dragmerging" name="dragmerging"></a> DragMerging

• `Static` **DragMerging**: `string`

在用户拖动合并单元格之前发生

**`name`** GC.Spread.Sheets.Worksheet#DragMerging

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.Range](GC.Spread.Sheets.Range.md)* `mergeRange` 将要合并的区域

**`param`** *boolean* `cancel` 是否应取消操作

**`代码示例`**
```
//本示例返回行索引
// 按Ctrl键合并
$(document).keydown(function (e) {
     if (e.keyCode === 17) {
         spread.options.allowUserDragMerge = true;
     }
});
$(document).keyup(function (e) {
     if (e.keyCode === 17) {
         spread.options.allowUserDragMerge = false;
     }
});
activeSheet.bind(GC.Spread.Sheets.Events.DragMerging, function (e, data) {
     var mergeRange = data.mergeRange;
     alert(mergeRange.row);
});
activeSheet.bind(GC.Spread.Sheets.Events.DragMerged, function (e, data) {
     var mergeRange = data.mergeRange;
     alert(mergeRange.row);
});
```

___

### <a id="editchange" name="editchange"></a> EditChange

• `Static` **EditChange**: `string`

当单元格处于编辑模式且文本被更改时触发

**`name`** GC.Spread.Sheets.Worksheet#EditChange

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `row` 单元格的行索引

**`param`** *number* `col` 单元格的列索引

**`param`** *Object* `editingText` 当前编辑器中的值

**`代码示例`**
```
//本示例为EditChange事件创建日志
// Use web browser to see the console log text
activeSheet.bind(GC.Spread.Sheets.Events.EditChange, function (sender, args) {
    console.log("Cell (" + args.row + ", " + args.col + ") data has been changed.")
});
```

___

### <a id="editended" name="editended"></a> EditEnded

• `Static` **EditEnded**: `string`

当单元格离开编辑模式时触发

**`name`** GC.Spread.Sheets.Worksheet#EditEnded

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `row` 单元格的行索引

**`param`** *number* `col` 单元格的列索引

**`param`** *Object* `editingText` 当前编辑器中的值

**`param`** *boolean* `committed` Whether the value change was committed

**`代码示例`**
```
//本示例为editstart和EditEnded事件创建日志
 // Use web browser to see the console log text
var activeSheet = spread.getActiveSheet();
activeSheet.bind(GC.Spread.Sheets.Events.EditStarting, function (sender, args) {
    console.log("Start cell editing.");
});
activeSheet.bind(GC.Spread.Sheets.Events.EditEnded, function (sender, args) {
    console.log("Finish cell editing.");
});
```

___

### <a id="editending" name="editending"></a> EditEnding

• `Static` **EditEnding**: `string`

当单元格离开编辑模式时触发

**`name`** GC.Spread.Sheets.Worksheet#EditEnding

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `row` 单元格的行索引

**`param`** *number* `col` 单元格的列索引

**`param`** *Object* `editor` 当前编辑器

**`param`** *Object* `editingText` 当前编辑器中的值

**`param`** *boolean* `cancel` 是否应取消操作

**`param`** *boolean* `committed` Whether the value change was committed

**`代码示例`**
```
//本示例使用EditEnding事件
activeSheet.bind(GC.Spread.Sheets.Events.EditStarting, function (sender, args) {
    console.log("Start cell editing.");
});
activeSheet.bind(GC.Spread.Sheets.Events.EditEnding, function (sender, args) {
    console.log("EditEnding event.");
});
activeSheet.bind(GC.Spread.Sheets.Events.EditEnded, function (sender, args) {
    console.log("EditEnded event.");
});
```

___

### <a id="editstarting" name="editstarting"></a> EditStarting

• `Static` **EditStarting**: `string`

当单元格进入编辑模式时触发

**`name`** GC.Spread.Sheets.Worksheet#EditStarting

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `row` 单元格的行索引

**`param`** *number* `col` 单元格的列索引

**`param`** *boolean* `cancel` 是否应取消操作

**`代码示例`**
```
//本示例为editstart和EditEnded事件创建日志
// Use web browser to see the console log text
var activeSheet = spread.getActiveSheet();
activeSheet.bind(GC.Spread.Sheets.Events.EditStarting, function (sender, args) {
    console.log("Start cell editing.");
});
activeSheet.bind(GC.Spread.Sheets.Events.EditEnded, function (sender, args) {
    console.log("Finish cell editing.");
});
```

___

### <a id="editorstatuschanged" name="editorstatuschanged"></a> EditorStatusChanged

• `Static` **EditorStatusChanged**: `string`

当编辑器的状态发生更改时触发

**`name`** GC.Spread.Sheets.Worksheet#EditorStatusChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.EditorStatus](../enums/GC.Spread.Sheets.EditorStatus.md)* `oldStatus` 编辑的旧状态

**`param`** *[GC.Spread.Sheets.EditorStatus](../enums/GC.Spread.Sheets.EditorStatus.md)* `newStatus` 编辑的新状态

**`代码示例`**
```
//本示例使用EditorStatusChanged事件
activeSheet.bind(GC.Spread.Sheets.Events.EditorStatusChanged, function (e, info) {
        alert("Column (" + info.newStatus + ")");
});
```

___

### <a id="entercell" name="entercell"></a> EnterCell

• `Static` **EnterCell**: `string`

当焦点进入单元格时触发

**`name`** GC.Spread.Sheets.Worksheet#EnterCell

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `row` 正在输入的单元格的行索引

**`param`** *number* `col` 正在输入的单元格的列索引

**`代码示例`**
```
//本例使用EnterCell事件
activeSheet.bind(GC.Spread.Sheets.Events.EnterCell, function (e, info) {
        alert("Cell (" + info.row + ", " + info.col +")");
});
```

___

### <a id="floatingobjectchanged" name="floatingobjectchanged"></a> FloatingObjectChanged

• `Static` **FloatingObjectChanged**: `string`

当任何浮动对象发生改变时触发

**`name`** GC.Spread.Sheets.Worksheet#FloatingObjectsChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.FloatingObjects.FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md)* `floatingObject` 触发事件的浮动对象

**`param`** *string* `propertyName` 已更改的浮动对象的属性的名称

**`代码示例`**
```
//本示例使用了FloatingObjectChanged事件
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
activeSheet.bind(GC.Spread.Sheets.Events.FloatingObjectChanged, function (e, info) {
       alert("changed");
});
```

___

### <a id="floatingobjectloaded" name="floatingobjectloaded"></a> FloatingObjectLoaded

• `Static` **FloatingObjectLoaded**: `string`

在加载自定义浮动对象内容时触发

**`name`** GC.Spread.Sheets.Worksheet#FloatingObjectLoaded

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.FloatingObjects.FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md)* `floatingObject` 触发事件的自定义浮动对象

**`param`** *HTMLElement* `element` 自定义浮动对象的HTMLElement

___

### <a id="floatingobjectremoved" name="floatingobjectremoved"></a> FloatingObjectRemoved

• `Static` **FloatingObjectRemoved**: `string`

当用户移除浮动对象时触发

**`name`** GC.Spread.Sheets.Worksheet#FloatingObjectRemoved

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.FloatingObjects.FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md)* `floatingObject` 浮动对象已被移除

**`代码示例`**
```
//本示例使用了FloatingObjectRemoved事件
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
activeSheet.bind(GC.Spread.Sheets.Events.FloatingObjectRemoved, function (e, info) {
        alert(info.sheetName);
});
```

___

### <a id="floatingobjectremoving" name="floatingobjectremoving"></a> FloatingObjectRemoving

• `Static` **FloatingObjectRemoving**: `string`

当用户移除任何浮动对象时触发

**`name`** GC.Spread.Sheets.Worksheet#FloatingObjectRemoving

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.FloatingObjects.FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md)* `floatingObject` 浮动对象已被移除

**`param`** *boolean* `cancel` 是否应取消操作

**`代码示例`**
```
//本示例使用了FloatingObjectRemoving事件
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
activeSheet.bind(GC.Spread.Sheets.Events.FloatingObjectRemoving, function (e, info) {
        info.cancel = true;
});
```

___

### <a id="floatingobjectselectionchanged" name="floatingobjectselectionchanged"></a> FloatingObjectSelectionChanged

• `Static` **FloatingObjectSelectionChanged**: `string`

当浮动对象的选择发生改变时触发

**`name`** GC.Spread.Sheets.Worksheet#FloatingObjectsSelectionChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.FloatingObjects.FloatingObject](GC.Spread.Sheets.FloatingObjects.FloatingObject.md)* `floatingObject` 触发事件的浮动对象

**`代码示例`**
```
//本示例使用了FloatingObjectSelectionChanged事件
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
// 使用IE查看控制台日志
activeSheet.bind(GC.Spread.Sheets.Events.FloatingObjectSelectionChanged, function (e, info) {
       console.log("sheet name: " + info.sheetName);
});
```

___

### <a id="formcontrolbuttonclicked" name="formcontrolbuttonclicked"></a> FormControlButtonClicked

• `Static` **FormControlButtonClicked**: `string`

单击按钮表单控件时发生。

**`name`** GC.Spread.Sheets.Worksheet#FormControlButtonClicked

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.Shapes.Shape](GC.Spread.Sheets.Shapes.Shape.md)* `shape` 触发事件的形状

**`代码示例`**
```
//This example uses the FormControlButtonClicked event.
var shape = sheet.shapes.addFormControl("button", GC.Spread.Sheets.Shapes.FormControlType.button, 50, 50, 150, 100);
activeSheet.bind(GC.Spread.Sheets.Events.FormControlButtonClicked, function (e, info) {
       console.log("event info: " + info);
});
```

___

### <a id="formcontrolvaluechanged" name="formcontrolvaluechanged"></a> FormControlValueChanged

• `Static` **FormControlValueChanged**: `string`

当表单控件的值发生更改时发生。

**`name`** GC.Spread.Sheets.Worksheet#FormControlValueChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.Shapes.Shape](GC.Spread.Sheets.Shapes.Shape.md)* `shape` 触发事件的形状

**`param`** *any* `newValue` 表单控件的新值。

**`param`** *any* `oldValue` 表单控件的旧值。

**`代码示例`**
```
//This example uses the FormControlValueChanged event.
var shape = sheet.shapes.addFormControl('spin', GC.Spread.Sheets.Shapes.FormControlType.spinButton, 50, 50, 150, 100);
activeSheet.bind(GC.Spread.Sheets.Events.FormControlValueChanged, function (e, info) {
       console.log("event info: " + info);
});
```

___

### <a id="invalidoperation" name="invalidoperation"></a> InvalidOperation

• `Static` **InvalidOperation**: `string`

在执行无效操作时触发

**`name`** GC.Spread.Sheets.Worksheet#InvalidOperation

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.InvalidOperationType](../enums/GC.Spread.Sheets.InvalidOperationType.md)* `invalidType` 无效的操作

**`param`** *string* `message` 无效操作的描述。

**`param`** *[GC.Spread.Sheets.Range](GC.Spread.Sheets.Range.md)* `[fillRange]` When invalidType is dragFill, 填充操作使用的区域

**`代码示例`**
```
//本示例使用InvalidOperation事件
activeSheet.bind(GC.Spread.Sheets.Events.InvalidOperation, function (e, info) {
        alert("Message (" + info.message + ")");
});
```

___

### <a id="leavecell" name="leavecell"></a> LeaveCell

• `Static` **LeaveCell**: `string`

当焦点离开单元格时触发

**`name`** GC.Spread.Sheets.Worksheet#LeaveCell

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `row` 左单元格的行索引

**`param`** *number* `col` 左单元格的列索引

**`param`** *boolean* `cancel` 是否应取消操作

**`代码示例`**
```
//本示例为LeaveCell事件创建日志
// Use web browser to see the console log text
activeSheet.bind(GC.Spread.Sheets.Events.LeaveCell, function (sender, args) {
    console.log("The column index before moving: " + args.col);
    console.log("The row index before moving: " + args.row);
});
```

___

### <a id="leftcolumnchanged" name="leftcolumnchanged"></a> LeftColumnChanged

• `Static` **LeftColumnChanged**: `string`

当左列更改时触发

**`name`** GC.Spread.Sheets.Worksheet#LeftColumnChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `oldLeftCol` 旧的左列索引

**`param`** *number* `newLeftCol` 新的左列索引

**`param`** *number* `oldOffset` 旧偏移

**`param`** *number* `newOffset` 新偏移

**`example`**
```
//本示例同步了表单1和表单2的垂直和水平滚动
var sheet1 = spread.getSheet(0),
sheet2 = spread.getSheet(1);
sheet1.bind(GC.Spread.Sheets.Events.TopRowChanged, function (sender, args) {
    //将显示的sheet1的第一行设置到sheet2(垂直滚动同步)
    sheet2.showRow(args.newTopRow, GC.Spread.Sheets.VerticalPosition.top);
});
sheet1.bind(GC.Spread.Sheets.Events.LeftColumnChanged, function (sender, args) {
    //将显示的sheet1的左列设置到sheet2(水平滚动同步)
    sheet2.showColumn(args.newLeftCol, GC.Spread.Sheets.HorizontalPosition.left);
});
```

___

### <a id="outlinecolumncheckstatuschanged" name="outlinecolumncheckstatuschanged"></a> OutlineColumnCheckStatusChanged

• `Static` **OutlineColumnCheckStatusChanged**: `string`

当分组列勾选状态发生更改时触发

**`name`** GC.Spread.Sheets.Worksheet#OutlineColumnCheckStatusChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `row` 分组列的更改行索引

**`param`** *number* `col` 分组列的更改列索引

**`param`** *boolean* `status` 分组列的更改状态

**`代码示例`**
```
//移除迷你图会引起一个变化
activeSheet.bind(GC.Spread.Sheets.Events.OutlineColumnCheckStatusChanged, function (e, info) {
     console.log("status: " + info.status);
});
```

___

### <a id="picturechanged" name="picturechanged"></a> PictureChanged

• `Static` **PictureChanged**: `string`

当图片发生变化时触发

**`name`** GC.Spread.Sheets.Worksheet#PictureChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.FloatingObjects.Picture](GC.Spread.Sheets.FloatingObjects.Picture.md)* `picture` 触发事件的图片

**`param`** *string* `propertyName` 已更改的图片属性的名称

**`代码示例`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var activeSheet = spread.getActiveSheet();
activeSheet.pictures.add("f2","Event.png",2,2,6,6);
activeSheet.pictures.add("f1","tsoutline.png",3,0,6,6);
// Use web browser to see the console log text
activeSheet.bind(GC.Spread.Sheets.Events.PictureChanged, function (e, info) {
console.log("Sheet: " + info.sheetName);
console.log("Property: " + info.propertyName);
});
```

___

### <a id="pictureselectionchanged" name="pictureselectionchanged"></a> PictureSelectionChanged

• `Static` **PictureSelectionChanged**: `string`

当图片的选择发生改变时触发

**`name`** GC.Spread.Sheets.Worksheet#PictureSelectionChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.FloatingObjects.Picture](GC.Spread.Sheets.FloatingObjects.Picture.md)* `picture` 触发事件的图片

**`代码示例`**
```
//本示例使用了PictureSelectionChanged事件
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var activeSheet = spread.getActiveSheet();
activeSheet.pictures.add("f2","Event.png",2,2,6,6);
activeSheet.pictures.add("f1","tsoutline.png",3,0,6,6);
// Use web browser to see the console log text
activeSheet.bind(GC.Spread.Sheets.Events.PictureSelectionChanged, function (e, info) {
console.log("Sheet: " + info.sheetName);
});
```

___

### <a id="pivottablechanged" name="pivottablechanged"></a> PivotTableChanged

• `Static` **PivotTableChanged**: `string`

数据透视表筛选/排序/折叠/字段更改时触发

**`name`** GC.Spread.Sheets.Worksheet#PivotTableChanged

**`param`** *string* `pivotTableName` 透视表名称

**`param`** *string* `type` The specific operation name("filter" | "sort" | "collapse" | "fieldChanged" | "summarizedValueBy" | "showValueAs" | "dataPositionChanged" | "viewChanged").

**`param`** *string* `[fieldName]` 更改的字段名

**`param`** *string* `[sourceName]` 更改了字段 sourceName。

**`param`** *boolean* `[oldValue]` 数据透视表更改上一个属性的值(collapse, summarizedValueBy, showValueAs)

**`param`** *boolean* `[newValue]` 数据透视表更改上一个属性的值(collapse, summarizedValueBy, showValueAs)

**`param`** *number* `[sortType]` 数据透视表排序更改属性的值(排序)

**`param`** *Object* `[filterInfo]` 数据透视表筛选更改属性(筛选)的值

**`param`** *number* `[clearType]` 数据透视表清除筛选更改属性(筛选)的值

**`param`** *number* `[oldArea]` 旧数据透视表字段类型(fieldChanged)

**`param`** *number* `[oldIndex]` 旧数据透视表字段索引(fieldChanged)

**`param`** *number* `[newArea]` 新数据透视表字段类型(fieldChanged)

**`param`** *number* `[newIndex]` 新数据透视表字段索引(fieldChanged)

**`param`** *string* `[viewName]` 应用数据透视表视图名称(viewChanged)

**`代码示例`**
```
//示例
sheet.bind(GC.Spread.Sheets.Events.PivotTableChanged, function (sender, args) {
    alert("pivotTableName: " + args.pivotTableName + "changeType: " + args.type);
});
```

___

### <a id="rangechanged" name="rangechanged"></a> RangeChanged

• `Static` **RangeChanged**: `string`

单元格区域更改时触发

**`name`** GC.Spread.Sheets.Worksheet#RangeChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `row` 区域的行索引

**`param`** *number* `col` 区域的列索引

**`param`** *number* `rowCount` 区域的行数

**`param`** *number* `colCount` 区域的列数

**`param`** *string[]* `tableNames` 表名的集合

**`param`** *Object[]* `changedCells` 数据已更改的单元格的位置，每个位置都有行和列

**`param`** *[GC.Spread.Sheets.RangeChangedAction](../enums/GC.Spread.Sheets.RangeChangedAction.md)* `action` 引发RangeChanged事件的操作类型

**`param`** *boolean* `isUndo` 此事件是否来自撤消操作

**`代码示例`**
```
//本示例返回在Microsoft Internet Explorer中更改单元格区域时的工作表名称和操作
 activeSheet.bind(GC.Spread.Sheets.Events.RangeChanged, function (sender, args) {
  console.log(args.sheetName, args.action);
});
```

___

### <a id="rangefiltercleared" name="rangefiltercleared"></a> RangeFilterCleared

• `Static` **RangeFilterCleared**: `string`

清除筛选过的区域时触发

**`name`** GC.Spread.Sheets.Worksheet#RangeFilterCleared

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `col` 表单列的索引已被清除筛选

**`代码示例`**
```
//本示例使用rangefilterclear事件
activeSheet.getCell(0,0).text("Name");
activeSheet.getCell(0,1).text("Value");
activeSheet.getCell(0,2).text("T/F");
activeSheet.getCell(1,0).text("AW");
activeSheet.getCell(1,1).text("5");
activeSheet.getCell(1,2).text("T");
var cellRange =new GC.Spread.Sheets.Range(0, 0, 5, 1);
var hideRowFilter =new GC.Spread.Sheets.Filter.HideRowFilter(cellRange);
activeSheet.rowFilter(hideRowFilter);
activeSheet.bind(GC.Spread.Sheets.Events.RangeFilterCleared, function (e, info) {
        alert("Col (" + info.col + ")");
});
```

___

### <a id="rangefilterclearing" name="rangefilterclearing"></a> RangeFilterClearing

• `Static` **RangeFilterClearing**: `string`

即将自动清除筛选中的区域时触发

**`name`** GC.Spread.Sheets.Worksheet#RangeFilterClearing

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `col` 要自动清除的表单列的索引

**`代码示例`**
```
//本示例使用rangefilterclear事件
activeSheet.getCell(0,0).text("Name");
activeSheet.getCell(0,1).text("Value");
activeSheet.getCell(0,2).text("T/F");
activeSheet.getCell(1,0).text("AW");
activeSheet.getCell(1,1).text("5");
activeSheet.getCell(1,2).text("T");
var cellRange =new GC.Spread.Sheets.Range(0, 0, 5, 1);
var hideRowFilter =new GC.Spread.Sheets.Filter.HideRowFilter(cellRange);
activeSheet.rowFilter(hideRowFilter);
activeSheet.bind(GC.Spread.Sheets.Events.RangeFilterClearing, function (e, info) {
        alert("Col (" + info.col + ")");
});
```

___

### <a id="rangefiltered" name="rangefiltered"></a> RangeFiltered

• `Static` **RangeFiltered**: `string`

列被自动筛选时触发

**`name`** GC.Spread.Sheets.Worksheet#RangeFiltered

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `col` 被自动筛选的列的索引

**`param`** *Array* `filterValues` 用于筛选列的值

**`param`** *Array* `conditionInfo` 条件规则说明所筛选的列

**`代码示例`**
```
//本示例使用RangeFiltered事件
var cellrange =new GC.Spread.Sheets.Range(0, 2, 5, 1);
var hideRowFilter =new GC.Spread.Sheets.Filter.HideRowFilter(cellrange);
activeSheet.rowFilter(hideRowFilter);
activeSheet.bind(GC.Spread.Sheets.Events.RangeFiltered, function (e, info) {
        alert("Col (" + info.col + ")");
});
```

___

### <a id="rangefiltering" name="rangefiltering"></a> RangeFiltering

• `Static` **RangeFiltering**: `string`

当要自动筛选列时触发

**`name`** GC.Spread.Sheets.Worksheet#RangeFiltering

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `col` 要自动筛选的列的索引

**`param`** *Array* `filterValues` 用于筛选列的值

**`param`** *Object* `conditionInfo` 用于筛选列的条件规则信息

**`代码示例`**
```
//本示例使用RangeFiltering事件
var cellrange =new GC.Spread.Sheets.Range(0, 2, 5, 1);
var hideRowFilter =new GC.Spread.Sheets.Filter.HideRowFilter(cellrange);
activeSheet.rowFilter(hideRowFilter);
activeSheet.bind(GC.Spread.Sheets.Events.RangeFiltering, function (e, info) {
       alert("Col (" + info.col + ")");
});
```

___

### <a id="rangegroupstatechanged" name="rangegroupstatechanged"></a> RangeGroupStateChanged

• `Static` **RangeGroupStateChanged**: `string`

当用户更改行或列的分组列状态(分组区域)时触发

**`name`** GC.Spread.Sheets.Worksheet#RangeGroupStateChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *boolean* `isRowGroup` 分组列(分组区域)是否为一组行

**`param`** *number* `index` 状态已更改的RangeGroupInfo对象的索引

**`param`** *number* `level` 状态已更改的RangeGroupInfo对象的级别

**`代码示例`**
```
//本例使用RangeGroupStateChanged事件
activeSheet.suspendPaint();
activeSheet.setRowCount(34);
activeSheet.setValue(0,0,"Western");
activeSheet.setValue(0,1,"Western");
activeSheet.setValue(0,2,"Western");
activeSheet.setValue(1,0,"A");
activeSheet.setValue(1,1,"B");
activeSheet.setValue(1,2,"C");
activeSheet.setValue(2,0,"A");
activeSheet.setValue(2,1,"B");
activeSheet.setValue(2,2,"C");
activeSheet.rowOutlines.group(0,2);
activeSheet.columnOutlines.group(0,1);
activeSheet.resumePaint();
activeSheet.bind(GC.Spread.Sheets.Events.RangeGroupStateChanged, function (e, info) {
        alert("Level (" + info.level + ")");
});
```

___

### <a id="rangegroupstatechanging" name="rangegroupstatechanging"></a> RangeGroupStateChanging

• `Static` **RangeGroupStateChanging**: `string`

在用户更改行或列的分组列状态(分组区域)之前发生

**`name`** GC.Spread.Sheets.Worksheet#RangeGroupStateChanging

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *boolean* `isRowGroup` 分组列(分组区域)是否为一组行

**`param`** *number* `index` 状态正在改变的RangeGroupInfo对象的索引

**`param`** *number* `level` 状态正在改变的RangeGroupInfo对象的级别

**`param`** *boolean* `cancel` 是否应取消操作

**`代码示例`**
```
//本示例使用RangeGroupStateChanging事件
activeSheet.suspendPaint();
activeSheet.setRowCount(34);
activeSheet.setValue(0,0,"Western");
activeSheet.setValue(0,1,"Western");
activeSheet.setValue(0,2,"Western");
activeSheet.setValue(1,0,"A");
activeSheet.setValue(1,1,"B");
activeSheet.setValue(1,2,"C");
activeSheet.setValue(2,0,"A");
activeSheet.setValue(2,1,"B");
activeSheet.setValue(2,2,"C");
activeSheet.rowOutlines.group(0,2);
activeSheet.columnOutlines.group(0,1);
activeSheet.resumePaint();
activeSheet.bind(GC.Spread.Sheets.Events.RangeGroupStateChanging, function (e, info) {
        alert("Level (" + info.level + ")");
});
```

___

### <a id="rangesorted" name="rangesorted"></a> RangeSorted

• `Static` **RangeSorted**: `string`

当一列刚被自动排序时触发

**`name`** GC.Spread.Sheets.Worksheet#RangeSorted

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `col` 被自动排序的列的索引

**`param`** *boolean* `ascending` 自动排序是否升序

**`代码示例`**
```
//本示例使用了区域排序的事件
activeSheet.setValue(0, 0, 10);
activeSheet.setValue(1, 0, 100);
activeSheet.setValue(2, 0, 50);
activeSheet.setValue(3, 0, 40);
activeSheet.setValue(4, 0, 80);
activeSheet.setValue(5, 0, 1);
activeSheet.setValue(6, 0, 65);
activeSheet.setValue(7, 0, 20);
activeSheet.setValue(8, 0, 30);
activeSheet.setValue(9, 0, 35);
var cellrange =new GC.Spread.Sheets.Range(0, 0, 5, 1);
var hideRowFilter =new GC.Spread.Sheets.Filter.HideRowFilter(cellrange);
activeSheet.rowFilter(hideRowFilter);
activeSheet.bind(GC.Spread.Sheets.Events.RangeSorted, function (e, info) {
        alert("Col (" + info.col + ", " + info.ascending +")");
});
```

___

### <a id="rangesorting" name="rangesorting"></a> RangeSorting

• `Static` **RangeSorting**: `string`

将对列进行排序时触发

**`name`** GC.Spread.Sheets.Worksheet#RangeSorting

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `col` 要自动排序的列的索引

**`param`** *boolean* `ascending` 自动排序是否升序

**`param`** *boolean* `cancel` 是否应取消操作

**`param`** *[GC.Spread.Sheets.Range](GC.Spread.Sheets.Range.md)* `range` 自动排序的区域

**`param`** *[GC.Spread.Sheets.GroupSort](../enums/GC.Spread.Sheets.GroupSort.md)* `groupSort` 排序时使用的groupSort级别，如果包含组，则默认使用组级别；如果不包含组，则默认使用平面级别

**`param`** *boolean* `ignoreHidden` 是否忽略隐藏值，仅对可见值排序

**`param`** *Function* `compareFunction` 在排序时使用的自定义函数，在值排序时使用 function (value1, value2) {return 0;}

**`代码示例`**
```
//本示例使用RangeSorting事件
activeSheet.setValue(0, 0, 10);
activeSheet.setValue(1, 0, 100);
activeSheet.setValue(2, 0, 50);
activeSheet.setValue(3, 0, 40);
activeSheet.setValue(4, 0, 80);
activeSheet.setValue(5, 0, 1);
activeSheet.setValue(6, 0, 65);
activeSheet.setValue(7, 0, 20);
activeSheet.setValue(8, 0, 30);
activeSheet.setValue(9, 0, 35);
var cellrange =new GC.Spread.Sheets.Range(0, 0, 10, 1);
var hideRowFilter =new GC.Spread.Sheets.Filter.HideRowFilter(cellrange);
activeSheet.rowFilter(hideRowFilter);
activeSheet.bind(GC.Spread.Sheets.Events.RangeSorting, function (e, info) {
        alert("Col (" + info.col + ", " + info.ascending +")");
        info.groupSort = GC.Spread.Sheets.GroupSort.full; //使用完整级别排序
        info.ignoreHidden = false; // 用隐藏值排序
        info.compareFunction = (obj1, obj2)=>{return obj1.toString().localeCompare(obj2.toString())};
});
```

___

### <a id="reportsheetdatachanged" name="reportsheetdatachanged"></a> ReportSheetDataChanged

• `Static` **ReportSheetDataChanged**: `string`

当报表数据因更新、插入或删除而更改时发生。允许向服务器提交数据更改。

**`name`** GC.Spread.Report.ReportSheet#ReportSheetDataChanged

**`param`** *[GC.Spread.Report.ReportSheet](GC.Spread.Report.ReportSheet.md)* `sheet` The report sheet that triggered the event.

**`param`** *string* `sheetName` 报表的名称。

**`param`** *string* `type` 报表更改类型。插入、更新或删除。

**`param`** *number* `row` 更改后的行索引。

**`param`** *number* `col` 更改后的列索引。

**`example`**
```
//This example uses the ReportSheetDataChanged event.
const report = spread.addSheetTab(0, "Report", GC.Spread.Sheets.SheetType.reportSheet);
report.renderMode("Design");
const templateSheet = report.getTemplate();
templateSheet.setTemplateCell(0, 0, {
   binding: "Orders[orderId]",
   type: "Group",
});
templateSheet.setTemplateCell(0, 1, {
   binding: "Orders[customerId]",
   type: "Group",
});
templateSheet.setDataEntrySetting([ {
   name: "Write Back Rule 1",
   tableName: "Orders",
   fields: [
       { dbColumnName: "orderId", formula: "A1", isPrimary: true },
       { dbColumnName: "customerId", formula: "B1" },
   ],
   includeUnmodified: false,
   skipRecordWithEmptyValue: false
} ]);
report.renderMode("Preview");
report.bind(GC.Spread.Sheets.Events.ReportSheetDataChanged, (event, args) => {
    let reportsheet = args.sheet, changes = reportsheet.getChanges();
    if (allowSubmit(changes)) { // users can submit or drop this changing.
         reportsheet.submit(); // submit changes.
    } else {
         reportsheet.refresh(); // drop changes.
    }
});
// after reportsheet edit / update / delete records in UI will trigger ReportSheetDataChanged event.
// users can submit into server or drop this changing in this moment.
```

___

### <a id="reportsheetdatachanging" name="reportsheetdatachanging"></a> ReportSheetDataChanging

• `Static` **ReportSheetDataChanging**: `string`

当报表因更新、插入或删除而发生更改时发生。允许验证或取消数据操作。

**`name`** GC.Spread.Report.ReportSheet#ReportSheetDataChanging

**`param`** *[GC.Spread.Report.ReportSheet](GC.Spread.Report.ReportSheet.md)* `sheet` 触发事件的报表。

**`param`** *string* `sheetName` 报表的名称。

**`param`** *string* `type` 报表更改类型。插入、更新或删除。

**`param`** *number* `row` 变化的行索引。

**`param`** *number* `col` 变化的列索引。

**`param`** *any* `oldValue` 更新改变旧值。

**`param`** *any* `newValue` 更新改变了新值。

**`param`** *boolean* `cancel` 是否取消报表变更操作。

**`example`**
```
//This example uses the ReportSheetDataChanging event.
const report = spread.addSheetTab(0, "Report", GC.Spread.Sheets.SheetType.reportSheet);
report.renderMode("Design");
const templateSheet = report.getTemplate();
templateSheet.setTemplateCell(0, 0, {
   binding: "Orders[orderId]",
   type: "Group",
});
templateSheet.setTemplateCell(0, 1, {
   binding: "Orders[customerId]",
   type: "Group",
});
templateSheet.setDataEntrySetting([ {
   name: "Write Back Rule 1",
   tableName: "Orders",
   fields: [
       { dbColumnName: "orderId", formula: "A1", isPrimary: true },
       { dbColumnName: "customerId", formula: "B1" },
   ],
   includeUnmodified: false,
   skipRecordWithEmptyValue: false
} ]);
report.renderMode("Preview");
report.bind(GC.Spread.Sheets.Events.ReportSheetDataChanging, (event, args) => {
    let { type, row, col, oldValue, newValue } = args;
    if (allowChange(type, row, col, oldValue, newValue)) { // user validate this changing operation here.
        console.log(`${type} row: ${row}, col: ${col} from ${oldValue} to ${newValue}`);
    } else {
        args.cancel = true;
    }
});
// reportsheet edit / update / delete records in UI will trigger ReportSheetDataChanging event.
// users can also cancel the operation here if the changing is invalid.
```

___

### <a id="reportsheetrecordssubmitted" name="reportsheetrecordssubmitted"></a> ReportSheetRecordsSubmitted

• `Static` **ReportSheetRecordsSubmitted**: `string`

在报表将更改提交到服务器后发生。  允许用户提供服务器提交结果的 UI 反馈。

**`name`** GC.Spread.Report.ReportSheet#ReportSheetRecordsSubmitted

**`param`** *[GC.Spread.Report.ReportSheet](GC.Spread.Report.ReportSheet.md)* `sheet` 触发事件的报表。

**`param`** *string* `sheetName` 报表的名称。

**`param`** *{@link GC.Spread.Report.IRecord[]}* `updateSuccessRecords` 成功更新或插入记录。

**`param`** *{@link GC.Spread.Report.IFailedRecord[]}* `updateFailedRecords` 更新或插入记录失败。

**`param`** *{@link GC.Spread.Report.IRecord[]}* `deleteSuccessRecords` 删除记录成功。

**`param`** *{@link GC.Spread.Report.IFailedRecord[]}* `deleteFailedRecords` 删除记录失败。

**`example`**
```
//This example uses the ReportSheetDataChanged event.
const report = spread.addSheetTab(0, "Report", GC.Spread.Sheets.SheetType.reportSheet);
report.renderMode("Design");
const templateSheet = report.getTemplate();
templateSheet.setTemplateCell(0, 0, {
   binding: "Orders[orderId]",
   type: "Group",
});
templateSheet.setTemplateCell(0, 1, {
   binding: "Orders[customerId]",
   type: "Group",
});
templateSheet.setDataEntrySetting([ {
   name: "Write Back Rule 1",
   tableName: "Orders",
   fields: [
       { dbColumnName: "orderId", formula: "A1", isPrimary: true },
       { dbColumnName: "customerId", formula: "B1" },
   ],
   includeUnmodified: false,
   skipRecordWithEmptyValue: false
} ]);
report.renderMode("Preview");
report.bind(GC.Spread.Sheets.Events.ReportSheetRecordsSubmitted, (event, args) => {
    let { updateSuccessRecords, deleteSuccessRecords, updateFailedRecords, deleteFailedRecords } = args;
    for (let record of updateFailedRecords) {
        for (let fieldKey in record.info) {
            if (record.info.hasOwnproperty(fieldKey)) {
                let recordDetail = record.info[fieldKey];
                if (recordDetail.state === "updated") {
                    // user console the failed detail info.
                    console.log(`Updated failed in row: ${recordDetail.row} col: ${recordDetail.col}, oldValue: ${recordDetail.oldValue}, reason is ${record.reason}`);
                }
            }
        }
    }
});
// after submitting into the server, users can get the all success and failed records result.
```

___

### <a id="reportsheetrecordssubmitting" name="reportsheetrecordssubmitting"></a> ReportSheetRecordsSubmitting

• `Static` **ReportSheetRecordsSubmitting**: `string`

在报表向服务器提交更改之前发生。允许最终验证所有数据更改或取消操作。

**`name`** GC.Spread.Report.ReportSheet#ReportSheetRecordsSubmitting

**`param`** *[GC.Spread.Report.ReportSheet](GC.Spread.Report.ReportSheet.md)* `sheet` 触发事件的报表。

**`param`** *string* `sheetName` 报表的名称。

**`param`** *boolean* `cancel` 是否取消报表提交操作。

**`example`**
```
//This example uses the ReportSheetDataChanged event.
const report = spread.addSheetTab(0, "Report", GC.Spread.Sheets.SheetType.reportSheet);
report.renderMode("Design");
const templateSheet = report.getTemplate();
templateSheet.setTemplateCell(0, 0, {
   binding: "Orders[orderId]",
   type: "Group",
});
templateSheet.setTemplateCell(0, 1, {
   binding: "Orders[customerId]",
   type: "Group",
});
templateSheet.setDataEntrySetting([ {
   name: "Write Back Rule 1",
   tableName: "Orders",
   fields: [
       { dbColumnName: "orderId", formula: "A1", isPrimary: true },
       { dbColumnName: "customerId", formula: "B1" },
   ],
   includeUnmodified: false,
   skipRecordWithEmptyValue: false
} ]);
report.renderMode("Preview");
report.bind(GC.Spread.Sheets.Events.ReportSheetRecordsSubmitting, (event, args) => {
    let reportsheet = args.sheet, changes = reportsheet.getChanges();
    if (isInvalidate(changes)) {
        args.cancel = true;
    }
});
// after submitting the report chages, users can validate the changes and cancel this submit.
```

___

### <a id="rowchanged" name="rowchanged"></a> RowChanged

• `Static` **RowChanged**: `string`

当对此表单中的行或行区域进行更改，可能需要重新绘制行或行区域时触发

**`name`** GC.Spread.Sheets.Worksheet#RowChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `row` 行索引

**`param`** *[GC.Spread.Sheets.SheetArea](../enums/GC.Spread.Sheets.SheetArea.md)* `sheetArea` 表单区域

**`param`** *string* `propertyName` 已更改的行属性的名称

**`param`** *boolean* `isUndo` 此事件是否来自撤消操作

**`代码示例`**
```
//本示例使用了RowChanged事件
activeSheet.bind(GC.Spread.Sheets.Events.RowChanged, function (e, info) {
        alert("Row (" + info.row + ")");
});
```

___

### <a id="rowchanging" name="rowchanging"></a> RowChanging

• `Static` **RowChanging**: `string`

在对此表单中的行或行区域进行更改之前发生，可能需要重新绘制行或行区域

**`name`** GC.Spread.Sheets.Worksheet#RowChanging

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `row` 行索引

**`param`** *[GC.Spread.Sheets.SheetArea](../enums/GC.Spread.Sheets.SheetArea.md)* `sheetArea` 表单区域

**`param`** *string* `propertyName` 已更改的行属性的名称

**`代码示例`**
```
//本示例使用了RowChanging事件
activeSheet.bind(GC.Spread.Sheets.Events.RowChanging, function (e, info) {
        alert("Row (" + info.row + ")");
});
```

___

### <a id="rowheightchanged" name="rowheightchanged"></a> RowHeightChanged

• `Static` **RowHeightChanged**: `string`

当行高度发生更改时触发

**`name`** GC.Spread.Sheets.Worksheet#RowHeightChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *Array* `rowList` 高度已更改的行列表

**`param`** *boolean* `header` 列是否为列标题列

**`代码示例`**
```
//本例使用了RowHeightChanged事件
activeSheet.bind(GC.Spread.Sheets.Events.RowHeightChanged, function (e, info) {
        alert("Row List (" + info.rowList + ")");
});
```

___

### <a id="rowheightchanging" name="rowheightchanging"></a> RowHeightChanging

• `Static` **RowHeightChanging**: `string`

当行高发生变化时触发

**`name`** GC.Spread.Sheets.Worksheet#RowHeightChanging

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *Array* `rowList` 高度发生变化的行列表

**`param`** *boolean* `header` 列是否为列标题列

**`param`** *boolean* `cancel` 是否应取消操作

**`代码示例`**
```
//本例使用了RowHeightChanging事件
activeSheet.bind(GC.Spread.Sheets.Events.RowHeightChanging, function (e, info) {
        alert("Row List (" + info.rowList + ")");
});
```

___

### <a id="rowoperation" name="rowoperation"></a> RowOperation

• `Static` **RowOperation**: `string`

应用于行操作时触发

**`name`** GC.Spread.Sheets.TableSheet.TableSheet#RowOperation

**`param`** *[GC.Spread.Sheets.TableSheet.TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md)* `sheet` 触发事件的集算表

**`param`** *string* `sheetName` 集算表名称

**`param`** *[GC.Spread.Sheets.TableSheet.ActionType](../enums/GC.Spread.Sheets.TableSheet.ActionType.md)* `actionType` 行操作类型

**`param`** *number* `row` 行索引

**`代码示例`**
```
//本例使用了RowHeightChanging事件
workbook.bind(GC.Spread.Sheets.Events.RowOperation, function (e, info) {
    console.log(info.sheetName, info.actionType, info.row);
});
```

___

### <a id="selectionchanged" name="selectionchanged"></a> SelectionChanged

• `Static` **SelectionChanged**: `string`

当表单上的单元格选区发生更改时触发

**`name`** GC.Spread.Sheets.Worksheet#SelectionChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *{@link GC.Spread.Sheets.Range[]}* `oldSelections` 旧的选择区域

**`param`** *{@link GC.Spread.Sheets.Range[]}* `newSelections` 新的选择区域

**`代码示例`**
```
//本例使用SelectionChanged事件
activeSheet.bind(GC.Spread.Sheets.Events.SelectionChanged, function (e, info) {
        alert("Name (" + info.sheetName + ")");
});
```

___

### <a id="selectionchanging" name="selectionchanging"></a> SelectionChanging

• `Static` **SelectionChanging**: `string`

当表单上的单元格选择发生改变时触发

**`name`** GC.Spread.Sheets.Worksheet#SelectionChanging

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *{@link GC.Spread.Sheets.Range[]}* `oldSelections` 旧的选择区域

**`param`** *{@link GC.Spread.Sheets.Range[]}* `newSelections` 新的选择区域

**`代码示例`**
```
//本例使用SelectionChanging事件
activeSheet.bind(GC.Spread.Sheets.Events.SelectionChanging, function (e, info) {
//使用浏览器查看控制台
        console.log("Name (" + info.sheetName + ")");
});
```

___

### <a id="shapechanged" name="shapechanged"></a> ShapeChanged

• `Static` **ShapeChanged**: `string`

当任何形状发生变化时触发

**`name`** GC.Spread.Sheets.Worksheet#ShapeChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.Shapes.Shape](GC.Spread.Sheets.Shapes.Shape.md)* `shape` 触发事件的形状

**`param`** *string* `propertyName` 已更改的形状属性的名称

**`代码示例`**
```
//本例使用ShapeChanged事件
var shape1 = activeSheet.shapes.add("shape1", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 20, 20, 200, 200);
activeSheet.bind(GC.Spread.Sheets.Events.ShapeChanged, function (e, info) {
       alert("changed");
});
```

___

### <a id="shaperemoved" name="shaperemoved"></a> ShapeRemoved

• `Static` **ShapeRemoved**: `string`

当用户删除形状时触发

**`name`** GC.Spread.Sheets.Worksheet#ShapeRemoved

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.Shapes.Shape](GC.Spread.Sheets.Shapes.Shape.md)* `shape` 形状已经被移除

**`代码示例`**
```
//本示例使用ShapeRemoved事件
var shape = activeSheet.shapes.add("myShape", GC.Spread.Sheets.Shapes.AutoShapeType.diamond, 0, 90, 200, 200);
activeSheet.bind(GC.Spread.Sheets.Events.ShapeRemoved, function (e, info) {
        alert(info.shape.name());
});
```

___

### <a id="shaperemoving" name="shaperemoving"></a> ShapeRemoving

• `Static` **ShapeRemoving**: `string`

当用户移除任何形状时触发

**`name`** GC.Spread.Sheets.Worksheet#ShapeRemoving

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.Shapes.Shape](GC.Spread.Sheets.Shapes.Shape.md)* `shape` 形状正在被移除

**`param`** *boolean* `cancel` 是否应取消操作

**`代码示例`**
```
//本示例使用ShapeRemoving事件
var shape = sheet.shapes.add("myShape", GC.Spread.Sheets.Shapes.AutoShapeType.diamond, 0, 90, 200, 200);
activeSheet.bind(GC.Spread.Sheets.Events.ShapeRemoving, function (e, info) {
        info.cancel = true;// 形状不会被移除
});
```

___

### <a id="shapeselectionchanged" name="shapeselectionchanged"></a> ShapeSelectionChanged

• `Static` **ShapeSelectionChanged**: `string`

当形状的选择发生变化时触发

**`name`** GC.Spread.Sheets.Worksheet#ShapeSelectionChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.Shapes.Shape](GC.Spread.Sheets.Shapes.Shape.md)* `shape` 触发事件的形状

**`代码示例`**
```
//本示例使用ShapeSelectionChanged事件
var shape = sheet.shapes.add("myShape", GC.Spread.Sheets.Shapes.AutoShapeType.diamond, 0, 90, 200, 200);
activeSheet.bind(GC.Spread.Sheets.Events.ShapeSelectionChanged, function (e, info) {
       console.log("event info: " + info);
});
```

___

### <a id="sheetchanged" name="sheetchanged"></a> SheetChanged

• `Static` **SheetChanged**: `string`

表单改变后

**`name`** GC.Spread.Sheets.Worksheet#SheetChanged

**`param`** *string* `sheetName` 表单名称

**`param`** *string* `propertyName` 特定的操作名称

**`param`** *number* `sheetIndex` 工作表索引，与工作表集合或标签页集合相关

**`param`** *number* `sheetPosition` 表单的位置, 与包含所有工作表和标签页的组合集合相关

**`param`** *boolean* `oldValue` 表单改变了先前属性的值(isVisible, isSelected…)

**`param`** *boolean* `newValue` 表单改变属性的值(isVisible, isSelected…)

**`代码示例`**
```
//示例
spread.bind(GC.Spread.Sheets.Events.SheetChanged, function (sender, args) {
    var sheet = args.sheet;
});
```

___

### <a id="sheetchanging" name="sheetchanging"></a> SheetChanging

• `Static` **SheetChanging**: `string`

表单改变前

**`name`** GC.Spread.Sheets.Worksheet#SheetChanging

**`param`** *string* `sheetName` 表单名称

**`param`** *string* `propertyName` 特定的操作名称

**`param`** *number* `sheetIndex` 改变表单位置

**`param`** *boolean* `oldValue` 表单改变了先前属性的值(isVisible, isSelected…)

**`param`** *boolean* `oldValue` 工作表更改前一个属性的值（isVisible、isSelected...）

**`param`** *boolean* `newValue` 工作表更改属性的值（isVisible、isSelected...）

**`param`** *boolean* `cancel` Cancel the current operation.

**`example`**
```
//示例
spread.bind(GC.Spread.Sheets.Events.SheetChanging, function (sender, args) {
    var sheetIndex = args.sheetIndex;
    args.cancel = true;
});
```

___

### <a id="sheetmoved" name="sheetmoved"></a> SheetMoved

• `Static` **SheetMoved**: `string`

在用户拖动和移动表单之后发生

**`name`** GC.Spread.Sheets.Worksheet#SheetMoved

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `oldIndex` 前一个表单索引

**`param`** *number* `newIndex` 新的表单索引

**`代码示例`**
```
//本例使用了SheetMoved事件
window.onload = function(){
     var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
     var activeSheet = spread.getActiveSheet();
     spread.bind(GC.Spread.Sheets.Events.SheetMoving, function (e, data) {
         alert(data.sheetName + '\n' +  'oldIndex: ' + data.oldIndex + '\n' +  'newIndex: ' + data.newIndex + '\n' +  'cancel: ' + data.cancel);
     });
     spread.bind(GC.Spread.Sheets.Events.SheetMoved, function (e, data) {
         alert(data.sheetName + '\n' +  'oldIndex: ' + data.oldIndex + '\n' +  'newIndex: ' + data.newIndex);
     });
}
```

___

### <a id="sheetmoving" name="sheetmoving"></a> SheetMoving

• `Static` **SheetMoving**: `string`

在用户拖动和移动表单之前发生

**`name`** GC.Spread.Sheets.Worksheet#SheetMoving

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `oldIndex` 旧表索引

**`param`** *number* `newIndex` 索引将移动到的值

**`param`** *boolean* `cancel` 是否应取消操作

**`代码示例`**
```
//本例使用了SheetMoving事件
window.onload = function(){
     var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
     var activeSheet = spread.getActiveSheet();
     spread.bind(GC.Spread.Sheets.Events.SheetMoving, function (e, data) {
         alert(data.sheetName + '\n' +  'oldIndex: ' + data.oldIndex + '\n' +  'newIndex: ' + data.newIndex + '\n' +  'cancel: ' + data.cancel);
     });
     spread.bind(GC.Spread.Sheets.Events.SheetMoved, function (e, data) {
         alert(data.sheetName + '\n' +  'oldIndex: ' + data.oldIndex + '\n' +  'newIndex: ' + data.newIndex);
     });
}
```

___

### <a id="sheetnamechanged" name="sheetnamechanged"></a> SheetNameChanged

• `Static` **SheetNameChanged**: `string`

当用户更改了表单名称时触发

**`name`** GC.Spread.Sheets.Worksheet#SheetNameChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `oldValue` 表单的旧名字

**`param`** *string* `newValue` 表单的新名字

**`代码示例`**
```
//此示例使用 SheetNameChanged 事件
//使用网络浏览器查看控制台日志文本
spread.bind(GC.Spread.Sheets.Events.SheetNameChanging, function (sender, args) {
   console.log(args.oldValue);
});
spread.bind(GC.Spread.Sheets.Events.SheetNameChanged, function (sender, args) {
   console.log(args.newValue);
});
```

___

### <a id="sheetnamechanging" name="sheetnamechanging"></a> SheetNameChanging

• `Static` **SheetNameChanging**: `string`

当用户更改表单名称时触发

**`name`** GC.Spread.Sheets.Worksheet#SheetNameChanging

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `oldValue` 表单的旧名字

**`param`** *string* `newValue` 表单的新名字

**`param`** *boolean* `cancel` 是否应取消操作

**`代码示例`**
```
//本示例使用了SheetNameChanging事件
// Use web browser to see the console log text
spread.bind(GC.Spread.Sheets.Events.SheetNameChanging, function (sender, args) {
   console.log(args.oldValue);
});
spread.bind(GC.Spread.Sheets.Events.SheetNameChanged, function (sender, args) {
   console.log(args.newValue);
});
```

___

### <a id="sheettabclick" name="sheettabclick"></a> SheetTabClick

• `Static` **SheetTabClick**: `string`

当用户单击表单选项卡时触发

**`name`** GC.Spread.Sheets.Worksheet#SheetTabClick

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `sheetTabIndex` 用户单击的表单选项卡的索引

**`代码示例`**
```
//本例使用了SheetTabClick事件
spread.bind(GC.Spread.Sheets.Events.SheetTabClick, function (e, info) {
        alert("Index (" + info.sheetTabIndex + ")");
});
```

___

### <a id="sheettabdoubleclick" name="sheettabdoubleclick"></a> SheetTabDoubleClick

• `Static` **SheetTabDoubleClick**: `string`

当用户双击表单选项卡时触发

**`name`** GC.Spread.Sheets.Worksheet#SheetTabDoubleClick

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `sheetTabIndex` 用户双击的表单选项卡的索引

**`代码示例`**
```
//本示例使用SheetTabDoubleClick事件
spread.bind(GC.Spread.Sheets.Events.SheetTabDoubleClick, function (e, info) {
        alert("Index (" + info.sheetTabIndex + ")");
});
```

___

### <a id="slicerchanged" name="slicerchanged"></a> SlicerChanged

• `Static` **SlicerChanged**: `string`

任何切片器已改变触发

**`name`** GC.Spread.Sheets.Worksheet#SlicerChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.Slicers.ISlicer](../interfaces/GC.Spread.Sheets.Slicers.ISlicer.md)* `slicer` 触发事件的切片器

**`param`** *string* `propertyName` 已更改的切片器属性的名称

**`代码示例`**
```
//本示例使用了SlicerChanged事件
//创建一个表
datas = [
    ["1", "NewYork", "1968/6/8", "80", "180"],
    ["4", "NewYork", "1972/7/3", "72", "168"],
    ["4", "NewYork", "1964/3/2", "71", "179"],
    ["5", "Washington", "1972/8/8","80", "171"],
    ["6", "Washington", "1986/2/2", "89", "161"],
    ["7", "Washington", "2012/2/15", "71", "240"]];
var table = activeSheet.tables.addFromDataSource("table1", 2, 2, datas);
dataColumns = ["Name", "City", "Birthday", "Weight", "Height"];
table.setColumnName(0, dataColumns[0]);
table.setColumnName(1, dataColumns[1]);
table.setColumnName(2, dataColumns[2]);
table.setColumnName(3, dataColumns[3]);
table.setColumnName(4, dataColumns[4]);
//向表单添加一个切片器并返回切片器实例
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Name");
//改变切片器的属性
slicer.width(200);
slicer.height(200);
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.style(GC.Spread.Sheets.Slicers.SlicerStyles.dark4());
// Use web browser to see the console log text
activeSheet.bind(GC.Spread.Sheets.Events.SlicerChanged, function (e, info) {
console.log("name: " + info.propertyName);
});
```

___

### <a id="sparklinechanged" name="sparklinechanged"></a> SparklineChanged

• `Static` **SparklineChanged**: `string`

迷你图改变后触发

**`name`** GC.Spread.Sheets.Worksheet#SparklineChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.Sparklines.Sparkline](GC.Spread.Sheets.Sparklines.Sparkline.md)* `sparkline` 属性改变的迷你图

**`代码示例`**
```
//移除迷你图会引起一个变化
var data = new GC.Spread.Sheets.Range(1, 0, 8, 1);
var setting = new GC.Spread.Sheets.Sparklines.SparklineSetting();
setting.options.showMarkers = true;
setting.options.lineWeight = 3;
setting.options.displayXAxis = true;
setting.options.showFirst = true;
setting.options.showLast = true;
setting.options.showLow = true;
setting.options.showHigh = true;
setting.options.showNegative = true;
setting.options.seriesColor = "Text 2 1";
setting.options.firstMarkerColor = "Text 2 3";
setting.options.negativeColor = "Accent 2 1";
setting.options.markersColor = "Accent 3 1";
setting.options.lowMarkerColor = "Accent 4 1";
setting.options.highMarkerColor = "Accent 6 1";
setting.options.lastMarkerColor = "Accent 6 6";
setting.options.axisColor = "Text 1 1";
activeSheet.addSpan(13, 0, 4, 3, null);
activeSheet.setSparkline(13, 0, data, GC.Spread.Sheets.Sparklines.DataOrientation.vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
activeSheet.setValue(1, 0, 1);
activeSheet.setValue(2, 0, -2);
activeSheet.setValue(3, 0, -1);
activeSheet.setValue(4, 0, 6);
activeSheet.setValue(5, 0, 4);
activeSheet.setValue(6, 0, -4);
activeSheet.setValue(7, 0, 3);
activeSheet.setValue(8, 0, 8);
// Use web browser to see the console log text
activeSheet.bind(GC.Spread.Sheets.Events.SparklineChanged, function (e, info) {
     console.log("name: " + info.sheetName);
});
$("#button1").click(function () {
     activeSheet.removeSparkline(13, 0);
});
```

___

### <a id="tablecolumnschanged" name="tablecolumnschanged"></a> TableColumnsChanged

• `Static` **TableColumnsChanged**: `string`

当用户在表中插入/删除列时触发

**`name`** GC.Spread.Sheets.Worksheet#TableColumnsChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *[GC.Spread.Sheets.Tables.Table](GC.Spread.Sheets.Tables.Table.md)* `table` 插入/删除行的表

**`param`** *string* `propertyName` 触发事件的操作名称

**`param`** *number* `col` 根据表索引要插入/删除的起始列的索引

**`param`** *number* `count` 要插入/删除的列数

**`param`** *boolean* `isAfter` 是否在指定的列索引之前或之后插入列 默认情况下为false,插入之前

**`代码示例`**
```
//本示例使用TableColumnsChanged事件
window.onload = function(){
     var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
     var activeSheet = spread.getActiveSheet();
     spread.bind(GC.Spread.Sheets.Events.TableColumnsChanged, function (e, data) {});
}
```

___

### <a id="tablefiltercleared" name="tablefiltercleared"></a> TableFilterCleared

• `Static` **TableFilterCleared**: `string`

表列被清除筛选时触发

**`name`** GC.Spread.Sheets.Worksheet#TableFilterCleared

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.Tables.Table](GC.Spread.Sheets.Tables.Table.md)* `table` 要筛选的表列

**`param`** *number* `tableCol` 刚被清除的表列索引

**`代码示例`**
```
//本示例使用了TableFilterCleared事件
activeSheet.tables.add("Table1", 0, 0, 3, 3, GC.Spread.Sheets.Tables.TableTheme.dark1);
activeSheet.getCell(0,0).text("Name");
activeSheet.getCell(0,1).text("Value");
activeSheet.getCell(0,2).text("T/F");
activeSheet.getCell(1,0).text("AW");
activeSheet.getCell(1,1).text("5");
activeSheet.getCell(1,2).text("T");
activeSheet.bind(GC.Spread.Sheets.Events.TableFilterCleared, function (e, info) {
       alert("Sheet (" + info.sheetName + ")");
});
```

___

### <a id="tablefilterclearing" name="tablefilterclearing"></a> TableFilterClearing

• `Static` **TableFilterClearing**: `string`

表列清除筛选时触发

**`name`** GC.Spread.Sheets.Worksheet#TableFilterCleared

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.Tables.Table](GC.Spread.Sheets.Tables.Table.md)* `table` 要筛选的表列

**`param`** *number* `tableCol` 要清除的表列的索引筛选

**`代码示例`**
```
//本示例使用了TableFilterClearing事件
activeSheet.tables.add("Table1", 0, 0, 3, 3, GC.Spread.Sheets.Tables.TableTheme.dark1);
activeSheet.getCell(0,0).text("Name");
activeSheet.getCell(0,1).text("Value");
activeSheet.getCell(0,2).text("T/F");
activeSheet.getCell(1,0).text("AW");
activeSheet.getCell(1,1).text("5");
activeSheet.getCell(1,2).text("T");
activeSheet.bind(GC.Spread.Sheets.Events.TableFilterClearing, function (e, info) {
       alert("Sheet (" + info.sheetName + ")");
});
```

___

### <a id="tablefiltered" name="tablefiltered"></a> TableFiltered

• `Static` **TableFiltered**: `string`

自动筛选表列时触发

**`name`** GC.Spread.Sheets.Worksheet#TableFiltered

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.Tables.Table](GC.Spread.Sheets.Tables.Table.md)* `table` 要筛选的表列

**`param`** *number* `col` 要筛选的表列的索引

**`param`** *Array* `filterValues` 用于筛选列的值

**`param`** *Object* `conditionInfo` 用于筛选列的条件规则信息

**`代码示例`**
```
//本示例使用了TableFiltered事件
activeSheet.tables.add("Table1", 0, 0, 3, 3, GC.Spread.Sheets.Tables.TableTheme.dark1);
activeSheet.getCell(0,0).text("Name");
activeSheet.getCell(0,1).text("Value");
activeSheet.getCell(0,2).text("T/F");
activeSheet.getCell(1,0).text("AW");
activeSheet.getCell(1,1).text("5");
activeSheet.getCell(1,2).text("T");
activeSheet.bind(GC.Spread.Sheets.Events.TableFiltered, function (e, info) {
       alert("Sheet (" + info.sheetName + ")");
});
```

___

### <a id="tablefiltering" name="tablefiltering"></a> TableFiltering

• `Static` **TableFiltering**: `string`

当筛选表列时触发

**`name`** GC.Spread.Sheets.Worksheet#TableFiltering

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *[GC.Spread.Sheets.Tables.Table](GC.Spread.Sheets.Tables.Table.md)* `table` 要筛选的表列

**`param`** *number* `col` 要筛选的表列的索引

**`param`** *Array* `filterValues` 用于筛选列的值

**`param`** *Object* `conditionInfo` 用于筛选列的条件规则信息

**`代码示例`**
```
//本示例使用TableFiltering事件
activeSheet.tables.add("Table1", 0, 0, 3, 3, GC.Spread.Sheets.Tables.TableTheme.dark1);
activeSheet.getCell(0,0).text("Name");
activeSheet.getCell(0,1).text("Value");
activeSheet.getCell(0,2).text("T/F");
activeSheet.getCell(1,0).text("AW");
activeSheet.getCell(1,1).text("5");
activeSheet.getCell(1,2).text("T");
activeSheet.bind(GC.Spread.Sheets.Events.TableFiltering, function (e, info) {
       alert("Sheet (" + info.sheetName + ")");
});
```

___

### <a id="tableresized" name="tableresized"></a> TableResized

• `Static` **TableResized**: `string`

在用户调整表大小后触发

**`name`** GC.Spread.Sheets.Worksheet#TableResized

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *[GC.Spread.Sheets.Tables.Table](GC.Spread.Sheets.Tables.Table.md)* `table` 调整的表格

**`param`** *[GC.Spread.Sheets.Range](GC.Spread.Sheets.Range.md)* `oldRange` 调整前的区域

**`param`** *[GC.Spread.Sheets.Range](GC.Spread.Sheets.Range.md)* `newRange` 调整后的区域

___

### <a id="tableresizing" name="tableresizing"></a> TableResizing

• `Static` **TableResizing**: `string`

当用户通过调整大小句柄调整表格大小时发生

**`name`** GC.Spread.Sheets.Worksheet#TableResizing

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *[GC.Spread.Sheets.Tables.Table](GC.Spread.Sheets.Tables.Table.md)* `table` 调整的表格

**`param`** *[GC.Spread.Sheets.Range](GC.Spread.Sheets.Range.md)* `oldRange` 调整前的区域

**`param`** *[GC.Spread.Sheets.Range](GC.Spread.Sheets.Range.md)* `newRange` 调整后的区域

**`代码示例`**
```
//本示例使用TableResizing和TableResized事件
window.onload = function(){
     var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
     var activeSheet = spread.getActiveSheet();
     spread.bind(GC.Spread.Sheets.Events.TableResizing, function (e, data) {});
     spread.bind(GC.Spread.Sheets.Events.TableResized, function (e, data) {});
}
```

___

### <a id="tablerowschanged" name="tablerowschanged"></a> TableRowsChanged

• `Static` **TableRowsChanged**: `string`

用户在表中插入/删除行时触发

**`name`** GC.Spread.Sheets.Worksheet#TableRowsChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *[GC.Spread.Sheets.Tables.Table](GC.Spread.Sheets.Tables.Table.md)* `table` 插入/删除行的表

**`param`** *string* `propertyName` 触发事件的操作名称

**`param`** *number* `row` 基于表索引的要插入/删除的起始行的索引

**`param`** *number* `count` 要插入/删除的行数

**`param`** *boolean* `isAfter` 是在指定的行索引之前还是之后插入行默认情况下为false,在前面插入

**`param`** *Object[]* `deletedItem` 绑定中已删除的行集合数组中的每个项指定已删除的数据项

**`代码示例`**
```
//本例使用TableRowsChanged事件
window.onload = function(){
     var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
     var activeSheet = spread.getActiveSheet();
     spread.bind(GC.Spread.Sheets.Events.TableRowsChanged, function (e, data) {});
}
```

___

### <a id="toprowchanged" name="toprowchanged"></a> TopRowChanged

• `Static` **TopRowChanged**: `string`

在第一行更改时触发

**`name`** GC.Spread.Sheets.Worksheet#TopRowChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `oldTopRow` 旧的顶部行索引

**`param`** *number* `newTopRow` 新的顶部行索引

**`param`** *number* `oldOffset` 旧的偏移

**`param`** *number* `newOffset` 新的偏移

**`example`**
```
//本示例同步了表单1和表单2的垂直和水平滚动
var sheet1 = spread.getSheet(0),
sheet2 = spread.getSheet(1);
sheet1.bind(GC.Spread.Sheets.Events.TopRowChanged, function (sender, args) {
    //将显示的sheet1的第一行设置到sheet2(垂直滚动同步)
    sheet2.showRow(args.newTopRow, GC.Spread.Sheets.VerticalPosition.top);
});
sheet1.bind(GC.Spread.Sheets.Events.LeftColumnChanged, function (sender, args) {
    //将显示的sheet1的左列设置到sheet2(水平滚动同步)
    sheet2.showColumn(args.newLeftCol, GC.Spread.Sheets.HorizontalPosition.left);
});
```

___

### <a id="touchtoolstripopening" name="touchtoolstripopening"></a> TouchToolStripOpening

• `Static` **TouchToolStripOpening**: `string`

在触摸工具栏弹出之前发生

**`name`** GC.Spread.Sheets.Worksheet#TouchToolStripOpening

**`param`** *number* `x` <i>x</i>轴，水平位置坐标

**`param`** *number* `y` <i>y</i>轴，垂直位置坐标

**`param`** *boolean* `handled` 如果为`true`,触摸工具栏被阻止弹出；否则，工具栏将显示在默认位置

**`代码示例`**
```
//本示例使用了TouchToolStripOpening事件
 activeSheet.bind(GC.Spread.Sheets.Events.TouchToolStripOpening, function (e, info) {
        alert(info.x);
});
```

___

### <a id="userformulaentered" name="userformulaentered"></a> UserFormulaEntered

• `Static` **UserFormulaEntered**: `string`

在用户键入公式时触发

**`name`** GC.Spread.Sheets.Worksheet#UserFormulaEntered

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `row` 用户在其中输入公式的单元格的行索引

**`param`** *number* `col` 用户在其中输入公式的单元格的列索引

**`param`** *string* `formula` 用户输入的公式

**`param`** *boolean* `isCircularReference` 输入的公式为循环引用

**`代码示例`**
```
//本示例使用UserFormulaEntered事件
 activeSheet.bind(GC.Spread.Sheets.Events.UserFormulaEntered, function (e, info) {
        alert("Formula (" + info.formula + ")");
});
```

___

### <a id="validationerror" name="validationerror"></a> ValidationError

• `Static` **ValidationError**: `string`

当应用的单元格值无效时触发

**`name`** GC.Spread.Sheets.Worksheet#ValidationError

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `row` 单元格的行索引

**`param`** *number* `col` 单元格的列索引

**`param`** *[GC.Spread.Sheets.DataValidation.DefaultDataValidator](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md)* `validator` 导致错误的数据验证器

**`param`** *[GC.Spread.Sheets.DataValidation.DataValidationResult](../enums/GC.Spread.Sheets.DataValidation.DataValidationResult.md)* `validationResult` 用户可以设置以确定如何处理错误的策略

**`代码示例`**
```
//This example uses the ValidationError event.
var nCondition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.cellValueCondition);
nCondition.compareType(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.equalsTo);
nCondition.expected(0);
//When the option is false, the validation fails and the red alert is displayed.
//When the option is true, the blank cell is treated as zero and the validation is successful.
nCondition.treatNullValueAsZero(false);
var validator = new GC.Spread.Sheets.DataValidation.DefaultDataValidator(nCondition)
validator.ignoreBlank(false);
validator.type(GC.Spread.Sheets.DataValidation.CriteriaType.wholeNumber)
activeSheet.getCell(0, 0, GC.Spread.Sheets.SheetArea.viewport).validator(validator);
spread.options.highlightInvalidData = true;
activeSheet.setValue(0, 0, null);
//Type different values in cell (0,0). This event fires if the user types an invalid value.
activeSheet.bind("ValidationError", vError);
function vError(sender, args) {
    alert("error");
}
```

___

### <a id="valuechanged" name="valuechanged"></a> ValueChanged

• `Static` **ValueChanged**: `string`

值发生更改时触发

**`name`** GC.Spread.Sheets.Worksheet#ValueChanged

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `row` 单元格的行索引

**`param`** *number* `col` 单元格的列索引

**`param`** *Object* `oldValue` 单元格的旧值

**`param`** *Object* `newValue` 单元格的新值

**`代码示例`**
```
//本示例使用ValueChanged事件
activeSheet.bind(GC.Spread.Sheets.Events.ValueChanged, function (e, info) {
        alert("Value (" + info.newValue + ")");
});
```

___

### <a id="viewzoomed" name="viewzoomed"></a> ViewZoomed

• `Static` **ViewZoomed**: `string`

在用户缩放后触发

**`name`** GC.Spread.Sheets.Worksheet#ViewZoomed

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `newZoomFactor` 新的缩放系数

**`param`** *number* `oldZoomFactor` 原始的缩放系数

**`代码示例`**
```
//本示例使用ViewZoomed事件
spread.options.allowUserZoom = true;
activeSheet.bind(GC.Spread.Sheets.Events.ViewZoomed, function (e, info) {
     alert("Zoom (" + info.newZoomFactor + ")");
});
```

___

### <a id="viewzooming" name="viewzooming"></a> ViewZooming

• `Static` **ViewZooming**: `string`

用户缩放时触发

**`name`** GC.Spread.Sheets.Worksheet#ViewZooming

**`param`** *[GC.Spread.Sheets.Worksheet](GC.Spread.Sheets.Worksheet.md)* `sheet` 触发事件的表单

**`param`** *string* `sheetName` 表单名称

**`param`** *number* `newZoomFactor` 新的缩放系数，用户可以进行一些更改以干预实际的缩放动作

**`param`** *number* `oldZoomFactor` 原始的缩放系数

**`param`** *boolean* `cancel` 是否应取消操作

**`代码示例`**
```
//本示例使用ViewZooming事件来限制最大缩放系数
spread.options.allowUserZoom = true;
activeSheet.bind(GC.Spread.Sheets.Events.ViewZooming, function (e, info) {
     if (info.newZoomFactor >= 2) {
         info.newZoomFactor = 2;
     }
});
```
