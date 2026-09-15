# Class: Worksheet

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).Worksheet

## Hierarchy

- **`Worksheet`**

  ↳ [`TemplateSheet`](GC.Spread.Report.TemplateSheet.md)

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Worksheet.md#constructor)

### Properties

- [autoGenerateColumns](GC.Spread.Sheets.Worksheet.md#autogeneratecolumns)
- [cellStates](GC.Spread.Sheets.Worksheet.md#cellstates)
- [charts](GC.Spread.Sheets.Worksheet.md#charts)
- [columnOutlines](GC.Spread.Sheets.Worksheet.md#columnoutlines)
- [comments](GC.Spread.Sheets.Worksheet.md#comments)
- [conditionalFormats](GC.Spread.Sheets.Worksheet.md#conditionalformats)
- [dataCharts](GC.Spread.Sheets.Worksheet.md#datacharts)
- [dataRanges](GC.Spread.Sheets.Worksheet.md#dataranges)
- [defaults](GC.Spread.Sheets.Worksheet.md#defaults)
- [floatingObjects](GC.Spread.Sheets.Worksheet.md#floatingobjects)
- [options](GC.Spread.Sheets.Worksheet.md#options)
- [outlineColumn](GC.Spread.Sheets.Worksheet.md#outlinecolumn)
- [pictures](GC.Spread.Sheets.Worksheet.md#pictures)
- [pivotTables](GC.Spread.Sheets.Worksheet.md#pivottables)
- [rowOutlines](GC.Spread.Sheets.Worksheet.md#rowoutlines)
- [shapes](GC.Spread.Sheets.Worksheet.md#shapes)
- [slicers](GC.Spread.Sheets.Worksheet.md#slicers)
- [tables](GC.Spread.Sheets.Worksheet.md#tables)

### Methods

- [addColumns](GC.Spread.Sheets.Worksheet.md#addcolumns)
- [addCustomFunction](GC.Spread.Sheets.Worksheet.md#addcustomfunction)
- [addCustomName](GC.Spread.Sheets.Worksheet.md#addcustomname)
- [addNamedStyle](GC.Spread.Sheets.Worksheet.md#addnamedstyle)
- [addRows](GC.Spread.Sheets.Worksheet.md#addrows)
- [addSelection](GC.Spread.Sheets.Worksheet.md#addselection)
- [addSpan](GC.Spread.Sheets.Worksheet.md#addspan)
- [addSpans](GC.Spread.Sheets.Worksheet.md#addspans)
- [autoFitColumn](GC.Spread.Sheets.Worksheet.md#autofitcolumn)
- [autoFitRow](GC.Spread.Sheets.Worksheet.md#autofitrow)
- [autoMerge](GC.Spread.Sheets.Worksheet.md#automerge)
- [backgroundImage](GC.Spread.Sheets.Worksheet.md#backgroundimage)
- [bind](GC.Spread.Sheets.Worksheet.md#bind)
- [bindColumn](GC.Spread.Sheets.Worksheet.md#bindcolumn)
- [bindColumns](GC.Spread.Sheets.Worksheet.md#bindcolumns)
- [clear](GC.Spread.Sheets.Worksheet.md#clear)
- [clearCustomFunctions](GC.Spread.Sheets.Worksheet.md#clearcustomfunctions)
- [clearCustomNames](GC.Spread.Sheets.Worksheet.md#clearcustomnames)
- [clearPendingChanges](GC.Spread.Sheets.Worksheet.md#clearpendingchanges)
- [clearSelection](GC.Spread.Sheets.Worksheet.md#clearselection)
- [copyTo](GC.Spread.Sheets.Worksheet.md#copyto)
- [currentTheme](GC.Spread.Sheets.Worksheet.md#currenttheme)
- [deleteColumns](GC.Spread.Sheets.Worksheet.md#deletecolumns)
- [deleteRows](GC.Spread.Sheets.Worksheet.md#deleterows)
- [editorStatus](GC.Spread.Sheets.Worksheet.md#editorstatus)
- [endEdit](GC.Spread.Sheets.Worksheet.md#endedit)
- [fillAuto](GC.Spread.Sheets.Worksheet.md#fillauto)
- [fromJSON](GC.Spread.Sheets.Worksheet.md#fromjson)
- [frozenColumnCount](GC.Spread.Sheets.Worksheet.md#frozencolumncount)
- [frozenRowCount](GC.Spread.Sheets.Worksheet.md#frozenrowcount)
- [frozenTrailingColumnCount](GC.Spread.Sheets.Worksheet.md#frozentrailingcolumncount)
- [frozenTrailingRowCount](GC.Spread.Sheets.Worksheet.md#frozentrailingrowcount)
- [getActiveColumnIndex](GC.Spread.Sheets.Worksheet.md#getactivecolumnindex)
- [getActiveRowIndex](GC.Spread.Sheets.Worksheet.md#getactiverowindex)
- [getActualStyle](GC.Spread.Sheets.Worksheet.md#getactualstyle)
- [getAltText](GC.Spread.Sheets.Worksheet.md#getalttext)
- [getArray](GC.Spread.Sheets.Worksheet.md#getarray)
- [getBindingPath](GC.Spread.Sheets.Worksheet.md#getbindingpath)
- [getCell](GC.Spread.Sheets.Worksheet.md#getcell)
- [getCellRect](GC.Spread.Sheets.Worksheet.md#getcellrect)
- [getCellType](GC.Spread.Sheets.Worksheet.md#getcelltype)
- [getColumnCount](GC.Spread.Sheets.Worksheet.md#getcolumncount)
- [getColumnPageBreak](GC.Spread.Sheets.Worksheet.md#getcolumnpagebreak)
- [getColumnResizable](GC.Spread.Sheets.Worksheet.md#getcolumnresizable)
- [getColumnVisible](GC.Spread.Sheets.Worksheet.md#getcolumnvisible)
- [getColumnWidth](GC.Spread.Sheets.Worksheet.md#getcolumnwidth)
- [getCsv](GC.Spread.Sheets.Worksheet.md#getcsv)
- [getCustomFunction](GC.Spread.Sheets.Worksheet.md#getcustomfunction)
- [getCustomName](GC.Spread.Sheets.Worksheet.md#getcustomname)
- [getCustomNames](GC.Spread.Sheets.Worksheet.md#getcustomnames)
- [getDataColumnName](GC.Spread.Sheets.Worksheet.md#getdatacolumnname)
- [getDataItem](GC.Spread.Sheets.Worksheet.md#getdataitem)
- [getDataSource](GC.Spread.Sheets.Worksheet.md#getdatasource)
- [getDataValidator](GC.Spread.Sheets.Worksheet.md#getdatavalidator)
- [getDefaultStyle](GC.Spread.Sheets.Worksheet.md#getdefaultstyle)
- [getDefaultValue](GC.Spread.Sheets.Worksheet.md#getdefaultvalue)
- [getDeletedRows](GC.Spread.Sheets.Worksheet.md#getdeletedrows)
- [getDependents](GC.Spread.Sheets.Worksheet.md#getdependents)
- [getDirtyCells](GC.Spread.Sheets.Worksheet.md#getdirtycells)
- [getDirtyRows](GC.Spread.Sheets.Worksheet.md#getdirtyrows)
- [getFormatter](GC.Spread.Sheets.Worksheet.md#getformatter)
- [getFormula](GC.Spread.Sheets.Worksheet.md#getformula)
- [getFormulaInformation](GC.Spread.Sheets.Worksheet.md#getformulainformation)
- [getHyperlink](GC.Spread.Sheets.Worksheet.md#gethyperlink)
- [getId](GC.Spread.Sheets.Worksheet.md#getid)
- [getInsertRows](GC.Spread.Sheets.Worksheet.md#getinsertrows)
- [getNamedStyle](GC.Spread.Sheets.Worksheet.md#getnamedstyle)
- [getNamedStyles](GC.Spread.Sheets.Worksheet.md#getnamedstyles)
- [getParent](GC.Spread.Sheets.Worksheet.md#getparent)
- [getPrecedents](GC.Spread.Sheets.Worksheet.md#getprecedents)
- [getRange](GC.Spread.Sheets.Worksheet.md#getrange)
- [getRowCount](GC.Spread.Sheets.Worksheet.md#getrowcount)
- [getRowHeight](GC.Spread.Sheets.Worksheet.md#getrowheight)
- [getRowPageBreak](GC.Spread.Sheets.Worksheet.md#getrowpagebreak)
- [getRowResizable](GC.Spread.Sheets.Worksheet.md#getrowresizable)
- [getRowVisible](GC.Spread.Sheets.Worksheet.md#getrowvisible)
- [getSelections](GC.Spread.Sheets.Worksheet.md#getselections)
- [getSortState](GC.Spread.Sheets.Worksheet.md#getsortstate)
- [getSpans](GC.Spread.Sheets.Worksheet.md#getspans)
- [getSparkline](GC.Spread.Sheets.Worksheet.md#getsparkline)
- [getStyle](GC.Spread.Sheets.Worksheet.md#getstyle)
- [getStyleName](GC.Spread.Sheets.Worksheet.md#getstylename)
- [getTag](GC.Spread.Sheets.Worksheet.md#gettag)
- [getText](GC.Spread.Sheets.Worksheet.md#gettext)
- [getUsedRange](GC.Spread.Sheets.Worksheet.md#getusedrange)
- [getValue](GC.Spread.Sheets.Worksheet.md#getvalue)
- [getViewportBottomRow](GC.Spread.Sheets.Worksheet.md#getviewportbottomrow)
- [getViewportHeight](GC.Spread.Sheets.Worksheet.md#getviewportheight)
- [getViewportLeftColumn](GC.Spread.Sheets.Worksheet.md#getviewportleftcolumn)
- [getViewportRightColumn](GC.Spread.Sheets.Worksheet.md#getviewportrightcolumn)
- [getViewportTopRow](GC.Spread.Sheets.Worksheet.md#getviewporttoprow)
- [getViewportWidth](GC.Spread.Sheets.Worksheet.md#getviewportwidth)
- [groupSparkline](GC.Spread.Sheets.Worksheet.md#groupsparkline)
- [hasPassword](GC.Spread.Sheets.Worksheet.md#haspassword)
- [hasPendingChanges](GC.Spread.Sheets.Worksheet.md#haspendingchanges)
- [hitTest](GC.Spread.Sheets.Worksheet.md#hittest)
- [invalidateLayout](GC.Spread.Sheets.Worksheet.md#invalidatelayout)
- [isDirtySuspended](GC.Spread.Sheets.Worksheet.md#isdirtysuspended)
- [isEditing](GC.Spread.Sheets.Worksheet.md#isediting)
- [isPaintSuspended](GC.Spread.Sheets.Worksheet.md#ispaintsuspended)
- [isPrintLineVisible](GC.Spread.Sheets.Worksheet.md#isprintlinevisible)
- [isSelected](GC.Spread.Sheets.Worksheet.md#isselected)
- [isValid](GC.Spread.Sheets.Worksheet.md#isvalid)
- [moveTo](GC.Spread.Sheets.Worksheet.md#moveto)
- [name](GC.Spread.Sheets.Worksheet.md#name)
- [printInfo](GC.Spread.Sheets.Worksheet.md#printinfo)
- [protect](GC.Spread.Sheets.Worksheet.md#protect)
- [recalcAll](GC.Spread.Sheets.Worksheet.md#recalcall)
- [removeCustomFunction](GC.Spread.Sheets.Worksheet.md#removecustomfunction)
- [removeCustomName](GC.Spread.Sheets.Worksheet.md#removecustomname)
- [removeNamedStyle](GC.Spread.Sheets.Worksheet.md#removenamedstyle)
- [removeSpan](GC.Spread.Sheets.Worksheet.md#removespan)
- [removeSparkline](GC.Spread.Sheets.Worksheet.md#removesparkline)
- [repaint](GC.Spread.Sheets.Worksheet.md#repaint)
- [reset](GC.Spread.Sheets.Worksheet.md#reset)
- [resumeCalcService](GC.Spread.Sheets.Worksheet.md#resumecalcservice)
- [resumeDirty](GC.Spread.Sheets.Worksheet.md#resumedirty)
- [resumeEvent](GC.Spread.Sheets.Worksheet.md#resumeevent)
- [resumePaint](GC.Spread.Sheets.Worksheet.md#resumepaint)
- [rowFilter](GC.Spread.Sheets.Worksheet.md#rowfilter)
- [scroll](GC.Spread.Sheets.Worksheet.md#scroll)
- [search](GC.Spread.Sheets.Worksheet.md#search)
- [selectionPolicy](GC.Spread.Sheets.Worksheet.md#selectionpolicy)
- [selectionUnit](GC.Spread.Sheets.Worksheet.md#selectionunit)
- [setActiveCell](GC.Spread.Sheets.Worksheet.md#setactivecell)
- [setAltText](GC.Spread.Sheets.Worksheet.md#setalttext)
- [setArray](GC.Spread.Sheets.Worksheet.md#setarray)
- [setArrayFormula](GC.Spread.Sheets.Worksheet.md#setarrayformula)
- [setBindingPath](GC.Spread.Sheets.Worksheet.md#setbindingpath)
- [setCellType](GC.Spread.Sheets.Worksheet.md#setcelltype)
- [setColumnCount](GC.Spread.Sheets.Worksheet.md#setcolumncount)
- [setColumnPageBreak](GC.Spread.Sheets.Worksheet.md#setcolumnpagebreak)
- [setColumnResizable](GC.Spread.Sheets.Worksheet.md#setcolumnresizable)
- [setColumnVisible](GC.Spread.Sheets.Worksheet.md#setcolumnvisible)
- [setColumnWidth](GC.Spread.Sheets.Worksheet.md#setcolumnwidth)
- [setCsv](GC.Spread.Sheets.Worksheet.md#setcsv)
- [setDataSource](GC.Spread.Sheets.Worksheet.md#setdatasource)
- [setDataValidator](GC.Spread.Sheets.Worksheet.md#setdatavalidator)
- [setDefaultStyle](GC.Spread.Sheets.Worksheet.md#setdefaultstyle)
- [setDefaultValue](GC.Spread.Sheets.Worksheet.md#setdefaultvalue)
- [setFormatter](GC.Spread.Sheets.Worksheet.md#setformatter)
- [setFormula](GC.Spread.Sheets.Worksheet.md#setformula)
- [setHyperlink](GC.Spread.Sheets.Worksheet.md#sethyperlink)
- [setRowCount](GC.Spread.Sheets.Worksheet.md#setrowcount)
- [setRowHeight](GC.Spread.Sheets.Worksheet.md#setrowheight)
- [setRowPageBreak](GC.Spread.Sheets.Worksheet.md#setrowpagebreak)
- [setRowResizable](GC.Spread.Sheets.Worksheet.md#setrowresizable)
- [setRowVisible](GC.Spread.Sheets.Worksheet.md#setrowvisible)
- [setSelection](GC.Spread.Sheets.Worksheet.md#setselection)
- [setSparkline](GC.Spread.Sheets.Worksheet.md#setsparkline)
- [setStyle](GC.Spread.Sheets.Worksheet.md#setstyle)
- [setStyleName](GC.Spread.Sheets.Worksheet.md#setstylename)
- [setTag](GC.Spread.Sheets.Worksheet.md#settag)
- [setText](GC.Spread.Sheets.Worksheet.md#settext)
- [setValue](GC.Spread.Sheets.Worksheet.md#setvalue)
- [showCell](GC.Spread.Sheets.Worksheet.md#showcell)
- [showColumn](GC.Spread.Sheets.Worksheet.md#showcolumn)
- [showColumnOutline](GC.Spread.Sheets.Worksheet.md#showcolumnoutline)
- [showRow](GC.Spread.Sheets.Worksheet.md#showrow)
- [showRowOutline](GC.Spread.Sheets.Worksheet.md#showrowoutline)
- [sortRange](GC.Spread.Sheets.Worksheet.md#sortrange)
- [startEdit](GC.Spread.Sheets.Worksheet.md#startedit)
- [suspendCalcService](GC.Spread.Sheets.Worksheet.md#suspendcalcservice)
- [suspendDirty](GC.Spread.Sheets.Worksheet.md#suspenddirty)
- [suspendEvent](GC.Spread.Sheets.Worksheet.md#suspendevent)
- [suspendPaint](GC.Spread.Sheets.Worksheet.md#suspendpaint)
- [tag](GC.Spread.Sheets.Worksheet.md#tag)
- [toJSON](GC.Spread.Sheets.Worksheet.md#tojson)
- [unbind](GC.Spread.Sheets.Worksheet.md#unbind)
- [unbindAll](GC.Spread.Sheets.Worksheet.md#unbindall)
- [ungroupSparkline](GC.Spread.Sheets.Worksheet.md#ungroupsparkline)
- [unprotect](GC.Spread.Sheets.Worksheet.md#unprotect)
- [visible](GC.Spread.Sheets.Worksheet.md#visible)
- [zoom](GC.Spread.Sheets.Worksheet.md#zoom)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Worksheet**(`name`)

表示一个工作表。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 工作表的名称。 |

## Properties

### <a id="autogeneratecolumns" name="autogeneratecolumns"></a> autoGenerateColumns

• **autoGenerateColumns**: `boolean`

指示在绑定数据上下文时是否自动生成列。

**`example`**
```
//此示例为工作表设置数据源。
 var test = [
       { "Series0": 2, "Series1": 1 },
       { "Series0": 4, "Series1": 2 },
       { "Series0": 3, "Series1": 4 }
            ];
activeSheet.autoGenerateColumns = true;
activeSheet.setDataSource(test, true);
```

___

### <a id="cellstates" name="cellstates"></a> cellStates

• **cellStates**: [`CellStateManager`](GC.Spread.Sheets.CellState.CellStateManager.md)

单元格状态管理器。

___

### <a id="charts" name="charts"></a> charts

• **charts**: [`ChartCollection`](GC.Spread.Sheets.Charts.ChartCollection.md)

工作表的图表管理器。

**`example`**
```
//此示例展示如何添加图表。
var dataRange = "A1:D4";
var chart = activeSheet.charts.add('Chart1', GC.Spread.Sheets.Charts.ChartType.columnClustered, 250, 20, 600, 400, dataRange);
```

___

### <a id="columnoutlines" name="columnoutlines"></a> columnOutlines

• **columnOutlines**: [`Outline`](GC.Spread.Sheets.Outlines.Outline.md)

指示列范围组。

___

### <a id="comments" name="comments"></a> comments

• **comments**: [`CommentManager`](GC.Spread.Sheets.Comments.CommentManager.md)

工作表的注释管理器。

___

### <a id="conditionalformats" name="conditionalformats"></a> conditionalFormats

• **conditionalFormats**: [`ConditionalFormats`](GC.Spread.Sheets.ConditionalFormatting.ConditionalFormats.md)

工作表的条件格式管理器。

**`example`**
```
//此示例创建一个规则。
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
var rule = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
rule.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.cellValueRule);
rule.ranges([new GC.Spread.Sheets.Range(0,0,5,1)]);
rule.operator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.between);
rule.style(style);
rule.value1(2);
rule.value2(100);
activeSheet.conditionalFormats.addRule(rule);
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,45,3);
var ruletest = activeSheet.conditionalFormats.getRules();
alert(ruletest[0].style().backColor);
```

___

### <a id="datacharts" name="datacharts"></a> dataCharts

• **dataCharts**: [`DataChartManager`](GC.Spread.Sheets.DataCharts.DataChartManager.md)

数据图表管理器。

**`example`**
```
//此示例创建一个数据图表。
var datacharts = sheet.dataCharts;
var datachart = datacharts.add('datachart1', 250, 20, 600, 400, GC.Spread.Sheets.DataCharts.DataChartType.column);
```

___

### <a id="dataranges" name="dataranges"></a> dataRanges

• **dataRanges**: [`DataRangeManager`](GC.Spread.Sheets.DataRange.DataRangeManager.md)

工作表的数据范围管理器。

___

### <a id="defaults" name="defaults"></a> defaults

• **defaults**: [`ISheetDefaultOption`](../interfaces/GC.Spread.Sheets.ISheetDefaultOption.md)

指示工作表的默认行高和列宽。

**`example`**
```
//此示例设置默认行高和列宽。
activeSheet.suspendPaint();
activeSheet.defaults.rowHeight = 40;
activeSheet.defaults.colWidth = 30;
activeSheet.resumePaint();
```

___

### <a id="floatingobjects" name="floatingobjects"></a> floatingObjects

• **floatingObjects**: [`FloatingObjectCollection`](GC.Spread.Sheets.FloatingObjects.FloatingObjectCollection.md)

工作表的浮动对象管理器。

**`example`**
```
//此示例创建一个浮动对象。
var customFloatingObject = new GC.Spread.Sheets.FloatingObjects.FloatingObject("f1", 10, 10, 60, 64);
var btn = document.createElement('button');
btn.style.width = "60px";
btn.style.height = "30px";
btn.innerText = "button";
customFloatingObject.content(btn);
activeSheet.floatingObjects.add(customFloatingObject);
```

___

### <a id="options" name="options"></a> options

• **options**: [`IWorksheetOptions`](../interfaces/GC.Spread.Sheets.IWorksheetOptions.md)

表示工作表的选项。

**`property`** {boolean} allowCellOverflow - 指示数据是否可以溢出到相邻的空单元格中。

**`property`** {boolean} showFormulas - 指示是否显示公式字符串而不是公式结果。

**`property`** {boolean} showZeros - 指示是否在包含零值的单元格中显示0。默认为true。

**`property`** {string} sheetTabColor - 用于表示工作表标签颜色的颜色字符串，如"red"、"#FFFF00"、"rgb(255,0,0)"、"Accent 5"等。

**`property`** {string} frozenlineColor - 用于表示冻结线颜色的颜色字符串，如"red"、"#FFFF00"、"rgb(255,0,0)"、"Accent 5"等。

**`property`** {GC.Spread.Sheets.ClipboardPasteOptions} clipBoardOptions - 剪贴板选项。

**`property`** {Object} gridline - 网格线的选项。

**`property`** {string} gridline.color - 网格线颜色。

**`property`** {boolean} gridline.showVerticalGridline - 是否显示垂直网格线。

**`property`** {boolean} gridline.showHorizontalGridline - 是否显示水平网格线。

**`property`** {boolean} rowHeaderVisible - 指示行标题是否可见。

**`property`** {boolean} colHeaderVisible - 指示列标题是否可见。

**`property`** {GC.Spread.Sheets.HeaderAutoText} rowHeaderAutoText - 指示行标题是否显示字母、数字或空白。

**`property`** {GC.Spread.Sheets.HeaderAutoText} colHeaderAutoText - 指示列标题是否显示字母、数字或空白。

**`property`** {number} rowHeaderAutoTextIndex - 当有多个行标题列时，指定哪个行标题列显示自动文本。

**`property`** {number} colHeaderAutoTextIndex - 当有多个列标题行时，指定哪个列标题行显示自动文本。

**`property`** {boolean} isProtected - 指示此工作表中标记为受保护的单元格是否不可编辑。

**`property`** {Object} protectionOptions - 指示您希望用户能够更改的元素的值。

**`property`** {boolean} [protectionOptions.allowSelectLockedCells] - 如果用户可以选择锁定的单元格，则为true或undefined。

**`property`** {boolean} [protectionOptions.allowSelectUnlockedCells] - 如果用户可以选择未锁定的单元格，则为true或undefined。

**`property`** {boolean} [protectionOptions.allowSort] - 如果用户可以排序范围，则为true。

**`property`** {boolean} [protectionOptions.allowFilter] - 如果用户可以筛选范围，则为true。

**`property`** {boolean} [protectionOptions.allowEditObjects] - 如果用户可以编辑浮动对象，则为true。

**`property`** {boolean} [protectionOptions.allowResizeRows] - 如果用户可以调整行大小，则为true。

**`property`** {boolean} [protectionOptions.allowResizeColumns] - 如果用户可以调整列大小，则为true。

**`property`** {boolean} [protectionOptions.allowDragInsertRows] - 如果用户可以拖动插入行，则为true。

**`property`** {boolean} [protectionOptions.allowDragInsertColumns] - 如果用户可以拖动插入列，则为true。

**`property`** {boolean} [protectionOptions.allowInsertRows] - 如果用户可以插入行，则为true。

**`property`** {boolean} [protectionOptions.allowInsertColumns] - 如果用户可以插入列，则为true。

**`property`** {boolean} [protectionOptions.allowDeleteRows] - 如果用户可以删除行，则为true。

**`property`** {boolean} [protectionOptions.allowDeleteColumns] - 如果用户可以删除列，则为true。

**`property`** {boolean} [protectionOptions.allowOutlineColumns] - 如果用户可以展开或折叠列组，则为true。

**`property`** {boolean} [protectionOptions.allowOutlineRows] - 如果用户可以展开或折叠行组，则为true。

**`property`** {string} selectionBackColor - 工作表的选择背景颜色。

**`property`** {string} selectionBorderColor - 工作表的选择边框颜色。

**`property`** {Object} sheetAreaOffset - sheetAreaOffset的选项。

**`property`** {number} [sheetAreaOffset.left] - 工作表相对于宿主的左侧偏移量。

**`property`** {number} [sheetAreaOffset.top] - 工作表相对于宿主的顶部偏移量。

**`property`** {boolean} keepUnknownFormulas - 指示未知公式是否可以包含在工作表json数据中。

**`property`** {GC.Spread.Sheets.IAddRowButtonOption} [addRowButtonOption] - 添加行按钮的选项。

**`property`** {GC.Spread.Sheets.IAddColumnButtonOption} [addColumnButtonOption] - 添加列按钮的选项。

**`property`** {boolean} rightToLeft - 指示工作表是否从右到左渲染。

**`property`** {string} backgroundImage - 指示背景图像的URL。

**`example`**
```
sheet.setRowCount(2,GC.Spread.Sheets.SheetArea.colHeader);
sheet.setColumnCount(2,GC.Spread.Sheets.SheetArea.rowHeader);
sheet.setValue(0, 2,"Column",GC.Spread.Sheets.SheetArea.colHeader);
sheet.options.colHeaderAutoTextIndex = 1;
sheet.options.colHeaderAutoText = GC.Spread.Sheets.HeaderAutoText.numbers;
```

___

### <a id="outlinecolumn" name="outlinecolumn"></a> outlineColumn

• **outlineColumn**: [`OutlineColumn`](GC.Spread.Sheets.OutlineColumn.OutlineColumn.md)

获取工作表的列大纲。

**`returns`**

___

### <a id="pictures" name="pictures"></a> pictures

• **pictures**: [`FloatingObjectCollection`](GC.Spread.Sheets.FloatingObjects.FloatingObjectCollection.md)

工作表的图片管理器。

**`deprecated`** 自版本15.2.0起，请使用'sheet.shapes'代替

**`example`**
```
//此示例添加一个图片。
activeSheet.pictures.add("f2","Event.png",2,2,10,10);
var picture = activeSheet.pictures.get("f2");
picture.pictureStretch(GC.Spread.Sheets.ImageLayout.center);
picture.backColor("Blue");
picture.borderWidth(2);
picture.borderColor("Red");
picture.borderStyle("dotted");
picture.borderRadius(5);
```

___

### <a id="pivottables" name="pivottables"></a> pivotTables

• **pivotTables**: [`PivotTableManager`](GC.Spread.Sheets.PivotTableManager.md)

数据透视表管理器。

**`example`**
```
//此示例创建一个数据透视表。
var pivotTableManager = sheet.pivotTables;
var sourceData = [["Date","Buyer","Type","Amount"],["01-Jan","Mom","Fuel",74],["15-Jan","Mom","Food",235],["17-Jan","Dad","Sports",20],["21-Jan","Kelly","Books",125],["02-Feb","Mom","Food",235],["20-Feb","Kelly","Music",20],["25-Feb","Kelly","Tickets",125]];
var options = {showRowHeader: true, showColumnHeader: true};
var myPivotTable = pivotTableManager.add("pivotTable_1", sourceData , 1, 1, GC.Spread.Pivot.PivotTableLayoutType.tabular, GC.Spread.Pivot.PivotTableThemes.medium2, option);
```

___

### <a id="rowoutlines" name="rowoutlines"></a> rowOutlines

• **rowOutlines**: [`Outline`](GC.Spread.Sheets.Outlines.Outline.md)

表示行范围组。

___

### <a id="shapes" name="shapes"></a> shapes

• **shapes**: [`ShapeCollection`](GC.Spread.Sheets.Shapes.ShapeCollection.md)

工作表的形状管理器。

**`example`**
```
//此示例展示如何添加一个形状。
var shape = activeSheet.shapes.add("shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 50, 100, 150);
```

___

### <a id="slicers" name="slicers"></a> slicers

• **slicers**: [`SlicerCollection`](GC.Spread.Sheets.Slicers.SlicerCollection.md)

切片器管理器。

**`example`**
```
//此示例添加一个切片器。
//创建一个表格
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
var style1 = new GC.Spread.Sheets.Slicers.SlicerStyles.light4();
//向工作表添加切片器并返回切片器实例。
var slicer = activeSheet.slicers.add("slicer1",table.name(),"Height");
 //更改切片器属性。
slicer.position(new GC.Spread.Sheets.Point(100, 200));
slicer.disableResizingAndMoving(true);
slicer.style(style1);
```

___

### <a id="tables" name="tables"></a> tables

• **tables**: [`TableManager`](GC.Spread.Sheets.Tables.TableManager.md)

表格管理器。

**`example`**
```
//此示例创建一个表格。
activeSheet.tables.add("Table1", 0, 0, 3, 3, GC.Spread.Sheets.Tables.TableThemes.dark1);
activeSheet.getCell(0,0).text("Name");
activeSheet.getCell(0,1).text("Value");
activeSheet.getCell(0,2).text("T/F");
activeSheet.getCell(1,0).text("AW");
activeSheet.getCell(1,1).text("5");
activeSheet.getCell(1,2).text("T");
```

## Methods

### <a id="addcolumns" name="addcolumns"></a> addColumns

▸ **addColumns**(`col`, `count`, `sheetArea?`): `void`

在指定索引处向数据模型添加一列或多列。

**`example`**
```
//此示例添加列。
sheet.setValue(0, 0, "value");
sheet.addRows(0, 2);
sheet.addColumns(0, 2);
sheet.setRowHeight(0, 50.0,GC.Spread.Sheets.SheetArea.viewport);
sheet.setColumnWidth(0, 150.0,GC.Spread.Sheets.SheetArea.viewport);
sheet.getRange(0, -1, 1, -1,GC.Spread.Sheets.SheetArea.viewport).backColor("Gray");
sheet.getRange(-1, 0, -1, 1,GC.Spread.Sheets.SheetArea.viewport).backColor ("Brown");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `col` | `number` | 要添加新列的列索引。 |
| `count` | `number` | 要添加的列数。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`void`

___

### <a id="addcustomfunction" name="addcustomfunction"></a> addCustomFunction

▸ **addCustomFunction**(`fn`): `void`

添加自定义函数。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fn` | [`Function`](GC.Spread.CalcEngine.Functions.Function.md) | 要添加的函数。 |

#### Returns

`void`

___

### <a id="addcustomname" name="addcustomname"></a> addCustomName

▸ **addCustomName**(`name`, `formula`, `baseRow`, `baseCol`, `comment?`, `isReadOnly?`): `void`

添加自定义名称。

**`example`**
```
//此示例创建自定义名称。
sheet.setValue(0, 0, 1);
sheet.setValue(0, 1, 2);
sheet.setValue(0, 2, 3);
sheet.addCustomName("customName1","=12", 0, 0);
sheet.addCustomName("customName2","Average(20,45)", 0, 0);
sheet.addCustomName("customName3", "=$A$1:$C$1", 0, 0);
sheet.setFormula(1, 0, "customName1");
sheet.setFormula(1, 1, "customName2");
sheet.setFormula(1, 2, "sum(customName3)");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 自定义名称。 |
| `formula` | `string` | 公式。 |
| `baseRow` | `number` | 行索引。 |
| `baseCol` | `number` | 列索引。 |
| `comment?` | `string` | - |
| `isReadOnly?` | `boolean` | - |

#### Returns

`void`

___

### <a id="addnamedstyle" name="addnamedstyle"></a> addNamedStyle

▸ **addNamedStyle**(`style`): `void`

向工作表的命名样式集合添加样式。

**`example`**
```
var namedStyle = new GC.Spread.Sheets.Style();
namedStyle.name = "style1";
namedStyle.backColor = "green";
activeSheet.addNamedStyle(namedStyle);
activeSheet.setStyleName(1, 1, "style1"); // 单元格(1,1)的背景色为绿色。
activeSheet.setStyleName(2, 1, "style1");
var style = activeSheet.getNamedStyle("style1");
style.foreColor = "red";    // 命名样式的前景色为红色。
activeSheet.repaint(); // 单元格(1,1)和单元格(2,1)的前景色为红色。
activeSheet.getCell(1,1).value("test");
$("#button1").click(function () {
activeSheet.removeNamedStyle("style1");
    });
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 要添加的样式。 |

#### Returns

`void`

___

### <a id="addrows" name="addrows"></a> addRows

▸ **addRows**(`row`, `count`, `sheetArea?`): `void`

在工作表中添加行。

**`example`**
```
//此示例添加行。
sheet.setValue(0, 0, "value");
sheet.addRows(0, 2);
sheet.addColumns(0, 2);
sheet.setRowHeight(0, 50.0,GC.Spread.Sheets.SheetArea.viewport);
sheet.setColumnWidth(0, 150.0,GC.Spread.Sheets.SheetArea.viewport);
sheet.getRange(0, -1, 1, -1,GC.Spread.Sheets.SheetArea.viewport).backColor("Gray");
sheet.getRange(-1, 0, -1, 1,GC.Spread.Sheets.SheetArea.viewport).backColor ("Brown");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 起始行的索引。 |
| `count` | `number` | 要添加的行数。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`void`

___

### <a id="addselection" name="addselection"></a> addSelection

▸ **addSelection**(`row`, `column`, `rowCount`, `columnCount`): `void`

向选择中添加一个或多个单元格。

**`example`**
```
//此示例添加一个选择并在规则中使用该选择。
sheet.setValue(0,0, 1,3);
sheet.setValue(1,0, 50,3);
sheet.setValue(2,0, 100,3);
sheet.setValue(3,0, 2,3);
sheet.setValue(4,0, 60,3);
sheet.setValue(5,0, 90,3);
sheet.setValue(6,0, 3,3);
sheet.setValue(7,0, 40,3);
sheet.setValue(8,0, 70,3);
sheet.setValue(9,0, 5,3);
sheet.setValue(10,0, 35,3);
sheet.addSelection(0,0,11,1);
sheet.conditionalFormats.add3ScaleRule(1, 10, "red", 0, 50, "blue",2, 100, "yellow", sheet.getSelections());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 要添加的第一个单元格的行索引。 |
| `column` | `number` | 要添加的第一个单元格的列索引。 |
| `rowCount` | `number` | 要添加的行数。 |
| `columnCount` | `number` | 要添加的列数。 |

#### Returns

`void`

___

### <a id="addspan" name="addspan"></a> addSpan

▸ **addSpan**(`row`, `col`, `rowCount`, `colCount`, `sheetArea?`): `void`

在指定的工作表区域中添加单元格合并。

**`example`**
```
//此示例创建单元格合并。
sheet.setRowCount(4,1);
sheet.setColumnCount(4,2);
sheet.addSpan(0,0,3,3,GC.Spread.Sheets.SheetArea.colHeader);
sheet.addSpan(0,0,3,3,GC.Spread.Sheets.SheetArea.rowHeader);
sheet.addSpan(0,0,3,3,GC.Spread.Sheets.SheetArea.viewport);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 开始合并的单元格的行索引。 |
| `col` | `number` | - |
| `rowCount` | `number` | 要合并的行数。 |
| `colCount` | `number` | 要合并的列数。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`void`

___

### <a id="addspans" name="addspans"></a> addSpans

▸ **addSpans**(`spans`, `sheetArea?`): `void`

在指定的工作表区域中添加多个单元格合并。

**`example`**
```
//此示例创建多个单元格合并。
sheet.addSpans([{row: 0, col: 0, rowCount: 2, colCount: 2}, {row: 3, col: 0, rowCount: 3, colCount: 3}, {row: 7, col: 0, rowCount: 4, colCount: 4}], GC.Spread.Sheets.SheetArea.viewport);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `spans` | [`IRange`](../interfaces/GC.Spread.Sheets.IRange.md)[] | 合并范围数组，每个范围包含 row、col、rowCount、colCount。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`void`

___

### <a id="autofitcolumn" name="autofitcolumn"></a> autoFitColumn

▸ **autoFitColumn**(`column`): `void`

自动调整视口列宽。

**`example`**
```
//此示例根据文本设置列宽。
activeSheet.setValue(0, 1, "testing");
activeSheet.autoFitColumn(1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `column` | `number` | 列索引。 |

#### Returns

`void`

___

### <a id="autofitrow" name="autofitrow"></a> autoFitRow

▸ **autoFitRow**(`row`): `void`

自动调整视口行高。

**`example`**
```
//此示例根据文本设置行高。
activeSheet.setValue(0, 1, "testing\r\nmultiple\r\nlines");
activeSheet.getCell(0,1).wordWrap(true);
activeSheet.autoFitRow(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |

#### Returns

`void`

___

### <a id="automerge" name="automerge"></a> autoMerge

▸ **autoMerge**(`range`, `direction?`, `mode?`, `sheetArea?`, `selectionMode?`): [`IRangeInfo`](../interfaces/GC.Spread.Sheets.AutoMerge.IRangeInfo.md)[]

为范围应用自动合并。

**`example`**
```
var range = new GC.Spread.Sheets.Range(-1, 0, -1, 1);
sheet.autoMerge(range);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](GC.Spread.Sheets.Range.md) | 自动合并的范围。 |
| `direction?` | [`AutoMergeDirection`](../enums/GC.Spread.Sheets.AutoMerge.AutoMergeDirection.md) | 自动合并的方向。如果未提供此参数，则默认为 `column`。特别地，如果方向为 `none`，将取消该范围的自动合并。 |
| `mode?` | [`AutoMergeMode`](../enums/GC.Spread.Sheets.AutoMerge.AutoMergeMode.md) | 自动合并的模式。如果未提供此参数，则默认为 `free`。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | 自动合并范围的工作表区域。如果未提供此参数，则默认为 `viewport`。 |
| `selectionMode?` | [`SelectionMode`](../enums/GC.Spread.Sheets.AutoMerge.SelectionMode.md) | 自动合并的选择模式。如果未提供此参数，则默认为 `source`。 |

#### Returns

[`IRangeInfo`](../interfaces/GC.Spread.Sheets.AutoMerge.IRangeInfo.md)[]

如果未提供参数，则返回当前工作表的所有自动合并范围信息。每个范围信息包含范围、方向、模式、工作表区域和选择模式。

___

### <a id="backgroundimage" name="backgroundimage"></a> backgroundImage

▸ **backgroundImage**(`src?`): ``null`` \| `string`

获取或设置工作表的背景图像，如果没有参数，则表示返回工作表的背景图像。

**`example`**
```
activeSheet.backgroundImage('./image/background.jpg');
let imageUrl = activeSheet.backgroundImage();
alert(imageUrl);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `src?` | `string` | 背景图像的URL。 |

#### Returns

``null`` \| `string`

返回工作表背景图像的URL。

___

### <a id="bind" name="bind"></a> bind

▸ **bind**(`type`, `data?`, `fn?`): `void`

将事件绑定到工作表。

**`example`**
```
//此示例绑定事件。
sheet.bind(GC.Spread.Sheets.Events.LeftColumnChanged,function(event,data)
  {
    var str = "----------------------------------------\n";
    var title = "Event [LeftColumnChanged ] Fired";
    str = str.substr(0, 4) + title + str.substr(4 + title.length);
    if (typeof data == "object") {
        for (var key in data) {
            str += key + " : " + data[key] + "\n";
          }
      } else {
        str += data + "\n";
      }
      alert(str);
  });
sheet.bind(GC.Spread.Sheets.Events.TopRowChanged,function(event,data)
  {
        var str = "----------------------------------------\n";
        var title = "Event [TopRowChanged] Fired";
        str = str.substr(0, 4) + title + str.substr(4 + title.length);
        if (typeof data == "object") {
            for (var key in data) {
                str += key + " : " + data[key] + "\n";
            }
        } else {
            str += data + "\n";
        }
        alert(str);
    });
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `string` | 事件类型。 |
| `data?` | `any` | 可选。指定要传递给函数的附加数据。 |
| `fn?` | `Function` | 指定事件发生时运行的函数。 |

#### Returns

`void`

___

### <a id="bindcolumn" name="bindcolumn"></a> bindColumn

▸ **bindColumn**(`index`, `column`): `void`

使用指定的数据字段绑定列。

**`example`**
```
var test = [
{"Series0":2,"Series1":1},
{"Series0":4,"Series1":2},
{"Series0":3,"Series1":4}
];
sheet.setDataSource(test);
sheet.bindColumn(1,"Series0");
sheet.bindColumn(0,"Series1");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 列索引。 |
| `column` | `string` \| [`IColumn`](../interfaces/GC.Spread.Sheets.IColumn.md) | 包含数据字段的列信息。如果其类型为字符串，则被视为名称。 |

#### Returns

`void`

___

### <a id="bindcolumns" name="bindcolumns"></a> bindColumns

▸ **bindColumns**(`columns`): `void`

使用指定的数据字段绑定列。

**`example`**
```
var datasource = [
                 { name: "Alice", age: 27, birthday: "1985/08/31", position: "Beijing", isMarried: false},
                 { name: "Aimee", age: 28, birthday: "1984/07/31", position: "Xi'An", isMarried: true},
                 { name: "Charles", age: 29, birthday: "1983/03/31", position: "ShangHai", isMarried: true},
            ];
var colInfos = [
                { name: "name", displayName: "Name", size: 70, pageBread: false},
                { name: "age", displayName: "Age", size: 40, resizable: false },
                { name: "birthday", displayName: "Birthday", formatter: "d/M/yy", size: 120 },
                { name: "position", displayName: "Position", size: 50, visible: true, value: function (item){
			             return 'China ' + item['position'];
		           }},
                { name: "isMarried", displayName: "IsMarried", size: 50, visible: true, cellType: new GC.Spread.Sheets.CellTypes.CheckBox()}
            ];
activeSheet.autoGenerateColumns = true;
activeSheet.setDataSource(datasource);
activeSheet.bindColumns(colInfos);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columns` | [`IColumn`](../interfaces/GC.Spread.Sheets.IColumn.md)[] | 包含数据字段的列信息数组。如果项目的类型为字符串，则该项目被视为名称。 |

#### Returns

`void`

___

### <a id="clear" name="clear"></a> clear

▸ **clear**(`row`, `column`, `rowCount`, `colCount`, `area`, `storageType`): `void`

清除指定区域。

**`example`**
```
//此示例清除指定范围的数据。
activeSheet.getCell(0,0).value("A1");
activeSheet.clear(0,0,3,3,GC.Spread.Sheets.SheetArea.viewport,GC.Spread.Sheets.StorageType.data);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 起始行索引。 |
| `column` | `number` | 起始列索引。 |
| `rowCount` | `number` | 要清除的行数。 |
| `colCount` | `number` | - |
| `area` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | 要清除的区域。 |
| `storageType` | [`StorageType`](../enums/GC.Spread.Sheets.StorageType.md) | 清除类型。 |

#### Returns

`void`

___

### <a id="clearcustomfunctions" name="clearcustomfunctions"></a> clearCustomFunctions

▸ **clearCustomFunctions**(): `void`

清除所有自定义函数。

**`example`**
```
//此示例清除活动工作表中的自定义函数。
activeSheet.clearCustomFunctions();
```

#### Returns

`void`

___

### <a id="clearcustomnames" name="clearcustomnames"></a> clearCustomNames

▸ **clearCustomNames**(): `void`

清除自定义名称。

**`example`**
```
//此示例创建自定义名称然后清除它们。
activeSheet.setValue(0, 0, 1);
activeSheet.setValue(0, 1, 2);
activeSheet.setValue(0, 2, 3);
activeSheet.addCustomName("customName1","=12", 0, 0);
activeSheet.addCustomName("customName2","Average(20,45)", 0, 0);
activeSheet.addCustomName("customName3", "=$A$1:$C$1", 0, 0);
activeSheet.setFormula(1, 0, "customName1");
activeSheet.setFormula(1, 1, "customName2");
activeSheet.setFormula(1, 2, "sum(customName3)");
activeSheet.clearCustomNames();
```

#### Returns

`void`

___

### <a id="clearpendingchanges" name="clearpendingchanges"></a> clearPendingChanges

▸ **clearPendingChanges**(`clearChangeInfo?`): `void`

清除当前工作表的脏数据、插入和删除状态。

**`example`**
```
sheet.clearPendingChanges({clearType: 1, row: 0, rowCount: 3, col: 0, colCount: 4});
sheet.clearPendingChanges({clearType: 2, row: 0, rowCount: 3, col: -1});
sheet.clearPendingChanges({clearType: 4, row: 0, rowCount: 10, col: -1});
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `clearChangeInfo?` | [`IClearChangeInfo`](../interfaces/GC.Spread.Sheets.IClearChangeInfo.md) |

#### Returns

`void`

___

### <a id="clearselection" name="clearselection"></a> clearSelection

▸ **clearSelection**(): `void`

清除选择。

**`example`**
```
//此示例清除选择。
sheet.addSelection(4, 0, 2, 2);
sheet.clearSelection();
```

#### Returns

`void`

___

### <a id="copyto" name="copyto"></a> copyTo

▸ **copyTo**(`fromRow`, `fromColumn`, `toRow`, `toColumn`, `rowCount`, `columnCount`, `option`): `void`

将数据从一个范围复制到另一个范围。

**`example`**
```
//此示例将数据复制到指定位置。
activeSheet.getCell(0,0).value("1");
activeSheet.copyTo(0,0,1,1,2,2,GC.Spread.Sheets.CopyToOptions.value);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fromRow` | `number` | 源行。 |
| `fromColumn` | `number` | 源列。 |
| `toRow` | `number` | 目标行。 |
| `toColumn` | `number` | 目标列。 |
| `rowCount` | `number` | 行数。 |
| `columnCount` | `number` | 列数。 |
| `option` | [`CopyToOptions`](../enums/GC.Spread.Sheets.CopyToOptions.md) | 复制选项。 |

#### Returns

`void`

___

### <a id="currenttheme" name="currenttheme"></a> currentTheme

▸ **currentTheme**(`value?`): `any`

获取或设置工作表的当前主题。

**`example`**
```
//此示例设置主题。
sheet.currentTheme("Civic");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` \| [`Theme`](GC.Spread.Sheets.Theme.md) |

#### Returns

`any`

如果未设置值，则返回当前主题；否则返回工作表。

___

### <a id="deletecolumns" name="deletecolumns"></a> deleteColumns

▸ **deleteColumns**(`col`, `count`, `sheetArea?`): `void`

删除此工作表中指定索引处的列。

**`example`**
```
activeSheet.getCell(0,0).value("A1");
activeSheet.getCell(0,4).value("Test")
activeSheet.deleteColumns(0,2);
activeSheet.deleteRows(3,1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `col` | `number` | 要删除的第一列的索引。 |
| `count` | `number` | 要删除的列数。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`void`

___

### <a id="deleterows" name="deleterows"></a> deleteRows

▸ **deleteRows**(`row`, `count`, `sheetArea?`): `void`

删除此工作表中指定索引处的行。

**`example`**
```
activeSheet.getCell(0,0).value("A1");
activeSheet.getCell(0,4).value("Test")
activeSheet.deleteColumns(0,2);
activeSheet.deleteRows(3,1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 要删除的第一行的索引。 |
| `count` | `number` | 要删除的行数。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`void`

___

### <a id="editorstatus" name="editorstatus"></a> editorStatus

▸ **editorStatus**(): [`EditorStatus`](../enums/GC.Spread.Sheets.EditorStatus.md)

返回编辑器的状态。

#### Returns

[`EditorStatus`](../enums/GC.Spread.Sheets.EditorStatus.md)

编辑器状态。

___

### <a id="endedit" name="endedit"></a> endEdit

▸ **endEdit**(`ignoreValueChange?`): `boolean`

停止编辑活动单元格。

**`example`**
```
//此示例在单元格中输入时移除文本"123"。
activeSheet.bind(GC.Spread.Sheets.Events.EditChange, function (sender,args) {
                if (args.editingText === "123") {
                    activeSheet.endEdit(true);
               }
            });
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ignoreValueChange?` | `boolean` | 如果设置为 `true`，则不将编辑的文本应用到单元格。 |

#### Returns

`boolean`

成功停止单元格编辑时返回 `true`；否则返回 `false`。

___

### <a id="fillauto" name="fillauto"></a> fillAuto

▸ **fillAuto**(`startRange`, `wholeRange`, `options`): `void`

自动填充指定范围。

**`example`**
```
activeSheet.setValue(0, 0, 5);
var start = new GC.Spread.Sheets.Range(0, 0, 1, 1);
var r3 = new GC.Spread.Sheets.Range(0, 0, 4, 1);
activeSheet.fillAuto(start,r3, {fillType:GC.Spread.Sheets.Fill.FillType.auto, series:GC.Spread.Sheets.Fill.FillSeries.column, direction:GC.Spread.Sheets.Fill.FillDirection.down});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startRange` | [`Range`](GC.Spread.Sheets.Range.md) | 填充起始范围。 |
| `wholeRange` | [`Range`](GC.Spread.Sheets.Range.md) | 要填充的整个范围。 |
| `options` | [`IFillOptions`](../interfaces/GC.Spread.Sheets.Fill.IFillOptions.md) | 范围填充信息。 |

#### Returns

`void`

___

### <a id="fromjson" name="fromjson"></a> fromJSON

▸ **fromJSON**(`sheetSettings`): `void`

从指定的 JSON 字符串加载对象状态。

**`example`**
```
//此示例使用 fromJSON 方法。
activeSheet.getCell(0,0).value(123);
var jsonStr = null;
//导出
jsonStr = JSON.stringify(activeSheet.toJSON());
//导入
activeSheet.fromJSON(JSON.parse(jsonStr));
alert(jsonStr);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheetSettings` | `Object` | 反序列化后的工作表数据。 |

#### Returns

`void`

___

### <a id="frozencolumncount" name="frozencolumncount"></a> frozenColumnCount

▸ **frozenColumnCount**(`colCount?`, `leftCol?`): `any`

获取或设置工作表的冻结列数。

**`example`**
```
sheet.frozenColumnCount(30, 20);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `colCount?` | `number` |
| `leftCol?` | `number` |

#### Returns

`any`

如果未设置值，则返回冻结列数；否则返回工作表。

___

### <a id="frozenrowcount" name="frozenrowcount"></a> frozenRowCount

▸ **frozenRowCount**(`rowCount?`, `topRow?`): `any`

获取或设置工作表的冻结行数。

**`example`**
```
sheet.frozenRowCount(60, 50);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `rowCount?` | `number` |
| `topRow?` | `number` |

#### Returns

`any`

如果未设置值，则返回冻结行数；否则返回工作表。

___

### <a id="frozentrailingcolumncount" name="frozentrailingcolumncount"></a> frozenTrailingColumnCount

▸ **frozenTrailingColumnCount**(`colCount?`, `stickToEdge?`): `any`

获取或设置工作表的尾部冻结列数。

**`example`**
```
sheet.frozenTrailingColumnCount(1, false);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `colCount?` | `number` |
| `stickToEdge?` | `boolean` |

#### Returns

`any`

如果未设置值，则返回尾部冻结列数；否则返回工作表。

___

### <a id="frozentrailingrowcount" name="frozentrailingrowcount"></a> frozenTrailingRowCount

▸ **frozenTrailingRowCount**(`rowCount?`, `stickToEdge?`): `any`

获取或设置工作表的尾部冻结行数。

**`example`**
```
sheet.frozenTrailingRowCount(1, false);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `rowCount?` | `number` |
| `stickToEdge?` | `boolean` |

#### Returns

`any`

如果未设置值，则返回尾部冻结行数；否则返回工作表。

___

### <a id="getactivecolumnindex" name="getactivecolumnindex"></a> getActiveColumnIndex

▸ **getActiveColumnIndex**(): `number`

获取此工作表的当前活动列索引。

**`example`**
```
//此示例获取活动列。
sheet.setActiveCell(5,5);
alert(sheet.getActiveColumnIndex());
alert(sheet.getActiveRowIndex());
spread.bind(GC.Spread.Sheets.Events.EnterCell, function (event, data) {
    alert(data.col);
    alert(data.row);
  });
spread.bind(GC.Spread.Sheets.Events.LeaveCell, function (event, data) {
    alert(data.col);
    alert(data.row);
  });
```

#### Returns

`number`

活动单元格的列索引。

___

### <a id="getactiverowindex" name="getactiverowindex"></a> getActiveRowIndex

▸ **getActiveRowIndex**(): `number`

获取此工作表的当前活动行索引。

**`example`**
```
//此示例获取活动行。
sheet.setActiveCell(5,5);
alert(sheet.getActiveColumnIndex());
alert(sheet.getActiveRowIndex());
spread.bind(GC.Spread.Sheets.Events.EnterCell, function (event, data) {
    alert(data.col);
    alert(data.row);
  });
spread.bind(GC.Spread.Sheets.Events.LeaveCell, function (event, data) {
    alert(data.col);
    alert(data.row);
  });
```

#### Returns

`number`

活动单元格的行索引。

___

### <a id="getactualstyle" name="getactualstyle"></a> getActualStyle

▸ **getActualStyle**(`row`, `column`, `sheetArea?`, `sheetStyleOnly?`): [`Style`](GC.Spread.Sheets.Style.md)

获取指定工作表区域中指定单元格的实际样式信息。

**`example`**
```
//此示例使用 getActualStyle 方法。
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
style.borderLeft =new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderTop = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderRight = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderBottom = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
var cstyle = activeSheet.getActualStyle(1,1,GC.Spread.Sheets.SheetArea.viewport, true);
alert(cstyle.backColor);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `column` | `number` | 列索引。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |
| `sheetStyleOnly?` | `boolean` | - |

#### Returns

[`Style`](GC.Spread.Sheets.Style.md)

返回指定单元格的单元格样式。

___

### <a id="getalttext" name="getalttext"></a> getAltText

▸ **getAltText**(`row`, `col`, `sheetArea?`): `any`

获取指定工作表区域中指定单元格的替代文本。

**`example`**
```
var SpreadIcon = {
    FolderOpen: '\ue685',
    InfoFilled: '\ue718',
    Library: '\ue69d',
    NotebookFilled: '\uD800\uDC0F',
    Browse: '\ue626'
};
activeSheet.setValue(1, 1, SpreadIcon.FolderOpen);
activeSheet.setAltText(1, 1, "Folder Open Icon");
alert(activeSheet.getAltText(1, 1));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | 工作表区域。如果未提供此参数，则默认为 `viewport`。 |

#### Returns

`any`

返回单元格的替代文本。

___

### <a id="getarray" name="getarray"></a> getArray

▸ **getArray**(`row`, `column`, `rowCount`, `columnCount`, `getFormula?`): `any`[]

从指定范围的单元格中获取对象数组。

**`example`**
```
//此示例使用 getArray 方法。
//设置值
var array = [[1,2,3],[4,5],[6,7,8,9]];
activeSheet.setArray(1, 2, array);
//设置公式
var array = [["=1+1","=2+2","=3+3"],["=4+4","=5+5"],["=6+6","=7+7","=8+8","=9+9"]];
activeSheet.setArray(1, 2, array, true);
//获取值
var newArray = activeSheet.getArray(1, 2, 3, 4);
//获取公式
var newArray = activeSheet.getArray(1, 2, 3, 4, true);
//alert(newArray[0]);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `column` | `number` | 列索引。 |
| `rowCount` | `number` | 行数。 |
| `columnCount` | `number` | - |
| `getFormula?` | `boolean` | 如果为 `true`，则返回公式；否则返回值。 |

#### Returns

`any`[]

指定范围单元格中的对象数组。

___

### <a id="getbindingpath" name="getbindingpath"></a> getBindingPath

▸ **getBindingPath**(`row`, `col`): `string`

获取指定工作表区域中指定单元格的单元格级绑定的绑定路径。

**`example`**
```
//此示例使用 getBindingPath 方法。
var person = {name: "Wang feng", age: 25, address: {postcode: "710075"}};
var source = new GC.Spread.Sheets.Bindings.CellBindingSource(person);
activeSheet.setBindingPath(0, 0, "name");
activeSheet.setBindingPath(1, 1, "age");
activeSheet.setBindingPath(3, 3, "address.postcode");
activeSheet.setDataSource(source);
alert(activeSheet.getBindingPath(0, 0, GC.Spread.Sheets.SheetArea.viewport));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |

#### Returns

`string`

返回单元格级绑定的单元格绑定路径。

___

### <a id="getcell" name="getcell"></a> getCell

▸ **getCell**(`row`, `col`, `sheetArea?`): [`CellRange`](GC.Spread.Sheets.CellRange.md)

获取指定工作表区域中的指定单元格。

**`example`**
```
//此示例获取单元格。
activeSheet.getCell(1,1).text("cell object");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | 工作表区域。如果未提供此参数，则默认为 `viewport`。 |

#### Returns

[`CellRange`](GC.Spread.Sheets.CellRange.md)

单元格。

___

### <a id="getcellrect" name="getcellrect"></a> getCellRect

▸ **getCellRect**(`row`, `col`, `rowViewportIndex?`, `colViewportIndex?`): [`Rect`](GC.Spread.Sheets.Rect.md)

获取单元格的矩形区域。

**`example`**
```
//此示例使用 getCellRect 方法。
activeSheet.bind(GC.Spread.Sheets.Events.CellClick, function (e, info) {
               if (info.sheetArea === GC.Spread.Sheets.SheetArea.viewport) {
                   alert("Clicked cell index (" + info.row + "," + info.col + ")");
                   //获取指定索引位置存在的常规单元格的坐标信息
                   var cellRect = activeSheet.getCellRect(info.row, info.col);
                   alert("X coordinate:" + cellRect.x);
                   alert("Y coordinate:" + cellRect.y);
                   alert("Cell width:" + cellRect.width);
                   alert("Cell height:" + cellRect.height);
               }
           });
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `rowViewportIndex?` | `number` | - |
| `colViewportIndex?` | `number` | - |

#### Returns

[`Rect`](GC.Spread.Sheets.Rect.md)

包含单元格矩形区域大小和位置的对象。

___

### <a id="getcelltype" name="getcelltype"></a> getCellType

▸ **getCellType**(`row`, `col`, `sheetArea?`): [`Base`](GC.Spread.Sheets.CellTypes.Base.md)

获取单元格类型。

**`example`**
```
//此示例获取单元格类型。
var cellType = new GC.Spread.Sheets.CellTypes.Button();
cellType.buttonBackColor("#FFFF00");
cellType.text("this is a button");
activeSheet.getCell(0, 2).cellType(cellType);
var cellType = activeSheet.getCellType(0,2,GC.Spread.Sheets.SheetArea.viewport)
if (cellType instanceof GC.Spread.Sheets.CellTypes.Button) {
      alert("This is a ButtonCellType");
}
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

[`Base`](GC.Spread.Sheets.CellTypes.Base.md)

返回指定单元格的单元格类型。

___

### <a id="getcolumncount" name="getcolumncount"></a> getColumnCount

▸ **getColumnCount**(`sheetArea?`): `number`

获取指定工作表区域中的列数。

**`example`**
```
//此示例获取列数。
var count = activeSheet.getColumnCount(GC.Spread.Sheets.SheetArea.viewport);
alert(count);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) |

#### Returns

`number`

列数。

___

### <a id="getcolumnpagebreak" name="getcolumnpagebreak"></a> getColumnPageBreak

▸ **getColumnPageBreak**(`column`): `boolean`

获取在打印时是否在指定列之前插入强制分页符。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `column` | `number` | 列索引。 |

#### Returns

`boolean`

如果在指定列之前插入了强制分页符，则为 `true`；否则为 `false`。

___

### <a id="getcolumnresizable" name="getcolumnresizable"></a> getColumnResizable

▸ **getColumnResizable**(`col`, `sheetArea?`): `boolean`

获取用户是否可以在指定工作表区域中调整指定列的大小。

**`example`**
```
//此示例获取列是否可调整大小。
sheet.setRowCount(10);
sheet.setColumnCount(7);
sheet.setValue(0, 0,"Western");
sheet.setValue(0, 1,"Western");
sheet.setValue(0, 2,"Western");
sheet.setValue(1, 0,"A");
sheet.setValue(1, 1,"B");
sheet.setValue(1, 2,"C");
sheet.setColumnResizable(0,true, GC.Spread.Sheets.SheetArea.colHeader);
sheet.setRowResizable(0,true, GC.Spread.Sheets.SheetArea.rowHeader);
alert( sheet.getColumnResizable(0));
alert( sheet.getRowResizable(0, GC.Spread.Sheets.SheetArea.rowHeader));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `col` | `number` | 列索引。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`boolean`

如果用户可以调整指定列的大小，则为 `true`；否则为 `false`。

___

### <a id="getcolumnvisible" name="getcolumnvisible"></a> getColumnVisible

▸ **getColumnVisible**(`col`, `sheetArea?`): `boolean`

获取指定工作表区域中的列是否显示。

**`example`**
```
//此示例返回列的可见性和宽度设置。
var visible = activeSheet.getColumnVisible(1, GC.Spread.Sheets.SheetArea.viewport);
var width = activeSheet.getColumnWidth(1, GC.Spread.Sheets.SheetArea.viewport);
alert(visible);
alert(width);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `col` | `number` | 列索引。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`boolean`

如果列在工作表区域中可见，则为 `true`；否则为 `false`。

___

### <a id="getcolumnwidth" name="getcolumnwidth"></a> getColumnWidth

▸ **getColumnWidth**(`col`, `sheetArea?`, `getDynamicSize?`): `any`

获取指定工作表区域中指定列的宽度（以像素为单位）或动态大小。

**`example`**
```
//此示例返回列的可见性和宽度设置。
var visible = activeSheet.getColumnVisible(1, GC.Spread.Sheets.SheetArea.viewport);
var width = activeSheet.getColumnWidth(1, GC.Spread.Sheets.SheetArea.viewport);
alert(visible);
alert(width);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `col` | `number` | 列索引。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |
| `getDynamicSize?` | `boolean` | - |

#### Returns

`any`

列宽度（以像素为单位）或动态大小。

___

### <a id="getcsv" name="getcsv"></a> getCsv

▸ **getCsv**(`row`, `column`, `rowCount`, `columnCount`, `rowDelimiter`, `columnDelimiter`): `string`

从范围中获取带分隔符的文本。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 起始行。 |
| `column` | `number` | 起始列。 |
| `rowCount` | `number` | 行数。 |
| `columnCount` | `number` | 列数。 |
| `rowDelimiter` | `string` | 添加到行末尾的行分隔符。 |
| `columnDelimiter` | `string` | 添加到列末尾的列分隔符。 |

#### Returns

`string`

带有指定分隔符的范围文本。

___

### <a id="getcustomfunction" name="getcustomfunction"></a> getCustomFunction

▸ **getCustomFunction**(`name`): `void`

获取自定义函数。

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |

#### Returns

`void`

自定义函数。

___

### <a id="getcustomname" name="getcustomname"></a> getCustomName

▸ **getCustomName**(`name`): [`NameInfo`](GC.Spread.Sheets.NameInfo.md)

获取指定的自定义名称信息。

**`example`**
```
//此示例获取自定义名称和公式。
activeSheet.setValue(0, 0, 1);
activeSheet.setValue(0, 1, 2);
activeSheet.setValue(0, 2, 3);
activeSheet.addCustomName("customName1", "=12", 0, 0);
activeSheet.addCustomName("customName2", "Average(20,45)", 0, 0);
activeSheet.addCustomName("customName3", "=$A$1:$C$1");
activeSheet.setFormula(1, 0, "customName1");
activeSheet.setFormula(1, 1, "customName2");
activeSheet.setFormula(1, 2, "sum(customName3)");
$("#button1").click(function () {
    let cname = activeSheet.getCustomName("customName2");
    if (cname instanceof GC.Spread.Sheets.NameInfo) {
        //获取自定义名称
        let name = cname.getName();
        //获取表达式
        let expression = cname.getExpression();
        //获取表达式字符串
        let expStr = GC.Spread.Sheets.CalcEngine.expressionToFormula(activeSheet, expression, 0, 0);
        alert("Name:" + name + ";Expression: =" + expStr);
    }
});
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |

#### Returns

[`NameInfo`](GC.Spread.Sheets.NameInfo.md)

指定自定义名称的信息。

___

### <a id="getcustomnames" name="getcustomnames"></a> getCustomNames

▸ **getCustomNames**(): [`NameInfo`](GC.Spread.Sheets.NameInfo.md)[]

获取所有自定义名称信息。

#### Returns

[`NameInfo`](GC.Spread.Sheets.NameInfo.md)[]

存储在数组中的 GC.Spread.Sheets.NameInfo 类型。

___

### <a id="getdatacolumnname" name="getdatacolumnname"></a> getDataColumnName

▸ **getDataColumnName**(`column`): `string`

获取指定位置的列名。

**`example`**
```
//此示例返回指定绑定列的名称。
var test = [
        {"Series0":2,"Series1":1},
        {"Series0":4,"Series1":2},
        {"Series0":3,"Series1":4}
    ];
activeSheet.setDataSource(test);
activeSheet.bindColumn(1,"Series0");
activeSheet.bindColumn(0,"Series1");
var colname = activeSheet.getDataColumnName(0);
alert(colname);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `column` | `number` | 请求名称的列索引。 |

#### Returns

`string`

数据绑定的列名。

___

### <a id="getdataitem" name="getdataitem"></a> getDataItem

▸ **getDataItem**(`row`): `any`

获取数据项。

**`example`**
```
//此示例使用 getDataItem 方法。
var test = [
      { "Series0": 2, "Series1": 1 },
      { "Series0": 4, "Series1": 2 },
      { "Series0": 3, "Series1": 4 }
           ];
           activeSheet.autoGenerateColumns = true;
           activeSheet.setDataSource(test, false);
           alert(JSON.stringify(activeSheet.getDataItem(0)));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |

#### Returns

`any`

行数据。

___

### <a id="getdatasource" name="getdatasource"></a> getDataSource

▸ **getDataSource**(): `any`

获取填充工作表的数据源。

**`function`**

**`example`**
```
var test = [
        {"Series0":2,"Series1":1},
        {"Series0":4,"Series1":2},
        {"Series0":3,"Series1":4}
    ];
activeSheet.setDataSource(test);
alert(activeSheet.getDataSource);
```

#### Returns

`any`

返回数据源。

___

### <a id="getdatavalidator" name="getdatavalidator"></a> getDataValidator

▸ **getDataValidator**(`row`, `col`, `sheetArea`): [`DefaultDataValidator`](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md)

获取单元格数据验证器。

**`example`**
```
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createListValidator("1,2,3");
dv.showInputMessage(true);
dv.inputMessage("Value must be 1,2 or 3");
dv.inputTitle("tip");
activeSheet.setDataValidator(1,1,1,1,dv,GC.Spread.Sheets.SheetArea.viewport);
alert(activeSheet.getDataValidator(1,1).getValidList(activeSheet,1,1));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `sheetArea` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | 工作表区域。如果未提供此参数，则默认为 `viewport`。 |

#### Returns

[`DefaultDataValidator`](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md)

返回指定单元格的数据验证器。

___

### <a id="getdefaultstyle" name="getdefaultstyle"></a> getDefaultStyle

▸ **getDefaultStyle**(`sheetArea?`): [`Style`](GC.Spread.Sheets.Style.md)

获取工作表的默认样式信息。

**`example`**
```
//此示例使用 getDefaultStyle 方法。
var defaultStyle = new GC.Spread.Sheets.Style();
defaultStyle.backColor = "LemonChiffon";
defaultStyle.foreColor = "Red";
defaultStyle.borderLeft = new GC.Spread.Sheets.LineBorder("Green");
defaultStyle.borderTop = new GC.Spread.Sheets.LineBorder("Green");
defaultStyle.borderRight = new GC.Spread.Sheets.LineBorder("Green");
defaultStyle.borderBottom = new GC.Spread.Sheets.LineBorder("Green");
activeSheet.setDefaultStyle(defaultStyle, GC.Spread.Sheets.SheetArea.viewport);
var cstyle = activeSheet.getDefaultStyle(GC.Spread.Sheets.SheetArea.viewport);
alert(cstyle.backColor);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) |

#### Returns

[`Style`](GC.Spread.Sheets.Style.md)

返回工作表的默认样式。

___

### <a id="getdefaultvalue" name="getdefaultvalue"></a> getDefaultValue

▸ **getDefaultValue**(`row`, `col`): `any`

获取指定单元格的默认值。

**`example`**
```
sheet.setDefaultValue(0, 0, 20);
let defaultValue = sheet.getDefaultValue(0, 0);
let value = sheet.getValue(0, 0); // 值等于 defaultValue
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |

#### Returns

`any`

返回单元格的默认值。

___

### <a id="getdeletedrows" name="getdeletedrows"></a> getDeletedRows

▸ **getDeletedRows**(): `any`[]

获取已删除的行集合。

#### Returns

`any`[]

已删除的行集合。数组中的项包含两个属性：row.row 指定已删除的行索引，row.originalItem 指定已删除的数据项。

___

### <a id="getdependents" name="getdependents"></a> getDependents

▸ **getDependents**(`row`, `col`): [`ICellsInfo`](../interfaces/GC.Spread.Sheets.ICellsInfo.md)[]

获取单元格的依赖 CellRange 信息对象数组。

**`example`**
```
sheet.getDependents(1, 1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |

#### Returns

[`ICellsInfo`](../interfaces/GC.Spread.Sheets.ICellsInfo.md)[]

返回依赖单元格信息对象数组
dependentsInfo.row {number} 表示 cellRange 行索引。
dependentsInfo.col {number} 表示 cellRange 列索引。
dependentsInfo.rowCount {number} 表示 cellRange 行数。
dependentsInfo.colCount {number} 表示 cellRange 列数。
dependentsInfo.sheetName {string} 表示工作表名称。

___

### <a id="getdirtycells" name="getdirtycells"></a> getDirtyCells

▸ **getDirtyCells**(`row`, `col`, `rowCount`, `colCount`): [`IDirtyCellInfo`](../interfaces/GC.Spread.Sheets.IDirtyCellInfo.md)[]

获取脏单元格集合。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `rowCount` | `number` | 脏单元格范围的行数。 |
| `colCount` | `number` | 脏单元格范围的列数。 |

#### Returns

[`IDirtyCellInfo`](../interfaces/GC.Spread.Sheets.IDirtyCellInfo.md)[]

脏单元格集合。

___

### <a id="getdirtyrows" name="getdirtyrows"></a> getDirtyRows

▸ **getDirtyRows**(): `any`[]

获取脏行集合。

#### Returns

`any`[]

脏行集合，数组中的项包含三个属性：row.row 指定行索引，row.item 指定当前行的数据项，row.originalItem 指定行的原始数据项。

___

### <a id="getformatter" name="getformatter"></a> getFormatter

▸ **getFormatter**(`row`, `col`, `sheetArea`): `any`

获取单元格格式化器。

**`example`**
```
//此示例返回活动工作表的格式对象。
activeSheet.getCell(0, 1).formatter("M");
activeSheet.setValue(0, 1, new Date(2011, 2, 9));
var style = activeSheet.getFormatter(0,1,GC.Spread.Sheets.SheetArea.viewport);
alert(style);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `sheetArea` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | 工作表区域。如果未提供此参数，则默认为 `viewport`。 |

#### Returns

`any`

返回指定单元格的格式化器字符串或对象。

___

### <a id="getformula" name="getformula"></a> getFormula

▸ **getFormula**(`row`, `col`, `sheetArea?`): `string`

获取此工作表中指定单元格的公式。

**`example`**
```
//此示例返回指定单元格中的公式。
activeSheet.setValue(0,0,1);
activeSheet.setValue(0,1,2);
activeSheet.setValue(0,2,10);
activeSheet.getCell(1,1).formula("=SUM(A1:C1)");
let formula = activeSheet.getFormula(1, 1, GC.Spread.Sheets.SheetArea.viewport);
alert(formula);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`string`

返回公式字符串。

___

### <a id="getformulainformation" name="getformulainformation"></a> getFormulaInformation

▸ **getFormulaInformation**(`row`, `col`): [`IFormulaInfo`](../interfaces/GC.Spread.Sheets.IFormulaInfo.md)

获取此工作表中指定单元格的公式详细信息。

**`example`**
```
activeSheet.setValue(0,0,1);
activeSheet.setValue(0,1,2);
activeSheet.setValue(0,2,10);
activeSheet.getCell(1,1).formula("=SUM(A1:C1)");
let test = activeSheet.getFormulaInformation(1,1, GC.Spread.Sheets.SheetArea.viewport);
alert(test.formula);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |

#### Returns

[`IFormulaInfo`](../interfaces/GC.Spread.Sheets.IFormulaInfo.md)

formulaInfo - 返回单元格的公式信息。
formulaInfo.hasFormula {boolean} 指示单元格中是否有公式。
formulaInfo.isArrayFormula {boolean} 指示公式是否为数组公式。
formulaInfo.formula {string} 公式字符串。
formulaInfo.formulaWithCulture {string} 带区域设置的公式字符串。

___

### <a id="gethyperlink" name="gethyperlink"></a> getHyperlink

▸ **getHyperlink**(`row`, `col`, `sheetArea?`): [`IHyperlink`](../interfaces/GC.Spread.Sheets.IHyperlink.md)

获取指定工作表区域中指定单元格的超链接数据。

**`example`**
```
//此示例使用 getHyperlink 方法。
let firstHyperlinkData = sheet.getHyperlink(0, 2, GC.Spread.Sheets.SheetArea.viewport);
let secondHyperlinkData = sheet.setHyperlink(1, 1, GC.Spread.Sheets.SheetArea.viewport);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | 工作表区域。如果未提供此参数，则默认为 `viewport`。 |

#### Returns

[`IHyperlink`](../interfaces/GC.Spread.Sheets.IHyperlink.md)

___

### <a id="getid" name="getid"></a> getId

▸ **getId**(): `string`

获取工作表的ID

#### Returns

`string`

工作表的ID

___

### <a id="getinsertrows" name="getinsertrows"></a> getInsertRows

▸ **getInsertRows**(): `any`[]

获取插入的行集合。

#### Returns

`any`[]

插入的行集合，数组中的项包含两个属性：row.row 指定插入行索引，row.item 指定插入数据项。

___

### <a id="getnamedstyle" name="getnamedstyle"></a> getNamedStyle

▸ **getNamedStyle**(`name`): [`Style`](GC.Spread.Sheets.Style.md)

从工作表的命名样式集合中获取具有指定名称的样式。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要返回的样式名称。 |

#### Returns

[`Style`](GC.Spread.Sheets.Style.md)

返回指定的命名样式。

___

### <a id="getnamedstyles" name="getnamedstyles"></a> getNamedStyles

▸ **getNamedStyles**(): [`Style`](GC.Spread.Sheets.Style.md)[]

从工作表中获取命名样式。

#### Returns

[`Style`](GC.Spread.Sheets.Style.md)[]

命名样式的 GC.Spread.Sheets.Style 数组。

___

### <a id="getparent" name="getparent"></a> getParent

▸ **getParent**(): [`Workbook`](GC.Spread.Sheets.Workbook.md)

获取当前工作表的父级 Spread 对象。

#### Returns

[`Workbook`](GC.Spread.Sheets.Workbook.md)

返回当前工作表的父级 Spread 对象。

___

### <a id="getprecedents" name="getprecedents"></a> getPrecedents

▸ **getPrecedents**(`row`, `col`): [`ICellsInfo`](../interfaces/GC.Spread.Sheets.ICellsInfo.md)[]

获取单元格的前置单元格范围信息对象数组。

**`example`**
```
sheet.getPrecedents(1, 1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |

#### Returns

[`ICellsInfo`](../interfaces/GC.Spread.Sheets.ICellsInfo.md)[]

返回前置单元格范围信息对象数组
precedentsInfo.row {number} 表示单元格范围的行索引。
precedentsInfo.col {number} 表示单元格范围的列索引。
precedentsInfo.rowCount {number} 表示单元格范围的行数。
precedentsInfo.colCount {number} 表示单元格范围的列数。
precedentsInfo.sheetName {string} 表示工作表名称。

___

### <a id="getrange" name="getrange"></a> getRange

▸ **getRange**(`row`, `col`, `rowCount?`, `colCount?`, `sheetArea?`): [`CellRange`](GC.Spread.Sheets.CellRange.md)

通过行信息和列信息在指定的工作表区域中获取单元格范围。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `rowCount?` | `number` | 范围的行数。如果未提供此参数，则默认为 `1`。 |
| `colCount?` | `number` | 范围的列数。如果未提供此参数，则默认为 `1`。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | 工作表区域。如果未提供此参数，则默认为 `viewport`。 |

#### Returns

[`CellRange`](GC.Spread.Sheets.CellRange.md)

单元格范围。
如果 row 为 -1 且 rowCount 为 -1，则范围表示列。例如，sheet.getRange(-1,4,-1,6) 返回列 "E:J"。
如果 col 为 -1 且 colCount 为 -1，则范围表示行。例如，sheet.getRange(4,-1,6,-1) 返回行 "5:10"。

▸ **getRange**(`address`, `sheetArea?`): [`CellRange`](GC.Spread.Sheets.CellRange.md)

通过 A1 样式的地址（不支持 R1C1 样式）在指定的工作表区域中获取单元格范围。

**`example`**
```
// 获取单个单元格，等同于 sheet.getRange(0, 0, 1, 1)
sheet.getRange("A1")
// 获取整列，等同于 sheet.getRange(-1, 0, -1, 3)
sheet.getRange("A:C")
// 获取整行，等同于 sheet.getRange(0, -1, 3, -1)
sheet.getRange("1:3")
// 获取范围，等同于 sheet.getRange(0, 0, 3, 3)
sheet.getRange("A1:C3")
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `address` | `string` | 范围地址字符串。例如 "C1"、"A:C"、"A1:C3"、"1:3"。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | 工作表区域。如果未提供此参数，则默认为 `viewport`。 |

#### Returns

[`CellRange`](GC.Spread.Sheets.CellRange.md)

单元格范围。

___

### <a id="getrowcount" name="getrowcount"></a> getRowCount

▸ **getRowCount**(`sheetArea?`): `number`

获取指定工作表区域中的行数。

**`example`**
```
//此示例获取行数。
var count = activeSheet.getRowCount(GC.Spread.Sheets.SheetArea.viewport);
alert(count);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) |

#### Returns

`number`

行数。

___

### <a id="getrowheight" name="getrowheight"></a> getRowHeight

▸ **getRowHeight**(`row`, `sheetArea?`, `getDynamicSize?`): `any`

获取指定工作表区域中指定行的高度（以像素为单位）或动态大小。

**`example`**
```
//此示例返回指定行的高度。
var rheight = activeSheet.getRowHeight(1,GC.Spread.Sheets.SheetArea.viewport);
alert(rheight);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |
| `getDynamicSize?` | `boolean` | - |

#### Returns

`any`

行高（以像素为单位）或动态大小。

___

### <a id="getrowpagebreak" name="getrowpagebreak"></a> getRowPageBreak

▸ **getRowPageBreak**(`row`): `boolean`

获取在打印时是否在指定行之前插入强制分页符。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |

#### Returns

`boolean`

如果在指定行之前插入了强制分页符，则为 `true`；否则为 `false`。

___

### <a id="getrowresizable" name="getrowresizable"></a> getRowResizable

▸ **getRowResizable**(`row`, `sheetArea?`): `boolean`

获取用户是否可以在指定的工作表区域中调整指定行的大小。

**`example`**
```
//此示例获取行是否可调整大小。
sheet.setRowCount(10);
sheet.setColumnCount(7);
sheet.setValue(0, 0,"Western");
sheet.setValue(0, 1,"Western");
sheet.setValue(0, 2,"Western");
sheet.setValue(1, 0,"A");
sheet.setValue(1, 1,"B");
sheet.setValue(1, 2,"C");
sheet.setColumnResizable(0,true, GC.Spread.Sheets.SheetArea.colHeader);
sheet.setRowResizable(0,true, GC.Spread.Sheets.SheetArea.rowHeader);
alert( sheet.getColumnResizable(0));
alert( sheet.getRowResizable(0, GC.Spread.Sheets.SheetArea.rowHeader));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`boolean`

如果用户可以调整指定行的大小，则为 `true`；否则为 `false`。

___

### <a id="getrowvisible" name="getrowvisible"></a> getRowVisible

▸ **getRowVisible**(`row`, `sheetArea?`): `boolean`

获取控件是否显示指定行。

**`example`**
```
//此示例返回指定行的可见性设置。
rvisible = activeSheet.getRowVisible(1,GC.Spread.Sheets.SheetArea.viewport);
alert(rvisible);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`boolean`

如果行在工作表区域中可见，则为 `true`；否则为 `false`。

___

### <a id="getselections" name="getselections"></a> getSelections

▸ **getSelections**(): [`Range`](GC.Spread.Sheets.Range.md)[]

获取当前工作表中的选择。

#### Returns

[`Range`](GC.Spread.Sheets.Range.md)[]

类型为 GC.Spread.Sheets.Range 的数组。

___

### <a id="getsortstate" name="getsortstate"></a> getSortState

▸ **getSortState**(): [`ISortState`](../interfaces/GC.Spread.Sheets.ISortState.md)

获取此工作表中的最后排序状态。

**`example`**
```
//此示例获取排序状态。
sheet.setValue(0,0,"112");
sheet.setValue(1,0,"10");
sheet.setValue(2,0,"223");
sheet.setValue(3,0,"20");
sheet.setValue(4,0,"334");
sheet.setValue(5,0,"30");
sheet.sortRange(0, 0, 6, 1, true, [{index:0, ascending:true}]);
let sortState = sheet.getSortState();
```

#### Returns

[`ISortState`](../interfaces/GC.Spread.Sheets.ISortState.md)

最后的排序状态信息。

___

### <a id="getspans" name="getspans"></a> getSpans

▸ **getSpans**(`range?`, `sheetArea?`): [`Range`](GC.Spread.Sheets.Range.md)[]

获取指定工作表区域中指定范围的合并单元格信息。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range?` | [`Range`](GC.Spread.Sheets.Range.md) | 单元格范围。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

[`Range`](GC.Spread.Sheets.Range.md)[]

包含合并单元格信息的数组，其项类型为 GC.Spread.Sheets.Range。

___

### <a id="getsparkline" name="getsparkline"></a> getSparkline

▸ **getSparkline**(`row`, `column`): [`Sparkline`](GC.Spread.Sheets.Sparklines.Sparkline.md)

获取指定单元格的迷你图。

**`example`**
```
//此示例创建并获取一个迷你图。
var cellr = new GC.Spread.Sheets.Range(0, 0, 1, 5);
var ex = new GC.Spread.Sheets.Sparklines.SparklineSetting();
ex.options.SeriesColor  = "Aquamarine";
sheet.setValue(0, 0, 2);
sheet.setValue(0, 1, 5);
sheet.setValue(0, 2, 4);
sheet.setValue(0, 3, -1);
sheet.setValue(0, 4, 3);
sheet.setSparkline(0, 5, cellr, GC.Spread.Sheets.Sparklines.DataOrientation.horizontal, GC.Spread.Sheets.Sparklines.SparklineType.column, ex);
alert(sheet.getSparkline(0, 5).toString());
//sheet.removeSparkline(0, 5);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `column` | `number` | - |

#### Returns

[`Sparkline`](GC.Spread.Sheets.Sparklines.Sparkline.md)

单元格的迷你图。

___

### <a id="getstyle" name="getstyle"></a> getStyle

▸ **getStyle**(`row`, `column`, `sheetArea?`): [`Style`](GC.Spread.Sheets.Style.md)

获取指定工作表区域中指定单元格的样式信息。

**`example`**
```
//此示例使用 getStyle 方法。
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
style.borderLeft =new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderTop = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderRight = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
style.borderBottom = new GC.Spread.Sheets.LineBorder("blue",GC.Spread.Sheets.LineStyle.medium);
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
var cstyle = activeSheet.getStyle(1,1,GC.Spread.Sheets.SheetArea.viewport);
alert(cstyle.backColor);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `column` | `number` | 列索引。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

[`Style`](GC.Spread.Sheets.Style.md)

返回指定单元格的样式。

___

### <a id="getstylename" name="getstylename"></a> getStyleName

▸ **getStyleName**(`row`, `column`, `sheetArea?`): `string`

获取指定工作表区域中指定单元格的样式名称。

**`example`**
```
//此示例使用 getStyleName 方法。
var namedStyle = new GC.Spread.Sheets.Style();
namedStyle.name = "style1";
namedStyle.backColor = "green";
activeSheet.addNamedStyle(namedStyle);
activeSheet.setStyleName(1, 1, "style1"); // cell(1,1)的背景色为绿色。
activeSheet.setStyleName(2, 1, "style1");
alert(activeSheet.getStyleName(1,1,GC.Spread.Sheets.SheetArea.viewport));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `column` | `number` | 列索引。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`string`

返回样式的名称字符串。

___

### <a id="gettag" name="gettag"></a> getTag

▸ **getTag**(`row`, `col`, `sheetArea?`): `any`

获取指定工作表区域中指定单元格的标签值。

**`example`**
```
//此示例添加并获取单元格标签。
activeSheet.getRange(1, -1, 1, -1).tag("row tag");
alert(activeSheet.getTag(1,-1,GC.Spread.Sheets.SheetArea.viewport));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | 工作表区域。如果未提供此参数，则默认为 `viewport`。 |

#### Returns

`any`

返回单元格的标签值。

___

### <a id="gettext" name="gettext"></a> getText

▸ **getText**(`row`, `col`, `sheetArea?`): `string`

获取指定工作表区域中单元格的格式化文本。

**`example`**
```
activeSheet.getText(1, 0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`string`

返回单元格的格式化文本。

___

### <a id="getusedrange" name="getusedrange"></a> getUsedRange

▸ **getUsedRange**(`type?`): [`Range`](GC.Spread.Sheets.Range.md)

获取工作表中使用的范围。

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:1});
var sheet = spread.getSheet(0);
sheet.setValue(2, 2, "value");
sheet.setValue(4, 2, "value");
sheet.setValue(6, 8, "value");
sheet.setValue(10, 15, "value");
sheet.setFormula(5, 5, "=C3");
sheet.setFormula(8, 8, "=I6");
sheet.setStyle(30,4, new GC.Spread.Sheets.Style())
sheet.setStyle(3, 24, new GC.Spread.Sheets.Style())
sheet.setRowHeight(8, 40);
sheet.getUsedRange(GC.Spread.Sheets.UsedRangeType.all);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `type?` | [`UsedRangeType`](../enums/GC.Spread.Sheets.UsedRangeType.md) |

#### Returns

[`Range`](GC.Spread.Sheets.Range.md)

如果未设置值，则返回 null；否则返回使用的范围。

___

### <a id="getvalue" name="getvalue"></a> getValue

▸ **getValue**(`row`, `col`, `sheetArea?`, `valueType?`): `any`

获取指定工作表区域中指定单元格的未格式化数据。

**`example`**
```
activeSheet.getValue(1, 1, GC.Spread.Sheets.SheetArea.viewport, GC.Spread.Sheets.ValueType.richText);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |
| `valueType?` | [`ValueType`](../enums/GC.Spread.Sheets.ValueType.md) | - |

#### Returns

`any`

返回单元格的值。

___

### <a id="getviewportbottomrow" name="getviewportbottomrow"></a> getViewportBottomRow

▸ **getViewportBottomRow**(`rowViewportIndex`): `number`

获取视口中底部行的索引。

**`example`**
```
//此示例返回当前工作表视图中底部和顶部行以及左右列的索引。
var brow = activeSheet.getViewportBottomRow(1);
var lcol = activeSheet.getViewportLeftColumn(1);
var rcol = activeSheet.getViewportRightColumn(1);
var trow = activeSheet.getViewportTopRow(1);
alert(brow);
alert(lcol);
alert(rcol);
alert(trow);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rowViewportIndex` | `number` | 视口索引。 |

#### Returns

`number`

视口中底部行的索引。

___

### <a id="getviewportheight" name="getviewportheight"></a> getViewportHeight

▸ **getViewportHeight**(`rowViewportIndex`): `number`

获取活动工作表指定视口行的高度。

**`example`**
```
//此示例使用 getViewportHeight 方法。
alert(activeSheet.getViewportHeight(1));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rowViewportIndex` | `number` | 行视口索引。 |

#### Returns

`number`

视口的高度。

___

### <a id="getviewportleftcolumn" name="getviewportleftcolumn"></a> getViewportLeftColumn

▸ **getViewportLeftColumn**(`columnViewportIndex`): `number`

获取视口中左侧列的索引。

**`example`**
```
//此示例返回当前工作表视图中底部和顶部行以及左右列的索引。
var brow = activeSheet.getViewportBottomRow(1);
var lcol = activeSheet.getViewportLeftColumn(1);
var rcol = activeSheet.getViewportRightColumn(1);
var trow = activeSheet.getViewportTopRow(1);
alert(brow);
alert(lcol);
alert(rcol);
alert(trow);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnViewportIndex` | `number` | 视口索引。 |

#### Returns

`number`

视口中左侧列的索引。

___

### <a id="getviewportrightcolumn" name="getviewportrightcolumn"></a> getViewportRightColumn

▸ **getViewportRightColumn**(`columnViewportIndex`): `number`

获取视口中右侧列的索引。

**`example`**
```
//此示例返回当前工作表视图中底部和顶部行以及左右列的索引。
var brow = activeSheet.getViewportBottomRow(1);
var lcol = activeSheet.getViewportLeftColumn(1);
var rcol = activeSheet.getViewportRightColumn(1);
var trow = activeSheet.getViewportTopRow(1);
alert(brow);
alert(lcol);
alert(rcol);
alert(trow);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnViewportIndex` | `number` | 视口索引。 |

#### Returns

`number`

视口中右侧列的索引。

___

### <a id="getviewporttoprow" name="getviewporttoprow"></a> getViewportTopRow

▸ **getViewportTopRow**(`rowViewportIndex`): `number`

获取视口中顶部行的索引。

**`example`**
```
//此示例返回当前工作表视图中底部和顶部行以及左右列的索引。
var brow = activeSheet.getViewportBottomRow(1);
var lcol = activeSheet.getViewportLeftColumn(1);
var rcol = activeSheet.getViewportRightColumn(1);
var trow = activeSheet.getViewportTopRow(1);
alert(brow);
alert(lcol);
alert(rcol);
alert(trow);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rowViewportIndex` | `number` | 视口索引。 |

#### Returns

`number`

视口中顶部行的索引。

___

### <a id="getviewportwidth" name="getviewportwidth"></a> getViewportWidth

▸ **getViewportWidth**(`columnViewportIndex`): `number`

获取活动工作表指定视口列的宽度。

**`example`**
```
//此示例使用 getViewportWidth 方法。
alert(activeSheet.getViewportWidth(1));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnViewportIndex` | `number` | 列视口索引。 |

#### Returns

`number`

视口的宽度。

___

### <a id="groupsparkline" name="groupsparkline"></a> groupSparkline

▸ **groupSparkline**(`sparklines`): [`SparklineGroup`](GC.Spread.Sheets.Sparklines.SparklineGroup.md)

对迷你图进行分组。

**`example`**
```
//此示例对迷你图进行分组。
sheet.setValue(0, 0, "Data Range is A2-A9");
sheet.setValue(1, 0, 1);
sheet.setValue(2, 0, -2);
sheet.setValue(3, 0, -1);
sheet.setValue(4, 0, 6);
sheet.setValue(5, 0, 4);
sheet.setValue(6, 0, -4);
sheet.setValue(7, 0, 3);
sheet.setValue(8, 0, 8);
var data = new GC.Spread.Sheets.Range(1, 0, 8, 1);
var setting = new GC.Spread.Sheets.Sparklines.SparklineSetting();
var s1=  sheet.setSparkline(13, 0, data
        , GC.Spread.Sheets.Sparklines.DataOrientation.vertical
        , GC.Spread.Sheets.Sparklines.SparklineType.line
        , setting
        );
var s2 =sheet.setSparkline(13, 3, data
        , GC.Spread.Sheets.Sparklines.DataOrientation.vertical
        , GC.Spread.Sheets.Sparklines.SparklineType.column
        , setting
        );
var s3=  sheet.setSparkline(13, 6, data
        , GC.Spread.Sheets.Sparklines.DataOrientation.vertical
        , GC.Spread.Sheets.Sparklines.SparklineType.winloss
        , setting
        );
var group = sheet.groupSparkline([s1,s2,s3]);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sparklines` | [`Sparkline`](GC.Spread.Sheets.Sparklines.Sparkline.md)[] | 要分组的迷你图。 |

#### Returns

[`SparklineGroup`](GC.Spread.Sheets.Sparklines.SparklineGroup.md)

迷你图组。

___

### <a id="haspassword" name="haspassword"></a> hasPassword

▸ **hasPassword**(): `boolean`

获取工作表是否设置了保护密码。

**`example`**
```
let password = "fe4c4be8"
sheet.protect(password);
if(sheet.hasPassword()) {
    sheet.unprotect(password);
} else {
    sheet.unprotect();
}
```

#### Returns

`boolean`

如果设置了密码则返回 true，否则返回 false。

___

### <a id="haspendingchanges" name="haspendingchanges"></a> hasPendingChanges

▸ **hasPendingChanges**(): `boolean`

获取指定范围内是否存在脏数据、插入或删除状态。

#### Returns

`boolean`

如果范围内的任何行或单元格是脏数据，或者已被插入或删除，则返回 `true`；否则返回 `false`。

___

### <a id="hittest" name="hittest"></a> hitTest

▸ **hitTest**(`x`, `y`): [`IHitTestInformation`](../interfaces/GC.Spread.Sheets.IHitTestInformation.md)

执行点击测试。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | <i>x</i> 坐标。 |
| `y` | `number` | <i>y</i> 坐标。 |

#### Returns

[`IHitTestInformation`](../interfaces/GC.Spread.Sheets.IHitTestInformation.md)

点击测试信息。

___

### <a id="invalidatelayout" name="invalidatelayout"></a> invalidateLayout

▸ **invalidateLayout**(): `void`

使工作表布局失效。

**`example`**
```
//此示例更新布局。
activeSheet.columnOutlines.group(0, 1);
activeSheet.invalidateLayout();
activeSheet.repaint();
```

#### Returns

`void`

___

### <a id="isdirtysuspended" name="isdirtysuspended"></a> isDirtySuspended

▸ **isDirtySuspended**(): `boolean`

获取是否暂停记录脏数据。

**`example`**
```
//此示例使用 isDirtySuspended 方法。
var customers = [
               { ID: 0, Name: 'A', Info1: 'Info0' },
               { ID: 1, Name: 'B', Info1: 'Info1' },
               { ID: 2, Name: 'C', Info1: 'Info2' },
            ];
activeSheet.setDataSource(customers);
activeSheet.suspendDirty();
alert(activeSheet.isDirtySuspended());
activeSheet.resumeDirty();
alert(activeSheet.isDirtySuspended());
```

#### Returns

`boolean`

脏数据是否被暂停。

___

### <a id="isediting" name="isediting"></a> isEditing

▸ **isEditing**(): `boolean`

获取工作表是否处于编辑模式。

**`example`**
```
//此示例使用 isEditing 方法。
alert(activeSheet.isEditing());
```

#### Returns

`boolean`

如果工作表处于编辑模式则返回 `true`；否则返回 `false`。

___

### <a id="ispaintsuspended" name="ispaintsuspended"></a> isPaintSuspended

▸ **isPaintSuspended**(): `boolean`

获取工作表绘制是否已暂停。

#### Returns

`boolean`

___

### <a id="isprintlinevisible" name="isprintlinevisible"></a> isPrintLineVisible

▸ **isPrintLineVisible**(`value?`): `boolean`

获取或设置是否显示工作表的打印线。

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`boolean`

如果未设置值，则返回表示是否显示打印线的值

___

### <a id="isselected" name="isselected"></a> isSelected

▸ **isSelected**(`selectedState?`): `any`

获取或设置工作表的选择状态。

**`example`**
```
spread.sheets[0].isSelected();
spread.sheets[1].isSelected(true);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `selectedState?` | `boolean` |

#### Returns

`any`

如果未设置 selectedState，则返回工作表的选择状态；否则返回工作表。

___

### <a id="isvalid" name="isvalid"></a> isValid

▸ **isValid**(`row`, `column`, `value`): `boolean`

确定单元格值是否有效。

**`example`**
```
//此示例使用 isValid 方法。
alert(activeSheet.isValid(0, 0, 10));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `column` | `number` | 列索引。 |
| `value` | `Object` | 单元格值。 |

#### Returns

`boolean`

如果值有效则返回 `true`；否则返回 `false`。

___

### <a id="moveto" name="moveto"></a> moveTo

▸ **moveTo**(`fromRow`, `fromColumn`, `toRow`, `toColumn`, `rowCount`, `columnCount`, `option`): `void`

将数据从一个范围移动到另一个范围。

**`example`**
```
//此示例将数据移动到指定位置。
activeSheet.getCell(0,0).value("A1");
activeSheet.getCell(1,1).value("Test")
activeSheet.moveTo(0,0,3,3,2,2,GC.Spread.Sheets.CopyToOptions.value);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fromRow` | `number` | 源行。 |
| `fromColumn` | `number` | 源列。 |
| `toRow` | `number` | 目标行。 |
| `toColumn` | `number` | 目标列。 |
| `rowCount` | `number` | 行数。 |
| `columnCount` | `number` | 列数。 |
| `option` | [`CopyToOptions`](../enums/GC.Spread.Sheets.CopyToOptions.md) | 复制选项。 |

#### Returns

`void`

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置工作表的名称。

**`example`**
```
spread.sheets[0].name("第一个工作表");
spread.sheets[1].name("第二个工作表");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置值，则返回工作表名称；否则返回工作表。

___

### <a id="printinfo" name="printinfo"></a> printInfo

▸ **printInfo**(`value?`): `any`

获取或设置工作表的打印信息。

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`PrintInfo`](GC.Spread.Sheets.Print.PrintInfo.md) |

#### Returns

`any`

如果未设置值，则返回工作表的打印信息；否则返回工作表。

___

### <a id="protect" name="protect"></a> protect

▸ **protect**(`password?`): `void`

保护工作表。如果工作表已经被保护，则不执行任何操作。

**`example`**
```
let password = "fe4c4be8"
sheet.protect(password);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `password?` | `string` | 工作表保护密码。 |

#### Returns

`void`

___

### <a id="recalcall" name="recalcall"></a> recalcAll

▸ **recalcAll**(`refreshAll?`): `void`

重新计算工作表中的所有公式。

**`deprecated`** 自版本 16.2.0 起已弃用，请使用 'spread.calculate' 代替

**`example`**
```
//此示例使用 recalcAll 方法。
activeSheet.setValue(0,0,1);
activeSheet.setValue(0,1,2);
activeSheet.setValue(0,2,10);
activeSheet.getCell(1,1).formula("=SUM(A1:C1)");
activeSheet.recalcAll();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `refreshAll?` | `boolean` | 指定是否重建所有公式引用、自定义名称和自定义函数。 |

#### Returns

`void`

___

### <a id="removecustomfunction" name="removecustomfunction"></a> removeCustomFunction

▸ **removeCustomFunction**(`name`): `void`

移除自定义函数。

**`example`**
```
//此示例使用 removeCustomFunction 方法。
// 添加自定义函数
// 在单元格中输入 =myfunc(1)
// 查看结果
function myfunc() {}
myfunc.prototype = new GC.Spread.CalcEngine.Functions.Function("myfunc", 0, 0, {name: "myfunc",description: "This is my first function"});
myfunc.prototype.evaluate = function (args) {
    return 100;
}
activeSheet.addCustomFunction(new myfunc());
activeSheet.removeCustomFunction("myfunc");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |

#### Returns

`void`

___

### <a id="removecustomname" name="removecustomname"></a> removeCustomName

▸ **removeCustomName**(`name`): `void`

移除指定的自定义名称。

**`example`**
```
//此示例使用 removeCustomName 方法。
activeSheet.setValue(0, 0, 1);
activeSheet.setValue(0, 1, 2);
activeSheet.setValue(0, 2, 3);
activeSheet.addCustomName("customName1","=12", 0, 0);
activeSheet.addCustomName("customName2","Average(20,45)", 0, 0);
activeSheet.addCustomName("customName3", "=$A$1:$C$1", 0, 0);
activeSheet.setFormula(1, 0, "customName1");
activeSheet.setFormula(1, 1, "customName2");
activeSheet.setFormula(1, 2, "sum(customName3)");
//activeSheet.removeCustomName("customName3");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |

#### Returns

`void`

___

### <a id="removenamedstyle" name="removenamedstyle"></a> removeNamedStyle

▸ **removeNamedStyle**(`name`): `void`

从工作表的命名样式集合中移除具有指定名称的样式。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要移除的样式名称。 |

#### Returns

`void`

___

### <a id="removespan" name="removespan"></a> removeSpan

▸ **removeSpan**(`row`, `col`, `sheetArea?`): `void`

移除指定工作表区域中包含指定锚点单元格的跨度。

**`example`**
```
activeSheet.addSpan(0,0,3,3,GC.Spread.Sheets.SheetArea.viewport);
//activeSheet.removeSpan(0, 0, GC.Spread.Sheets.SheetArea.viewport);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 跨度锚点单元格的行索引（跨单元格开始的位置）。 |
| `col` | `number` | 跨度锚点单元格的列索引（跨单元格开始的位置）。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`void`

___

### <a id="removesparkline" name="removesparkline"></a> removeSparkline

▸ **removeSparkline**(`row`, `col`): `void`

移除指定单元格的迷你图。

**`example`**
```
//此示例移除一个迷你图。
var cellr = new GC.Spread.Sheets.Range(0, 0, 1, 5);
var ex = new GC.Spread.Sheets.Sparklines.SparklineSetting();
ex.options.SeriesColor  = "Aquamarine";
sheet.setValue(0, 0, 2);
sheet.setValue(0, 1, 5);
sheet.setValue(0, 2, 4);
sheet.setValue(0, 3, -1);
sheet.setValue(0, 4, 3);
sheet.setSparkline(0, 5, cellr, GC.Spread.Sheets.Sparklines.DataOrientation.horizontal, GC.Spread.Sheets.Sparklines.SparklineType.column, ex);
alert(sheet.getSparkline(0, 5).toString());
//sheet.removeSparkline(0, 5);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |

#### Returns

`void`

___

### <a id="repaint" name="repaint"></a> repaint

▸ **repaint**(`clipRect?`): `void`

重绘指定的矩形区域。

**`example`**
```
//此示例执行重绘操作。
var cellrange =new GC.Spread.Sheets.Range(0, 0, 5, 1);
var hideRowFilter =new GC.Spread.Sheets.Filter.HideRowFilter(cellrange);
sheet.rowFilter(hideRowFilter);
sheet.resumePaint();
sheet.repaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `clipRect?` | [`Rect`](GC.Spread.Sheets.Rect.md) | 要重绘的矩形区域。 |

#### Returns

`void`

___

### <a id="reset" name="reset"></a> reset

▸ **reset**(): `void`

重置工作表。

**`example`**
```
//此示例使用 reset 方法。
activeSheet.reset();
```

#### Returns

`void`

___

### <a id="resumecalcservice" name="resumecalcservice"></a> resumeCalcService

▸ **resumeCalcService**(`recalcAll?`): `void`

恢复计算服务。

**`example`**
```
//此示例使用 resumeCalcService 方法。
activeSheet.suspendCalcService(false);
activeSheet.setValue(0,0,1);
activeSheet.setValue(0,1,2);
activeSheet.setValue(0,2,10);
activeSheet.getCell(1,1).formula("=SUM(A1:C1)");
activeSheet.resumeCalcService(true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `recalcAll?` | `boolean` | 指定是否重新计算所有公式。 |

#### Returns

`void`

___

### <a id="resumedirty" name="resumedirty"></a> resumeDirty

▸ **resumeDirty**(): `void`

恢复记录脏数据。

**`example`**
```
//此示例使用 resumeDirty 方法。
 var customers = [
               { ID: 0, Name: 'A', Info1: 'Info0' },
               { ID: 1, Name: 'B', Info1: 'Info1' },
               { ID: 2, Name: 'C', Info1: 'Info2' },
            ];
activeSheet.setDataSource(customers);
activeSheet.suspendDirty();
alert(activeSheet.isDirtySuspended());
activeSheet.resumeDirty();
alert(activeSheet.isDirtySuspended());
```

#### Returns

`void`

___

### <a id="resumeevent" name="resumeevent"></a> resumeEvent

▸ **resumeEvent**(): `void`

恢复事件。

**`example`**
```
//此示例演示暂停和恢复事件。
 activeSheet.bind(GC.Spread.Sheets.Events.CellChanged, function (sender, args) {
    if (args.propertyName === "value") {
        alert(activeSheet.getValue(args.row, args.col));
    }
});
activeSheet.suspendEvent();
activeSheet.setValue(0, 0, "111");
activeSheet.resumeEvent();
activeSheet.setValue(1, 1, "222");
```

#### Returns

`void`

___

### <a id="resumepaint" name="resumepaint"></a> resumePaint

▸ **resumePaint**(): `void`

恢复绘制。

#### Returns

`void`

___

### <a id="rowfilter" name="rowfilter"></a> rowFilter

▸ **rowFilter**(`value?`): `any`

获取或设置工作表的行过滤器。

**`example`**
```
//此示例创建一个行过滤器。
sheet.rowFilter(new GC.Spread.Sheets.Filter.HideRowFilter(new GC.Spread.Sheets.Range(1,1,10,3)));
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`RowFilterBase`](GC.Spread.Sheets.Filter.RowFilterBase.md) |

#### Returns

`any`

不带参数调用方法时，将返回过滤器实例，否则返回工作表实例。

___

### <a id="scroll" name="scroll"></a> scroll

▸ **scroll**(`vPixels`, `hPixels`): `void`

按指定像素滚动工作表。
当vPixels为正数时，工作表将向下滚动；当vPixels为负数时，工作表将向上滚动；当vPixels为0时，工作表在垂直方向不会滚动。
当hPixels为正数时，工作表将向右滚动；当hPixels为负数时，工作表将向左滚动；当hPixels为0时，工作表在水平方向不会滚动。
当Workbook的选项scrollByPixel为true时，工作表将滚动到新的顶部行/左侧列索引和新的顶部行/左侧列偏移量；
当Workbook的选项scrollByPixel为false时，工作表将滚动到新的顶部行/左侧列索引，并且新的顶部行/左侧列偏移量将始终为0。

**`example`**
```
//此示例将工作表向下滚动10像素，向右滚动5像素。
activeSheet.scroll(10, 5);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `vPixels` | `number` | 垂直方向滚动的像素数。 |
| `hPixels` | `number` | 水平方向滚动的像素数。 |

#### Returns

`void`

___

### <a id="search" name="search"></a> search

▸ **search**(`searchCondition`): [`SearchResult`](GC.Spread.Sheets.Search.SearchResult.md)

搜索指定内容。

**`example`**
```
//此示例使用search方法。
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

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `searchCondition` | [`SearchCondition`](GC.Spread.Sheets.Search.SearchCondition.md) | 搜索条件。 |

#### Returns

[`SearchResult`](GC.Spread.Sheets.Search.SearchResult.md)

搜索结果。

___

### <a id="selectionpolicy" name="selectionpolicy"></a> selectionPolicy

▸ **selectionPolicy**(`value?`): `any`

获取或设置用户是否可以在工作表上选择项目范围。

**`example`**
```
//此示例使用selectionPolicy方法。
activeSheet.selectionUnit(GC.Spread.Sheets.SelectionUnit.row);
activeSheet.selectionPolicy(GC.Spread.Sheets.SelectionPolicy.range);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SelectionPolicy`](../enums/GC.Spread.Sheets.SelectionPolicy.md) |

#### Returns

`any`

如果未设置值，则返回选择策略设置；否则返回工作表。

___

### <a id="selectionunit" name="selectionunit"></a> selectionUnit

▸ **selectionUnit**(`value?`): `any`

获取或设置用户是否可以在工作表上选择单元格、行或列。

**`example`**
```
//此示例使用selectionUnit方法。
activeSheet.selectionUnit(GC.Spread.Sheets.SelectionUnit.row);
activeSheet.selectionPolicy(GC.Spread.Sheets.SelectionPolicy.range);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`SelectionUnit`](../enums/GC.Spread.Sheets.SelectionUnit.md) |

#### Returns

`any`

如果未设置值，则返回选择单位设置；否则返回工作表。

___

### <a id="setactivecell" name="setactivecell"></a> setActiveCell

▸ **setActiveCell**(`row`, `col`): `void`

设置此工作表的活动单元格。

**`example`**
```
//此示例设置活动单元格。
sheet.setActiveCell(5,5);
alert(sheet.getActiveColumnIndex());
alert(sheet.getActiveRowIndex());
spread.bind(GC.Spread.Sheets.Events.EnterCell, function (event, data) {
    alert(data.col);
    alert(data.row);
  });
spread.bind(GC.Spread.Sheets.Events.LeaveCell, function (event, data) {
    alert(data.col);
    alert(data.row);
  });
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 单元格的行索引。 |
| `col` | `number` | 单元格的列索引。 |

#### Returns

`void`

___

### <a id="setalttext" name="setalttext"></a> setAltText

▸ **setAltText**(`row`, `col`, `value`, `sheetArea?`): `void`

在指定的工作表区域中为指定单元格设置替代文本。

**`example`**
```
var SpreadIcon = {
    FolderOpen: '\ue685',
    InfoFilled: '\ue718',
    Library: '\ue69d',
    NotebookFilled: '\uD800\uDC0F',
    Browse: '\ue626'
};
activeSheet.setValue(1, 1, SpreadIcon.FolderOpen);
activeSheet.setAltText(1, 1, "Folder Open Icon");

// 除了纯文本外，替代文本还可以包含占位符 {value} 或 {formatted}，它们分别表示单元格值或单元格格式化值。
// 例如，如果单元格值为 1000，且替代文本为 "Sales amount is {value}"，则最终的可访问内容应为 "Sales amount is 1000"。
activeSheet.setValue(1, 1, 1000);
activeSheet.setAltText(1, 1, "Sales amount is {value}");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `value` | `string` | 要为指定单元格设置的替代文本。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | 工作表区域。如果未提供此参数，则默认为 `viewport`。 |

#### Returns

`void`

___

### <a id="setarray" name="setarray"></a> setArray

▸ **setArray**(`row`, `column`, `array`, `setFormula?`): `void`

将指定的二维对象数组中的值设置到此工作表上指定范围的单元格中。

**`example`**
```
//此示例使用 setArray 方法。
//设置值
var array = [[1,2,3],[4,5],[6,7,8,9]];
activeSheet.setArray(1, 2, array);
//设置公式
var array = [["=1+1","=2+2","=3+3"],["=4+4","=5+5"],["=6+6","=7+7","=8+8","=9+9"]];
activeSheet.setArray(1, 2, array, true);
//获取值
var newArray = activeSheet.getArray(1, 2, 3, 4);
//获取公式
var newArray = activeSheet.getArray(1, 2, 3, 4, true);
//alert(newArray[0]);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `column` | `number` | 列索引。 |
| `array` | `any`[] | 要从中设置值的数组。 |
| `setFormula?` | `boolean` | - |

#### Returns

`void`

___

### <a id="setarrayformula" name="setarrayformula"></a> setArrayFormula

▸ **setArrayFormula**(`row`, `col`, `rowCount`, `colCount`, `value`, `sheetArea?`): `void`

在指定的工作表区域中为指定单元格设置公式。

**`example`**
```
//此示例使用 setArrayFormula 方法。
activeSheet.getCell(1,1).value(3);
activeSheet.getCell(2,1).value(1);
activeSheet.getCell(3,1).value(3);
activeSheet.getCell(4,1).value(7);
activeSheet.getCell(1,2).value(7);
activeSheet.getCell(2,2).value(7);
activeSheet.getCell(3,2).value(7);
activeSheet.getCell(4,2).value(7);
spread.allowUserEditFormula(true);
activeSheet.setArrayFormula(0, 3, 4, 1, "B2:B5*C2:C5", GC.Spread.Sheets.SheetArea.viewport);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 起始行索引。 |
| `col` | `number` | 起始列索引。 |
| `rowCount` | `number` | 范围内的行数。 |
| `colCount` | `number` | 范围内的列数。 |
| `value` | `string` | 要放置在指定范围内的数组公式。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`void`

___

### <a id="setbindingpath" name="setbindingpath"></a> setBindingPath

▸ **setBindingPath**(`row`, `col`, `path`): [`Worksheet`](GC.Spread.Sheets.Worksheet.md)

在指定的工作表区域中为指定单元格设置单元格级绑定的绑定路径。

**`example`**
```
//此示例绑定一个单元格。
var test = {name: "John", gender: "male"};
sheet.setBindingPath(0, 0, "name");
sheet.setBindingPath(0, 1, "gender");
sheet.setDataSource(new GC.Spread.Sheets.Bindings.CellBindingSource(test));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `path` | `string` | 单元格绑定源的绑定路径。 |

#### Returns

[`Worksheet`](GC.Spread.Sheets.Worksheet.md)

___

### <a id="setcelltype" name="setcelltype"></a> setCellType

▸ **setCellType**(`row`, `col`, `value`, `sheetArea?`): `void`

设置单元格类型。

**`example`**
```
//此示例使用 setCellType 方法。
var cellType = new GC.Spread.Sheets.CellTypes.Button();
cellType.buttonBackColor("#FFFF00");
cellType.text("this is a button");
activeSheet.setCellType(1,1,cellType);
spread.bind(GC.Spread.Sheets.Events.ButtonClicked, function (e, args) {
    var sheet = args.sheet, row = args.row, col = args.col;
    var cellType = activeSheet.getCellType(row, col);
    if (cellType instanceof GC.Spread.Sheets.CellTypes.Button) {
        alert("Button Clicked");
    }
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `value` | [`Base`](GC.Spread.Sheets.CellTypes.Base.md) | 单元格类型。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`void`

___

### <a id="setcolumncount" name="setcolumncount"></a> setColumnCount

▸ **setColumnCount**(`colCount`, `sheetArea?`, `guardContent?`): `void`

设置指定工作表区域中的列数。

**`example`**
```
//此示例设置列数。
sheet.setRowCount(4,1);
sheet.setColumnCount(4,2);
sheet.addSpan(0,0,3,3,GC.Spread.Sheets.SheetArea.colHeader);
sheet.addSpan(0,0,3,3,GC.Spread.Sheets.SheetArea.rowHeader);
sheet.addSpan(0,0,3,3,GC.Spread.Sheets.SheetArea.viewport);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `colCount` | `number` | 列数。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |
| `guardContent?` | [`UsedRangeType`](../enums/GC.Spread.Sheets.UsedRangeType.md) | - |

#### Returns

`void`

___

### <a id="setcolumnpagebreak" name="setcolumnpagebreak"></a> setColumnPageBreak

▸ **setColumnPageBreak**(`column`, `value`): `void`

设置是否在打印时在指定列之前插入强制分页符。

**`example`**
```
//此示例设置分页符。
activeSheet.setColumnPageBreak(5, true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `column` | `number` | 列索引。 |
| `value` | `boolean` | 设置为 `true` 可在打印时在指定列之前插入强制分页符。 |

#### Returns

`void`

___

### <a id="setcolumnresizable" name="setcolumnresizable"></a> setColumnResizable

▸ **setColumnResizable**(`col`, `value`, `sheetArea?`): `void`

设置用户是否可以在指定工作表区域中调整指定列的大小。

**`example`**
```
//此示例设置 setColumnResizable 方法。
sheet.setRowResizable(3,false,GC.Spread.Sheets.SheetArea.viewport);
sheet.setColumnResizable(3,false,GC.Spread.Sheets.SheetArea.viewport);
sheet.getRange(1,-1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).resizable(false);
sheet.getRange(-1, 1, -1, 1, GC.Spread.Sheets.SheetArea.viewport).resizable(false);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `col` | `number` | 列索引。 |
| `value` | `boolean` | 设置为 `true` 允许用户调整列的大小。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`void`

___

### <a id="setcolumnvisible" name="setcolumnvisible"></a> setColumnVisible

▸ **setColumnVisible**(`col`, `value`, `sheetArea?`): `void`

设置指定工作表区域中的列是否显示。

**`example`**
```
//此示例设置指定列隐藏。
activeSheet.setColumnVisible(2,false,GC.Spread.Sheets.SheetArea.viewport);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `col` | `number` | 列索引。 |
| `value` | `boolean` | 是否显示该列。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`void`

___

### <a id="setcolumnwidth" name="setcolumnwidth"></a> setColumnWidth

▸ **setColumnWidth**(`col`, `value`, `sheetArea?`): `void`

设置指定工作表区域中指定列的宽度（以像素为单位）或动态大小。

**`example`**
```
//此示例设置列宽。
sheet.setValue(0, 0, "value");
sheet.addRows(0, 2);
sheet.addColumns(0, 2);
sheet.setRowHeight(0, 50.0, GC.Spread.Sheets.SheetArea.viewport);
sheet.setColumnWidth(0, 150.0, GC.Spread.Sheets.SheetArea.viewport);
sheet.setColumnWidth(1, "2*", GC.Spread.Sheets.SheetArea.viewport);
sheet.getRange(0, -1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).backColor("Gray");
sheet.getRange(-1, 0, -1, 1, GC.Spread.Sheets.SheetArea.viewport).backColor ("Brown");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `col` | `number` | 列索引。 |
| `value` | `string` \| `number` | 以像素为单位的宽度，或使用带"*"的字符串表示动态大小。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`void`

___

### <a id="setcsv" name="setcsv"></a> setCsv

▸ **setCsv**(`row`, `column`, `text`, `rowDelimiter`, `columnDelimiter`): `void`

在工作表中设置分隔文本（CSV）。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 起始行。 |
| `column` | `number` | 起始列。 |
| `text` | `string` | 分隔文本。 |
| `rowDelimiter` | `string` | 行分隔符。 |
| `columnDelimiter` | `string` | 列分隔符。 |

#### Returns

`void`

___

### <a id="setdatasource" name="setdatasource"></a> setDataSource

▸ **setDataSource**(`data`, `reset?`): `void`

设置填充工作表的数源。

**`example`**
```
var test = [
       { "Series0": 2, "Series1": 1 },
       { "Series0": 4, "Series1": 2 },
       { "Series0": 3, "Series1": 4 }
            ];
activeSheet.autoGenerateColumns = true;
activeSheet.setDataSource(test, true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `any` | 数据源。 |
| `reset?` | `boolean` | 如果工作表被重置则为 `true`；否则为 `false`。 |

#### Returns

`void`

___

### <a id="setdatavalidator" name="setdatavalidator"></a> setDataValidator

▸ **setDataValidator**(`row`, `col`, `value`, `sheetArea?`): `void`

设置单元格数据验证器。

**`example`**
```
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createListValidator("1,2,3");
dv.showInputMessage(true);
dv.inputMessage("Value must be 1,2 or 3");
dv.inputTitle("tip");
activeSheet.setDataValidator(1,1,dv,GC.Spread.Sheets.SheetArea.viewport);
alert(activeSheet.getDataValidator(1,1).getValidList(activeSheet,1,1));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `value` | [`DefaultDataValidator`](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md) | 数据验证器。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`void`

▸ **setDataValidator**(`row`, `col`, `rowCount`, `colCount`, `value`, `sheetArea?`): `void`

设置单元格数据验证器。

**`example`**
```
spread.options.highlightInvalidData = true;
var dv = GC.Spread.Sheets.DataValidation.createListValidator("1,2,3");
dv.showInputMessage(true);
dv.inputMessage("Value must be 1,2 or 3");
dv.inputTitle("tip");
activeSheet.setDataValidator(1,1,1,1,dv,GC.Spread.Sheets.SheetArea.viewport);
alert(activeSheet.getDataValidator(1,1).getValidList(activeSheet,1,1));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `rowCount` | `number` | 行数。 |
| `colCount` | `number` | 列数。 |
| `value` | [`DefaultDataValidator`](GC.Spread.Sheets.DataValidation.DefaultDataValidator.md) | 数据验证器。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`void`

___

### <a id="setdefaultstyle" name="setdefaultstyle"></a> setDefaultStyle

▸ **setDefaultStyle**(`style`, `sheetArea?`): `void`

设置工作表的默认样式信息。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 要设置的样式。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`void`

___

### <a id="setdefaultvalue" name="setdefaultvalue"></a> setDefaultValue

▸ **setDefaultValue**(`row`, `col`, `value`): `void`

设置单元格的默认值，可以是值数据或公式字符串。当单元格没有数据时生效。

**`example`**
```
sheet.setDefaultValue(0, 0, "name");
sheet.setDefaultValue(0, 1, "=A1");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `value` | `any` | 单元格的默认值。 |

#### Returns

`void`

___

### <a id="setformatter" name="setformatter"></a> setFormatter

▸ **setFormatter**(`row`, `col`, `value`, `sheetArea`): `void`

设置单元格格式化器。

**`example`**
```
//此示例为活动工作表设置格式对象。
activeSheet.setValue(2, 3, new Date(2011, 2, 9));
activeSheet.setFormatter(2,3,"M",GC.Spread.Sheets.SheetArea.viewport);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `value` | `string` \| [`FormatterBase`](GC.Spread.Formatter.FormatterBase.md) | 格式化器字符串或对象。 |
| `sheetArea` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | 工作表区域。如果未提供此参数，则默认为 `viewport`。 |

#### Returns

`void`

___

### <a id="setformula" name="setformula"></a> setFormula

▸ **setFormula**(`row`, `col`, `value`, `sheetArea?`): `void`

在指定工作表区域的指定单元格中设置公式。

**`example`**
```
//此示例为指定单元格设置公式。
activeSheet.setValue(0, 2, 3);
activeSheet.setFormula(1, 1, "C1+D1");

// 此示例清除指定单元格中的公式。
activeSheet.setFormula(1, 1, null);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `value` | ``null`` \| `string` | 要放置在指定单元格中的公式。如果为 null, 这会清除单元格中的公式。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`void`

___

### <a id="sethyperlink" name="sethyperlink"></a> setHyperlink

▸ **setHyperlink**(`row`, `col`, `value`, `sheetArea?`): `void`

在指定工作表区域的指定单元格中设置超链接数据。

**`example`**
```
//此示例使用 setHyperlink 方法。
sheet.setHyperlink(0, 2, {
    url: 'https://www.spreadjs.com',
    tooltip: 'spreadjs',
    linkColor: 'blue',
    visitedLinkColor: 'red',
    target: GC.Spread.Sheets.Hyperlink.HyperlinkTargetType.blank,
    command: 'navigationLeft'
});
sheet.setValue(0,2, 'spreadjs');
sheet.setHyperlink(1, 1, {
    url: 'https://www.spreadjs.com',
    tooltip: 'spreadjs',
    target: GC.Spread.Sheets.Hyperlink.HyperlinkTargetType.top,
    command: function () { console.log('Only show this message when click the hyperlink.') }
});
sheet.setValue(1,1, 'spreadjs');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `value` | [`IHyperlink`](../interfaces/GC.Spread.Sheets.IHyperlink.md) | 要为指定单元格设置的超链接数据。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | 工作表区域。如果未提供此参数，则默认为 `viewport`。 |

#### Returns

`void`

___

### <a id="setrowcount" name="setrowcount"></a> setRowCount

▸ **setRowCount**(`rowCount`, `sheetArea?`, `guardContent?`): `void`

在指定的工作表区域中设置行数。

**`example`**
```
//此示例设置行数。
sheet.setRowCount(4,1);
sheet.setColumnCount(4,2);
sheet.addSpan(0,0,3,3,GC.Spread.Sheets.SheetArea.colHeader);
sheet.addSpan(0,0,3,3,GC.Spread.Sheets.SheetArea.rowHeader);
sheet.addSpan(0,0,3,3,GC.Spread.Sheets.SheetArea.viewport);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rowCount` | `number` | 行数。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |
| `guardContent?` | [`UsedRangeType`](../enums/GC.Spread.Sheets.UsedRangeType.md) | - |

#### Returns

`void`

___

### <a id="setrowheight" name="setrowheight"></a> setRowHeight

▸ **setRowHeight**(`row`, `value`, `sheetArea?`): `void`

在指定的工作表区域中设置指定行的高度（以像素为单位）或动态大小。

**`example`**
```
//此示例设置行高。
sheet.setValue(0, 0, "value");
sheet.addRows(0, 2);
sheet.addColumns(0, 2);
sheet.setRowHeight(0, 50.0, GC.Spread.Sheets.SheetArea.viewport);
sheet.setRowHeight(1, "3*", GC.Spread.Sheets.SheetArea.viewport);
sheet.setColumnWidth(0, 150.0, GC.Spread.Sheets.SheetArea.viewport);
sheet.getRange(0, -1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).backColor("Gray");
sheet.getRange(-1, 0, -1, 1, GC.Spread.Sheets.SheetArea.viewport).backColor ("Brown");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `value` | `string` \| `number` | 以像素为单位的高度，或使用带"*"的字符串表示动态大小。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`void`

___

### <a id="setrowpagebreak" name="setrowpagebreak"></a> setRowPageBreak

▸ **setRowPageBreak**(`row`, `value`): `void`

设置是否在打印时在此工作表的指定行之前插入强制分页符。

**`example`**
```
activeSheet.setRowPageBreak(3, true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `value` | `boolean` | 设置为 `true` 可在打印时在此工作表的指定行之前插入强制分页符。 |

#### Returns

`void`

___

### <a id="setrowresizable" name="setrowresizable"></a> setRowResizable

▸ **setRowResizable**(`row`, `value`, `sheetArea?`): `void`

设置用户是否可以在指定的工作表区域中调整指定行的大小。

**`example`**
```
//此示例禁止调整某些行和列的大小。
sheet.setRowResizable(3,false,GC.Spread.Sheets.SheetArea.viewport);
sheet.setColumnResizable(3,false,GC.Spread.Sheets.SheetArea.viewport);
sheet.getRange(1,-1, 1, -1, GC.Spread.Sheets.SheetArea.viewport).resizable(false);
sheet.getRange(-1, 1, -1, 1, GC.Spread.Sheets.SheetArea.viewport).resizable(false);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `value` | `boolean` | 设置为 `true` 允许用户调整指定行的大小。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`void`

___

### <a id="setrowvisible" name="setrowvisible"></a> setRowVisible

▸ **setRowVisible**(`row`, `value`, `sheetArea?`): `void`

设置控件是否在指定的工作表区域中显示指定的行。

**`example`**
```
//此示例将指定行设置为隐藏。
activeSheet.setRowVisible(1,false,GC.Spread.Sheets.SheetArea.viewport);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `value` | `boolean` | 设置为 `true` 可显示指定的行。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`void`

___

### <a id="setselection" name="setselection"></a> setSelection

▸ **setSelection**(`row`, `column`, `rowCount`, `columnCount`): `void`

设置单元格或范围的选中状态，并将活动单元格设置为第一个单元格。

**`example`**
```
//此示例选择了一个单元格范围。
sheet.setValue(0,0, 1,3);
sheet.setValue(1,0, 50,3);
sheet.setValue(2,0, 100,3);
sheet.setValue(3,0, 2,3);
sheet.setValue(4,0, 60,3);
sheet.setValue(5,0, 90,3);
sheet.setValue(6,0, 3,3);
sheet.setValue(7,0, 40,3);
sheet.setValue(8,0, 70,3);
sheet.setValue(9,0, 5,3);
sheet.setValue(10,0, 35,3);
sheet.setSelection(0,0,11,1);
sheet.conditionalFormats.add3ScaleRule(1, 10, "red", 0, 50, "blue",2, 100, "yellow", sheet.getSelections());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 要添加的第一个单元格的行索引。 |
| `column` | `number` | 要添加的第一个单元格的列索引。 |
| `rowCount` | `number` | 要添加的行数。 |
| `columnCount` | `number` | 要添加的列数。 |

#### Returns

`void`

___

### <a id="setsparkline" name="setsparkline"></a> setSparkline

▸ **setSparkline**(`row`, `col`, `dataRange`, `dataOrientation`, `sparklineType`, `sparklineSetting`, `dateAxisRange?`, `dateAxisOrientation?`): [`Sparkline`](GC.Spread.Sheets.Sparklines.Sparkline.md)

为单元格设置迷你图。

**`example`**
```
//此示例为指定范围创建迷你图。
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
setting.options.axisColor ="Text 1 1";
sheet.addSpan(13, 0, 4, 3, null);
sheet.setSparkline(13, 0, data, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
sheet.setValue(1, 0, 1);
sheet.setValue(2, 0, -2);
sheet.setValue(3, 0, -1);
sheet.setValue(4, 0, 6);
sheet.setValue(5, 0, 4);
sheet.setValue(6, 0, -4);
sheet.setValue(7, 0, 3);
sheet.setValue(8, 0, 8);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `dataRange` | `string` \| [`Range`](GC.Spread.Sheets.Range.md) | 数据范围。 |
| `dataOrientation` | [`DataOrientation`](../enums/GC.Spread.Sheets.Sparklines.DataOrientation.md) | 数据方向。 |
| `sparklineType` | [`SparklineType`](../enums/GC.Spread.Sheets.Sparklines.SparklineType.md) | 迷你图类型。 |
| `sparklineSetting` | [`SparklineSetting`](GC.Spread.Sheets.Sparklines.SparklineSetting.md) | 迷你图设置。 |
| `dateAxisRange?` | `string` \| [`Range`](GC.Spread.Sheets.Range.md) | 日期轴范围。 |
| `dateAxisOrientation?` | [`DataOrientation`](../enums/GC.Spread.Sheets.Sparklines.DataOrientation.md) | 日期轴范围方向。 |

#### Returns

[`Sparkline`](GC.Spread.Sheets.Sparklines.Sparkline.md)

迷你图。

___

### <a id="setstyle" name="setstyle"></a> setStyle

▸ **setStyle**(`row`, `col`, `value`, `sheetArea?`): `void`

在指定的工作表区域中设置指定单元格的样式信息。

**`example`**
```
//此示例使用 setStyle 方法。
var style = new GC.Spread.Sheets.Style();
style.backColor = "lightgreen";
style.backgroundImage = "./css/images/quarter1.png";
activeSheet.setStyle(1,1,style,GC.Spread.Sheets.SheetArea.viewport);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | - |
| `value` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格样式。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`void`

___

### <a id="setstylename" name="setstylename"></a> setStyleName

▸ **setStyleName**(`row`, `column`, `value`, `sheetArea?`): `void`

在指定的工作表区域中为指定单元格设置指定的样式名称。

**`example`**
```
var namedStyle = new GC.Spread.Sheets.Style();
namedStyle.name = "style1";
namedStyle.backColor = "green";
activeSheet.addNamedStyle(namedStyle);
activeSheet.setStyleName(1, 1, "style1"); // 单元格(1,1)的背景色为绿色。
activeSheet.setStyleName(2, 1, "style1");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `column` | `number` | 列索引。 |
| `value` | `string` | 要设置的样式名称。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`void`

___

### <a id="settag" name="settag"></a> setTag

▸ **setTag**(`row`, `col`, `tag`, `sheetArea?`): `void`

在指定的工作表区域中为指定单元格设置标签值。

**`example`**
```
activeSheet.setTag(1,1,"test");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `tag` | `any` | 要为指定单元格设置的标签值。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | 不包含角落的工作表区域。如果未提供此参数，则默认为 `viewport`。 |

#### Returns

`void`

___

### <a id="settext" name="settext"></a> setText

▸ **setText**(`row`, `col`, `value`, `sheetArea?`): `void`

在指定的工作表区域中设置单元格的格式化文本。

**`example`**
```
activeSheet.setText(1, 0, "10");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `value` | `string` | 指定单元格的文本。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`void`

___

### <a id="setvalue" name="setvalue"></a> setValue

▸ **setValue**(`row`, `col`, `value`, `sheetArea?`, `ignoreRecalc?`): `void`

在指定的工作表区域中设置指定单元格的值。

**`example`**
```
//此示例使用 setValue 方法。
sheet.setValue(0,2,"ColumnHeader", GC.Spread.Sheets.SheetArea.colHeader);
sheet.setValue(2,0,{richText:[{style:{font:'bold 24px Arial'},text:'SpreadJS'}]}, GC.Spread.Sheets.SheetArea.rowHeader);
sheet.setValue(1, 1, {richText:[{style:{vertAlign: GC.Spread.Sheets.VertAlign.subscript},text:'SpreadJS'}]}, GC.Spread.Sheets.SheetArea.viewport);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `value` | `any` | 要为指定单元格设置的值。如果值是富文本格式，则应包含一个类型为富文本样式数组的 richText 字段。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |
| `ignoreRecalc?` | `boolean` | 是否忽略重新计算。 |

#### Returns

`void`

___

### <a id="showcell" name="showcell"></a> showCell

▸ **showCell**(`row`, `col`, `verticalPosition`, `horizontalPosition`): `void`

将单元格视图移动到视口中的指定位置。

**`example`**
```
//此示例使用 showCell 方法。
//将单元格(3,3)设置为活动单元格
activeSheet.setActiveCell(3, 3);
//在左上角显示活动单元格
activeSheet.showCell(3, 3, GC.Spread.Sheets.VerticalPosition.top, GC.Spread.Sheets.HorizontalPosition.left);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `verticalPosition` | [`VerticalPosition`](../enums/GC.Spread.Sheets.VerticalPosition.md) | 显示单元格的垂直位置。 |
| `horizontalPosition` | [`HorizontalPosition`](../enums/GC.Spread.Sheets.HorizontalPosition.md) | 显示单元格的水平位置。 |

#### Returns

`void`

___

### <a id="showcolumn" name="showcolumn"></a> showColumn

▸ **showColumn**(`col`, `horizontalPosition`): `void`

将列视图移动到视口中的指定位置。

**`example`**
```
activeSheet.showColumn(9, GC.Spread.Sheets.HorizontalPosition.left);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `col` | `number` | 列索引。 |
| `horizontalPosition` | [`HorizontalPosition`](../enums/GC.Spread.Sheets.HorizontalPosition.md) | 显示列的水平位置。 |

#### Returns

`void`

___

### <a id="showcolumnoutline" name="showcolumnoutline"></a> showColumnOutline

▸ **showColumnOutline**(`value?`): `any`

获取或设置列大纲（范围组）是否可见。

**`example`**
```
//此示例使用 showColumnOutline 方法。
activeSheet.showColumnOutline(false);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否显示列大纲。 |

#### Returns

`any`

如果未设置值，则返回一个指示此工作表上是否显示列大纲的值；否则返回工作表。

___

### <a id="showrow" name="showrow"></a> showRow

▸ **showRow**(`row`, `verticalPosition`): `void`

将行视图移动到视口中的指定位置。

**`example`**
```
activeSheet.showRow(9, GC.Spread.Sheets.VerticalPosition.top);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `verticalPosition` | [`VerticalPosition`](../enums/GC.Spread.Sheets.VerticalPosition.md) | 显示行的垂直位置。 |

#### Returns

`void`

___

### <a id="showrowoutline" name="showrowoutline"></a> showRowOutline

▸ **showRowOutline**(`value?`): `any`

获取或设置行大纲（范围组）是否可见。

**`example`**
```
//此示例使用 showRowOutline 方法。
activeSheet.showRowOutline(false);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否显示行大纲。 |

#### Returns

`any`

如果未设置值，则返回一个指示此工作表上是否显示行大纲的值；否则返回工作表。

___

### <a id="sortrange" name="sortrange"></a> sortRange

▸ **sortRange**(`row`, `column`, `rowCount`, `columnCount`, `byRows`, `sortInfo`, `sortOption?`): `boolean`

在数据模型中对此工作表中的单元格范围进行排序。

**`example`**
```
//此示例对范围进行排序。
sheet.setValue(0,0,"112");
sheet.setValue(1,0,"10");
sheet.setValue(2,0,"223");
sheet.setValue(3,0,"20");
sheet.setValue(4,0,"334");
sheet.setValue(5,0,"30");
function pinyinCompare (obj1, obj2) {
    return obj1.toString().localeCompare(obj2.toString(), 'zh');
}
sheet.sortRange(0, 0, 6, 1, true, [
                {index:0, ascending:true, compareFunction: pinyinCompare}
                ], {groupSort: GC.Spread.Sheets.GroupSort.full, ignoreHidden: true});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 要排序的单元格块的起始行索引。 |
| `column` | `number` | 要排序的单元格块的起始列索引。 |
| `rowCount` | `number` | 单元格块中的行数。 |
| `columnCount` | `number` | 单元格块中的列数。 |
| `byRows` | `boolean` | 设置为 `true` 表示按行排序，`false` 表示按列排序。 |
| `sortInfo` | ([`IValueSortInfo`](../interfaces/GC.Spread.Sheets.IValueSortInfo.md) \| [`ICellColorSortInfo`](../interfaces/GC.Spread.Sheets.ICellColorSortInfo.md) \| [`IFontColorSortInfo`](../interfaces/GC.Spread.Sheets.IFontColorSortInfo.md) \| [`ICustomSortInfo`](../interfaces/GC.Spread.Sheets.ICustomSortInfo.md))[] | 包含排序条件和执行排序信息的 SortInfo 对象。例如，[{index:0,ascending:true}] |
| `sortOption?` | [`ISortOptions`](../interfaces/GC.Spread.Sheets.ISortOptions.md) | sortOption 指示排序的详细性能。 |

#### Returns

`boolean`

如果数据排序成功则返回 `true`；否则返回 `false`。

___

### <a id="startedit" name="startedit"></a> startEdit

▸ **startEdit**(`selectAll?`, `defaultText?`): `void`

开始编辑单元格。

**`example`**
```
//此示例使用 startEdit 方法。
activeSheet.setActiveCell(5,5);
activeSheet.startEdit(true, "Test");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selectAll?` | `boolean` | 设置为 `true` 可选择单元格中的所有文本。 |
| `defaultText?` | `string` | 编辑单元格时显示的默认文本。 |

#### Returns

`void`

___

### <a id="suspendcalcservice" name="suspendcalcservice"></a> suspendCalcService

▸ **suspendCalcService**(`ignoreDirty?`): `void`

暂停计算服务。

**`example`**
```
//此示例使用 suspendCalcService 方法。
activeSheet.suspendCalcService(false);
activeSheet.setValue(0,0,1);
activeSheet.setValue(0,1,2);
activeSheet.setValue(0,2,10);
activeSheet.getCell(1,1).formula("=SUM(A1:C1)");
activeSheet.resumeCalcService(true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ignoreDirty?` | `boolean` | 指定是否使依赖单元格失效。 |

#### Returns

`void`

___

### <a id="suspenddirty" name="suspenddirty"></a> suspendDirty

▸ **suspendDirty**(): `void`

暂停记录脏数据。

**`example`**
```
//此示例使用 suspendDirty 方法。
 var customers = [
               { ID: 0, Name: 'A', Info1: 'Info0' },
               { ID: 1, Name: 'B', Info1: 'Info1' },
               { ID: 2, Name: 'C', Info1: 'Info2' },
            ];
activeSheet.setDataSource(customers);
activeSheet.suspendDirty();
alert(activeSheet.isDirtySuspended());
activeSheet.resumeDirty();
alert(activeSheet.isDirtySuspended());
```

#### Returns

`void`

___

### <a id="suspendevent" name="suspendevent"></a> suspendEvent

▸ **suspendEvent**(): `void`

暂停事件。

**`example`**
```
//此示例暂停并恢复事件。
activeSheet.bind(GC.Spread.Sheets.Events.CellChanged, function (sender, args) {
    if (args.propertyName === "value") {
        alert(activeSheet.getValue(args.row, args.col));
    }
});
activeSheet.suspendEvent();
activeSheet.setValue(0, 0, "111");
activeSheet.resumeEvent();
activeSheet.setValue(1, 1, "222");
```

#### Returns

`void`

___

### <a id="suspendpaint" name="suspendpaint"></a> suspendPaint

▸ **suspendPaint**(): `void`

暂停绘制。

#### Returns

`void`

___

### <a id="tag" name="tag"></a> tag

▸ **tag**(`value?`): `any`

获取或设置当前工作表的标签值。

**`example`**
```
//此示例设置工作表标签。
activeSheet.tag("test");
alert(activeSheet.tag());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `any` | 要设置的标签值。 |

#### Returns

`any`

如果未设置值，则返回当前工作表的标签值；否则返回工作表。

___

### <a id="tojson" name="tojson"></a> toJSON

▸ **toJSON**(`serializationOption?`): `Object`

将对象状态保存为 JSON 字符串。

**`example`**
```
//此示例使用 toJSON 方法。
activeSheet.getCell(0,0).value(123);
var jsonStr = null;
//导出
jsonStr = JSON.stringify(activeSheet.toJSON());
//导入
activeSheet.fromJSON(JSON.parse(jsonStr));
alert(jsonStr);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `serializationOption?` | `Object` | 序列化选项，包含 <i>includeBindingSource</i> 参数。有关更多信息，请参阅备注。 |

#### Returns

`Object`

工作表数据。

___

### <a id="unbind" name="unbind"></a> unbind

▸ **unbind**(`type`, `fn?`): `void`

移除工作表的事件绑定。

**`example`**
```
//此示例在设置第一个值后移除事件绑定。
activeSheet.bind(GC.Spread.Sheets.Events.CellChanged, function (sender, args) {
    if (args.propertyName === "value") {
        alert(activeSheet.getValue(args.row, args.col));
    }
});
activeSheet.setValue(0, 0, "111");
activeSheet.unbind(GC.Spread.Sheets.Events.CellChanged);
activeSheet.setValue(1, 0, "222");
activeSheet.setValue(2, 0, "333");
activeSheet.setValue(3, 0, "444");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `string` | 事件类型。 |
| `fn?` | `Function` | 指定要移除绑定的函数。 |

#### Returns

`void`

___

### <a id="unbindall" name="unbindall"></a> unbindAll

▸ **unbindAll**(): `void`

移除工作表的所有事件绑定。

**`example`**
```
//此示例取消所有事件的监控。
activeSheet.bind(GC.Spread.Sheets.Events.CellChanged, function (sender, args) {
    if (args.propertyName === "value") {
        alert(activeSheet.getValue(args.row, args.col));
    }
});
activeSheet.setValue(0, 0, "111");
activeSheet.unbindAll(); //取消所有事件的监控。
activeSheet.setValue(1, 0, "222");
activeSheet.setValue(2, 0, "333");
activeSheet.setValue(3, 0, "444");
```

#### Returns

`void`

___

### <a id="ungroupsparkline" name="ungroupsparkline"></a> ungroupSparkline

▸ **ungroupSparkline**(`group`): `void`

取消指定组中迷你图的组合。

**`example`**
```
//此示例使用 ungroupSparkline 方法。
activeSheet.setValue(0, 0, "数据范围是 A2-A9");
activeSheet.setValue(1, 0, 1);
activeSheet.setValue(2, 0, -2);
activeSheet.setValue(3, 0, -1);
activeSheet.setValue(4, 0, 6);
activeSheet.setValue(5, 0, 4);
activeSheet.setValue(6, 0, -4);
activeSheet.setValue(7, 0, 3);
activeSheet.setValue(8, 0, 8);
var data = new GC.Spread.Sheets.Range(1, 0, 8, 1);
var setting = new GC.Spread.Sheets.Sparklines.SparklineSetting();
var s1=  activeSheet.setSparkline(11, 0, data, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
var s2 =activeSheet.setSparkline(11, 3, data, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.column, setting);
var s3=  activeSheet.setSparkline(11, 6, data, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.winloss, setting);
var group = activeSheet.groupSparkline([s1,s2,s3]);
//activeSheet.ungroupSparkline(group);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `group` | [`SparklineGroup`](GC.Spread.Sheets.Sparklines.SparklineGroup.md) | 迷你图组。 |

#### Returns

`void`

___

### <a id="unprotect" name="unprotect"></a> unprotect

▸ **unprotect**(`password?`): `boolean`

取消工作表的保护。

**`example`**
```
let password = "fe4c4be8"
sheet.protect(password);
sheet.unprotect(password);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `password?` | `string` | 工作表保护密码。 |

#### Returns

`boolean`

如果密码正确或 isProtect 为 false，则返回 true，否则返回 false。

___

### <a id="visible" name="visible"></a> visible

▸ **visible**(`value?`): `any`

设置工作表是否显示。

**`example`**
```
activeSheet.visible(false);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` \| [`SheetTabVisible`](../enums/GC.Spread.Sheets.SheetTabVisible.md) |

#### Returns

`any`

如果不带参数调用此函数，则返回一个布尔值，指示工作表是否可见；
否则返回当前工作表对象。

___

### <a id="zoom" name="zoom"></a> zoom

▸ **zoom**(`factor?`): `any`

获取或设置工作表的缩放因子。

**`example`**
```
//此示例缩放工作表。
spread.options.allowUserZoom = false;
sheet.zoom(3);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `factor?` | `number` |

#### Returns

`any`

如果未设置值，则返回缩放因子；否则返回工作表。
