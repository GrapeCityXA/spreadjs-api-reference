# Class: DataRangeManager

[Sheets](../modules/GC.Spread.Sheets.md).[DataRange](../modules/GC.Spread.Sheets.DataRange.md).DataRangeManager

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.DataRange.DataRangeManager.md#constructor)

### Methods

- [add](GC.Spread.Sheets.DataRange.DataRangeManager.md#add)
- [all](GC.Spread.Sheets.DataRange.DataRangeManager.md#all)
- [clear](GC.Spread.Sheets.DataRange.DataRangeManager.md#clear)
- [get](GC.Spread.Sheets.DataRange.DataRangeManager.md#get)
- [remove](GC.Spread.Sheets.DataRange.DataRangeManager.md#remove)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new DataRangeManager**(`sheet`)

**`description`** 表示一个数据范围管理器。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheet` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 工作表。 |

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`name`, `dataProvider`, `range`, `options?`): [`DataRange`](GC.Spread.Sheets.DataRange.DataRange.md)

**`description`** 添加一个数据范围。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 数据范围名称。 |
| `dataProvider` | `string` \| [`IDataProvider`](../interfaces/GC.Spread.Sheets.DataRange.IDataProvider.md) | 数据提供者。字符串类型表示计算表名称，它将创建一个TableSheetDataProvider。 |
| `range` | [`Range`](GC.Spread.Sheets.Range.md) | 数据范围的范围。 |
| `options?` | [`IDataRangeOptions`](../interfaces/GC.Spread.Sheets.DataRange.IDataRangeOptions.md) | - |

#### Returns

[`DataRange`](GC.Spread.Sheets.DataRange.DataRange.md)

添加的数据范围。

___

### <a id="all" name="all"></a> all

▸ **all**(): [`DataRange`](GC.Spread.Sheets.DataRange.DataRange.md)[]

**`description`** 获取所有数据范围。

#### Returns

[`DataRange`](GC.Spread.Sheets.DataRange.DataRange.md)[]

数据范围实例数组。默认为空数组。

___

### <a id="clear" name="clear"></a> clear

▸ **clear**(): `void`

**`description`** 移除所有数据范围。

#### Returns

`void`

___

### <a id="get" name="get"></a> get

▸ **get**(`name`): [`DataRange`](GC.Spread.Sheets.DataRange.DataRange.md)

**`description`** 获取一个数据范围。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 数据范围名称。 |

#### Returns

[`DataRange`](GC.Spread.Sheets.DataRange.DataRange.md)

目标数据范围。

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`name`): `void`

**`description`** 移除一个数据范围。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 数据范围名称。 |

#### Returns

`void`
