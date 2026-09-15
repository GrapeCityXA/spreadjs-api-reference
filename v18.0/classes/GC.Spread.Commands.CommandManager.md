# Class: CommandManager

[Spread](../modules/GC.Spread.md).[Commands](../modules/GC.Spread.Commands.md).CommandManager

## Table of contents

### Constructors

- [constructor](GC.Spread.Commands.CommandManager.md#constructor)

### Methods

- [execute](GC.Spread.Commands.CommandManager.md#execute)
- [register](GC.Spread.Commands.CommandManager.md#register)
- [setShortcutKey](GC.Spread.Commands.CommandManager.md#setshortcutkey)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new CommandManager**(`context`)

命令管理器

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context` | `Object` | 命令管理器中所有命令的执行上下文 |

## Methods

### <a id="execute" name="execute"></a> execute

▸ **execute**(`commandOptions`): `boolean`

执行命令并将该命令添加到UndoManager中

**`代码示例`**
``` javascript
//例如，下面的代码执行autoFitColumn命令
var spread = GC.Spread.Sheets.findControl(document.getElementById("ss"));
spread.commandManager().execute({cmd: "autoFitColumn", sheetName: "Sheet1", columns: [{col: 1}], rowHeader: false, autoFitType: GC.Spread.Sheets.AutoFitType.cell});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `commandOptions` | `Object` | 命令的选项 |

#### Returns

`boolean`

执行命令的结果

___

### <a id="register" name="register"></a> register

▸ **register**(`name`, `command`, `key?`, `ctrl?`, `shift?`, `alt?`, `meta?`): `void`

向命令管理器注册命令

**`代码示例`**
``` javascript
//例如，以下代码注册了 `changeBackColor` 命令，然后执行该命令。
var command = {
    canUndo: true,
    execute: function (context, options, isUndo) {
        var Commands = GC.Spread.Sheets.Commands;
        options.cmd = 'changeBackColor';
        if (isUndo) {
            Commands.undoTransaction(context, options);
            return true;
        } else {
            Commands.startTransaction(context, options);
            var sheet = context.getSheetFromName(options.sheetName);
            var cell = sheet.getCell(options.row, options.col);
            cell.backColor(options.backColor);
            Commands.endTransaction(context, options);
            return true;
        }
    },
};
var spread = GC.Spread.Sheets.findControl(document.getElementById('ss'));
var commandManager = spread.commandManager();
commandManager.register('changeBackColor', command);
commandManager.execute({ cmd: 'changeBackColor', sheetName: spread.getSheet(0).name(), row: 1, col: 2, backColor: 'red' });

```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 命令的名称 |
| `command` | `Object` | 定义命令的对象 |
| `key?` | `number` | 按键编码 |
| `ctrl?` | `boolean` | 为`true`时, 命令需要 Ctrl 键; 若 `false`则不需要 |
| `shift?` | `boolean` | 为`true`时, 命令需要 Shift 键;  若 `false`则不需要 |
| `alt?` | `boolean` | 为`true`时, 命令需要 Alt 键;  若 `false`则不需要 |
| `meta?` | `boolean` | 为`true`时, 命令需要Mac上的Command键或Windows上的Windows键；若 `false`则不需要 |

#### Returns

`void`

___

### <a id="setshortcutkey" name="setshortcutkey"></a> setShortcutKey

▸ **setShortcutKey**(`commandName`, `key?`, `ctrl?`, `shift?`, `alt?`, `meta?`): `void`

将快捷键绑定到命令

**`代码示例`**
``` javascript
// 本示例改变了默认键的行为
var activeSheet = spread.getActiveSheet();
// 为活动单元格将默认的向上箭头键操作更改为“向上翻页”。
spread.commandManager().setShortcutKey('navigationPageUp', GC.Spread.Commands.Key.up, false, false, false, false);
// 为活动单元格将默认的向下箭头键操作更改为“向下翻页”。
spread.commandManager().setShortcutKey('navigationPageDown', GC.Spread.Commands.Key.down, false, false, false, false); 
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `commandName` | `string` | 命令名，将commandName设置为undefined将删除快捷键的绑定命令 |
| `key?` | `number` | 将key设置为undefined将删除命令的快捷键 |
| `ctrl?` | `boolean` | 为`true`时, 命令需要 Ctrl 键; 若 `false`则不需要 |
| `shift?` | `boolean` | 为`true`时, 命令需要 Shift 键;  若 `false`则不需要 |
| `alt?` | `boolean` | 为`true`时, 命令需要 Alt 键;  若 `false`则不需要 |
| `meta?` | `boolean` | 为`true`时, 命令需要Mac上的Command键或Windows上的Windows键；若 `false`则不需要 |

#### Returns

`void`
