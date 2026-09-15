# Class: DataRange

[Sheets](../modules/GC.Spread.Sheets.md).[DataRange](../modules/GC.Spread.Sheets.DataRange.md).DataRange

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.DataRange.DataRange.md#constructor)

### Methods

- [name](GC.Spread.Sheets.DataRange.DataRange.md#name)
- [range](GC.Spread.Sheets.DataRange.DataRange.md#range)
- [repaint](GC.Spread.Sheets.DataRange.DataRange.md#repaint)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new DataRange**(`name`, `dataProvider`, `range`, `options?`)

表示一个数据范围。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 数据范围的名称。 |
| `dataProvider` | [`IDataProvider`](../interfaces/GC.Spread.Sheets.DataRange.IDataProvider.md) | 数据范围的数据提供者。 |
| `range` | [`Range`](GC.Spread.Sheets.Range.md) | 数据范围的范围。 |
| `options?` | [`IDataRangeOptions`](../interfaces/GC.Spread.Sheets.DataRange.IDataRangeOptions.md) | 数据范围的选项。 |

## Methods

### <a id="name" name="name"></a> name

▸ **name**(`name?`): `string`

**`description`** 获取或设置数据范围的名称。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name?` | `string` | 数据范围的名称 |

#### Returns

`string`

如果未设置值，则返回数据范围的名称。

___

### <a id="range" name="range"></a> range

▸ **range**(`range?`): [`Range`](GC.Spread.Sheets.Range.md)

**`description`** 获取或设置数据范围的范围。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range?` | [`Range`](GC.Spread.Sheets.Range.md) | 数据范围的范围 |

#### Returns

[`Range`](GC.Spread.Sheets.Range.md)

如果未设置值，则返回数据范围的范围。

___

### <a id="repaint" name="repaint"></a> repaint

▸ **repaint**(): `void`

**`description`** 重绘数据范围

#### Returns

`void`
