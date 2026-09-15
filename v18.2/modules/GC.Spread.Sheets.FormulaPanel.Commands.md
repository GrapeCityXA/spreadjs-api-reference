# Namespace: Commands

[Sheets](GC.Spread.Sheets.md).[FormulaPanel](GC.Spread.Sheets.FormulaPanel.md).Commands

## Table of contents

### Variables

- [closeHints](GC.Spread.Sheets.FormulaPanel.Commands.md#closehints)
- [commitContentToActiveCell](GC.Spread.Sheets.FormulaPanel.Commands.md#commitcontenttoactivecell)
- [exitEdit](GC.Spread.Sheets.FormulaPanel.Commands.md#exitedit)
- [formatDocument](GC.Spread.Sheets.FormulaPanel.Commands.md#formatdocument)
- [showHints](GC.Spread.Sheets.FormulaPanel.Commands.md#showhints)
- [toggleAbsoluteRelativeReferences](GC.Spread.Sheets.FormulaPanel.Commands.md#toggleabsoluterelativereferences)

## Variables

### <a id="closehints" name="closehints"></a> closeHints

• **closeHints**: `Object`

表示用于关闭提示的命令。

**`property`** {function} execute - 执行操作。

**`example`**
```
//此示例展示如何将closeHints命令绑定到esc快捷键。
spread.commandManager().setShortcutKey("closeHints", 27);
```

#### Type declaration

| Name | Type |
| :------ | :------ |
| `execute` | (`context`: [`FormulaEditor`](../classes/GC.Spread.Sheets.FormulaPanel.FormulaEditor.md)) => `any` |

___

### <a id="commitcontenttoactivecell" name="commitcontenttoactivecell"></a> commitContentToActiveCell

• **commitContentToActiveCell**: `Object`

表示用于将内容提交到活动单元格的命令。

**`property`** {function} execute - 执行操作。

**`example`**
```
//此示例展示如何将commitContentToActiveCell命令绑定到ctrl-s快捷键。
spread.commandManager().setShortcutKey("commitContentToActiveCell", 83, true);
```

#### Type declaration

| Name | Type |
| :------ | :------ |
| `execute` | (`context`: [`FormulaEditor`](../classes/GC.Spread.Sheets.FormulaPanel.FormulaEditor.md)) => `any` |

___

### <a id="exitedit" name="exitedit"></a> exitEdit

• **exitEdit**: `Object`

表示用于退出编辑的命令。

**`property`** {function} execute - 执行操作。

**`example`**
```
//此示例展示如何将exitEdit命令绑定到esc快捷键。
spread.commandManager().setShortcutKey("exitEdit", 27);
```

#### Type declaration

| Name | Type |
| :------ | :------ |
| `execute` | (`context`: [`FormulaEditor`](../classes/GC.Spread.Sheets.FormulaPanel.FormulaEditor.md)) => `any` |

___

### <a id="formatdocument" name="formatdocument"></a> formatDocument

• **formatDocument**: `Object`

表示用于格式化文档的命令。

**`property`** {function} execute - 执行操作。

**`example`**
```
//此示例展示如何将formatDocument命令绑定到alt-shift-f快捷键。
spread.commandManager().setShortcutKey("formatDocument", 70, false, true, true);
```

#### Type declaration

| Name | Type |
| :------ | :------ |
| `execute` | (`context`: [`FormulaEditor`](../classes/GC.Spread.Sheets.FormulaPanel.FormulaEditor.md)) => `any` |

___

### <a id="showhints" name="showhints"></a> showHints

• **showHints**: `Object`

表示用于显示提示的命令。

**`property`** {function} execute - 执行操作。

**`example`**
```
//此示例展示如何将showHints命令绑定到ctrl-shift-空格快捷键。
spread.commandManager().setShortcutKey("showHints", 32, true, true);
```

#### Type declaration

| Name | Type |
| :------ | :------ |
| `execute` | (`context`: [`FormulaEditor`](../classes/GC.Spread.Sheets.FormulaPanel.FormulaEditor.md)) => `any` |

___

### <a id="toggleabsoluterelativereferences" name="toggleabsoluterelativereferences"></a> toggleAbsoluteRelativeReferences

• **toggleAbsoluteRelativeReferences**: `Object`

表示用于切换绝对/相对引用的命令。

**`property`** {function} execute - 执行操作。

**`example`**
```
//此示例展示如何将toggleAbsoluteRelativeReferences命令绑定到f4快捷键。
spread.commandManager().setShortcutKey("toggleAbsoluteRelativeReferences", 115);
```

#### Type declaration

| Name | Type |
| :------ | :------ |
| `execute` | (`context`: [`FormulaEditor`](../classes/GC.Spread.Sheets.FormulaPanel.FormulaEditor.md)) => `any` |
