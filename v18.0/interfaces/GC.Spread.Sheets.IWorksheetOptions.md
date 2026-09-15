# Interface: IWorksheetOptions

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).IWorksheetOptions

## Table of contents

### Properties

- [addColumnButtonOption](GC.Spread.Sheets.IWorksheetOptions.md#addcolumnbuttonoption)
- [addRowButtonOption](GC.Spread.Sheets.IWorksheetOptions.md#addrowbuttonoption)
- [allowCellOverflow](GC.Spread.Sheets.IWorksheetOptions.md#allowcelloverflow)
- [clipBoardOptions](GC.Spread.Sheets.IWorksheetOptions.md#clipboardoptions)
- [colHeaderAutoText](GC.Spread.Sheets.IWorksheetOptions.md#colheaderautotext)
- [colHeaderAutoTextIndex](GC.Spread.Sheets.IWorksheetOptions.md#colheaderautotextindex)
- [colHeaderVisible](GC.Spread.Sheets.IWorksheetOptions.md#colheadervisible)
- [frozenlineColor](GC.Spread.Sheets.IWorksheetOptions.md#frozenlinecolor)
- [gridline](GC.Spread.Sheets.IWorksheetOptions.md#gridline)
- [isProtected](GC.Spread.Sheets.IWorksheetOptions.md#isprotected)
- [keepUnknownFormulas](GC.Spread.Sheets.IWorksheetOptions.md#keepunknownformulas)
- [protectionOptions](GC.Spread.Sheets.IWorksheetOptions.md#protectionoptions)
- [rightToLeft](GC.Spread.Sheets.IWorksheetOptions.md#righttoleft)
- [rowHeaderAutoText](GC.Spread.Sheets.IWorksheetOptions.md#rowheaderautotext)
- [rowHeaderAutoTextIndex](GC.Spread.Sheets.IWorksheetOptions.md#rowheaderautotextindex)
- [rowHeaderVisible](GC.Spread.Sheets.IWorksheetOptions.md#rowheadervisible)
- [selectionBackColor](GC.Spread.Sheets.IWorksheetOptions.md#selectionbackcolor)
- [selectionBorderColor](GC.Spread.Sheets.IWorksheetOptions.md#selectionbordercolor)
- [sheetAreaOffset](GC.Spread.Sheets.IWorksheetOptions.md#sheetareaoffset)
- [sheetTabColor](GC.Spread.Sheets.IWorksheetOptions.md#sheettabcolor)
- [showFormulas](GC.Spread.Sheets.IWorksheetOptions.md#showformulas)
- [showZeros](GC.Spread.Sheets.IWorksheetOptions.md#showzeros)

## Properties

### <a id="addcolumnbuttonoption" name="addcolumnbuttonoption"></a> addColumnButtonOption

• `Optional` **addColumnButtonOption**: [`IAddColumnButtonOption`](GC.Spread.Sheets.IAddColumnButtonOption.md)

添加列按钮的选项。

___

### <a id="addrowbuttonoption" name="addrowbuttonoption"></a> addRowButtonOption

• `Optional` **addRowButtonOption**: [`IAddRowButtonOption`](GC.Spread.Sheets.IAddRowButtonOption.md)

添加行按钮的选项。

___

### <a id="allowcelloverflow" name="allowcelloverflow"></a> allowCellOverflow

• **allowCellOverflow**: `boolean`

指示数据是否可以溢出到相邻的空单元格中。

___

### <a id="clipboardoptions" name="clipboardoptions"></a> clipBoardOptions

• **clipBoardOptions**: [`ClipboardPasteOptions`](../enums/GC.Spread.Sheets.ClipboardPasteOptions.md)

剪贴板选项。

___

### <a id="colheaderautotext" name="colheaderautotext"></a> colHeaderAutoText

• **colHeaderAutoText**: [`HeaderAutoText`](../enums/GC.Spread.Sheets.HeaderAutoText.md)

指示列标题是显示字母、数字还是空白。

___

### <a id="colheaderautotextindex" name="colheaderautotextindex"></a> colHeaderAutoTextIndex

• **colHeaderAutoTextIndex**: [`HeaderAutoText`](../enums/GC.Spread.Sheets.HeaderAutoText.md)

指定当存在多个列标题行时，哪个列标题行显示自动文本。

___

### <a id="colheadervisible" name="colheadervisible"></a> colHeaderVisible

• **colHeaderVisible**: `boolean`

指示列标题是否可见。

___

### <a id="frozenlinecolor" name="frozenlinecolor"></a> frozenlineColor

• **frozenlineColor**: `string`

用于表示冻结线颜色的颜色字符串，例如“red”、“#FFFF00”、“rgb(255,0,0)”、“Accent 5”等。

___

### <a id="gridline" name="gridline"></a> gridline

• **gridline**: [`IWorkSheetGridlineOption`](GC.Spread.Sheets.IWorkSheetGridlineOption.md)

网格线的选项。

___

### <a id="isprotected" name="isprotected"></a> isProtected

• **isProtected**: `boolean`

指示此工作表上标记为受保护的单元格是否无法编辑。

___

### <a id="keepunknownformulas" name="keepunknownformulas"></a> keepUnknownFormulas

• **keepUnknownFormulas**: `boolean`

指示未知公式是否可以包含在工作表 JSON 数据中

___

### <a id="protectionoptions" name="protectionoptions"></a> protectionOptions

• **protectionOptions**: [`IProtectionOptions`](GC.Spread.Sheets.IProtectionOptions.md)

工作表保护配置项

### <a id="righttoleft" name="righttoleft"></a> rightToLeft

• **rightToLeft**: `boolean`

指示工作表是否从右向左渲染。

___

### <a id="rowheaderautotext" name="rowheaderautotext"></a> rowHeaderAutoText

• **rowHeaderAutoText**: [`HeaderAutoText`](../enums/GC.Spread.Sheets.HeaderAutoText.md)

指示行标头是显示字母还是数字还是空白

___

### <a id="rowheaderautotextindex" name="rowheaderautotextindex"></a> rowHeaderAutoTextIndex

• **rowHeaderAutoTextIndex**: [`HeaderAutoText`](../enums/GC.Spread.Sheets.HeaderAutoText.md)

指定有多个行标头列时哪个行标头列显示自动文本

___

### <a id="rowheadervisible" name="rowheadervisible"></a> rowHeaderVisible

• **rowHeaderVisible**: `boolean`

指示行是否可见

___

### <a id="selectionbackcolor" name="selectionbackcolor"></a> selectionBackColor

• **selectionBackColor**: `string`

工作表的选定区域背景颜色

___

### <a id="selectionbordercolor" name="selectionbordercolor"></a> selectionBorderColor

• **selectionBorderColor**: `string`

工作表的选定区域边框颜色

___

### <a id="sheetareaoffset" name="sheetareaoffset"></a> sheetAreaOffset

• **sheetAreaOffset**: [`IWorkSheetSheetAreaOffsetOption`](GC.Spread.Sheets.IWorkSheetSheetAreaOffsetOption.md)

SheetAreaOffset 的选项

___

### <a id="sheettabcolor" name="sheettabcolor"></a> sheetTabColor

• **sheetTabColor**: `string`

用于表示工作表标签颜色的颜色字符串，例如"red"，"#FFFF00"，"rgb(255,0,0)"，"Accent 5"等

___

### <a id="showformulas" name="showformulas"></a> showFormulas

• **showFormulas**: `boolean`

指示是否显示公式字符串而不是公式结果

___

### <a id="showzeros" name="showzeros"></a> showZeros

• **showZeros**: `boolean`

指示是否在包含零值的单元格中显示0。默认为true
