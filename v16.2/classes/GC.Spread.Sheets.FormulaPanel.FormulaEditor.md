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

公式编辑器

**`代码示例`**
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
| `host` | `HTMLElement` | DOM 容器 |
| `options?` | [`IFormulaEditorOptions`](../interfaces/GC.Spread.Sheets.FormulaPanel.IFormulaEditorOptions.md) | - |

## Properties

### <a id="options" name="options"></a> options

• **options**: [`IFormulaEditorOptions`](../interfaces/GC.Spread.Sheets.FormulaPanel.IFormulaEditorOptions.md)

指示公式编辑器的选项。

**`property`** {number} tabSize - 指示按下“ TAB”键时插入的空间数量。默认值为4。

**`property`** {number} formatWidthLimit - 格式化时指示宽度限制，默认值为“自动”。“自动”表示这遵循DOM的宽度，并将尝试避免一条超过DOM宽度的线的宽度。

**`代码示例`**
```
formulaEditor.options.tabSize = 2;
formulaEditor.options.formatWidthLimit = -1;
```

## Methods

### <a id="attach" name="attach"></a> attach

▸ **attach**(`workbook`): `any`

**`description`** 附加到公式编辑器的工作簿。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workbook` | [`Workbook`](GC.Spread.Sheets.Workbook.md) | 指示附加的工作簿。 |

#### Returns

`any`

void

___

### <a id="commandmanager" name="commandmanager"></a> commandManager

▸ **commandManager**(): [`CommandManager`](GC.Spread.Commands.CommandManager.md)

获取命令经理。

**`代码示例`**
```
//此示例执行执行指定操作的命令。
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

**`description`** 移除公式编辑器的工作簿。

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
| `value?` | `string` | 文本 |

#### Returns

`string`

如果未设置值，请返回文本；否则，没有返回值。
