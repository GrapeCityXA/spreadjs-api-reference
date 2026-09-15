# Class: Collection<T\>

[Sheets](../modules/GC.Spread.Sheets.md).[GanttSheet](../modules/GC.Spread.Sheets.GanttSheet.md).Collection

## Type parameters

| Name |
| :------ |
| `T` |

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.GanttSheet.Collection.md#constructor)

### Methods

- [add](GC.Spread.Sheets.GanttSheet.Collection.md#add)
- [all](GC.Spread.Sheets.GanttSheet.Collection.md#all)
- [clear](GC.Spread.Sheets.GanttSheet.Collection.md#clear)
- [getIndexByItem](GC.Spread.Sheets.GanttSheet.Collection.md#getindexbyitem)
- [getItemAt](GC.Spread.Sheets.GanttSheet.Collection.md#getitemat)
- [getRule](GC.Spread.Sheets.GanttSheet.Collection.md#getrule)
- [insert](GC.Spread.Sheets.GanttSheet.Collection.md#insert)
- [length](GC.Spread.Sheets.GanttSheet.Collection.md#length)
- [remove](GC.Spread.Sheets.GanttSheet.Collection.md#remove)
- [removeAt](GC.Spread.Sheets.GanttSheet.Collection.md#removeat)
- [setItemAt](GC.Spread.Sheets.GanttSheet.Collection.md#setitemat)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Collection**<`T`\>()

创建一个集合实例。

**`classdesc`** 一个对象集合。

#### Type parameters

| Name |
| :------ |
| `T` |

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`item`): `void`

将项目添加到列表中。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | `T` | 要添加的项目 |

#### Returns

`void`

___

### <a id="all" name="all"></a> all

▸ **all**(): `T`[]

获取所有项目表单集合。

#### Returns

`T`[]

收集项列表。

___

### <a id="clear" name="clear"></a> clear

▸ **clear**(): `void`

从列表中删除所有项目。

#### Returns

`void`

___

### <a id="getindexbyitem" name="getindexbyitem"></a> getIndexByItem

▸ **getIndexByItem**(`item`): `number`

从收集列表中获取项目索引。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | `T` | 集合的项目 |

#### Returns

`number`

集合列表中的项目索引。

___

### <a id="getitemat" name="getitemat"></a> getItemAt

▸ **getItemAt**(`index`): `T`

获取具有相应索引的项目

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 收集列表索引 |

#### Returns

`T`

指定名称的规则。

___

### <a id="getrule" name="getrule"></a> getRule

▸ **getRule**(`name`): ``null`` \| `T`

获取带有指定名称的项目。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 字符串值指示规则的名称 |

#### Returns

``null`` \| `T`

指定名称的规则。

___

### <a id="insert" name="insert"></a> insert

▸ **insert**(`item`): `void`

将项目插入列表中。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | `T` | 要插入的项目 |

#### Returns

`void`

___

### <a id="length" name="length"></a> length

▸ **length**(): `number`

获取收集列表长度。

#### Returns

`number`

收集列表长度。

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`item`): `void`

从列表中删除项目。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | `T` | 要删除的项目 |

#### Returns

`void`

___

### <a id="removeat" name="removeat"></a> removeAt

▸ **removeAt**(`index`): `void`

从索引中删除相应的项目

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 收集列表索引 |

#### Returns

`void`

___

### <a id="setitemat" name="setitemat"></a> setItemAt

▸ **setItemAt**(`index`, `item`): `void`

将项目设置为索引。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 插入的索引 |
| `item` | `T` | 项目 |

#### Returns

`void`
