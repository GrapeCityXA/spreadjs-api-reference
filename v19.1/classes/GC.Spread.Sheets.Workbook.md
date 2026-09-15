# Class: Workbook

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).Workbook

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Workbook.md#constructor)

### Properties

- [collaboration](GC.Spread.Sheets.Workbook.md#collaboration)
- [contextMenu](GC.Spread.Sheets.Workbook.md#contextmenu)
- [customPivotTableThemes](GC.Spread.Sheets.Workbook.md#custompivottablethemes)
- [customSlicerThemes](GC.Spread.Sheets.Workbook.md#customslicerthemes)
- [customTableThemes](GC.Spread.Sheets.Workbook.md#customtablethemes)
- [customTimelineThemes](GC.Spread.Sheets.Workbook.md#customtimelinethemes)
- [docProps](GC.Spread.Sheets.Workbook.md#docprops)
- [name](GC.Spread.Sheets.Workbook.md#name)
- [namedCellTemplates](GC.Spread.Sheets.Workbook.md#namedcelltemplates)
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
- [injectAI](GC.Spread.Sheets.Workbook.md#injectai)
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
- [waitForAllCalculations](GC.Spread.Sheets.Workbook.md#waitforallcalculations)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Workbook**(`host?`, `options?`)

表示具有指定托管 DOM 元素或 DOM id 和选项设置的电子表格。

**`example`**
```javascript
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
| `host?` | `string` \| `HTMLElement` | 托管 DOM 元素或 id。 |
| `options?` | [`IWorkBookDefaultOptions`](../interfaces/GC.Spread.Sheets.IWorkBookDefaultOptions.md) | 初始化选项。 |

## Properties

### <a id="collaboration" name="collaboration"></a> collaboration

• **collaboration**: [`Collaboration`](GC.Spread.Sheets.Collaboration.Collaboration.md)

工作簿的协作管理器。

**`example`**
```javascript
var snapshot = workbook.collaboration.toSnapshot();
```

___

### <a id="contextmenu" name="contextmenu"></a> contextMenu

• **contextMenu**: [`ContextMenu`](GC.Spread.Sheets.ContextMenu.ContextMenu.md)

Spread的上下文菜单。

**`example`**
```javascript
//此示例展示如何获取contextMenu的menuData。
var menuData = spread.contextMenu.menuData;
```

___

### <a id="custompivottablethemes" name="custompivottablethemes"></a> customPivotTableThemes

• **customPivotTableThemes**: [`CustomPivotTableThemeManager`](GC.Spread.Pivot.CustomPivotTableThemeManager.md)

表示自定义数据透视表主题管理器。

___

### <a id="customslicerthemes" name="customslicerthemes"></a> customSlicerThemes

• **customSlicerThemes**: [`CustomSlicerThemeManager`](GC.Spread.Sheets.Slicers.CustomSlicerThemeManager.md)

表示自定义项目切片器主题管理器。

___

### <a id="customtablethemes" name="customtablethemes"></a> customTableThemes

• **customTableThemes**: [`CustomTableThemeManager`](GC.Spread.Sheets.Tables.CustomTableThemeManager.md)

表示自定义表格主题管理器。

___

### <a id="customtimelinethemes" name="customtimelinethemes"></a> customTimelineThemes

• **customTimelineThemes**: [`CustomTimelineThemeManager`](GC.Spread.Sheets.Slicers.CustomTimelineThemeManager.md)

表示自定义时间轴切片器主题管理器。

___

### <a id="docprops" name="docprops"></a> docProps

• **docProps**: [`IDocProps`](../interfaces/GC.Spread.Sheets.IDocProps.md)

文档属性。

___

### <a id="name" name="name"></a> name

• **name**: `string`

表示 Spread 控件的名称。

**`example`**
```javascript
spread.name = "Spread1";
```

___

### <a id="namedcelltemplates" name="namedcelltemplates"></a> namedCellTemplates

• **namedCellTemplates**: [`NamedCellTemplatesManager`](GC.Spread.Sheets.NamedCellTemplates.NamedCellTemplatesManager.md)

命名单元格模板管理器。

___

### <a id="options" name="options"></a> options

• **options**: [`IWorkbookOptions`](../interfaces/GC.Spread.Sheets.IWorkbookOptions.md)

表示 Spread 控件的选项。

**`property`** {boolean} allowUserDragMerge - 是否允许用户拖动合并单元格。默认值为 false.

**`property`** {GC.Spread.Sheets.AllowDragHeaderToMove} [options.allowDragHeaderToMove] - 指定如何允许拖动表头移动。默认值为 GC.Spread.Sheets.AllowDragHeaderToMove.none.

**`property`** {boolean} allowUserDragDrop - 是否允许用户拖动和放置范围数据。默认值为 true.

**`property`** {boolean} allowUserDragFill - 是否允许用户拖动填充范围。默认值为 true.

**`property`** {boolean} allowUserZoom - 是否通过按住 Ctrl 键滚动鼠标滚轮来缩放显示。默认值为 true.

**`property`** {boolean} allowUserResize - 是否允许用户调整列和行。默认值为 true.

**`property`** {boolean} allowUndo - 是否允许用户撤销编辑。默认值为 true.

**`property`** {boolean} allowSheetReorder - 是否允许用户重新排列工作表。默认值为 true.

**`property`** {boolean} allowContextMenu - 是否允许用户打开内置上下文菜单。默认值为 true.

**`property`** {boolean} allowUserDeselect - 是否允许用户在选择中使用 deselect。默认值为 true.

**`property`** {GC.Spread.Sheets.Fill.AutoFillType} defaultDragFillType - 默认填充类型。默认值为 GC.Spread.Sheets.Fill.AutoFillType.auto.

**`property`** {boolean} showDragFillSmartTag - 是否显示拖动填充对话框。默认值为 true.

**`property`** {boolean} showHorizontalScrollbar - 是否显示水平滚动条。默认值为 true.

**`property`** {boolean} showVerticalScrollbar - 是否显示垂直滚动条。默认值为 true.

**`property`** {boolean} scrollbarShowMax - 是否根据工作表中的所有列和行显示滚动条。默认值为 true.

**`property`** {boolean} scrollbarMaxAlign - 滚动条是否与活动工作表的最后一行和最后一列对齐。默认值为 false.

**`property`** {boolean} tabStripVisible - 是否显示工作表标签栏。默认值为 true.

**`property`** {number} tabStripRatio - 工作表标签栏的宽度，以水平滚动条宽度的百分比表示。默认值为 0.5.

**`property`** {number} tabStripWidth - 工作表标签栏的宽度，当它位于左侧或右侧时。默认值和最小值为 80。

**`property`** {boolean} tabEditable - 是否允许用户编辑工作表标签栏。默认值为 true.

**`property`** {GC.Spread.Sheets.TabStripPosition} tabStripPosition - 工作表标签栏的位置。默认值为 GC.Spread.Sheets.TabStripPosition.bottom.

**`property`** {boolean} newTabVisible - 是否显示特殊标签以允许用户插入新工作表。默认值为 true.

**`property`** {GC.Spread.Sheets.AllSheetsListVisibility} allSheetsListVisible - 是否显示特殊标签以允许用户打开对话框以显示所有工作表。默认值为 GC.Spread.Sheets.AllSheetsListVisibility.auto.

**`property`** {boolean} tabNavigationVisible - 是否显示工作表标签导航。默认值为 true.

**`property`** {boolean} cutCopyIndicatorVisible - 是否在复制或剪切选中的项目时显示指示器。默认值为 true.

**`property`** {string} cutCopyIndicatorBorderColor - 在用户剪切或复制选中的项目时显示的指示器的边框颜色。默认值为 "#217346".

**`property`** {string} backColor - 用于表示 Spread 组件背景颜色的颜色字符串，如 "red"、"#FFFF00"、"rgb(255,0,0)"、"Accent 5" 等。默认值为 "white".

**`property`** {string} backgroundImage - Spread 组件的背景图像。默认值为 null.

**`property`** {GC.Spread.Sheets.ImageLayout} backgroundImageLayout - Spread 组件的背景图像布局。默认值为 GC.Spread.Sheets.ImageLayout.stretch.

**`property`** {string} grayAreaBackColor - 用于表示灰色区域背景颜色的颜色字符串，如 "red"、"#FFFF00"、"rgb(255,0,0)"、"Accent 5" 等。默认值为 null.

**`property`** {GC.Spread.Sheets.ShowResizeTip} showResizeTip - 如何显示调整大小提示。默认值为 GC.Spread.Sheets.ShowResizeTip.none.

**`property`** {boolean} showDragDropTip - 是否显示拖放提示。默认值为 true.

**`property`** {boolean} showDragFillTip - 是否显示拖放填充提示。默认值为 true.

**`property`** {GC.Spread.Sheets.ShowScrollTip} showScrollTip - 如何显示滚动提示。默认值为 GC.Spread.Sheets.ShowScrollTip.none.

**`property`** {boolean} scrollIgnoreHidden - 滚动条是否忽略隐藏的行或列。默认值为 false.

**`property`** {boolean} highlightInvalidData - 是否高亮显示无效数据。默认值为 false.

**`property`** {boolean} useTouchLayout - 是否使用触摸布局来呈现 Spread 组件。默认值为 false.

**`property`** {boolean} hideSelection - 当 Spread 组件没有焦点时是否显示选择高亮。默认值为 false.

**`property`** {GC.Spread.Sheets.ResizeZeroIndicator} resizeZeroIndicator - 当行或列调整大小时绘制策略。默认值为 GC.Spread.Sheets.ResizeZeroIndicator.enhanced.

**`property`** {boolean} allowUserEditFormula - 是否允许用户在电子表格的单元格中编辑公式。默认值为 true.

**`property`** {boolean} enableFormulaTextbox - 是否在电子表格中启用公式文本框。默认值为 true.

**`property`** {GC.Spread.Sheets.AutoFitType} autoFitType - 内容是否将格式化以适应单元格或单元格和表头。默认值为 GC.Spread.Sheets.AutoFitType.cell.

**`property`** {GC.Spread.Sheets.ReferenceStyle} referenceStyle - 工作簿中单元格公式的单元格和范围引用的样式。默认值为 GC.Spread.Sheets.ReferenceStyle.a1.

**`property`** {boolean} allowDynamicArray - 是否启用动态数组。默认值为 false.

**`property`** {boolean} iterativeCalculation - 是否启用迭代计算。默认值为 true.

**`property`** {number} iterativeCalculationMaximumIterations - 迭代计算时的最大迭代次数。默认值为 1000.

**`property`** {number} iterativeCalculationMaximumChange - 迭代计算时的最大变化。默认值为 0.01.

**`property`** {boolean} calcOnDemand - 是否仅在需要时计算公式。默认值为 false.

**`property`** {boolean} incrementalCalculation - 是否在不阻塞 UI 的情况下增量计算公式。默认值为 false.

**`property`** {boolean} dynamicReferences - 是否计算具有动态引用的函数。默认值为 true.

**`property`** {boolean} allowCopyPasteExcelStyle - 用户是否可以从 Spread Sheets 复制样式然后粘贴到 Excel，或从 Excel 复制样式然后粘贴到 Spread Sheets。默认值为 true.

**`property`** {boolean} allowExtendPasteRange - 如果粘贴范围不足以粘贴，是否扩展粘贴范围。默认值为 false.

**`property`** {GC.Spread.Sheets.CopyPasteHeaderOptions} copyPasteHeaderOptions - 复制或粘贴数据时包含哪些表头。默认值为 GC.Spread.Sheets.CopyPasteHeaderOptions.allHeaders.

**`property`** {GC.Spread.Sheets.CalculationMode} calculationMode - 工作簿的重新计算行为。默认值为 GC.Spread.Sheets.CalculationMode.auto.

**`property`** {boolean} scrollByPixel - 是否启用按像素精确滚动。默认值为 false.

**`property`** {number} scrollPixel - 当 scrollByPixel 为 true 时，决定每次滚动该数量的像素。最终滚动像素是滚动增量乘以 scrollPixel 的结果。例如，滚动增量为 3，scrollPixel 为 5，则最终滚动像素为 15。默认值为 5.

**`property`** {boolean} enableAccessibility - 是否在电子表格中启用辅助功能支持。默认值为 false.

**`property`** {boolean} allowAutoCreateHyperlink - 是否在电子表格中启用自动创建超链接。默认值为 true.

**`property`** {GC.Spread.Sheets.ResizeMode} columnResizeMode - 指定调整列的方式。默认值为 GC.Spread.Sheets.ResizeMode.normal.

**`property`** {GC.Spread.Sheets.ResizeMode} rowResizeMode - 指定调整行的方式。默认值为 GC.Spread.Sheets.ResizeMode.normal.

**`property`** {Array} customList - 用户自定义拖动填充的列表，在每次填充中优先匹配此列表。每个数组项都是字符串数组类型。

**`property`** {GC.Spread.Sheets.ScrollbarAppearance} scrollbarAppearance - 滚动条外观，包含 skin 和 mobile 两个枚举。默认值为 GC.Spread.Sheets.ScrollbarAppearance.skin.

**`property`** {boolean} pasteSkipInvisibleRange - 是否跳过不可见范围进行粘贴。默认值为 false.

**`property`** {boolean} allowAutoExtendFilterRange - 是否允许像 excel 一样自动扩展筛选范围。默认值为 false.

**`property`** {boolean} allowInvalidFormula - 是否允许输入无效的公式字符串。默认值为 false.

**`property`** {boolean} formulaFormatHint - 是否在公式输入时自动生成格式。默认值为 true.

**`property`** {GC.Spread.Pivot.PivotAreaReference} pivotAreaReference  - 选择数据透视表数据区域时是否自动生成 getPivotData 公式或单元格引用。默认值为 GC.Spread.Pivot.PivotAreaReference.getPivotData.

**`property`** {GC.Spread.Sheets.SheetTabStyles} defaultSheetTabStyles - 工作表标签的所有默认状态样式。

**`property`** {GC.Spread.Sheets.IBuiltInFileIcons} [options.builtInFileIcons] - 所有内置文件图标。

**`example`**
```javascript
// var workbook = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:5,showHorizontalScrollbar:false});
var workbook = new GC.Spread.Sheets.Workbook("ss",{sheetCount:5,showHorizontalScrollbar:false});
workbook.options.allowUserDragDrop = false;
workbook.options.allowUserZoom = false;
```

___

### <a id="sheettabstyles" name="sheettabstyles"></a> sheetTabStyles

• **sheetTabStyles**: [`SheetTabStyleManager`](GC.Spread.Sheets.SheetTabStyleManager.md)

表示工作表标签样式管理器。

___

### <a id="sheets" name="sheets"></a> sheets

• **sheets**: [`Worksheet`](GC.Spread.Sheets.Worksheet.md)[]

表示工作表集合。

___

### <a id="touchtoolstrip" name="touchtoolstrip"></a> touchToolStrip

• **touchToolStrip**: [`TouchToolStrip`](GC.Spread.Sheets.Touch.TouchToolStrip.md)

表示触摸工具栏。

## Methods

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

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 自定义名称。 |
| `formula` | `string` | 公式。 |
| `baseRow` | `number` | 行索引。 |
| `baseCol` | `number` | 列索引。 |
| `comment?` | `string` | 自定义注释。 |
| `isReadOnly?` | `boolean` | 自定义名称是否可编辑。 |

#### Returns

`void`

___

### <a id="addnamedstyle" name="addnamedstyle"></a> addNamedStyle

▸ **addNamedStyle**(`style`): `void`

向工作簿的命名样式集合中添加样式。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 要添加的样式。 |

#### Returns

`void`

___

### <a id="addsheet" name="addsheet"></a> addSheet

▸ **addSheet**(`index`, `sheet?`): `void`

在指定索引处插入工作表。

**`example`**
```javascript
//此示例向电子表格添加一个工作表。
spread.addSheet(0,new GC.Spread.Sheets.Worksheet("custom"));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 要添加工作表的索引位置。 |
| `sheet?` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 要添加的工作表。 |

#### Returns

`void`

___

### <a id="addsheettab" name="addsheettab"></a> addSheetTab

▸ **addSheetTab**(`index`, `name`, `type`): `any`

在指定索引处插入工作表标签。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 要添加工作表标签的索引位置。 |
| `name` | `string` | 要添加的工作表标签名称。 |
| `type` | [`SheetType`](../enums/GC.Spread.Sheets.SheetType.md) | 要添加的工作表标签类型。 |

#### Returns

`any`

添加的工作表标签。

___

### <a id="addsparklineex" name="addsparklineex"></a> addSparklineEx

▸ **addSparklineEx**(`sparklineEx`): `void`

向SparklineEx集合添加一个SparklineEx。

**`example`**
```javascript
window.MySparklineEx = function(color) {
    GC.Spread.Sheets.Sparklines.SparklineEx.apply(this, arguments);
    this.typeName = 'MySparklineEx';
    this.color = color;
}
MySparklineEx.prototype = new GC.Spread.Sheets.Sparklines.SparklineEx();
MySparklineEx.prototype.createFunction = function () {
    var func = new GC.Spread.CalcEngine.Functions.Function('CIRCLE', 0, 0);
    func.evaluate = function (args) {
          return {};
    };
    return func;
 };
MySparklineEx.prototype.paint = function (context, value, x, y, width, height) {
     context.beginPath();
     context.arc(x + width / 2, y + height / 2, (Math.min(width, height) - 6) / 2, 0, Math.PI * 2);
     context.strokeStyle = this.color;
     context.stroke();
};
spread.addSparklineEx(new MySparklineEx('green'));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sparklineEx` | [`SparklineEx`](GC.Spread.Sheets.Sparklines.SparklineEx.md) | 要添加的SparklineEx。 |

#### Returns

`void`

___

### <a id="bind" name="bind"></a> bind

▸ **bind**(`type`, `data?`, `fn?`): `void`

为工作簿绑定事件。

**`example`**
```javascript
//此示例将事件绑定到函数。
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
| `type` | `string` | 事件类型。 |
| `data?` | `any` | 指定要传递给函数的附加数据。 |
| `fn?` | `Function` | 指定事件发生时运行的函数。 |

#### Returns

`void`

___

### <a id="calculate" name="calculate"></a> calculate

▸ **calculate**(`type?`, `address?`): `void`

重建、标记脏数据、广播脏数据并重新计算公式。
首先根据计算类型在地址中重建并标记脏数据。
然后广播脏数据将递归地将工作簿中脏单元格的依赖项设置为脏。
在自动模式下，所有脏单元格都将被计算。
在手动模式下，只计算地址中的单元格，其他单元格保持脏状态。
如果CalcService被暂停，将跳过重新计算。

**`example`**
```javascript
spread.sheets[0].setFormula(0,0,"RAND()");
spread.sheets[0].setFormula(1,0,"=Sheet2!A1");
spread.sheets[0].setFormula(2,0,"=1+2");
spread.sheets[1].setFormula(0,0,"RAND()");
spread.sheets[1].setFormula(1,0,"=Sheet1!A1");

// 所有单元格都被重新计算。
spread.calculate();
spread.calculate(GC.Spread.Sheets.CalculationType.regular);

// Sheet1!A1 Sheet2!A2被计算为新数字，Sheet1!A2 Sheet1!A3也被计算。
spread.calculate(GC.Spread.Sheets.CalculationType.all, "Sheet1");

// Sheet1!A1 Sheet2!A2被计算为新数字。
spread.calculate(GC.Spread.Sheets.CalculationType.regular, "Sheet1!A1");

// 没有单元格被计算。
spread.calculate(GC.Spread.Sheets.CalculationType.regular, "Sheet1!A2");

spread.options.calculationMode = GC.Spread.Sheets.CalculationMode.manual; // 切换到手动模式

// Sheet1!A1被计算为新数字，Sheet1!A2 Sheet1!A3被计算但未改变，Sheet2!A2在手动模式下保持脏状态。
spread.calculate(GC.Spread.Sheets.CalculationType.all, "Sheet1");

// Sheet1!A1被计算为新数字，Sheet2!A2在手动模式下保持脏状态。
spread.calculate(GC.Spread.Sheets.CalculationType.regular, "Sheet1");

// Sheet2!A2因为脏而被计算。
spread.calculate(GC.Spread.Sheets.CalculationType.minimal);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type?` | [`CalculationType`](../enums/GC.Spread.Sheets.CalculationType.md) | 指定计算的重建和标记脏数据类型。 |
| `address?` | `string` | 指定要标记脏数据并计算的工作表或范围。如果省略，则为整个工作簿。 注意，在自动模式下，范围外的脏依赖项也将被计算。 |

#### Returns

`void`

___

### <a id="changesheetindex" name="changesheetindex"></a> changeSheetIndex

▸ **changeSheetIndex**(`sheetName`, `targetIndex`): `boolean`

更改工作表索引并重新排序工作表。

**`example`**
```javascript
//此示例展示如何更改工作表索引。
var spread = GC.Spread.Sheets.findControl(ss);
spread.setSheetCount(5); // 工作表顺序应为 "Sheet1", "Sheet2", "Sheet3", "Sheet4", "Sheet5"。
spread.changeSheetIndex("Sheet1", 3); // 工作表顺序应为 "Sheet2", "Sheet3", "Sheet4", "Sheet1", "Sheet5"。
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheetName` | `string` | 工作表名称。 |
| `targetIndex` | `number` | 目标索引。 |

#### Returns

`boolean`

___

### <a id="changesheetposition" name="changesheetposition"></a> changeSheetPosition

▸ **changeSheetPosition**(`sheetName`, `targetPosition`): `boolean`

更改工作表位置并重新排序工作表。

**`example`**
```javascript
//此示例展示如何更改工作表位置。
var spread = GC.Spread.Sheets.findControl(ss);
spread.setSheetCount(5);
spread.addSheetTab(0, "tableSheet1", GC.Spread.Sheets.SheetType.tableSheet); // 工作表顺序应为 "Sheet1", "Sheet2", "Sheet3", "Sheet4", "Sheet5", "tableSheet1"。
spread.changeSheetPosition("tableSheet1", 3); // 工作表顺序应为 "Sheet1", "Sheet2", "Sheet3", "tableSheet1", "Sheet4", "Sheet5"。
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheetName` | `string` | 工作表名称。 |
| `targetPosition` | `number` | 目标位置。 |

#### Returns

`boolean`

___

### <a id="clearcustomfunctions" name="clearcustomfunctions"></a> clearCustomFunctions

▸ **clearCustomFunctions**(): `void`

清除所有自定义函数。

#### Returns

`void`

___

### <a id="clearcustomnames" name="clearcustomnames"></a> clearCustomNames

▸ **clearCustomNames**(): `void`

清除自定义名称。

#### Returns

`void`

___

### <a id="clearsheettabs" name="clearsheettabs"></a> clearSheetTabs

▸ **clearSheetTabs**(): `void`

清除控件中的所有工作表标签。

#### Returns

`void`

___

### <a id="clearsheets" name="clearsheets"></a> clearSheets

▸ **clearSheets**(): `void`

清除控件中的所有工作表。

**`example`**
```javascript
//此示例使用clearSheets方法。
spread.clearSheets();
```

#### Returns

`void`

___

### <a id="commandmanager" name="commandmanager"></a> commandManager

▸ **commandManager**(): [`CommandManager`](GC.Spread.Commands.CommandManager.md)

获取命令管理器。

**`example`**
```javascript
//此示例执行一个执行指定操作的命令。
spread.options.allowUndo = true;
spread.commandManager().execute({cmd: "outlineRow", sheetName: "Sheet1", index: 3, count: 5});
```

#### Returns

[`CommandManager`](GC.Spread.Commands.CommandManager.md)

命令管理器。

___

### <a id="datamanager" name="datamanager"></a> dataManager

▸ **dataManager**(): [`DataManager`](GC.Data.DataManager.md)

获取数据管理器。

#### Returns

[`DataManager`](GC.Data.DataManager.md)

返回数据管理器。

___

### <a id="defaultpivottabletheme" name="defaultpivottabletheme"></a> defaultPivotTableTheme

▸ **defaultPivotTableTheme**(`themeName?`): `undefined` \| [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md)

设置或获取默认数据透视表主题。

**`example`**
```javascript
// 将默认数据透视表主题名称设置为 "custom0"
spread.defaultPivotTableTheme("custom0");
let newPivotTable = activeSheet.pivotTables.add("pivotTable1", 1, 1, 10, 5);
// 由于未指定特定主题，上面的数据透视表将使用 "custom0" 作为主题。

// 获取默认数据透视表主题
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

设置或获取默认切片器主题。

**`example`**
```javascript
// 将默认切片器主题名称设置为 "custom0"
spread.defaultSlicerTheme("custom0");
let newSlicer = activeSheet.slicers.add("slicer1", 1, 1, 10, 5);
// 由于未指定特定主题，上面的切片器将使用 "custom0" 作为主题。

// 获取默认切片器主题
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

设置或获取默认表格主题。

**`example`**
```javascript
// 将默认表格主题名称设置为 "custom0"
spread.defaultTableTheme("custom0");
let newable = activeSheet.tables.add("table1", 1, 1, 10, 5);
// 由于未指定特定主题，上面的表格将使用 "custom0" 作为主题。

// 获取默认表格主题
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

设置或获取默认时间线主题。

**`example`**
```javascript
// 将默认时间线主题名称设置为 "custom0"
spread.defaultTimelineTheme("custom0");
let newTimeline = activeSheet.timeLines.add("timeLine1", 1, 1, 10, 5);
// 由于未指定特定主题，上面的时间线将使用 "custom0" 作为主题。

// 获取默认时间线主题
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

销毁工作簿及其包含的所有工作表。

**`example`**
```javascript
//此示例销毁工作簿实例。
spread.destroy();
```

#### Returns

`void`

___

### <a id="export" name="export"></a> export

▸ **export**(`successCallBack?`, `errorCallBack?`, `exportOptions?`): `void`

将对象状态导出为 excel、ssjson 或 csv 文件。

**`example`**
```javascript
spread.export(function (blob) {
   // 将 blob 保存到文件
   saveAs(blob, fileName);
}, function (e) {
   console.log(e);
}, {
   fileType: GC.Spread.Sheets.FileType.excel,
   includeBindingSource: true
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `successCallBack?` | `Function` | 导出对象状态完成时的成功回调，接受 Blob 作为参数。 |
| `errorCallBack?` | `Function` | 导出对象状态出错时的错误回调。 |
| `exportOptions?` | [`ExportOptions`](../modules/GC.Spread.Sheets.md#exportoptions) | 导出选项。 |

#### Returns

`void`

___

### <a id="focus" name="focus"></a> focus

▸ **focus**(`focusIn?`): `void`

使工作簿组件获得或失去焦点。

**`example`**
```javascript
//此示例设置 Spread 控件的焦点。
$("#button1").click(function () {
spread.focus(true);
   });
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `focusIn?` | `boolean` | `false` 使工作簿组件失去焦点；否则获得焦点。 |

#### Returns

`void`

___

### <a id="fromjson" name="fromjson"></a> fromJSON

▸ **fromJSON**(`workbookData`, `deserializationOptions?`): `Promise`<`any`\>

从指定的 JSON 字符串加载对象状态。

**`example`**
```javascript
//此示例使用 fromJSON 方法。
activeSheet.getCell(0,0).value(123);
var jsonStr = null;
//导出
jsonStr = JSON.stringify(spread.toJSON());
//导入
var fromJSONPromise = spread.fromJSON(JSON.parse(jsonStr));
fromJSONPromise.then(() => {
     alert(jsonStr);
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workbookData` | `Object` | 反序列化后的电子表格数据。 |
| `deserializationOptions?` | [`IDeserializationOptions`](../interfaces/GC.Spread.Sheets.IDeserializationOptions.md) | 反序列化选项。 |

#### Returns

`Promise`<`any`\>

- fromJSON Promise。

___

### <a id="getactivesheet" name="getactivesheet"></a> getActiveSheet

▸ **getActiveSheet**(): [`Worksheet`](GC.Spread.Sheets.Worksheet.md)

获取活动工作表。

#### Returns

[`Worksheet`](GC.Spread.Sheets.Worksheet.md)

活动工作表实例。

___

### <a id="getactivesheetindex" name="getactivesheetindex"></a> getActiveSheetIndex

▸ **getActiveSheetIndex**(): `number`

获取控件的活动工作表索引。

**`example`**
```javascript
//此示例使用 getActiveSheetIndex 方法。
var index = spread.getActiveSheetIndex();
alert(index);
```

#### Returns

`number`

活动工作表索引。

___

### <a id="getactivesheettab" name="getactivesheettab"></a> getActiveSheetTab

▸ **getActiveSheetTab**(): `any`

获取活动工作表标签。

#### Returns

`any`

活动工作表标签实例。

___

### <a id="getactivesheettabindex" name="getactivesheettabindex"></a> getActiveSheetTabIndex

▸ **getActiveSheetTabIndex**(): `number`

获取控件的活动工作表标签索引。

#### Returns

`number`

活动工作表标签索引。

___

### <a id="getcircularreference" name="getcircularreference"></a> getCircularReference

▸ **getCircularReference**(): [`ICellsInfo`](../interfaces/GC.Spread.Sheets.ICellsInfo.md)[]

获取工作簿中所有循环引用单元格的信息。

**`example`**
```javascript
spread.getCircularReference();
```

#### Returns

[`ICellsInfo`](../interfaces/GC.Spread.Sheets.ICellsInfo.md)[]

返回循环引用单元格信息对象数组
cellsInfo.row {number} 表示单元格范围的行索引。
cellsInfo.col {number} 表示单元格范围的列索引。
cellsInfo.rowCount {number} 表示单元格范围的行数。
cellsInfo.colCount {number} 表示单元格范围的列数。
cellsInfo.sheetName {string} 表示工作表名称。

___

### <a id="getcustomfunction" name="getcustomfunction"></a> getCustomFunction

▸ **getCustomFunction**(`name`): `void`

获取自定义函数。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 自定义函数名称。 |

#### Returns

`void`

自定义函数。

___

### <a id="getcustomname" name="getcustomname"></a> getCustomName

▸ **getCustomName**(`name`): [`NameInfo`](GC.Spread.Sheets.NameInfo.md)

获取指定的自定义名称信息。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 自定义名称。 |

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

### <a id="getexternalreferences" name="getexternalreferences"></a> getExternalReferences

▸ **getExternalReferences**(`includeItemDetail?`): [`IExternalReference`](../interfaces/GC.Spread.Sheets.IExternalReference.md)[]

获取当前工作簿的跨工作簿引用列表。

**`example`**
```javascript
//此示例获取并更新使用的数据源。
spread.getActiveSheet().setFormula(0, 0, "='[Jackson.xlsx]Sheet1'!B6+SUM('[Petrosky.xlsx]Sheet2'!B7:B8)");
spread.getExternalReferences().forEach(item=>{
     spread.updateExternalReference(item.name, spreadList[item.name], item.filePath);
})
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `includeItemDetail?` | `boolean` | 指定是否包含目标单元格和源范围。默认值为 false. |

#### Returns

[`IExternalReference`](../interfaces/GC.Spread.Sheets.IExternalReference.md)[]

externalReference 数组。<br/>
externalReference.name {string} 跨工作簿引用的文件名。<br/>
externalReference.filePath {string} 跨工作簿引用的文件路径。

___

### <a id="gethost" name="gethost"></a> getHost

▸ **getHost**(): `HTMLElement`

获取当前 Workbook 实例的主机元素。

#### Returns

`HTMLElement`

host 当前 Workbook 实例的主机元素。

___

### <a id="getnamedstyle" name="getnamedstyle"></a> getNamedStyle

▸ **getNamedStyle**(`name`): [`Style`](GC.Spread.Sheets.Style.md)

从 Workbook 命名样式集合中获取具有指定名称的样式。

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

从 Workbook 获取命名样式。

#### Returns

[`Style`](GC.Spread.Sheets.Style.md)[]

命名样式的 GC.Spread.Sheets.Style 数组。

___

### <a id="getsheet" name="getsheet"></a> getSheet

▸ **getSheet**(`index`): [`Worksheet`](GC.Spread.Sheets.Worksheet.md)

获取指定的工作表。

**`example`**
```javascript
//此示例获取工作表并设置单元格前景色。
var sheet1 = spread.getSheet(1);
sheet1.getCell(0,0).value("A1").foreColor("red");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 要返回的工作表索引。 |

#### Returns

[`Worksheet`](GC.Spread.Sheets.Worksheet.md)

指定的工作表。

___

### <a id="getsheetcount" name="getsheetcount"></a> getSheetCount

▸ **getSheetCount**(): `number`

获取工作表的数量。

**`example`**
```javascript
//此示例使用getSheetCount方法。
var index = spread.getSheetCount();
alert(index);
```

#### Returns

`number`

工作表的数量。

___

### <a id="getsheetfromname" name="getsheetfromname"></a> getSheetFromName

▸ **getSheetFromName**(`name`): [`Worksheet`](GC.Spread.Sheets.Worksheet.md)

获取指定名称的工作表。

**`example`**
```javascript
//此示例获取工作表并设置单元格前景色。
var sheet1 = spread.getSheetFromName("Sheet2");
sheet1.getCell(0,0).value("A1").foreColor("red");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 工作表名称。 |

#### Returns

[`Worksheet`](GC.Spread.Sheets.Worksheet.md)

指定名称的工作表。

___

### <a id="getsheetindex" name="getsheetindex"></a> getSheetIndex

▸ **getSheetIndex**(`name`): `number`

获取指定名称的工作表索引。

**`example`**
```javascript
//此示例使用getSheetIndex方法。
spread.setSheetCount(5);
var index = spread.getSheetIndex("Sheet2");
alert(index); // 1
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 工作表名称。 |

#### Returns

`number`

基于Worksheet集合的工作表索引。

___

### <a id="getsheetposition" name="getsheetposition"></a> getSheetPosition

▸ **getSheetPosition**(`name`): `number`

获取指定名称的工作表标签位置。

**`example`**
```javascript
//此示例使用getSheetPosition方法。
spread.setSheetCount(5);
spread.addSheetTab(0, "tableSheet1", GC.Spread.Sheets.SheetType.tableSheet);
var position = spread.getSheetPosition("tableSheet1");
alert(position); // 5
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 工作表标签名称。 |

#### Returns

`number`

基于Worksheet和TableSheet集合的工作表标签位置。

___

### <a id="getsheettab" name="getsheettab"></a> getSheetTab

▸ **getSheetTab**(`indexOrName`): `any`

通过索引或名称获取指定的工作表标签。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `indexOrName` | `string` \| `number` | 要返回的工作表标签的索引或名称。 |

#### Returns

`any`

指定的工作表标签。

___

### <a id="getsheettabcount" name="getsheettabcount"></a> getSheetTabCount

▸ **getSheetTabCount**(): `number`

获取工作表标签的数量。

#### Returns

`number`

工作表标签的数量。

___

### <a id="getsheettabindex" name="getsheettabindex"></a> getSheetTabIndex

▸ **getSheetTabIndex**(`name`): `number`

获取指定名称的工作表标签索引。

**`example`**
```javascript
//此示例使用getSheetTabIndex方法。
spread.setSheetCount(5);
spread.addSheetTab(0, "tableSheet1", GC.Spread.Sheets.SheetType.tableSheet);
var index = spread.getSheetTabIndex("tableSheet1");
alert(index); // 0
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 工作表标签名称。 |

#### Returns

`number`

基于TabSheet集合的工作表标签索引。

___

### <a id="hittest" name="hittest"></a> hitTest

▸ **hitTest**(`x`, `y`): [`IWorkbookHitTestInformation`](../interfaces/GC.Spread.Sheets.IWorkbookHitTestInformation.md)

执行点击测试。

**`example`**
```javascript
//此示例使用 hitTest 方法。
      window.onload = function(){
          var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
          var activeSheet = spread.getActiveSheet();
          $("#ss").click(function (e) {
              //从既不是固定行/列也不是行/列表头的常规单元格的鼠标点击点获取单元格索引。
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
| `x` | `number` | 相对于电子表格水平轴的 <i>x</i> 坐标。 |
| `y` | `number` | 相对于电子表格垂直轴的 <i>y</i> 坐标。 |

#### Returns

[`IWorkbookHitTestInformation`](../interfaces/GC.Spread.Sheets.IWorkbookHitTestInformation.md)

点击测试信息。如果选择工作表，则返回工作表信息。该信息包含 x、y 和 worksheetHitInfo；
如果选择工作表标签栏，则返回工作表标签栏信息。该信息包含 x、y 和 tabStripHitInfo；
如果选择水平滚动条，则返回水平滚动条信息。该信息包含 x、y 和 horizontalScrollBarHitInfo；
如果选择垂直滚动条，则返回垂直滚动条信息。该信息包含 x、y 和 verticalScrollBarHitInfo；
如果选择页脚角落，则返回页脚角落信息。该信息包含 x、y 和 footerCornerHitInfo。

___

### <a id="import" name="import"></a> import

▸ **import**(`file`, `successCallback?`, `errorCallback?`, `importOptions?`): `void`

从 excel 或 ssJson 或 csv 文件或 javascript 文件导入对象状态。

**`example`**
```javascript
//此示例使用 import 方法。
//获取文件 blob。
var file = document.getElementById("importFileName").files[0];
// 导入
spread.import(file, function () {
   // 成功回调以执行某些操作
}, function (e) {
   console.log(e); // 错误回调
}, {
   fileType: GC.Spread.Sheets.FileType.excel
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `file` | `File` | 用于导入的 ssJson 或 csv 或 Excel 文件或 javascript 文件。 |
| `successCallback?` | `Function` | - |
| `errorCallback?` | `Function` | - |
| `importOptions?` | [`ImportOptions`](../modules/GC.Spread.Sheets.md#importoptions) | 导入选项。 |

#### Returns

`void`

___

### <a id="injectai" name="injectai"></a> injectAI

▸ **injectAI**(`callbackOrEnv`): `void`

将 AI 回调函数或环境注入到工作簿中。

**`example`**
```javascript
// 1. 如果您不担心暴露 API 密钥，则注入环境
workbook.injectAI({
    model: 'your model',
    key: 'your-api-key',
    basePath: 'your base path'
});

// 2. 如果您想控制请求主体并自己发送到 AI 服务，则注入请求回调
const httpCallback = async (requestBody) => {
    const AI_BATH_PATH = 'your base path';
    const AI_KEY = 'your api key';

    requestBody.model = 'your model name';

    const response = await fetch(AI_BASE_PATH, {
        method: 'POST',
        headers: {
            'Authorization': `Bearer ${AI_KEY}`,
            'Content-Type': 'application/json'
        },
        body: JSON.stringify(requestBody)
    });

    if (!response.ok) {
        throw new Error(`HTTP error! status: ${response.status}`);
    }
    return response;
};
workbook.injectAI(httpCallback);

// 3. 如果您想将请求发送到您的服务器，然后发送到 AI 服务，则注入请求回调
const serverCallback = async (requestBody) => {
    requestBody.model = 'your model name';
    let response = await fetch('/api/queryAI', {
        method: 'POST',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify(requestBody)
    });
    if (!response.ok) {
        throw new Error(`HTTP error! status: ${response.status}`);
    }
    return response;
}
workbook.injectAI(serverCallback);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `callbackOrEnv` | [`AIRequestCallback`](../modules/GC.Spread.Sheets.AI.md#airequestcallback) \| [`IAIEnvironment`](../modules/GC.Spread.Sheets.AI.md#iaienvironment) | AI 请求的回调函数，它将发送 AI 请求的主体到 AI 请求的环境，SpreadJS 将发送请求到 AI 服务。 |

#### Returns

`void`

___

### <a id="invalidatelayout" name="invalidatelayout"></a> invalidateLayout

▸ **invalidateLayout**(): `void`

更新控件布局信息。

**`example`**
```javascript
//此示例更新布局。
spread.invalidateLayout();
spread.repaint();
```

#### Returns

`void`

___

### <a id="ispaintsuspended" name="ispaintsuspended"></a> isPaintSuspended

▸ **isPaintSuspended**(): `boolean`

获取电子表格绘制是否已暂停。

#### Returns

`boolean`

___

### <a id="nextcontrol" name="nextcontrol"></a> nextControl

▸ **nextControl**(`value?`): `any`

获取或设置由 GC.Spread.Sheets.Actions.selectNextControl 和 GC.Spread.Sheets.Actions.moveToNextCellThenControl 使用的下一个控件。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `HTMLElement` | 下一个控件。该控件必须具有 focus 方法。 |

#### Returns

`any`

如果未设置值，则返回下一个控件；否则返回电子表格。

___

### <a id="open" name="open"></a> open

▸ **open**(`file`, `successCallback?`, `errorCallback?`, `openOptions?`): `void`

从 sjs 压缩文件加载对象状态。

**`example`**
```javascript
//此示例使用 open 方法。
//获取文件 blob。
var file = document.getElementById("importFileName").files[0];
// 导入
spread.open(file, function () {
   // 成功回调以执行某些操作
}, function (e) {
 console.log(e); // 错误回调
}, { openMode: GC.Spread.Sheets.OpenMode.lazy });
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `file` | `File` | 压缩的电子表格数据文件。 |
| `successCallback?` | `Function` | - |
| `errorCallback?` | `Function` | - |
| `openOptions?` | [`OpenOptions`](../modules/GC.Spread.Sheets.md#openoptions) | 反序列化选项。 |

#### Returns

`void`

___

### <a id="pageinfo" name="pageinfo"></a> pageInfo

▸ **pageInfo**(`sheetIndex?`): `any`

获取工作表的页面信息

**`example`**
```javascript
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
| `sheetIndex?` | `number` | 工作表索引。 |

#### Returns

`any`

返回工作表的页面信息，如果忽略工作表索引，则返回所有工作表的页面信息数组

___

### <a id="previouscontrol" name="previouscontrol"></a> previousControl

▸ **previousControl**(`value?`): `any`

获取或设置由 GC.Spread.Sheets.Actions.selectPreviousControl 和 GC.Spread.Sheets.Actions.moveToPreviousCellThenControl 使用的前一个控件。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `HTMLElement` | 前一个控件。该控件必须具有 focus 方法。 |

#### Returns

`any`

如果未设置值，则返回前一个控件；否则返回电子表格。

___

### <a id="print" name="print"></a> print

▸ **print**(`sheetIndex?`): `void`

打印指定的工作表。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheetIndex?` | `number` | 工作表索引。如果忽略工作表索引，则打印所有可见的工作表。 |

#### Returns

`void`

___

### <a id="refresh" name="refresh"></a> refresh

▸ **refresh**(): `void`

手动刷新 Workbook 对象的布局和渲染。

**`example`**
```javascript
//此示例使用 refresh 方法。
spread.refresh();
```

#### Returns

`void`

___

### <a id="removecustomfunction" name="removecustomfunction"></a> removeCustomFunction

▸ **removeCustomFunction**(`name`): `void`

移除自定义函数。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 自定义函数名称。 |

#### Returns

`void`

___

### <a id="removecustomname" name="removecustomname"></a> removeCustomName

▸ **removeCustomName**(`name`): `void`

移除指定的自定义名称。

**`example`**
```javascript
//此示例使用 removeCustomName 方法。
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
| `name` | `string` | 自定义名称。 |

#### Returns

`void`

___

### <a id="removenamedstyle" name="removenamedstyle"></a> removeNamedStyle

▸ **removeNamedStyle**(`name`): `void`

从工作簿命名样式集合中移除具有指定名称的样式。

**`example`**
```javascript
var namedStyle = new GC.Spread.Sheets.Style();
namedStyle.name = "style1";
namedStyle.backColor = "green";
spread.addNamedStyle(namedStyle);
activeSheet.setStyleName(1, 1, "style1"); // 单元格(1,1)的背景色为绿色
activeSheet.setStyleName(2, 1, "style1");
var style = spread.getNamedStyle("style1");
style.foreColor = "red";    // 命名样式的前景色为红色
activeSheet.repaint(); // 单元格(1,1)和单元格(2,1)的前景色为红色
activeSheet.getCell(1,1).value("test");
$("#button1").click(function () {
     spread.removeNamedStyle("style1");
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要移除的样式名称。 |

#### Returns

`void`

___

### <a id="removesheet" name="removesheet"></a> removeSheet

▸ **removeSheet**(`index`): `void`

移除指定的工作表。

**`example`**
```javascript
//此示例从电子表格中移除一个工作表。
spread.setSheetCount(5);
spread.removeSheet(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 要移除的工作表索引。 |

#### Returns

`void`

___

### <a id="removesheettab" name="removesheettab"></a> removeSheetTab

▸ **removeSheetTab**(`indexOrName`): `void`

通过索引或名称移除指定的工作表标签。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `indexOrName` | `string` \| `number` | 要移除的工作表标签的索引或名称。 |

#### Returns

`void`

___

### <a id="removesparklineex" name="removesparklineex"></a> removeSparklineEx

▸ **removeSparklineEx**(`name`): `void`

从SparklineEx集合中移除一个SparklineEx。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要移除的SparklineEx的名称。 |

#### Returns

`void`

___

### <a id="repaint" name="repaint"></a> repaint

▸ **repaint**(): `void`

重绘工作簿控件。

**`example`**
```javascript
//此示例更新布局。
spread.invalidateLayout();
spread.repaint();
```

#### Returns

`void`

___

### <a id="resumecalcservice" name="resumecalcservice"></a> resumeCalcService

▸ **resumeCalcService**(`recalcAll?`): `void`

恢复计算服务。

**`example`**
```javascript
//此示例使用resumeCalcService方法。
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
| `recalcAll?` | `boolean` | 指定是否重新计算所有公式。 |

#### Returns

`void`

___

### <a id="resumeevent" name="resumeevent"></a> resumeEvent

▸ **resumeEvent**(): `void`

恢复事件。

**`example`**
```javascript
//此示例演示了暂停和恢复事件。
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

恢复活动工作表和标签栏的绘制。

#### Returns

`void`

___

### <a id="save" name="save"></a> save

▸ **save**(`successCallBack?`, `errorCallBack?`, `saveOptions?`): `void`

将 spreadJS 状态保存为 sjs 文件。

**`example`**
```javascript
spread.save(function (blob) {
   // 将 blob 保存到文件
   saveAs(blob, fileName);
}, function (e) {
   console.log(e);
}, { includeUnusedNames: false });
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `successCallBack?` | `Function` | 保存 spreadJS 状态完成时的成功回调函数，接受 Blob 作为参数。 |
| `errorCallBack?` | `Function` | 保存 spreadJS 状态出错时的错误回调函数。 |
| `saveOptions?` | [`SaveOptions`](../modules/GC.Spread.Sheets.md#saveoptions) | 保存选项。 |

#### Returns

`void`

___

### <a id="savepdf" name="savepdf"></a> savePDF

▸ **savePDF**(`successCallback`, `errorCallback`, `options?`, `sheetIndex?`): `void`

将指定工作表导出为 PDF。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `successCallback` | `Function` | 导出成功时调用的函数。function (blob) {}。 |
| `errorCallback` | `Function` | 发生错误时调用的函数。异常参数对象结构为 { errorCode: GC.Spread.Sheets.PDF.ErrorCode, errorMessage: string}。 |
| `options?` | `Object` | 导出 PDF 的选项。 |
| `sheetIndex?` | `number` | 工作表索引。如果忽略工作表索引，则导出所有可见工作表。 |

#### Returns

`void`

___

### <a id="search" name="search"></a> search

▸ **search**(`searchCondition`): [`SearchResult`](GC.Spread.Sheets.Search.SearchResult.md)

使用指定的条件在指定工作表的单元格中搜索指定的文本。

**`example`**
```javascript
//此示例使用指定的搜索条件搜索活动工作表。
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
| `searchCondition` | [`SearchCondition`](GC.Spread.Sheets.Search.SearchCondition.md) | 搜索条件。 |

#### Returns

[`SearchResult`](GC.Spread.Sheets.Search.SearchResult.md)

搜索结果。

___

### <a id="setactivesheet" name="setactivesheet"></a> setActiveSheet

▸ **setActiveSheet**(`name`): `void`

通过名称设置活动工作表。

**`example`**
```javascript
//此示例设置活动工作表。
spread.setSheetCount(3);
spread.setActiveSheet("Sheet2");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要设置为活动工作表的工作表名称。 |

#### Returns

`void`

___

### <a id="setactivesheetindex" name="setactivesheetindex"></a> setActiveSheetIndex

▸ **setActiveSheetIndex**(`value`): `void`

设置控件的活动工作表索引。

**`example`**
```javascript
//此示例使用 setActiveSheetIndex 方法。
spread.setActiveSheetIndex(1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `number` | 活动工作表索引。 |

#### Returns

`void`

___

### <a id="setactivesheettab" name="setactivesheettab"></a> setActiveSheetTab

▸ **setActiveSheetTab**(`indexOrName`): `void`

通过索引或名称设置活动工作表标签。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `indexOrName` | `string` \| `number` | 要设置为活动工作表标签的工作表标签的索引或名称。 |

#### Returns

`void`

___

### <a id="setsheetcount" name="setsheetcount"></a> setSheetCount

▸ **setSheetCount**(`count`): `void`

设置工作表数量。

**`example`**
```javascript
spread.setSheetCount(5);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `count` | `number` | 工作表数量。 |

#### Returns

`void`

___

### <a id="startsheetindex" name="startsheetindex"></a> startSheetIndex

▸ **startSheetIndex**(`value?`): `any`

获取或设置电子表格中显示的第一个工作表的索引。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 电子表格中显示的第一个工作表的索引。 |

#### Returns

`any`

如果未设置值，则返回电子表格中显示的第一个工作表的索引；否则返回电子表格。

___

### <a id="suspendcalcservice" name="suspendcalcservice"></a> suspendCalcService

▸ **suspendCalcService**(`ignoreDirty?`): `void`

暂停计算服务。

**`example`**
```javascript
//此示例使用 suspendCalcService 方法。
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
| `ignoreDirty?` | `boolean` | 指定是否使依赖单元格失效。 |

#### Returns

`void`

___

### <a id="suspendevent" name="suspendevent"></a> suspendEvent

▸ **suspendEvent**(): `void`

暂停事件。

**`example`**
```javascript
//此示例暂停和恢复事件。
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

暂停活动工作表和标签栏的绘制。

#### Returns

`void`

___

### <a id="tojson" name="tojson"></a> toJSON

▸ **toJSON**(`serializationOption?`): `Object`

将对象状态保存为 JSON 字符串。

**`example`**
```javascript
activeSheet.getCell(0,0).value(123);
var jsonStr = null;
// 导出
jsonStr = JSON.stringify(spread.toJSON());
// 导入
spread.fromJSON(JSON.parse(jsonStr));
alert(jsonStr);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `serializationOption?` | [`ISerializationOption`](../interfaces/GC.Spread.Sheets.ISerializationOption.md) | 序列化选项。 |

#### Returns

`Object`

电子表格数据。

___

### <a id="unbind" name="unbind"></a> unbind

▸ **unbind**(`type`, `fn?`): `void`

移除 Workbook 的事件绑定。

**`example`**
```javascript
//此示例移除事件绑定。
activeSheet.bind(GC.Spread.Sheets.Events.CellChanged, function (sender, args) {
    if (args.propertyName === "value") {
        alert(activeSheet.getValue(args.row, args.col));
    }
});
activeSheet.setValue(0, 0, "111");
spread.unbind(GC.Spread.Sheets.Events.CellChanged);
//spread.unbindAll(); //取消所有事件的监控。
activeSheet.setValue(1, 0, "222");
activeSheet.setValue(2, 0, "333");
activeSheet.setValue(3, 0, "444");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `string` | 事件类型。 |
| `fn?` | `Function` | 指定在事件发生时运行的函数。 |

#### Returns

`void`

___

### <a id="unbindall" name="unbindall"></a> unbindAll

▸ **unbindAll**(): `void`

移除 Workbook 的所有事件绑定。

**`example`**
```javascript
//此示例移除事件绑定。取消注释 unbindAll 方法以移除所有事件绑定。
activeSheet.bind(GC.Spread.Sheets.Events.CellChanged, function (sender, args) {
    if (args.propertyName === "value") {
        alert(activeSheet.getValue(args.row, args.col));
    }
});
activeSheet.setValue(0, 0, "111");
spread.unbind(GC.Spread.Sheets.Events.CellChanged);
//spread.unbindAll(); //取消所有事件的监控。
activeSheet.setValue(1, 0, "222");
activeSheet.setValue(2, 0, "333");
activeSheet.setValue(3, 0, "444");
```

#### Returns

`void`

___

### <a id="undomanager" name="undomanager"></a> undoManager

▸ **undoManager**(): [`UndoManager`](GC.Spread.Commands.UndoManager.md)

获取与该工作簿实例关联的撤销管理器。
该撤销管理器负责处理电子表格中用户操作的撤销（Undo）与重做（Redo）操作。
它会维护一个操作历史栈，存储所有可被撤销或重新执行的操作记录。

**`example`**
```javascript
// 获取撤销管理器
var undoManager = workbook.undoManager();
// 检查是否可以撤销
if (undoManager.canUndo()) {
    // 执行撤销操作
    undoManager.undo();
}
// 检查是否可以重做
if (undoManager.canRedo()) {
    // 执行重做操作
    undoManager.redo();
}
```

#### Returns

[`UndoManager`](GC.Spread.Commands.UndoManager.md)

撤销管理器。

___

### <a id="updateexternalreference" name="updateexternalreference"></a> updateExternalReference

▸ **updateExternalReference**(`linkInfo`, `data?`, `filePath?`, `isMergeUpdate?`): `void`

使用工作簿 JSON 或来自 GC.Spread.Sheets.IO.getPartialValues 的 successCallback 结果的外部值设置或更新外部源的数据。

**`example`**
```javascript
// 此示例使用工作簿 JSON 设置外部源。
spread.getActiveSheet().setFormula(0, 0, "[calc.xlsx]Sheet1!A1");  // spread 单元格 A1 的值为 #REF!
spread2.getActiveSheet().setFormula(0, 0, "=123+1"); \xa0// spread2 单元格 A1 的值为 124
spread.updateExternalReference("calc.xlsx", spread2.toJSON());  // spread 单元格 A1 的值为 124
// 使用简单的 JSON 数据设置数据：
spread.getActiveSheet().setFormula(0, 0, "=SUM([calc.xlsx]Sheet1!A1:B2"); \xa0// spread 单元格 A1 的值为 #REF!
spread.updateExternalReference("calc.xlsx", {"Sheet1":[[1, 2],[1, 3]]}); \xa0// spread 单元格 A1 的值为 7
spread.updateExternalReference("calc.xlsx", {"Sheet1":{0:{0:10, 1:10}, 1:{0:10, 1:10}}}); \xa0// spread 单元格 A1 的值为 40
spread.updateExternalReference("calc.xlsx", {"Sheet1":{1:{0:2, 1:2}}}, null, true); \xa0// spread 单元格 A1 的值为 24（合并更新后）。
// 此示例使用 GC.Spread.Sheets.IO.getPartialValues 的 successCallback 结果设置外部值
let refList = spread.getExternalReferences(true);
GC.Spread.Sheets.IO.getPartialValues(refList, getFile, (externalValues) => {
  // 成功回调
  spread.updateExternalReference(externalValues);
}, (errorMsg) => {
  // 错误回调
  console.log(errorMsg);
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `linkInfo` | `string` \| [`ExternalPartialValues`](../modules/GC.Spread.Sheets.md#externalpartialvalues) | 字符串类型是外部源的文件名，通常以 ".xlsx" 结尾。另一种类型应该是从 GC.Spread.Sheets.IO.getPartialValues 的回调中获取的外部部分值数组。 |
| `data?` | `object` | 外部源的 JSON 数据。可以是 spread.toJSON() 或通过 data[sheetName][rowIndex][colIndex] 获取的值。仅在 linkInfo 为字符串类型时需要。 |
| `filePath?` | `string` | 文件路径或文件链接，如果没有重复的 linkNames 可以为空。 |
| `isMergeUpdate?` | `boolean` | 指示是否通过合并进行更新。如果不是 true，整个外部工作表数据将被覆盖。 |

#### Returns

`void`

___

### <a id="waitforallcalculations" name="waitforallcalculations"></a> waitForAllCalculations

▸ **waitForAllCalculations**(): `Promise`<`void`\>

等待所有增量计算任务完成。

**`example`**
```javascript
spread.options.incrementalCalculation = true;
sheet.setValue(0, 0, 12);
sheet.setFormula(1, 1, "=A1+1");
await spread.waitForAllCalculations();
sheet.getValue(1, 1); // the result is 13
```

#### Returns

`Promise`<`void`\>

一个 Promise 对象，当所有计算完成时该对象兑现（无返回值）。
