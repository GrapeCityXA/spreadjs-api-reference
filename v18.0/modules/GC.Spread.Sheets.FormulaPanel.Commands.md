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

表示用于关闭提示的命令

 **`property`** {function} execute - 执行关闭提示操作的函数

**`示例`**
```
//此示例演示将 closeHints 命令绑定到 ESC 快捷键
spread.commandManager().setShortcutKey("closeHints", 27);
```

#### Type declaration

| Name | Type |
| :------ | :------ |
| `execute` | (`context`: [`FormulaEditor`](../classes/GC.Spread.Sheets.FormulaPanel.FormulaEditor.md)) => `any` |

___

### <a id="commitcontenttoactivecell" name="commitcontenttoactivecell"></a> commitContentToActiveCell

• **commitContentToActiveCell**: `Object`

表示用于将内容提交到活动单元格的命令

 **`property`** {function} execute - 执行提交内容到活动单元格操作的函数

**`示例`**
```
//此示例演示将 commitContentToActiveCell 命令绑定到 Ctrl+S 快捷键
spread.commandManager().setShortcutKey("commitContentToActiveCell", 83, true);
```

#### Type declaration

| Name | Type |
| :------ | :------ |
| `execute` | (`context`: [`FormulaEditor`](../classes/GC.Spread.Sheets.FormulaPanel.FormulaEditor.md)) => `any` |

___

### <a id="exitedit" name="exitedit"></a> exitEdit

• **exitEdit**: `Object`

表示用于退出编辑的命令

 **`property`** {function} execute - 执行退出编辑操作的函数

**`示例`**
```
//此示例演示将 exitEdit 命令绑定到 ESC 快捷键
spread.commandManager().setShortcutKey("exitEdit", 27);
```

#### Type declaration

| Name | Type |
| :------ | :------ |
| `execute` | (`context`: [`FormulaEditor`](../classes/GC.Spread.Sheets.FormulaPanel.FormulaEditor.md)) => `any` |

___

### <a id="formatdocument" name="formatdocument"></a> formatDocument

• **formatDocument**: `Object`

表示用于格式化文档的命令

 **`property`** {function} execute - 执行格式化文档操作的函数

**`示例`**
```
//此示例演示将 formatDocument 命令绑定到 Alt+Shift+F 快捷键
spread.commandManager().setShortcutKey("formatDocument", 70, false, true, true);
```

#### Type declaration

| Name | Type |
| :------ | :------ |
| `execute` | (`context`: [`FormulaEditor`](../classes/GC.Spread.Sheets.FormulaPanel.FormulaEditor.md)) => `any` |

___

### <a id="showhints" name="showhints"></a> showHints

• **showHints**: `Object`

表示用于显示提示的命令

 **`property`** {function} execute - 执行显示提示操作的函数

**`示例`**
```
//此示例演示将 showHints 命令绑定到 Ctrl+Shift+空格 快捷键
spread.commandManager().setShortcutKey("showHints", 32, true, true);
```

#### Type declaration

| Name | Type |
| :------ | :------ |
| `execute` | (`context`: [`FormulaEditor`](../classes/GC.Spread.Sheets.FormulaPanel.FormulaEditor.md)) => `any` |

___

### <a id="toggleabsoluterelativereferences" name="toggleabsoluterelativereferences"></a> toggleAbsoluteRelativeReferences

• **toggleAbsoluteRelativeReferences**: `Object`

表示用于切换绝对引用和相对引用的命令

 **`property`** {function} execute - 执行切换绝对引用和相对引用操作的函数

**`示例`**
```
//此示例演示将 toggleAbsoluteRelativeReferences 命令绑定到 F4 快捷键
spread.commandManager().setShortcutKey("toggleAbsoluteRelativeReferences", 115);
```

#### Type declaration

| Name | Type |
| :------ | :------ |
| `execute` | (`context`: [`FormulaEditor`](../classes/GC.Spread.Sheets.FormulaPanel.FormulaEditor.md)) => `any` |
