# Class: FormulaEditor

[Sheets](../modules/GC.Spread.Sheets.md).[FormulaPanel](../modules/GC.Spread.Sheets.FormulaPanel.md).FormulaEditor

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.FormulaPanel.FormulaEditor.md#constructor)

### Properties

- [options](GC.Spread.Sheets.FormulaPanel.FormulaEditor.md#options)

### Methods

- [attach](GC.Spread.Sheets.FormulaPanel.FormulaEditor.md#attach)
- [commandManager](GC.Spread.Sheets.FormulaPanel.FormulaEditor.md#commandmanager)
- [destroy](GC.Spread.Sheets.FormulaPanel.FormulaEditor.md#destroy)
- [detach](GC.Spread.Sheets.FormulaPanel.FormulaEditor.md#detach)
- [format](GC.Spread.Sheets.FormulaPanel.FormulaEditor.md#format)
- [refresh](GC.Spread.Sheets.FormulaPanel.FormulaEditor.md#refresh)
- [text](GC.Spread.Sheets.FormulaPanel.FormulaEditor.md#text)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new FormulaEditor**(`host`, `options?`)

表示一个公式编辑器。

**`example`**
```
window.onload = function(){
     var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
     formulaEditor = new GC.Spread.Sheets.FormulaPanel.FormulaEditor(document.getElementById("fe"));
     formulaEditor.attach(spread);
}
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `host` | `HTMLElement` | 宿主元素。 |
| `options?` | [`IFormulaEditorOptions`](../interfaces/GC.Spread.Sheets.FormulaPanel.IFormulaEditorOptions.md) | - |

## Properties

### <a id="options" name="options"></a> options

• **options**: [`IFormulaEditorOptions`](../interfaces/GC.Spread.Sheets.FormulaPanel.IFormulaEditorOptions.md)

表示公式编辑器的选项。

**`property`** {number} tabSize - 指示当按下"Tab"键时插入的空格数。默认是4。

**`property`** {number} formatWidthLimit - 指示格式化时的宽度限制，默认是'auto'。'auto'表示跟随dom的宽度，并尝试避免一行宽度超过dom的宽度。

**`example`**
```
formulaEditor.options.tabSize = 2;
formulaEditor.options.formatWidthLimit = -1;
```

## Methods

### <a id="attach" name="attach"></a> attach

▸ **attach**(`workbook`): `any`

将公式编辑器附加到工作簿。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workbook` | [`Workbook`](GC.Spread.Sheets.Workbook.md) | 要附加的工作簿。 |

#### Returns

`any`

void

___

### <a id="commandmanager" name="commandmanager"></a> commandManager

▸ **commandManager**(): [`CommandManager`](GC.Spread.Commands.CommandManager.md)

获取命令管理器。

**`example`**
```
//此示例执行一个执行指定操作的命令。
formulaEditor.commandManager().execute({ cmd: "formatDocument" });
```

#### Returns

[`CommandManager`](GC.Spread.Commands.CommandManager.md)

命令管理器。

___

### <a id="destroy" name="destroy"></a> destroy

▸ **destroy**(): `void`

销毁当前公式编辑器。

#### Returns

`void`

___

### <a id="detach" name="detach"></a> detach

▸ **detach**(): `void`

将公式编辑器从工作簿分离。

#### Returns

`void`

void

___

### <a id="format" name="format"></a> format

▸ **format**(): `void`

格式化文档（公式字符串）。

#### Returns

`void`

___

### <a id="refresh" name="refresh"></a> refresh

▸ **refresh**(): `void`

刷新公式编辑器。

#### Returns

`void`

___

### <a id="text" name="text"></a> text

▸ **text**(`value?`): `string`

获取或设置文本。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 文本值。 |

#### Returns

`string`

如果未设置值，则返回文本；否则无返回值。
