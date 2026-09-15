# Class: Workbook

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).Workbook

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Workbook.md#constructor)

### Properties

- [contextMenu](GC.Spread.Sheets.Workbook.md#contextmenu)
- [customPivotTableThemes](GC.Spread.Sheets.Workbook.md#custompivottablethemes)
- [customSlicerThemes](GC.Spread.Sheets.Workbook.md#customslicerthemes)
- [customTableThemes](GC.Spread.Sheets.Workbook.md#customtablethemes)
- [customTimelineThemes](GC.Spread.Sheets.Workbook.md#customtimelinethemes)
- [docProps](GC.Spread.Sheets.Workbook.md#docprops)
- [name](GC.Spread.Sheets.Workbook.md#name)
- [options](GC.Spread.Sheets.Workbook.md#options)
- [sheetTabStyles](GC.Spread.Sheets.Workbook.md#sheettabstyles)
- [sheets](GC.Spread.Sheets.Workbook.md#sheets)
- [touchToolStrip](GC.Spread.Sheets.Workbook.md#touchtoolstrip)

### Methods

- [addCustomFunction](GC.Spread.Sheets.Workbook.md#addcustomfunction)
- [addCustomName](GC.Spread.Sheets.Workbook.md#addcustomname)
- [addNamedStyle](GC.Spread.Sheets.Workbook.md#addnamedstyle)
- [addSheet](GC.Spread.Sheets.Workbook.md#addsheet)
- [addSheetTab](GC.Spread.Sheets.Workbook.md#addsheettab)
- [addSparklineEx](GC.Spread.Sheets.Workbook.md#addsparklineex)
- [bind](GC.Spread.Sheets.Workbook.md#bind)
- [calculate](GC.Spread.Sheets.Workbook.md#calculate)
- [changeSheetIndex](GC.Spread.Sheets.Workbook.md#changesheetindex)
- [changeSheetPosition](GC.Spread.Sheets.Workbook.md#changesheetposition)
- [clearCustomFunctions](GC.Spread.Sheets.Workbook.md#clearcustomfunctions)
- [clearCustomNames](GC.Spread.Sheets.Workbook.md#clearcustomnames)
- [clearSheetTabs](GC.Spread.Sheets.Workbook.md#clearsheettabs)
- [clearSheets](GC.Spread.Sheets.Workbook.md#clearsheets)
- [commandManager](GC.Spread.Sheets.Workbook.md#commandmanager)
- [dataManager](GC.Spread.Sheets.Workbook.md#datamanager)
- [defaultPivotTableTheme](GC.Spread.Sheets.Workbook.md#defaultpivottabletheme)
- [defaultSlicerTheme](GC.Spread.Sheets.Workbook.md#defaultslicertheme)
- [defaultTableTheme](GC.Spread.Sheets.Workbook.md#defaulttabletheme)
- [defaultTimelineTheme](GC.Spread.Sheets.Workbook.md#defaulttimelinetheme)
- [destroy](GC.Spread.Sheets.Workbook.md#destroy)
- [export](GC.Spread.Sheets.Workbook.md#export)
- [focus](GC.Spread.Sheets.Workbook.md#focus)
- [fromJSON](GC.Spread.Sheets.Workbook.md#fromjson)
- [getActiveSheet](GC.Spread.Sheets.Workbook.md#getactivesheet)
- [getActiveSheetIndex](GC.Spread.Sheets.Workbook.md#getactivesheetindex)
- [getActiveSheetTab](GC.Spread.Sheets.Workbook.md#getactivesheettab)
- [getActiveSheetTabIndex](GC.Spread.Sheets.Workbook.md#getactivesheettabindex)
- [getCircularReference](GC.Spread.Sheets.Workbook.md#getcircularreference)
- [getCustomFunction](GC.Spread.Sheets.Workbook.md#getcustomfunction)
- [getCustomName](GC.Spread.Sheets.Workbook.md#getcustomname)
- [getCustomNames](GC.Spread.Sheets.Workbook.md#getcustomnames)
- [getExternalReferences](GC.Spread.Sheets.Workbook.md#getexternalreferences)
- [getHost](GC.Spread.Sheets.Workbook.md#gethost)
- [getNamedStyle](GC.Spread.Sheets.Workbook.md#getnamedstyle)
- [getNamedStyles](GC.Spread.Sheets.Workbook.md#getnamedstyles)
- [getSheet](GC.Spread.Sheets.Workbook.md#getsheet)
- [getSheetCount](GC.Spread.Sheets.Workbook.md#getsheetcount)
- [getSheetFromName](GC.Spread.Sheets.Workbook.md#getsheetfromname)
- [getSheetIndex](GC.Spread.Sheets.Workbook.md#getsheetindex)
- [getSheetPosition](GC.Spread.Sheets.Workbook.md#getsheetposition)
- [getSheetTab](GC.Spread.Sheets.Workbook.md#getsheettab)
- [getSheetTabCount](GC.Spread.Sheets.Workbook.md#getsheettabcount)
- [getSheetTabIndex](GC.Spread.Sheets.Workbook.md#getsheettabindex)
- [hitTest](GC.Spread.Sheets.Workbook.md#hittest)
- [import](GC.Spread.Sheets.Workbook.md#import)
- [invalidateLayout](GC.Spread.Sheets.Workbook.md#invalidatelayout)
- [isPaintSuspended](GC.Spread.Sheets.Workbook.md#ispaintsuspended)
- [nextControl](GC.Spread.Sheets.Workbook.md#nextcontrol)
- [open](GC.Spread.Sheets.Workbook.md#open)
- [pageInfo](GC.Spread.Sheets.Workbook.md#pageinfo)
- [previousControl](GC.Spread.Sheets.Workbook.md#previouscontrol)
- [print](GC.Spread.Sheets.Workbook.md#print)
- [refresh](GC.Spread.Sheets.Workbook.md#refresh)
- [removeCustomFunction](GC.Spread.Sheets.Workbook.md#removecustomfunction)
- [removeCustomName](GC.Spread.Sheets.Workbook.md#removecustomname)
- [removeNamedStyle](GC.Spread.Sheets.Workbook.md#removenamedstyle)
- [removeSheet](GC.Spread.Sheets.Workbook.md#removesheet)
- [removeSheetTab](GC.Spread.Sheets.Workbook.md#removesheettab)
- [removeSparklineEx](GC.Spread.Sheets.Workbook.md#removesparklineex)
- [repaint](GC.Spread.Sheets.Workbook.md#repaint)
- [resumeCalcService](GC.Spread.Sheets.Workbook.md#resumecalcservice)
- [resumeEvent](GC.Spread.Sheets.Workbook.md#resumeevent)
- [resumePaint](GC.Spread.Sheets.Workbook.md#resumepaint)
- [save](GC.Spread.Sheets.Workbook.md#save)
- [savePDF](GC.Spread.Sheets.Workbook.md#savepdf)
- [search](GC.Spread.Sheets.Workbook.md#search)
- [setActiveSheet](GC.Spread.Sheets.Workbook.md#setactivesheet)
- [setActiveSheetIndex](GC.Spread.Sheets.Workbook.md#setactivesheetindex)
- [setActiveSheetTab](GC.Spread.Sheets.Workbook.md#setactivesheettab)
- [setSheetCount](GC.Spread.Sheets.Workbook.md#setsheetcount)
- [startSheetIndex](GC.Spread.Sheets.Workbook.md#startsheetindex)
- [suspendCalcService](GC.Spread.Sheets.Workbook.md#suspendcalcservice)
- [suspendEvent](GC.Spread.Sheets.Workbook.md#suspendevent)
- [suspendPaint](GC.Spread.Sheets.Workbook.md#suspendpaint)
- [toJSON](GC.Spread.Sheets.Workbook.md#tojson)
- [unbind](GC.Spread.Sheets.Workbook.md#unbind)
- [unbindAll](GC.Spread.Sheets.Workbook.md#unbindall)
- [undoManager](GC.Spread.Sheets.Workbook.md#undomanager)
- [updateExternalReference](GC.Spread.Sheets.Workbook.md#updateexternalreference)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Workbook**(`host?`, `options?`)

带有指定宿主DOM容器或者DOM ID的表单及其可选设置

**`代码示例`**
```
var workbook = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), {sheetCount:3, font:"12pt Arial"});
var workbook = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), {sheetCount:3, newTabVisible:false});
var workbook = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 3, tabEditable: false });
var workbook = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), {sheetCount:3, tabStripVisible:false});
var workbook = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), {sheetCount:3, allowUserResize:false});
var workbook = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 3, allowUserZoom: false});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `host?` | `string` \| `HTMLElement` | SpreadJS 所在的 DOM 容器或者 ID |
| `options?` | [`IWorkBookDefaultOptions`](../interfaces/GC.Spread.Sheets.IWorkBookDefaultOptions.md) | - |

## Properties

### <a id="contextmenu" name="contextmenu"></a> contextMenu

• **contextMenu**: [`ContextMenu`](GC.Spread.Sheets.ContextMenu.ContextMenu.md)

上下文菜单

**`代码示例`**
```
//本示例展示了如何获取上下文菜单
var menuData = spread.contextMenu.menuData;
```

___

### <a id="custompivottablethemes" name="custompivottablethemes"></a> customPivotTableThemes

• **customPivotTableThemes**: [`CustomPivotTableThemeManager`](GC.Spread.Pivot.CustomPivotTableThemeManager.md)

Represents the custom pivot table theme manager.

___

### <a id="customslicerthemes" name="customslicerthemes"></a> customSlicerThemes

• **customSlicerThemes**: [`CustomSlicerThemeManager`](GC.Spread.Sheets.Slicers.CustomSlicerThemeManager.md)

Represents the custom item slicer theme manager.

___

### <a id="customtablethemes" name="customtablethemes"></a> customTableThemes

• **customTableThemes**: [`CustomTableThemeManager`](GC.Spread.Sheets.Tables.CustomTableThemeManager.md)

Represents the custom table theme manager.

___

### <a id="customtimelinethemes" name="customtimelinethemes"></a> customTimelineThemes

• **customTimelineThemes**: [`CustomTimelineThemeManager`](GC.Spread.Sheets.Slicers.CustomTimelineThemeManager.md)

Represents the custom timeline slicer theme manager.

___

### <a id="docprops" name="docprops"></a> docProps

• **docProps**: [`IDocProps`](../interfaces/GC.Spread.Sheets.IDocProps.md)

Document properties.

___

### <a id="name" name="name"></a> name

• **name**: `string`

Spread的名称

**`代码示例`**
```
spread.name = "Spread1";
```

___

### <a id="options" name="options"></a> options

• **options**: [`IWorkbookOptions`](../interfaces/GC.Spread.Sheets.IWorkbookOptions.md)

控制选项
**`property`** {boolean} allowUserDragMerge - 是否允许用户拖动合并单元格。

**`property`** {GC.Spread.Sheets.AllowDragHeaderToMove} [options.allowDragHeaderToMove] - 指定如何允许拖动标题移动。

**`property`** {boolean} allowUserDragDrop - 是否允许用户拖放范围数据。

**`property`** {boolean} allowUserDragFill - 是否允许用户拖动填充范围。

**`property`** {boolean} allowUserZoom - 是否允许通过按住 Ctrl 键并滚动鼠标滚轮来缩放显示。

**`property`** {boolean} allowUserResize - 是否允许用户调整列和行的大小。

**`property`** {boolean} allowUndo - 是否允许用户撤销编辑。

**`property`** {boolean} allowSheetReorder - 是否允许用户重新排序 Spread 组件中的工作表。

**`property`** {boolean} allowContextMenu - 是否允许用户打开内置上下文菜单。

**`property`** {boolean} allowUserDeselect - 是否允许用户在选择时取消选择。

**`property`** {GC.Spread.Sheets.Fill.AutoFillType} defaultDragFillType - 默认的填充类型。

**`property`** {boolean} showDragFillSmartTag - 是否显示拖动填充对话框。

**`property`** {boolean} showHorizontalScrollbar - 是否显示水平滚动条。

**`property`** {boolean} showVerticalScrollbar - 是否显示垂直滚动条。

**`property`** {boolean} scrollbarShowMax - 是否基于工作表中的所有列和行显示滚动条。

**`property`** {boolean} scrollbarMaxAlign - 滚动条是否与活动工作表的最后一行和最后一列对齐。

**`property`** {boolean} tabStripVisible - 是否显示工作表标签条。

**`property`** {number} tabStripRatio - 标签条宽度表示为整体水平滚动条宽度的百分比。

**`property`** {number} tabStripWidth - 当标签条位于左侧或右侧位置时的宽度。默认值和最小值为 80。

**`property`** {boolean} tabEditable - 是否允许用户编辑工作表标签条。

**`property`** {GC.Spread.Sheets.TabStripPosition} tabStripPosition - 标签条的位置。默认值为底部。

**`property`** {boolean} newTabVisible - 电子表格是否显示特殊标签以允许用户插入新工作表。

**`property`** {GC.Spread.Sheets.AllSheetsListVisibility} allSheetsListVisible - 电子表格是否显示特殊标签以允许用户打开对话框以显示所有工作表。

**`property`** {boolean} tabNavigationVisible - 是否显示工作表标签导航。

**`property`** {boolean} cutCopyIndicatorVisible - 是否在复制或剪切选定项时显示指示器。

**`property`** {string} cutCopyIndicatorBorderColor - 用户剪切或复制选择时显示的指示器的边框颜色。

**`property`** {string} backColor - 用于表示 Spread 组件背景颜色的颜色字符串，例如 "red", "#FFFF00", "rgb(255,0,0)", "Accent 5" 等。

**`property`** {string} backgroundImage - Spread 组件的背景图像。

**`property`** {GC.Spread.Sheets.ImageLayout} backgroundImageLayout - Spread 组件的背景图像布局。

**`property`** {string} grayAreaBackColor - 用于表示灰色区域背景颜色的颜色字符串，例如 "red", "#FFFF00", "rgb(255,0,0)", "Accent 5" 等。

**`property`** {GC.Spread.Sheets.ShowResizeTip} showResizeTip - 如何显示调整大小提示。

**`property`** {boolean} showDragDropTip - 是否显示拖放提示。

**`property`** {boolean} showDragFillTip - 是否显示拖动填充提示。

**`property`** {GC.Spread.Sheets.ShowScrollTip} showScrollTip - 如何显示滚动提示。

**`property`** {boolean} scrollIgnoreHidden - 滚动条是否忽略隐藏的行或列。

**`property`** {boolean} highlightInvalidData - 是否突出显示无效数据。

**`property`** {boolean} useTouchLayout - 是否使用触摸布局来呈现 Spread 组件。

**`property`** {boolean} hideSelection - 当 Spread 组件没有焦点时是否显示选择高亮。

**`property`** {GC.Spread.Sheets.ResizeZeroIndicator} resizeZeroIndicator - 当行或列调整到零时的绘图策略。

**`property`** {boolean} allowUserEditFormula - 是否允许用户在电子表格的单元格中编辑公式。

**`property`** {boolean} enableFormulaTextbox - 是否启用电子表格中的公式文本框。

**`property`** {GC.Spread.Sheets.AutoFitType} autoFitType - 内容是否将在单元格或单元格和标题中格式化以适应。

**`property`** {GC.Spread.Sheets.ReferenceStyle} referenceStyle - 此工作表上单元格公式中单元格和范围引用的样式。

**`property`** {boolean} allowDynamicArray - 是否启用动态数组。

**`property`** {boolean} iterativeCalculation - 是否启用迭代计算。

**`property`** {number} iterativeCalculationMaximumIterations - 迭代计算时的最大迭代次数。

**`property`** {number} iterativeCalculationMaximumChange - 迭代计算时的最大变化。

**`property`** {boolean} calcOnDemand - 是否仅在需要时才计算公式。

**`property`** {boolean} incrementalCalculation - 是否增量计算公式而不阻塞 UI。

**`property`** {boolean} dynamicReferences - 是否计算具有动态引用的函数。

**`property`** {boolean} allowCopyPasteExcelStyle - 用户是否可以从电子表格复制样式然后粘贴到 Excel，或者从 Excel 复制样式然后粘贴到电子表格。

**`property`** {boolean} allowExtendPasteRange - 如果粘贴范围不够粘贴，是否扩大粘贴范围。

**`property`** {GC.Spread.Sheets.CopyPasteHeaderOptions} copyPasteHeaderOptions -复制或粘贴数据时包含哪些标头。

**`property`** {GC.Spread.Sheets.CalculationMode} 计算模式 -工作簿的重新计算行为。默认为自动。

**`property`** {boolean} scrollByPixel - 是否开启按像素精确滚动。

**`property`** {number} scrollPixel - 当scrollByPixel为true时，决定一次滚动该像素数。最终的滚动像素是滚动增量乘以scrollPixel的结果。例如，滚动增量为3，滚动像素为5，最终滚动像素为15。

**`property`** {boolean} enableAccessibility - 是否在电子表格中启用辅助功能支持。

**`property`** {boolean} allowAutoCreateHyperlink - 是否启用在电子表格中自动创建超链接。

**`property`** {GC.Spread.Sheets.ResizeMode} columnResizeMode - 指定调整列大小的方式。

**`property`** {GC.Spread.Sheets.ResizeMode} rowResizeMode - 指定调整行大小的方式。

**`property`** {Array} customList - 供用户自定义拖动填充的列表，每次填充时优先匹配此列表。每个数组项都是字符串数组类型。

**`property`** {GC.Spread.Sheets.ScrollbarAppearance} scrollbarAppearance - 滚动条的外观，包含skin和mobile两个枚举。默认是皮肤。

**`property`** {boolean} pasteSkipInvisibleRange - 粘贴是否跳过不可见范围。默认为 false。

**`property`** {boolean} allowAutoExtendFilterRange - 是否允许像Excel一样自动扩展过滤范围。默认为 false。

**`property`** {boolean} allowInvalidFormula - 是否允许输入无效的公式字符串。默认为 false。

**`property`** {boolean} formulaFormatHint - 公式输入时是否自动生成格式。默认为 true。

**`property`** {GC.Spread.Pivot.PivotAreaReference} pivotAreaReference  - 选择数据透视表数据区域时是否自动生成 getPivotData 公式或单元格引用。默认为 getPivotData。

**`property`** {GC.Spread.Sheets.SheetTabStyles} defaultSheetTabStyles - 工作表选项卡的所有默认状态样式。

**`property`** {GC.Spread.Sheets.IBuiltInFileIcons} [options.builtInFileIcons] - 所有内置文件图标。

**`example`**
```
// var workbook = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:5,showHorizontalScrollbar:false});
var workbook = new GC.Spread.Sheets.Workbook("ss",{sheetCount:5,showHorizontalScrollbar:false});
workbook.options.allowUserDragDrop = false;
workbook.options.allowUserZoom = false;
```

___

### <a id="sheettabstyles" name="sheettabstyles"></a> sheetTabStyles

• **sheetTabStyles**: [`SheetTabStyleManager`](GC.Spread.Sheets.SheetTabStyleManager.md)

代表工作表选项卡的状态样式管理器

___

### <a id="sheets" name="sheets"></a> sheets

• **sheets**: [`Worksheet`](GC.Spread.Sheets.Worksheet.md)[]

表单集合

___

### <a id="touchtoolstrip" name="touchtoolstrip"></a> touchToolStrip

• **touchToolStrip**: [`TouchToolStrip`](GC.Spread.Sheets.Touch.TouchToolStrip.md)

触摸工具条

## Methods

### <a id="addcustomfunction" name="addcustomfunction"></a> addCustomFunction

▸ **addCustomFunction**(`fn`): `void`

添加自定义函数

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fn` | [`Function`](GC.Spread.CalcEngine.Functions.Function.md) | 需要添加的函数 |

#### Returns

`void`

___

### <a id="addcustomname" name="addcustomname"></a> addCustomName

▸ **addCustomName**(`name`, `formula`, `baseRow`, `baseCol`, `comment?`, `isReadOnly?`): `void`

添加自定义名称

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 自定义名称 |
| `formula` | `string` | 公式 |
| `baseRow` | `number` | 行索引 |
| `baseCol` | `number` | 列索引 |
| `comment` | `string` | 自定义批注 |
| `isReadOnly?` | `boolean` | - |

#### Returns

`void`

___

### <a id="addnamedstyle" name="addnamedstyle"></a> addNamedStyle

▸ **addNamedStyle**(`style`): `void`

将样式添加到名为样式集的工作簿中

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 要添加的样式 |

#### Returns

`void`

___

### <a id="addsheet" name="addsheet"></a> addSheet

▸ **addSheet**(`index`, `sheet?`): `void`

在特定索引处插入一个表单

**`代码示例`**
```
//本示例将表单添加到表单
spread.addSheet(0,new GC.Spread.Sheets.Worksheet("custom"));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 添加表单的索引 |
| `sheet?` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 要添加的表单 |

#### Returns

`void`

___

### <a id="addsheettab" name="addsheettab"></a> addSheetTab

▸ **addSheetTab**(`index`, `name`, `type`): `any`

在指定索引处插入集算表

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 要添加集算表的索引 |
| `name` | `string` | 要添加集算表的名称 |
| `type` | [`SheetType`](../enums/GC.Spread.Sheets.SheetType.md) | 表单标签类型 |

#### Returns

`any`

添加的集算表

___

### <a id="addsparklineex" name="addsparklineex"></a> addSparklineEx

▸ **addSparklineEx**(`sparklineEx`): `void`

将 SparklineEx 添加到 SparklineEx 集合

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sparklineEx` | [`SparklineEx`](GC.Spread.Sheets.Sparklines.SparklineEx.md) | 要添加的SparklineEx |

#### Returns

`void`

___

### <a id="bind" name="bind"></a> bind

▸ **bind**(`type`, `data?`, `fn?`): `void`

将事件绑定到工作簿

**`代码示例`**
```
//本示例将事件绑定到函数
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
| `type` | `string` | 事件类型 |
| `data?` | `any` | 要传递给函数的其他数据 |
| `fn?` | `Function` | 事件触发时要执行的函数 |

#### Returns

`void`

___

### <a id="calculate" name="calculate"></a> calculate

▸ **calculate**(`type?`, `address?`): `void`

重新构建、标记为脏、广播脏数据并重新计算公式
首先按照计算类型在地址中进行重新构建和标记为脏
然后，广播脏数据将递归地将脏单元格的依赖项设置为脏数据在工作簿中
在自动模式下，所有脏单元格将被计算
在手动模式下，只有地址中的单元格会被计算，其他单元格保持脏状态
如果 CalcService 被暂停，则会跳过重新计算

**`example`**
```
spread.sheets[0].setFormula(0,0,"RAND()");
spread.sheets[0].setFormula(1,0,"=Sheet2!A1");
spread.sheets[0].setFormula(2,0,"=1+2");
spread.sheets[1].setFormula(0,0,"RAND()");
spread.sheets[1].setFormula(1,0,"=Sheet1!A1");

// 所有单元格都会重新计算
spread.calculate();
spread.calculate(GC.Spread.Sheets.CalculationType.regular);

// Sheet1!A1 和 Sheet2!A2 被计算出新的数值，并且计算了 Sheet1!A2 和 Sheet1!A3
spread.calculate(GC.Spread.Sheets.CalculationType.all, "Sheet1");

// Sheet1!A1 和 Sheet2!A2 被计算出新的数值
spread.calculate(GC.Spread.Sheets.CalculationType.regular, "Sheet1!A1");

// 没有任何单元格被计算
spread.calculate(GC.Spread.Sheets.CalculationType.regular, "Sheet1!A2");

spread.options.calculationMode = GC.Spread.Sheets.CalculationMode.manual; // 切换到手动模式

// Sheet1!A1 被计算出新的数值，Sheet1!A2 和 Sheet1!A3 被计算但未更改，Sheet2!A2 在手动模式下保持脏状态
spread.calculate(GC.Spread.Sheets.CalculationType.all, "Sheet1");

// Sheet1!A1 被计算出新的数值，Sheet2!A2 在手动模式下保持脏状态
spread.calculate(GC.Spread.Sheets.CalculationType.regular, "Sheet1");

// Sheet2!A2 被计算，因为它是脏的
spread.calculate(GC.Spread.Sheets.CalculationType.minimal);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type?` | [`CalculationType`](../enums/GC.Spread.Sheets.CalculationType.md) | 指定重新构建和标记脏数据的计算类型 |
| `address?` | `string` | 指定要标记为脏并计算的工作表或范围。如果省略，则为整个工作簿。请注意，在自动模式下，范围之外的脏依赖项将被计算 |

#### Returns

`void`

___

### <a id="changesheetindex" name="changesheetindex"></a> changeSheetIndex

▸ **changeSheetIndex**(`sheetName`, `targetIndex`): `boolean`

更改表单索引并重新排序表单

**`代码示例`**
```
//本示例演示如何更改表单索引
var spread = GC.Spread.Sheets.findControl(ss);
spread.setSheetCount(5); // The sheets sequence should be "Sheet1", "Sheet2", "Sheet3", "Sheet4", "Sheet5".
spread.changeSheetIndex("Sheet1", 3); // The sheets sequence should be "Sheet2", "Sheet3", "Sheet4", "Sheet1", "Sheet5".
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheetName` | `string` | 表单名称 |
| `targetIndex` | `number` | 目标索引 |

#### Returns

`boolean`

___

### <a id="changesheetposition" name="changesheetposition"></a> changeSheetPosition

▸ **changeSheetPosition**(`sheetName`, `targetPosition`): `boolean`

修改表单的位置及顺序

**`example`**
```
//这个例子表示如何修改集算表的位置
var spread = GC.Spread.Sheets.findControl(ss);
spread.setSheetCount(5);
spread.addSheetTab(0, "tableSheet1", GC.Spread.Sheets.SheetType.tableSheet); // The sheets sequence should be "Sheet1", "Sheet2", "Sheet3", "Sheet4", "Sheet5", "tableSheet1".
spread.changeSheetPosition("tableSheet1", 3); // The sheets sequence should be "Sheet1", "Sheet2", "Sheet3", "tableSheet1", "Sheet4", "Sheet5".
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheetName` | `string` | 表单名称 |
| `targetPosition` | `number` | 目标位置 |

#### Returns

`boolean`

___

### <a id="clearcustomfunctions" name="clearcustomfunctions"></a> clearCustomFunctions

▸ **clearCustomFunctions**(): `void`

清除所有自定义功能

#### Returns

`void`

___

### <a id="clearcustomnames" name="clearcustomnames"></a> clearCustomNames

▸ **clearCustomNames**(): `void`

清除自定义名称

#### Returns

`void`

___

### <a id="clearsheettabs" name="clearsheettabs"></a> clearSheetTabs

▸ **clearSheetTabs**(): `void`

清除所有工作表

#### Returns

`void`

___

### <a id="clearsheets" name="clearsheets"></a> clearSheets

▸ **clearSheets**(): `void`

清除控件中的所有表单

**`代码示例`**
```
//本示例使用clearSheets方法
spread.clearSheets();
```

#### Returns

`void`

___

### <a id="commandmanager" name="commandmanager"></a> commandManager

▸ **commandManager**(): [`CommandManager`](GC.Spread.Commands.CommandManager.md)

获取命令管理器

**`代码示例`**
```
//本示例执行一个执行指定动作的命令
spread.options.allowUndo = true;
spread.commandManager().execute({cmd: "outlineRow", sheetName: "Sheet1", index: 3, count: 5});
```

#### Returns

[`CommandManager`](GC.Spread.Commands.CommandManager.md)

The command manager.

___

### <a id="datamanager" name="datamanager"></a> dataManager

▸ **dataManager**(): [`DataManager`](GC.Data.DataManager.md)

获取数据管理器

#### Returns

[`DataManager`](GC.Data.DataManager.md)

返回数据管理器

### <a id="defaultpivottabletheme" name="defaultpivottabletheme"></a> defaultPivotTableTheme

▸ **defaultPivotTableTheme**(`themeName?`): `undefined` \| [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md)

set or get the default pivot table theme.

**`example`**
```
// set Default pivot table theme name as "custom0"
spread.defaultPivotTableTheme("custom0");
let newPivotTable = activeSheet.pivotTables.add("pivotTable1", 1, 1, 10, 5);
// The pivot table above will use "custom0" as the theme since no specific theme has been specified.

// get default pivot table theme
spread.defaultPivotTableTheme();
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `themeName?` | `string` |

#### Returns

`undefined` \| [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md)

___

### <a id="defaultslicertheme" name="defaultslicertheme"></a> defaultSlicerTheme

▸ **defaultSlicerTheme**(`themeName?`): `undefined` \| [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

set or get the default slicer theme.

**`example`**
```
// set default slicer theme name as "custom0"
spread.defaultSlicerTheme("custom0");
let newSlicer = activeSheet.slicers.add("slicer1", 1, 1, 10, 5);
// The slicer above will use "custom0" as the theme since no specific theme has been specified.

// get default slicer theme
spread.defaultSlicerTheme();
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `themeName?` | `string` |

#### Returns

`undefined` \| [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

___

### <a id="defaulttabletheme" name="defaulttabletheme"></a> defaultTableTheme

▸ **defaultTableTheme**(`themeName?`): `undefined` \| [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md)

set or get the default table theme.

**`example`**
```
// set default table theme name as "custom0"
spread.defaultTableTheme("custom0");
let newable = activeSheet.tables.add("table1", 1, 1, 10, 5);
// The table above will use "custom0" as the theme since no specific theme has been specified.

// get the default table theme
spread.defaultTableTheme();
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `themeName?` | `string` |

#### Returns

`undefined` \| [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md)

___

### <a id="defaulttimelinetheme" name="defaulttimelinetheme"></a> defaultTimelineTheme

▸ **defaultTimelineTheme**(`themeName?`): `undefined` \| [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

set or get the default timeLine theme.

**`example`**
```
// set default timeLine theme name as "custom0"
spread.defaultTimelineTheme("custom0");
let newTimeline = activeSheet.timeLines.add("timeLine1", 1, 1, 10, 5);
// The timeLine above will use "custom0" as the theme since no specific theme has been specified.

// get default timeLine theme
spread.defaultTimelineTheme();
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `themeName?` | `string` |

#### Returns

`undefined` \| [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

___

### <a id="destroy" name="destroy"></a> destroy

▸ **destroy**(): `void`

销毁工作簿及其包含的所有表单

**`代码示例`**
```
//本示例销毁工作簿实例
spread.destroy();
```

#### Returns

`void`

___

### <a id="export" name="export"></a> export

▸ **export**(`successCallBack?`, `errorCallBack?`, `exportOptions?`): `void`

将对象状态导出到 Excel、SSJSON 或 CSV 文件

**`代码示例`**
```
spread.export(function (blob) {
   // save blob to a file
   saveAs(blob, fileName);
}, function (e) {
   console.log(e);
}, {
   fileType: GC.Spread.Sheets.FileType.excel,
   includeBindingSource: true
});
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `successCallBack?` | `Function` |
| `errorCallBack?` | `Function` |
| `exportOptions?` | [`ExportOptions`](../modules/GC.Spread.Sheets.md#exportoptions) |

#### Returns

`void`

___

### <a id="focus" name="focus"></a> focus

▸ **focus**(`focusIn?`): `void`

让工作簿获取焦点或失去焦点

**`代码示例`**
```
//本示例让工作簿获取焦点
$("#button1").click(function () {
spread.focus(true);
   });
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `focusIn?` | `boolean` | 为`false`时，工作簿失去焦点; 否则，获取焦点 |

#### Returns

`void`

___

### <a id="fromjson" name="fromjson"></a> fromJSON

▸ **fromJSON**(`workbookData`, `deserializationOptions?`): `Promise`<`any`\>

从指定的JSON字符串加载对象状态

**`代码示例`**
```
//本示例使用fromJSON方法
activeSheet.getCell(0,0).value(123);
var jsonStr = null;
//export
jsonStr = JSON.stringify(spread.toJSON());
//import
var fromJSONPromise = spread.fromJSON(JSON.parse(jsonStr));
fromJSONPromise.then(() => {
     alert(jsonStr);
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workbookData` | `Object` | 反序列化的表单数据 |
| `deserializationOptions?` | `Object` | - |

#### Returns

`Promise`<`any`\>

- The fromJSON promise.

___

### <a id="getactivesheet" name="getactivesheet"></a> getActiveSheet

▸ **getActiveSheet**(): [`Worksheet`](GC.Spread.Sheets.Worksheet.md)

获取当前表单

#### Returns

[`Worksheet`](GC.Spread.Sheets.Worksheet.md)

当前表单实例

___

### <a id="getactivesheetindex" name="getactivesheetindex"></a> getActiveSheetIndex

▸ **getActiveSheetIndex**(): `number`

获取控件的当前表单索引

**`代码示例`**
```
//本示例使用getActiveSheetIndex方法
var index = spread.getActiveSheetIndex();
alert(index);
```

#### Returns

`number`

当前表单索引

___

### <a id="getactivesheettab" name="getactivesheettab"></a> getActiveSheetTab

▸ **getActiveSheetTab**(): `any`

获取当前表单选项卡

#### Returns

`any`

活动的表单选项卡实例

___

### <a id="getactivesheettabindex" name="getactivesheettabindex"></a> getActiveSheetTabIndex

▸ **getActiveSheetTabIndex**(): `number`

获取当前表单选项卡索引

#### Returns

`number`

当前表单选项卡索引

___

### <a id="getcircularreference" name="getcircularreference"></a> getCircularReference

▸ **getCircularReference**(): [`ICellsInfo`](../interfaces/GC.Spread.Sheets.ICellsInfo.md)[]

 获取工作簿中的所有循环引用单元格信息

**`代码示例`**
```
spread.getCircularReference();
```

#### Returns

[`ICellsInfo`](../interfaces/GC.Spread.Sheets.ICellsInfo.md)[]

返回循环引用单元格信息对象数组
- cellsInfo.row {number} 单元格区域行索引
- cellsInfo.col {number} 单元格区域列索引
- cellsInfo.rowCount {number} 单元格区域行数
- cellsInfo.colCount {number} 单元格范围
- cellsInfo.sheetName {string} 工作表名称

___

### <a id="getcustomfunction" name="getcustomfunction"></a> getCustomFunction

▸ **getCustomFunction**(`name`): `void`

获取自定义函数

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 自定义函数名称 |

#### Returns

`void`

自定义函数

___

### <a id="getcustomname" name="getcustomname"></a> getCustomName

▸ **getCustomName**(`name`): [`NameInfo`](GC.Spread.Sheets.NameInfo.md)

获取指定的自定义名称信息

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 自定义名称 |

#### Returns

[`NameInfo`](GC.Spread.Sheets.NameInfo.md)

自定义名称的信息

___

### <a id="getcustomnames" name="getcustomnames"></a> getCustomNames

▸ **getCustomNames**(): [`NameInfo`](GC.Spread.Sheets.NameInfo.md)[]

获取所有自定义名称信息

#### Returns

[`NameInfo`](GC.Spread.Sheets.NameInfo.md)[]

类型GC.Spread.Sheets.NameInfo存储在数组中

___

### <a id="getexternalreferences" name="getexternalreferences"></a> getExternalReferences

▸ **getExternalReferences**(`includeItemDetail?`): [`IExternalReference`](../interfaces/GC.Spread.Sheets.IExternalReference.md)[]

获取当前工作簿的跨工作簿引用列表

**`代码示例`**
```
//本示例获取并更新使用的数据源
spread.getActiveSheet().setFormula(0, 0, "='[Jackson.xlsx]Sheet1'!B6+SUM('[Petrosky.xlsx]Sheet2'!B7:B8)");
spread.getExternalReferences().forEach(item=>{
     spread.updateExternalReference(item.name, spreadList[item.name], item.filePath);
})
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `includeItemDetail?` | `boolean` | 是否包括目标单元格和源范围。默认值为false |

#### Returns

[`IExternalReference`](../interfaces/GC.Spread.Sheets.IExternalReference.md)[]

- externalReference数组
- externalReference.name {string} 跨工作簿引用的文件名
- externalReference.filePath {string} 跨工作簿引用的文件路径

___

### <a id="gethost" name="gethost"></a> getHost

▸ **getHost**(): `HTMLElement`

获取当前工作簿实例的宿主元素

#### Returns

`HTMLElement`

host 当前工作簿实例的宿主元素

___

### <a id="getnamedstyle" name="getnamedstyle"></a> getNamedStyle

▸ **getNamedStyle**(`name`): [`Style`](GC.Spread.Sheets.Style.md)

从名为styles的工作簿中获取具有指定名称的样式

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要返回的样式的名称 |

#### Returns

[`Style`](GC.Spread.Sheets.Style.md)

返回指定的命名样式

___

### <a id="getnamedstyles" name="getnamedstyles"></a> getNamedStyles

▸ **getNamedStyles**(): [`Style`](GC.Spread.Sheets.Style.md)[]

从工作簿中获取命名样式

#### Returns

[`Style`](GC.Spread.Sheets.Style.md)[]

命名样式的GC.Spread.Sheets.Style数组

___

### <a id="getsheet" name="getsheet"></a> getSheet

▸ **getSheet**(`index`): [`Worksheet`](GC.Spread.Sheets.Worksheet.md)

获取指定的表单

**`代码示例`**
```
//本示例获取表单并设置单元格前面板
var sheet1 = spread.getSheet(1);
sheet1.getCell(0,0).value("A1").foreColor("red");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 要返回的表单的索引 |

#### Returns

[`Worksheet`](GC.Spread.Sheets.Worksheet.md)

指定的表

___

### <a id="getsheetcount" name="getsheetcount"></a> getSheetCount

▸ **getSheetCount**(): `number`

获取表单的数量

**`代码示例`**
```
//本例使用了getSheetCount方法
var index = spread.getSheetCount();
alert(index);
```

#### Returns

`number`

表单的数量

___

### <a id="getsheetfromname" name="getsheetfromname"></a> getSheetFromName

▸ **getSheetFromName**(`name`): [`Worksheet`](GC.Spread.Sheets.Worksheet.md)

获取具有指定名称的表单

**`代码示例`**
```
//本示例获取表单并设置单元格前面板
var sheet1 = spread.getSheetFromName("Sheet2");
sheet1.getCell(0,0).value("A1").foreColor("red");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 表单名称 |

#### Returns

[`Worksheet`](GC.Spread.Sheets.Worksheet.md)

具有指定名称的表单

___

### <a id="getsheetindex" name="getsheetindex"></a> getSheetIndex

▸ **getSheetIndex**(`name`): `number`

获取指定名称的表单索引

**`代码示例`**
```
//本示例使用getSheetIndex方法
spread.setSheetCount(5);
var index = spread.getSheetIndex("Sheet2");
alert(index); // 1
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 表单名称 |

#### Returns

`number`

基于工作表集合的表单索引

___

### <a id="getsheetposition" name="getsheetposition"></a> getSheetPosition

▸ **getSheetPosition**(`name`): `number`

根据名字获取表单选项卡的位置

**`example`**
```
spread.setSheetCount(5);
spread.addSheetTab(0, "tableSheet1", GC.Spread.Sheets.SheetType.tableSheet);
var position = spread.getSheetPosition("tableSheet1");
alert(position); // 5
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 表单选项卡的名字 |

#### Returns

`number`

表单选项卡位置，基于工作表和集算表的集合

___

### <a id="getsheettab" name="getsheettab"></a> getSheetTab

▸ **getSheetTab**(`indexOrName`): `any`

按索引或名称获取指定的工作表选项卡

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `indexOrName` | `string` \| `number` | 要返回的工作表选项卡的索引或名称 |

#### Returns

`any`

指定的表单选项卡

___

### <a id="getsheettabcount" name="getsheettabcount"></a> getSheetTabCount

▸ **getSheetTabCount**(): `number`

获取工作表选项卡的数目

#### Returns

`number`

工作表选项卡的数目

___

### <a id="getsheettabindex" name="getsheettabindex"></a> getSheetTabIndex

▸ **getSheetTabIndex**(`name`): `number`

获取具有指定名称的集算表选项卡索引

**`example`**
```
spread.setSheetCount(5);
spread.addSheetTab(0, "tableSheet1", GC.Spread.Sheets.SheetType.tableSheet);
var index = spread.getSheetTabIndex("tableSheet1");
alert(index); // 0
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 集算表选项卡名称 |

#### Returns

`number`

表单选项卡位置，基于工作表和集算表的集合

___

### <a id="hittest" name="hittest"></a> hitTest

▸ **hitTest**(`x`, `y`): [`IWorkbookHitTestInformation`](../interfaces/GC.Spread.Sheets.IWorkbookHitTestInformation.md)

执行命中测试

**`代码示例`**
```
//本示例使用hitTest方法
      window.onload = function(){
          var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
          var activeSheet = spread.getActiveSheet();
          $("#ss").click(function (e) {
              //从鼠标单击的常规单元格中获取单元格索引，这些常规单元格既不是固定的行/列也不是行/列标题
              var offset = $("#ss").offset();
              var x = e.pageX - offset.left;
              var y = e.pageY - offset.top;
              var target = spread.hitTest(x, y);
              if(target.worksheetHitInfo) {
                  if(target.worksheetHitInfo.hitTestType === 0) {
                      str = 'corner';
                  } else if (target.worksheetHitInfo.hitTestType === 1) {
                      str = 'colHeader';
                  } else if (target.worksheetHitInfo.hitTestType === 2) {
                      str = 'rowHeader';
                  } else {
                      str = 'viewport';
                  }
              } else if(target.tabStripHitInfo) {
                  if(target.tabStripHitInfo.navButton){
                      str = target.tabStripHitInfo.navButton;
                  } else if(target.tabStripHitInfo.sheetTab) {
                      str = target.tabStripHitInfo.sheetTab.sheetName;
                  } else if(target.tabStripHitInfo.resize === true) {
                      str = "resize";
                  } else {
                      str = "blank";
                  }
              } else if(target.horizontalScrollBarHitInfo) {
                  str = target.horizontalScrollBarHitInfo.element;
              } else if(target.verticalScrollBarHitInfo) {
                  str = target.verticalScrollBarHitInfo.element;
              } else if(target.footerCornerHitInfo) {
                  str = target.footerCornerHitInfo.element;
              }
        alert(str);
});
}
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | 相对于 SpreadJS 水平轴的<i> x </i>坐标x |
| `y` | `number` | 相对于 SpreadJS 垂直轴的<i> y </i>坐标y |

#### Returns

[`IWorkbookHitTestInformation`](../interfaces/GC.Spread.Sheets.IWorkbookHitTestInformation.md)

- 命中测试信息 如果选择表单，则返回表单信息 该信息包含x,y和worksheetHitInfo;
- 如果选择sheetsTabStrip,则返回sheetsTabStrip信息 此信息包含x,y和tabStripHitInfo;
- 如果选择horizontalScrollbar,则返回horizontalScrollbar信息 该信息包含x,y和horizontalScrollBarHitInfo;
- 如果选择verticalScrollbar,则返回verticalScrollbar信息 此信息包含x,y和verticalScrollBarHitInfo;
- 如果选择footerCorner,则返回footerCorner信息 此信息包含x,y和footerCornerHitInfo

___

### <a id="import" name="import"></a> import

▸ **import**(`file`, `successCallback?`, `errorCallback?`, `importOptions?`): `void`

从 Excel、SSJOSN、csv文件、JavaScript 文件导入对象状态

**`代码示例`**
```
//This example uses the import method.
//Get file blob.
var file = document.getElementById("importFileName").files[0];
// import
spread.import(file, function () {
   // success callback to do something
}, function (e) {
   console.log(e); // error callback
}, {
   fileType: GC.Spread.Sheets.FileType.excel
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `file` | `File` | Excel、SSJOSN、csv文件、JavaScript 文件 |
| `successCallback?` | `Function` | - |
| `errorCallback?` | `Function` | - |
| `importOptions?` | [`ImportOptions`](../modules/GC.Spread.Sheets.md#importoptions) | - |

#### Returns

`void`

___

### <a id="invalidatelayout" name="invalidatelayout"></a> invalidateLayout

▸ **invalidateLayout**(): `void`

更新控件布局信息

**`代码示例`**
```
//本示例更新布局
spread.invalidateLayout();
spread.repaint();
```

#### Returns

`void`

___

### <a id="ispaintsuspended" name="ispaintsuspended"></a> isPaintSuspended

▸ **isPaintSuspended**(): `boolean`

获取 SpreadJS 是否已暂停绘制

#### Returns

`boolean`

___

### <a id="nextcontrol" name="nextcontrol"></a> nextControl

▸ **nextControl**(`value?`): `any`

通过 GC.Spread.Sheets.Actions.selectNextControl 和 GC.Spread.Sheets.Actions.moveToNextCellThenControl 获取或设置使用的下一个控件

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `HTMLElement` | 下一个控件，控件必须具有获取焦点方法 |

#### Returns

`any`

如果未设置任何值，则返回下一个控件；否则，返回表单

___

### <a id="open" name="open"></a> open

▸ **open**(`file`, `successCallback?`, `errorCallback?`, `openOptions?`): `void`

加载 SJS 文件到 SpreadJS 实例

**`代码示例`**
```
//This example uses the open method.
//Get file blob.
var file = document.getElementById("importFileName").files[0];
// import
spread.open(file, function () {
   // success callback to 做一些事请
}, function (e) {
 console.log(e); // error callback
}, { openMode: GC.Spread.Sheets.OpenMode.lazy });
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `file` | `File` | SJS 文件流 |
| `successCallback?` | `Function` | - |
| `errorCallback?` | `Function` | - |
| `openOptions?` | [`OpenOptions`](../modules/GC.Spread.Sheets.md#openoptions) | - |

#### Returns

`void`

___

### <a id="pageinfo" name="pageinfo"></a> pageInfo

▸ **pageInfo**(`sheetIndex?`): `any`

获取表单的页面信息

**`代码示例`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
spread.suspendPaint();
var sheet = spread.getActiveSheet();
for(var i=0;i<20;i++){
   for(var j=0;j<20;j++){
       sheet.setValue(i,j,"Row"+i+"_Column"+j);
   }
}
var pageInfos =  spread.pageInfo(0);
console.table(pageInfos.pages);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheetIndex?` | `number` | 表单索引 |

#### Returns

`any`

返回表单的页面信息，如果忽略表单索引，则返回数组中所有表单的页面信息

___

### <a id="previouscontrol" name="previouscontrol"></a> previousControl

▸ **previousControl**(`value?`): `any`

通过GC.Spread.Sheets.Actions.selectPreviousControl和GC.Spread.Sheets.Actions.moveToPreviousCellThenControl获取或设置使用的先前控件

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `HTMLElement` | 先前的控件控件必须具有焦点方法 |

#### Returns

`any`

如果未设置任何值，则返回先前的控件；否则，返回表单

___

### <a id="print" name="print"></a> print

▸ **print**(`sheetIndex?`): `void`

打印指定的表单

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheetIndex?` | `number` | 表单索引，如果忽略表单索引，则打印所有可见的表单 |

#### Returns

`void`

___

### <a id="refresh" name="refresh"></a> refresh

▸ **refresh**(): `void`

手动刷新工作簿对象的布局和呈现

**`代码示例`**
```
//本示例使用refresh方法
spread.refresh();
```

#### Returns

`void`

___

### <a id="removecustomfunction" name="removecustomfunction"></a> removeCustomFunction

▸ **removeCustomFunction**(`name`): `void`

删除自定义函数

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 自定义函数名称 |

#### Returns

`void`

___

### <a id="removecustomname" name="removecustomname"></a> removeCustomName

▸ **removeCustomName**(`name`): `void`

删除指定的自定义名称

**`代码示例`**
```
//本示例使用removeCustomName方法
activeSheet.setValue(0, 0, 1);
activeSheet.setValue(0, 1, 2);
activeSheet.setValue(0, 2, 3);
spread.addCustomName("customName1","=12", 0, 0);
activeSheet.setFormula(1, 0, "customName1");
//spread.removeCustomName("customName1");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 自定义名称 |

#### Returns

`void`

___

### <a id="removenamedstyle" name="removenamedstyle"></a> removeNamedStyle

▸ **removeNamedStyle**(`name`): `void`

从名为styles的工作簿中删除具有指定名称的样式

**`代码示例`**
```
var namedStyle = new GC.Spread.Sheets.Style();
namedStyle.name = "style1";
namedStyle.backColor = "green";
spread.addNamedStyle(namedStyle);
activeSheet.setStyleName(1, 1, "style1"); // 单元格(1,1)的背景色为绿色
activeSheet.setStyleName(2, 1, "style1");
var style = spread.getNamedStyle("style1");
style.foreColor = "red";    // namedStyle的前景色为红色
activeSheet.repaint(); // 单元格(1,1)和单元格(2,1)的前颜色为红色
activeSheet.getCell(1,1).value("test");
$("#button1").click(function () {
     spread.removeNamedStyle("style1");
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要删除的样式的名称 |

#### Returns

`void`

___

### <a id="removesheet" name="removesheet"></a> removeSheet

▸ **removeSheet**(`index`): `void`

删除指定的表单

**`代码示例`**
```
//本示例从表单中删除表
spread.setSheetCount(5);
spread.removeSheet(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 要删除的表单的索引 |

#### Returns

`void`

___

### <a id="removesheettab" name="removesheettab"></a> removeSheetTab

▸ **removeSheetTab**(`indexOrName`): `void`

按索引或名称删除指定的工作表选项卡

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `indexOrName` | `string` \| `number` | 要删除的工作表选项卡的索引或名称 |

#### Returns

`void`

___

### <a id="removesparklineex" name="removesparklineex"></a> removeSparklineEx

▸ **removeSparklineEx**(`name`): `void`

从SparklineEx集合中移除SparklineEx

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要删除的SparklineEx的名称 |

#### Returns

`void`

___

### <a id="repaint" name="repaint"></a> repaint

▸ **repaint**(): `void`

重新绘制工作簿控件

**`代码示例`**
```
//本示例更新布局
spread.invalidateLayout();
spread.repaint();
```

#### Returns

`void`

___

### <a id="resumecalcservice" name="resumecalcservice"></a> resumeCalcService

▸ **resumeCalcService**(`recalcAll?`): `void`

恢复计算服务

**`代码示例`**
```
//本示例使用resumeCalcService方法
spread.suspendCalcService(false);
activeSheet.setValue(0,0,1);
activeSheet.setValue(0,1,2);
activeSheet.setValue(0,2,10);
activeSheet.getCell(1,1).formula("=SUM(A1:C1)");
spread.resumeCalcService(true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `recalcAll?` | `boolean` | 指定是否重新计算所有公式 |

#### Returns

`void`

___

### <a id="resumeevent" name="resumeevent"></a> resumeEvent

▸ **resumeEvent**(): `void`

恢复事件

**`代码示例`**
```
//本示例暂停并恢复事件
 activeSheet.bind(GC.Spread.Sheets.Events.CellChanged, function (sender, args) {
    if (args.propertyName === "value") {
        alert(activeSheet.getValue(args.row, args.col));
    }
});
spread.suspendEvent();
activeSheet.setValue(0, 0, "111");
spread.resumeEvent();
activeSheet.setValue(1, 1, "222");
```

#### Returns

`void`

___

### <a id="resumepaint" name="resumepaint"></a> resumePaint

▸ **resumePaint**(): `void`

恢复活动表单和标签条的绘制

#### Returns

`void`

___

### <a id="save" name="save"></a> save

▸ **save**(`successCallBack?`, `errorCallBack?`, `saveOptions?`): `void`

将 SpreadJS 保存为 SJS 文件流

**`代码示例`**
```
spread.save(function (blob) {
   // save blob to a file
   saveAs(blob, fileName);
}, function (e) {
   console.log(e);
}, { includeUnusedNames: false });
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `successCallBack?` | `Function` | 成功时的回调函数 |
| `errorCallBack?` | `Function` | 发生错误时的回调函数 |
| `saveOptions?` | [`SaveOptions`](../modules/GC.Spread.Sheets.md#saveoptions) | 保存选项 |

#### Returns

`void`

___

### <a id="savepdf" name="savepdf"></a> savePDF

▸ **savePDF**(`successCallback`, `errorCallback`, `options?`, `sheetIndex?`): `void`

将指定的表单导出为PDF

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `successCallback` | `Function` | 成功时的回调函数 |
| `errorCallback` | `Function` | 发生错误时的回调函数 |
| `options?` | `Object` | - |
| `sheetIndex?` | `number` | 表单索引 如果忽略表单索引，则导出所有可见表单 |

#### Returns

`void`

___

### <a id="search" name="search"></a> search

▸ **search**(`searchCondition`): [`SearchResult`](GC.Spread.Sheets.Search.SearchResult.md)

在指定表单的单元格中的文本中搜索具有指定条件的指定字符串

**`代码示例`**
```
//本示例使用指定的搜索条件搜索活动表
activeSheet.getCell(2,3).value("testSearch");
var searchCondition = new GC.Spread.Sheets.Search.SearchCondition();
searchCondition.searchString = "testSearch";
searchCondition.startSheetIndex = spread.getActiveSheetIndex();
searchCondition.endSheetIndex = spread.getActiveSheetIndex();
searchCondition.searchOrder = GC.Spread.Sheets.Search.SearchOrder.nOrder;
searchCondition.searchTarget = GC.Spread.Sheets.Search.SearchFoundFlags.cellText;
searchCondition.searchFlags = GC.Spread.Sheets.Search.SearchFlags.ignoreCase| GC.Spread.Sheets.Search.SearchFlags.useWildCards;
var searchresult= spread.search(searchCondition);
var str ="[searchFoundFlag:"+ searchresult.searchFoundFlag+",\r\n foundSheetIndex:"+searchresult.foundSheetIndex+",foundRowIndex:" +
searchresult.foundRowIndex+", foundColumnIndex:"+searchresult.foundColumnIndex+", foundString:"+searchresult.foundSheetIndex+"]";
alert(str);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `searchCondition` | [`SearchCondition`](GC.Spread.Sheets.Search.SearchCondition.md) | 搜索条件 |

#### Returns

[`SearchResult`](GC.Spread.Sheets.Search.SearchResult.md)

搜索结果

___

### <a id="setactivesheet" name="setactivesheet"></a> setActiveSheet

▸ **setActiveSheet**(`name`): `void`

通过名称设置活动表单

**`代码示例`**
```
//本示例设置活动表单
spread.setSheetCount(3);
spread.setActiveSheet("Sheet2");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 用来制作活动表单的表单名称 |

#### Returns

`void`

___

### <a id="setactivesheetindex" name="setactivesheetindex"></a> setActiveSheetIndex

▸ **setActiveSheetIndex**(`value`): `void`

设置控件的活动表单索引

**`代码示例`**
```
//本示例使用setActiveSheetIndex方法
spread.setActiveSheetIndex(1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `number` | 活动表单索引 |

#### Returns

`void`

___

### <a id="setactivesheettab" name="setactivesheettab"></a> setActiveSheetTab

▸ **setActiveSheetTab**(`indexOrName`): `void`

按索引或名称设置活动表单选项卡

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `indexOrName` | `string` \| `number` | 用于创建活动表单选项卡的索引或名称 |

#### Returns

`void`

___

### <a id="setsheetcount" name="setsheetcount"></a> setSheetCount

▸ **setSheetCount**(`count`): `void`

设置表单数

**`代码示例`**
```
spread.setSheetCount(5);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `count` | `number` | 表单的数量 |

#### Returns

`void`

___

### <a id="startsheetindex" name="startsheetindex"></a> startSheetIndex

▸ **startSheetIndex**(`value?`): `any`

获取或设置要在表单中显示的第一张表单的索引

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 要在表单中显示的第一张表单的索引 |

#### Returns

`any`

如果未设置任何值，则返回表单中显示的第一张表单的索引；否则，返回表单

___

### <a id="suspendcalcservice" name="suspendcalcservice"></a> suspendCalcService

▸ **suspendCalcService**(`ignoreDirty?`): `void`

挂起计算服务

**`代码示例`**
```
//本示例使用suspendCalcService方法
spread.suspendCalcService(false);
activeSheet.setValue(0,0,1);
activeSheet.setValue(0,1,2);
activeSheet.setValue(0,2,10);
activeSheet.getCell(1,1).formula("=SUM(A1:C1)");
spread.resumeCalcService(true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ignoreDirty?` | `boolean` | 是否使依赖关系单元格无效 |

#### Returns

`void`

___

### <a id="suspendevent" name="suspendevent"></a> suspendEvent

▸ **suspendEvent**(): `void`

挂起事件

**`代码示例`**
```
//本示例暂停并恢复事件
activeSheet.bind(GC.Spread.Sheets.Events.CellChanged, function (sender, args) {
    if (args.propertyName === "value") {
        alert(activeSheet.getValue(args.row, args.col));
    }
});
spread.suspendEvent();
activeSheet.setValue(0, 0, "111");
spread.resumeEvent();
activeSheet.setValue(1, 1, "222");
```

#### Returns

`void`

___

### <a id="suspendpaint" name="suspendpaint"></a> suspendPaint

▸ **suspendPaint**(): `void`

挂起活动表单和标签条的绘制

#### Returns

`void`

___

### <a id="tojson" name="tojson"></a> toJSON

▸ **toJSON**(`serializationOption?`): `Object`

将对象状态保存为JSON字符串

**`代码示例`**
```
activeSheet.getCell(0,0).value(123);
var jsonStr = null;
//export
jsonStr = JSON.stringify(spread.toJSON());
//import
spread.fromJSON(JSON.parse(jsonStr));
alert(jsonStr);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `serializationOption?` | `Object` | 序列化选项 |

#### Returns

`Object`

___

### <a id="unbind" name="unbind"></a> unbind

▸ **unbind**(`type`, `fn?`): `void`

删除事件到工作簿的绑定

**`代码示例`**
```
//本示例删除事件绑定
activeSheet.bind(GC.Spread.Sheets.Events.CellChanged, function (sender, args) {
    if (args.propertyName === "value") {
        alert(activeSheet.getValue(args.row, args.col));
    }
});
activeSheet.setValue(0, 0, "111");
spread.unbind(GC.Spread.Sheets.Events.CellChanged);
//spread.unbindAll(); //取消监视所有事件
activeSheet.setValue(1, 0, "222");
activeSheet.setValue(2, 0, "333");
activeSheet.setValue(3, 0, "444");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `string` | 事件类型 |
| `fn?` | `Function` | 事件触发时要执行的函数 |

#### Returns

`void`

___

### <a id="unbindall" name="unbindall"></a> unbindAll

▸ **unbindAll**(): `void`

删除所有事件到工作簿的绑定

**`代码示例`**
```
//本示例删除事件绑定 取消批注unbindAll方法以删除所有事件绑定
activeSheet.bind(GC.Spread.Sheets.Events.CellChanged, function (sender, args) {
    if (args.propertyName === "value") {
        alert(activeSheet.getValue(args.row, args.col));
    }
});
activeSheet.setValue(0, 0, "111");
spread.unbind(GC.Spread.Sheets.Events.CellChanged);
//spread.unbindAll(); //取消监视所有事件
activeSheet.setValue(1, 0, "222");
activeSheet.setValue(2, 0, "333");
activeSheet.setValue(3, 0, "444");
```

#### Returns

`void`

___

### <a id="undomanager" name="undomanager"></a> undoManager

▸ **undoManager**(): [`UndoManager`](GC.Spread.Commands.UndoManager.md)

获取撤消管理器

#### Returns

[`UndoManager`](GC.Spread.Commands.UndoManager.md)

撤消管理器

___

### <a id="updateexternalreference" name="updateexternalreference"></a> updateExternalReference

▸ **updateExternalReference**(`linkInfo`, `data?`, `filePath?`, `isMergeUpdate?`): `void`

使用工作簿 JSON 数据或 GC.Spread.Sheets.IO.getPartialValues 的 successCallback 返回结果中的外部值，设置或更新外部数据源的数据

**`代码示例`**
```
// 本示例使用工作簿JSON设置外部源
spread.getActiveSheet().setFormula(0, 0, "[calc.xlsx]Sheet1!A1");  // spread cell A1 value is #REF!
spread2.getActiveSheet().setFormula(0, 0, "=123+1"); \xa0// spread2 cell A1 value is 124
spread.updateExternalReference("calc.xlsx", spread2.toJSON());  // spread cell A1 value is 124
// 使用JSON设置数据
spread.getActiveSheet().setFormula(0, 0, "=SUM([calc.xlsx]Sheet1!A1:B2"); \xa0// spread cell A1 value is #REF!
spread.updateExternalReference("calc.xlsx", {"Sheet1":[[1, 2],[1, 3]]}); \xa0// spread cell A1 value is 7
spread.updateExternalReference("calc.xlsx", {"Sheet1":{0:{0:10, 1:10}, 1:{0:10, 1:10}}}); \xa0// spread cell A1 value is 40
// This example sets the external values with the successCallback result of GC.Spread.Sheets.IO.getPartialValues
let refList = spread.getExternalReferences(true);
GC.Spread.Sheets.IO.getPartialValues(refList, getFile, (externalValues) => {
  // successCallback
  spread.updateExternalReference(externalValues);
}, (errorMsg) => {
  // errorCallback
  console.log(errorMsg);
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `linkInfo` | `string` \| [`ExternalPartialValues`](../modules/GC.Spread.Sheets.md#externalpartialvalues) | 字符串是外部源的文件名，大多以".xlsx"结尾。另一种类型应该是从GC.Spread.Sheets.IO.getPartialValues的回调中获得的外部部分值数组 |
| `data?` | `object` | - |
| `filePath?` | `string` | - |
| `isMergeUpdate?` | `boolean` | Indicates whether to update by merging. If it's not true, the whole external sheet data will be overwritten. |

#### Returns

`void`
