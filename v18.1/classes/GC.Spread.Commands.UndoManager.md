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

表示撤销管理器。

## Methods

### <a id="canredo" name="canredo"></a> canRedo

▸ **canRedo**(): `boolean`

获取是否允许重做操作。

#### Returns

`boolean`

如果允许重做操作则为`true`；否则为`false`。

___

### <a id="canundo" name="canundo"></a> canUndo

▸ **canUndo**(): `boolean`

获取是否允许撤销操作。

#### Returns

`boolean`

如果允许撤销操作则为`true`；否则为`false`。

___

### <a id="clear" name="clear"></a> clear

▸ **clear**(): `void`

清除所有撤销栈和重做栈。

#### Returns

`void`

___

### <a id="getredostack" name="getredostack"></a> getRedoStack

▸ **getRedoStack**(): `any`[]

获取重做栈。

#### Returns

`any`[]

返回一个对象。该对象必须包含sheetName和cmd。sheetName和cmd的类型都是string。

___

### <a id="getundostack" name="getundostack"></a> getUndoStack

▸ **getUndoStack**(): `any`[]

获取撤销栈。

#### Returns

`any`[]

返回一个对象。该对象必须包含sheetName和cmd。sheetName和cmd的类型都是string。

___

### <a id="maxsize" name="maxsize"></a> maxSize

▸ **maxSize**(`value?`): `any`

获取或设置撤销/重做栈的最大大小。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 该值应该大于或等于0。 |

#### Returns

`any`

如果未设置值，返回撤销/重做栈的最大大小；否则返回UndoManager。

___

### <a id="redo" name="redo"></a> redo

▸ **redo**(): `boolean`

重做最后一个命令。

#### Returns

`boolean`

如果重做操作成功则为`true`；否则为`false`。

___

### <a id="undo" name="undo"></a> undo

▸ **undo**(): `boolean`

撤销最后一个命令。

#### Returns

`boolean`

如果撤销操作成功则为`true`；否则为`false`。
