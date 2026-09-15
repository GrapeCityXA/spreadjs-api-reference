# Class: ThreadedCommentManager

[Sheets](../modules/GC.Spread.Sheets.md).[ThreadedComments](../modules/GC.Spread.Sheets.ThreadedComments.md).ThreadedCommentManager

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.ThreadedComments.ThreadedCommentManager.md#constructor)

### Methods

- [add](GC.Spread.Sheets.ThreadedComments.ThreadedCommentManager.md#add)
- [all](GC.Spread.Sheets.ThreadedComments.ThreadedCommentManager.md#all)
- [clear](GC.Spread.Sheets.ThreadedComments.ThreadedCommentManager.md#clear)
- [get](GC.Spread.Sheets.ThreadedComments.ThreadedCommentManager.md#get)
- [remove](GC.Spread.Sheets.ThreadedComments.ThreadedCommentManager.md#remove)
- [size](GC.Spread.Sheets.ThreadedComments.ThreadedCommentManager.md#size)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new ThreadedCommentManager**()

表示一个用于在工作表上添加、检索、删除、枚举和序列化嵌套评论的嵌套评论管理器。

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`row`, `col`, `replies?`): ``null`` \| [`ThreadedComment`](GC.Spread.Sheets.ThreadedComments.ThreadedComment.md)

向指定单元格添加评论。

**`example`**
```javascript
const activeSheet = spread.getActiveSheet();
const threadedCommentManager = activeSheet.threadedComments;
const tc = threadedCommentManager.add(1, 1);
tc.add({ message: [{ type: GC.Spread.Sheets.ThreadedComments.ContentType.text, value: 'hello' }] });
const allReplies = tc.all();
console.log(allReplies);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |
| `replies?` | [`IReply`](../interfaces/GC.Spread.Sheets.ThreadedComments.IReply.md)[] | 要追加的回复。 |

#### Returns

``null`` \| [`ThreadedComment`](GC.Spread.Sheets.ThreadedComments.ThreadedComment.md)

评论实例。

___

### <a id="all" name="all"></a> all

▸ **all**(): [`ThreadedComment`](GC.Spread.Sheets.ThreadedComments.ThreadedComment.md)[]

获取工作表上所有的评论，并将其放入一个数组中。

**`example`**
```javascript
const activeSheet = spread.getActiveSheet();
const threadedCommentManager = activeSheet.threadedComments;
const allComments = threadedCommentManager.all();
console.log(allComments);
```

#### Returns

[`ThreadedComment`](GC.Spread.Sheets.ThreadedComments.ThreadedComment.md)[]

___

### <a id="clear" name="clear"></a> clear

▸ **clear**(`range?`): `void`

清除指定范围内的评论。如果未指定范围，则清除工作表中的所有评论。

**`example`**
```javascript
const activeSheet = spread.getActiveSheet();
const threadedCommentManager = activeSheet.threadedComments;
threadedCommentManager.clear(new GC.Spread.Sheets.Range(1, 1, 3, 3));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range?` | [`Range`](GC.Spread.Sheets.Range.md) | 要从中清除所有评论的范围。 |

#### Returns

`void`

___

### <a id="get" name="get"></a> get

▸ **get**(`row`, `col`): `undefined` \| [`ThreadedComment`](GC.Spread.Sheets.ThreadedComments.ThreadedComment.md)

获取指定单元格的评论。

**`example`**
```javascript
const activeSheet = spread.getActiveSheet();
const threadedCommentManager = activeSheet.threadedComments;
const threadedComment = threadedCommentManager.get(1, 1);
console.log(threadedComment);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |

#### Returns

`undefined` \| [`ThreadedComment`](GC.Spread.Sheets.ThreadedComments.ThreadedComment.md)

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`row`, `col`): `undefined` \| [`ThreadedComment`](GC.Spread.Sheets.ThreadedComments.ThreadedComment.md)

删除指定单元格处的评论。

**`example`**
```javascript
const activeSheet = spread.getActiveSheet();
const threadedCommentManager = activeSheet.threadedComments;
threadedCommentManager.remove(1, 1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `col` | `number` | 列索引。 |

#### Returns

`undefined` \| [`ThreadedComment`](GC.Spread.Sheets.ThreadedComments.ThreadedComment.md)

___

### <a id="size" name="size"></a> size

▸ **size**(): `number`

获取工作表上的评论数量。

**`example`**
```javascript
const activeSheet = spread.getActiveSheet();
const threadedCommentManager = activeSheet.threadedComments;
const size = threadedCommentManager.size();
console.log(size);
```

#### Returns

`number`
