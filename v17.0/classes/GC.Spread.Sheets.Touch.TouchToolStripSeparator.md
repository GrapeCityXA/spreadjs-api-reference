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

工具栏中的分隔符

**`代码示例`**
```
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripItem("Cut", "Delete", "cut.png", function(){ }))
spread.touchToolStrip.getItem("Cut").font("15px Arial").foreColor("red");
spread.touchToolStrip.add(new GC.Spread.Sheets.Touch.TouchToolStripSeparator());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `canExecute?` | `Function` | 定义何时显示带有函数的分隔符。如果显示分隔符，则返回true;否则为false |

## Methods

### <a id="name" name="name"></a> name

▸ **name**(): `string`

获取分隔符的名称

#### Returns

`string`

返回当前的分隔符名称
