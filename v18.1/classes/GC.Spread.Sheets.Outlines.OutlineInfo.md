# Class: OutlineInfo

[Sheets](../modules/GC.Spread.Sheets.md).[Outlines](../modules/GC.Spread.Sheets.Outlines.md).OutlineInfo

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Outlines.OutlineInfo.md#constructor)

### Properties

- [children](GC.Spread.Sheets.Outlines.OutlineInfo.md#children)
- [end](GC.Spread.Sheets.Outlines.OutlineInfo.md#end)
- [level](GC.Spread.Sheets.Outlines.OutlineInfo.md#level)
- [model](GC.Spread.Sheets.Outlines.OutlineInfo.md#model)
- [parent](GC.Spread.Sheets.Outlines.OutlineInfo.md#parent)
- [start](GC.Spread.Sheets.Outlines.OutlineInfo.md#start)

### Methods

- [addChild](GC.Spread.Sheets.Outlines.OutlineInfo.md#addchild)
- [contains](GC.Spread.Sheets.Outlines.OutlineInfo.md#contains)
- [state](GC.Spread.Sheets.Outlines.OutlineInfo.md#state)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new OutlineInfo**(`model`, `start`, `end`, `level`)

表示大纲（范围组）信息。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `model` | [`Outline`](GC.Spread.Sheets.Outlines.Outline.md) | 大纲的所有者。 |
| `start` | `number` | 大纲的起始索引。 |
| `end` | `number` | 大纲的结束索引。 |
| `level` | `number` | 大纲的级别。 |

## Properties

### <a id="children" name="children"></a> children

• **children**: `any`[]

组的子项。

**`example`**
```
activeSheet.rowOutlines.group(2, 10);
activeSheet.rowOutlines.group(4, 2);
var outlineInfo = activeSheet.rowOutlines.find(2, 0);
console.log(outlineInfo.children[0] === activeSheet.rowOutlines.find(4, 1)); // true
```

___

### <a id="end" name="end"></a> end

• **end**: `number`

组的结束索引。

**`example`**
```
activeSheet.rowOutlines.group(2, 10);
var outlineInfo = activeSheet.rowOutlines.find(2, 0);
console.log(outlineInfo.end); // 11
```

___

### <a id="level" name="level"></a> level

• **level**: `number`

组的级别。

**`example`**
```
activeSheet.rowOutlines.group(2, 10);
var outlineInfo = activeSheet.rowOutlines.find(2, 0);
console.log(outlineInfo.level); // 0
```

___

### <a id="model" name="model"></a> model

• **model**: [`Outline`](GC.Spread.Sheets.Outlines.Outline.md)

组的所有者。

**`example`**
```
activeSheet.rowOutlines.group(2, 10);
var outlineInfo = activeSheet.rowOutlines.find(2, 0);
console.log(outlineInfo.model === activeSheet.rowOutlines); // true
```

___

### <a id="parent" name="parent"></a> parent

• **parent**: [`OutlineInfo`](GC.Spread.Sheets.Outlines.OutlineInfo.md)

组的父级。

**`example`**
```
activeSheet.rowOutlines.group(2, 10);
activeSheet.rowOutlines.group(4, 2);
var outlineInfo = activeSheet.rowOutlines.find(4, 1);
console.log(outlineInfo.parent === activeSheet.rowOutlines.find(2, 0)); // true
```

___

### <a id="start" name="start"></a> start

• **start**: `number`

组的起始索引。

**`example`**
```
activeSheet.rowOutlines.group(2, 10);
var outlineInfo = activeSheet.rowOutlines.find(2, 0);
console.log(outlineInfo.start); // 2
```

## Methods

### <a id="addchild" name="addchild"></a> addChild

▸ **addChild**(`child`): `void`

添加子项。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `child` | `Object` | 子项。 |

#### Returns

`void`

___

### <a id="contains" name="contains"></a> contains

▸ **contains**(`index`): `boolean`

将此实例与指定的 OutlineInfo 对象进行比较，并返回它们的相对值的指示。

**`example`**
```
activeSheet.rowOutlines.group(2, 10);
activeSheet.rowOutlines.group(4, 2);
var outlineInfo1 = activeSheet.rowOutlines.find(2, 0);
var outlineInfo2 = activeSheet.rowOutlines.find(4, 1);
console.log(outlineInfo1.contains(5)); // true;
console.log(outlineInfo2.contains(5)); // true;
console.log(outlineInfo1.contains(6)); // true;
console.log(outlineInfo2.contains(6)); // false;
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 组项的索引。 |

#### Returns

`boolean`

如果范围组包含指定的索引，则为 `true`；否则为 `false`。

___

### <a id="state" name="state"></a> state

▸ **state**(`value?`): [`OutlineState`](../enums/GC.Spread.Sheets.Outlines.OutlineState.md)

获取或设置此大纲（范围组）的状态。

**`example`**
```
activeSheet.rowOutlines.group(2, 10);
activeSheet.rowOutlines.group(4, 2);
var outlineInfo = activeSheet.rowOutlines.find(4, 1);
console.log(outlineInfo.state()); // 等于 GC.Spread.Sheets.Outlines.OutlineState.expanded
outlineInfo.state(GC.Spread.Sheets.Outlines.OutlineState.collapsed);
console.log(outlineInfo.state()); // 等于 GC.Spread.Sheets.Outlines.OutlineState.collapsed
activeSheet.repaint(); // 大纲已折叠
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`OutlineState`](../enums/GC.Spread.Sheets.Outlines.OutlineState.md) |

#### Returns

[`OutlineState`](../enums/GC.Spread.Sheets.Outlines.OutlineState.md)

此大纲（范围组）的状态。
