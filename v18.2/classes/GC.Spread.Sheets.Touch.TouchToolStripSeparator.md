# Class: TouchToolStripSeparator

[Sheets](../modules/GC.Spread.Sheets.md).[Touch](../modules/GC.Spread.Sheets.Touch.md).TouchToolStripSeparator

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Touch.TouchToolStripSeparator.md#constructor)

### Methods

- [name](GC.Spread.Sheets.Touch.TouchToolStripSeparator.md#name)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new TouchToolStripSeparator**(`canExecute?`)

表示工具栏中的分隔符。

**`example`**
```
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripItem("Cut", "Delete", "cut.png", function(){ }))
spread.touchToolStrip.getItem("Cut").font("15px Arial").foreColor("red");
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripSeparator());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `canExecute?` | `Function` | 通过函数定义何时显示分隔符。如果返回 `true`，则显示分隔符；否则隐藏分隔符。 |

## Methods

### <a id="name" name="name"></a> name

▸ **name**(): `string`

获取分隔符的名称。

#### Returns

`string`

返回当前分隔符的名称。
