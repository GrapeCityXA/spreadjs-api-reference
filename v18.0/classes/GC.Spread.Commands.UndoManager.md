# Class: UndoManager

[Spread](../modules/GC.Spread.md).[Commands](../modules/GC.Spread.Commands.md).UndoManager

## Table of contents

### Constructors

- [constructor](GC.Spread.Commands.UndoManager.md#constructor)

### Methods

- [canRedo](GC.Spread.Commands.UndoManager.md#canredo)
- [canUndo](GC.Spread.Commands.UndoManager.md#canundo)
- [clear](GC.Spread.Commands.UndoManager.md#clear)
- [getRedoStack](GC.Spread.Commands.UndoManager.md#getredostack)
- [getUndoStack](GC.Spread.Commands.UndoManager.md#getundostack)
- [maxSize](GC.Spread.Commands.UndoManager.md#maxsize)
- [redo](GC.Spread.Commands.UndoManager.md#redo)
- [undo](GC.Spread.Commands.UndoManager.md#undo)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new UndoManager**()

撤销管理器

## Methods

### <a id="canredo" name="canredo"></a> canRedo

▸ **canRedo**(): `boolean`

获取是否允许重做操作

#### Returns

`boolean`

为`true`时, 允许重做操作; 若为`false`则不支持

___

### <a id="canundo" name="canundo"></a> canUndo

▸ **canUndo**(): `boolean`

获取是否允许撤消操作

#### Returns

`boolean`

为`true`时, 允许撤消操作; 若为`false`则不支持

___

### <a id="clear" name="clear"></a> clear

▸ **clear**(): `void`

清除所有撤消堆栈和重做堆栈

#### Returns

`void`

___

### <a id="getredostack" name="getredostack"></a> getRedoStack

▸ **getRedoStack**(): `any`[]

获取撤消栈

#### Returns

`any`[]

返回一个对象这必须包括sheetName和cmdsheetName和cmd的类型都是string

___

### <a id="getundostack" name="getundostack"></a> getUndoStack

▸ **getUndoStack**(): `any`[]

获取重做栈

#### Returns

`any`[]

返回一个对象此对象必须包含sheetName和cmdsheetName和cmd的类型都是string

___

### <a id="maxsize" name="maxsize"></a> maxSize

▸ **maxSize**(`value?`): `any`

获取或设置撤消/重做栈的最大大小

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 此值应大于或等于0 |

#### Returns

`any`

如果未设置值返回撤消/重做堆栈的最大大小否则，返回UndoManager

___

### <a id="redo" name="redo"></a> redo

▸ **redo**(): `boolean`

重做最后一个命令

#### Returns

`boolean`

为`true`时, 重做操作成功; 为`false`则不成功

___

### <a id="undo" name="undo"></a> undo

▸ **undo**(): `boolean`

撤消最后一个命令

#### Returns

`boolean`

为`true`时, 撤销操作成功; 为`false`则不成功
