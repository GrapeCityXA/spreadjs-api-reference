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

该数据结构描述了一个用于关闭提示的命令。该命令具有 `execute` 属性，其值为一个函数，用于执行关闭提示的操作

在示例中，通过 `spread.commandManager().setShortcutKey("closeHints", 27)` 方法将 `closeHints` 命令与 ESC 快捷键进行绑定。这意味着当用户按下 ESC 键时，将执行与 `closeHints` 命令关联的操作，即关闭提示

通过使用这个命令和相应的快捷键，用户可以方便地关闭提示，并继续进行其他操作

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

该数据结构描述了一个用于将内容提交到活动单元格的命令。该命令具有 `execute` 属性，其值为一个函数，用于执行将内容提交到活动单元格的操作

在示例中，通过 `spread.commandManager().setShortcutKey("commitContentToActiveCell", 83, true)` 方法将 `commitContentToActiveCell` 命令与 Ctrl+S 快捷键进行绑定。这意味着当用户按下 Ctrl+S 键时，将执行与 `commitContentToActiveCell` 命令关联的操作，即将内容提交到活动单元格

通过使用这个命令和相应的快捷键，用户可以方便地将编辑的内容提交到当前活动的单元格中，并进行相应的更新和处理

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

该数据结构描述了一个用于退出编辑的命令。该命令具有 `execute` 属性，其值为一个函数，用于执行退出编辑的操作

在示例中，通过 `spread.commandManager().setShortcutKey("exitEdit", 27)` 方法将 `exitEdit` 命令与 ESC 快捷键进行绑定。这意味着当用户按下 ESC 键时，将执行与 `exitEdit` 命令关联的操作，即退出当前的编辑状态

通过使用这个命令和相应的快捷键，用户可以方便地退出当前的编辑模式，并返回到查看或其他操作的状态

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

该数据结构描述了一个用于格式化文档的命令。该命令具有 `execute` 属性，其值为一个函数，用于执行格式化文档的操作

在示例中，通过 `spread.commandManager().setShortcutKey("formatDocument", 70, false, true, true)` 方法将 `formatDocument` 命令与 Alt+Shift+F 快捷键进行绑定。这意味着当用户按下 Alt+Shift+F 键时，将执行与 `formatDocument` 命令关联的操作，即对文档进行格式化

通过使用这个命令和相应的快捷键，用户可以方便地对文档进行格式化，使其具有统一的样式和排版效果

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

该数据结构描述了一个用于显示提示的命令。该命令具有 `execute` 属性，其值为一个函数，用于执行显示提示的操作

在示例中，通过 `spread.commandManager().setShortcutKey("showHints", 32, true, true)` 方法将 `showHints` 命令与 Ctrl+Shift+空格 快捷键进行绑定。这意味着当用户按下 Ctrl+Shift+空格 键时，将执行与 `showHints` 命令关联的操作，即显示相应的提示信息

通过使用这个命令和相应的快捷键，用户可以方便地查看并获取与当前上下文相关的提示信息，帮助用户更好地理解和使用应用程序的功能

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

该数据结构描述了一个用于切换绝对引用和相对引用的命令。该命令具有 `execute` 属性，其值为一个函数，用于执行切换操作

在示例中，通过 `spread.commandManager().setShortcutKey("toggleAbsoluteRelativeReferences", 115)` 方法将 `toggleAbsoluteRelativeReferences` 命令与 F4 快捷键进行绑定。这意味着当用户按下 F4 键时，将执行与 `toggleAbsoluteRelativeReferences` 命令关联的操作，即切换当前引用的类型（绝对引用或相对引用）

通过使用这个命令和相应的快捷键，用户可以方便地在公式中切换绝对引用和相对引用的方式，以适应不同的计算需求

#### Type declaration

| Name | Type |
| :------ | :------ |
| `execute` | (`context`: [`FormulaEditor`](../classes/GC.Spread.Sheets.FormulaPanel.FormulaEditor.md)) => `any` |
