# Namespace: FormulaTextBox

[Spread](GC.Spread.md).[Sheets](GC.Spread.Sheets.md).FormulaTextBox

## Table of contents

### Classes

- [FormulaTextBox](../classes/GC.Spread.Sheets.FormulaTextBox.FormulaTextBox.md)

### Interfaces

- [IFormulaTextBoxOptions](../interfaces/GC.Spread.Sheets.FormulaTextBox.IFormulaTextBoxOptions.md)

### Functions

- [findControl](GC.Spread.Sheets.FormulaTextBox.md#findcontrol)

## Functions

### <a id="findcontrol" name="findcontrol"></a> findControl

▸ **findControl**(`host`): [`FormulaTextBox`](../classes/GC.Spread.Sheets.FormulaTextBox.FormulaTextBox.md)

通过宿主元素获取FormulaTextBox实例。

**`example`**
```
window.onload = function(){
     var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 1 });
     var rangeSelector = new GC.Spread.Sheets.FormulaTextBox.FormulaTextBox(document.getElementById("ftb"), {rangeSelectMode: true});
     rangeSelector.workbook(spread);
     var rangeSelectorInstance = GC.Spread.Sheets.FormulaTextBox.findControl("ftb");
}
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `host` | `string` \| `HTMLElement` | 宿主元素或宿主元素id。 |

#### Returns

[`FormulaTextBox`](../classes/GC.Spread.Sheets.FormulaTextBox.FormulaTextBox.md)

FormulaTextBox实例。
