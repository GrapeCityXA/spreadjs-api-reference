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

区域分组信息

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `model` | [`Outline`](GC.Spread.Sheets.Outlines.Outline.md) | 区域分组的所在者 |
| `start` | `number` | 区域分组的起始索引 |
| `end` | `number` | 区域分组的结束索引 |
| `level` | `number` | 区域分组的级别 |

## Properties

### <a id="children" name="children"></a> children

• **children**: `any`[]

分组的子级

___

### <a id="end" name="end"></a> end

• **end**: `number`

分组的结束索引

___

### <a id="level" name="level"></a> level

• **level**: `number`

分组的级别

___

### <a id="model" name="model"></a> model

• **model**: [`Outline`](GC.Spread.Sheets.Outlines.Outline.md)

分组的所在者

___

### <a id="parent" name="parent"></a> parent

• **parent**: [`OutlineInfo`](GC.Spread.Sheets.Outlines.OutlineInfo.md)

分组的父级

___

### <a id="start" name="start"></a> start

• **start**: `number`

分组的起始索引

## Methods

### <a id="addchild" name="addchild"></a> addChild

▸ **addChild**(`child`): `void`

添加子级

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `child` | `Object` | The child. |

#### Returns

`void`

___

### <a id="contains" name="contains"></a> contains

▸ **contains**(`index`): `boolean`

将此实例与指定的OutlineInfo对象进行比较,并返回其相对值的指示

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 组项的索引 |

#### Returns

`boolean`

如果区域分组包含指定的索引,返回true;否则返回false

___

### <a id="state" name="state"></a> state

▸ **state**(`value?`): [`OutlineState`](../enums/GC.Spread.Sheets.Outlines.OutlineState.md)

获取或设置此区域分组的状态

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`OutlineState`](../enums/GC.Spread.Sheets.Outlines.OutlineState.md) |

#### Returns

[`OutlineState`](../enums/GC.Spread.Sheets.Outlines.OutlineState.md)

区域分组的状态
