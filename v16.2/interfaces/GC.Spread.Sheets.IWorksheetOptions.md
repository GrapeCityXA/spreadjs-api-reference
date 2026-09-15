# Interface: IWorksheetOptions

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).IWorksheetOptions

## Table of contents

### Properties

- [allowCellOverflow](GC.Spread.Sheets.IWorksheetOptions.md#allowcelloverflow)
- [clipBoardOptions](GC.Spread.Sheets.IWorksheetOptions.md#clipboardoptions)
- [colHeaderAutoText](GC.Spread.Sheets.IWorksheetOptions.md#colheaderautotext)
- [colHeaderAutoTextIndex](GC.Spread.Sheets.IWorksheetOptions.md#colheaderautotextindex)
- [colHeaderVisible](GC.Spread.Sheets.IWorksheetOptions.md#colheadervisible)
- [frozenlineColor](GC.Spread.Sheets.IWorksheetOptions.md#frozenlinecolor)
- [gridline](GC.Spread.Sheets.IWorksheetOptions.md#gridline)
- [isProtected](GC.Spread.Sheets.IWorksheetOptions.md#isprotected)
- [protectionOptions](GC.Spread.Sheets.IWorksheetOptions.md#protectionoptions)
- [rowHeaderAutoText](GC.Spread.Sheets.IWorksheetOptions.md#rowheaderautotext)
- [rowHeaderAutoTextIndex](GC.Spread.Sheets.IWorksheetOptions.md#rowheaderautotextindex)
- [rowHeaderVisible](GC.Spread.Sheets.IWorksheetOptions.md#rowheadervisible)
- [selectionBackColor](GC.Spread.Sheets.IWorksheetOptions.md#selectionbackcolor)
- [selectionBorderColor](GC.Spread.Sheets.IWorksheetOptions.md#selectionbordercolor)
- [sheetTabColor](GC.Spread.Sheets.IWorksheetOptions.md#sheettabcolor)
- [showFormulas](GC.Spread.Sheets.IWorksheetOptions.md#showformulas)
- [showZeros](GC.Spread.Sheets.IWorksheetOptions.md#showzeros)

## Properties

### <a id="allowcelloverflow" name="allowcelloverflow"></a> allowCellOverflow

• **allowCellOverflow**: `boolean`

indicates whether data can overflow into adjacent empty cells.

___

### <a id="clipboardoptions" name="clipboardoptions"></a> clipBoardOptions

• **clipBoardOptions**: [`ClipboardPasteOptions`](../enums/GC.Spread.Sheets.ClipboardPasteOptions.md)

The clipboard option.

___

### <a id="colheaderautotext" name="colheaderautotext"></a> colHeaderAutoText

• **colHeaderAutoText**: [`HeaderAutoText`](../enums/GC.Spread.Sheets.HeaderAutoText.md)

Indicates whether the column header displays letters or numbers or is blank.

___

### <a id="colheaderautotextindex" name="colheaderautotextindex"></a> colHeaderAutoTextIndex

• **colHeaderAutoTextIndex**: [`HeaderAutoText`](../enums/GC.Spread.Sheets.HeaderAutoText.md)

Specifies which column header row displays the automatic text when there are multiple column header rows.

___

### <a id="colheadervisible" name="colheadervisible"></a> colHeaderVisible

• **colHeaderVisible**: `boolean`

Indicates whether the column header is visible.

___

### <a id="frozenlinecolor" name="frozenlinecolor"></a> frozenlineColor

• **frozenlineColor**: `string`

A color string used to represent the frozen line color, such as "red", "#FFFF00", "rgb(255,0,0)", "Accent 5", and so on.

___

### <a id="gridline" name="gridline"></a> gridline

• **gridline**: [`IWorkSheetGridlineOption`](GC.Spread.Sheets.IWorkSheetGridlineOption.md)

The grid line's options.

___

### <a id="isprotected" name="isprotected"></a> isProtected

• **isProtected**: `boolean`

Indicates whether cells on this sheet that are marked as protected cannot be edited.

___

### <a id="protectionoptions" name="protectionoptions"></a> protectionOptions

• **protectionOptions**: [`IProtectionOptions`](GC.Spread.Sheets.IProtectionOptions.md)

A value that indicates the elements that you want users to be able to change.

___

### <a id="rowheaderautotext" name="rowheaderautotext"></a> rowHeaderAutoText

• **rowHeaderAutoText**: [`HeaderAutoText`](../enums/GC.Spread.Sheets.HeaderAutoText.md)

Indicates whether the row header displays letters or numbers or is blank.

___

### <a id="rowheaderautotextindex" name="rowheaderautotextindex"></a> rowHeaderAutoTextIndex

• **rowHeaderAutoTextIndex**: [`HeaderAutoText`](../enums/GC.Spread.Sheets.HeaderAutoText.md)

Specifies which row header column displays the automatic text when there are multiple row header columns.

___

### <a id="rowheadervisible" name="rowheadervisible"></a> rowHeaderVisible

• **rowHeaderVisible**: `boolean`

Indicates whether the row header is visible.

___

### <a id="selectionbackcolor" name="selectionbackcolor"></a> selectionBackColor

• **selectionBackColor**: `string`

The selection's background color for the sheet.

___

### <a id="selectionbordercolor" name="selectionbordercolor"></a> selectionBorderColor

• **selectionBorderColor**: `string`

The selection's border color for the sheet.

___

### <a id="sheettabcolor" name="sheettabcolor"></a> sheetTabColor

• **sheetTabColor**: `string`

A color string used to represent the sheet tab color, such as "red", "#FFFF00", "rgb(255,0,0)", "Accent 5", and so on.

___

### <a id="showformulas" name="showformulas"></a> showFormulas

• **showFormulas**: `boolean`

indicates whether display the formulas string not the formula result.

___

### <a id="showzeros" name="showzeros"></a> showZeros

• **showZeros**: `boolean`

indicates whether display the 0 in cells containing zero value. Default is true.
