# Class: CommentManager

[Sheets](../modules/GC.Spread.Sheets.md).[Comments](../modules/GC.Spread.Sheets.Comments.md).CommentManager

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Comments.CommentManager.md#constructor)

### Methods

- [add](GC.Spread.Sheets.Comments.CommentManager.md#add)
- [all](GC.Spread.Sheets.Comments.CommentManager.md#all)
- [clear](GC.Spread.Sheets.Comments.CommentManager.md#clear)
- [get](GC.Spread.Sheets.Comments.CommentManager.md#get)
- [remove](GC.Spread.Sheets.Comments.CommentManager.md#remove)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new CommentManager**(`sheet`)

一个可以管理表单中所有批注的批注管理器

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheet` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 表单 |

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`row`, `col`, `text`): [`Comment`](GC.Spread.Sheets.Comments.Comment.md)

在单元格中为指定的行和列添加批注

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 单元格的行索引 |
| `col` | `number` | 单元格的列索引 |
| `text` | `string` | 批注文本 |

#### Returns

[`Comment`](GC.Spread.Sheets.Comments.Comment.md)

已添加到单元格的批注

___

### <a id="all" name="all"></a> all

▸ **all**(): [`Comment`](GC.Spread.Sheets.Comments.Comment.md)[]

获取表单中所有批注

#### Returns

[`Comment`](GC.Spread.Sheets.Comments.Comment.md)[]

___

### <a id="clear" name="clear"></a> clear

▸ **clear**(`range`): `void`

清除表单中指示区域内的所有批注如果未指定区域,它将清除表单中的所有批注

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](GC.Spread.Sheets.Range.md) | 您要清除的所有批注区域 |

#### Returns

`void`

___

### <a id="get" name="get"></a> get

▸ **get**(`row`, `col`): [`Comment`](GC.Spread.Sheets.Comments.Comment.md)

获取指定行和列的单元格中的批注

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 单元格的行索引 |
| `col` | `number` | 单元格的列索引 |

#### Returns

[`Comment`](GC.Spread.Sheets.Comments.Comment.md)

指定单元格中的批注

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`row`, `col`): `void`

从指定行和列的单元格中删除批注

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 单元格的行索引 |
| `col` | `number` | 单元格的列索引 |

#### Returns

`void`
