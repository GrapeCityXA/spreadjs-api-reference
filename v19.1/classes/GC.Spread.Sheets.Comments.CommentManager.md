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

表示可以管理工作表中所有批注的批注管理器。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheet` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 工作表。 |

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`row`, `col`, `text`): [`Comment`](GC.Spread.Sheets.Comments.Comment.md)

为指定行列的单元格添加批注。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 单元格的行索引。 |
| `col` | `number` | 单元格的列索引。 |
| `text` | `string` | 批注的文本。 |

#### Returns

[`Comment`](GC.Spread.Sheets.Comments.Comment.md)

已添加到单元格的批注。

___

### <a id="all" name="all"></a> all

▸ **all**(): [`Comment`](GC.Spread.Sheets.Comments.Comment.md)[]

获取工作表中的所有批注。

#### Returns

[`Comment`](GC.Spread.Sheets.Comments.Comment.md)[]

___

### <a id="clear" name="clear"></a> clear

▸ **clear**(`range`): `void`

清除工作表中指定范围内的所有批注。当未指定范围时，将清除工作表中的所有批注。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](GC.Spread.Sheets.Range.md) | 要清除所有批注的范围。 |

#### Returns

`void`

___

### <a id="get" name="get"></a> get

▸ **get**(`row`, `col`): [`Comment`](GC.Spread.Sheets.Comments.Comment.md)

获取指定行列单元格中的批注。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 单元格的行索引。 |
| `col` | `number` | 单元格的列索引。 |

#### Returns

[`Comment`](GC.Spread.Sheets.Comments.Comment.md)

指定单元格中的批注。

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`row`, `col`): `void`

移除指定行列单元格中的批注。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 单元格的行索引。 |
| `col` | `number` | 单元格的列索引。 |

#### Returns

`void`
