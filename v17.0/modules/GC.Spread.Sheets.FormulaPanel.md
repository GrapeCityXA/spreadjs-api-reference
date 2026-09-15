# Namespace: FormulaPanel

[Spread](GC.Spread.md).[Sheets](GC.Spread.Sheets.md).FormulaPanel

## Table of contents

### Namespaces

- [Commands](GC.Spread.Sheets.FormulaPanel.Commands.md)

### Classes

- [FormulaEditor](../classes/GC.Spread.Sheets.FormulaPanel.FormulaEditor.md)

### Interfaces

- [IFormulaEditorOptions](../interfaces/GC.Spread.Sheets.FormulaPanel.IFormulaEditorOptions.md)

### Functions

- [findControl](GC.Spread.Sheets.FormulaPanel.md#findcontrol)

## Functions

### <a id="findcontrol" name="findcontrol"></a> findControl

▸ **findControl**(`host`): [`FormulaEditor`](../classes/GC.Spread.Sheets.FormulaPanel.FormulaEditor.md)

通过宿主元素获取 FormulaEditor 实例

**`example`**
```
window.onload = function(){
     var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
     var formulaEditor = new GC.Spread.Sheets.FormulaPanel.FormulaEditor(document.getElementById("fe"));
     formulaEditor.workbook(spread);
     var formulaEditorInstance = GC.Spread.Sheets.FormulaPanel.findControl("fe");
}
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `host` | `string` \| `HTMLElement` | 宿主元素或宿主元素的ID |

#### Returns

[`FormulaEditor`](../classes/GC.Spread.Sheets.FormulaPanel.FormulaEditor.md)

FormulaEditor 实例
