# Class: ThreadedComment

[Sheets](../modules/GC.Spread.Sheets.md).[ThreadedComments](../modules/GC.Spread.Sheets.ThreadedComments.md).ThreadedComment

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.ThreadedComments.ThreadedComment.md#constructor)

### Methods

- [add](GC.Spread.Sheets.ThreadedComments.ThreadedComment.md#add)
- [all](GC.Spread.Sheets.ThreadedComments.ThreadedComment.md#all)
- [col](GC.Spread.Sheets.ThreadedComments.ThreadedComment.md#col)
- [get](GC.Spread.Sheets.ThreadedComments.ThreadedComment.md#get)
- [remove](GC.Spread.Sheets.ThreadedComments.ThreadedComment.md#remove)
- [resolved](GC.Spread.Sheets.ThreadedComments.ThreadedComment.md#resolved)
- [row](GC.Spread.Sheets.ThreadedComments.ThreadedComment.md#row)
- [set](GC.Spread.Sheets.ThreadedComments.ThreadedComment.md#set)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new ThreadedComment**()

支持添加、读取、更新、删除回复和序列化的评论对象。

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`reply`): ``null`` \| [`IReply`](../interfaces/GC.Spread.Sheets.ThreadedComments.IReply.md)

添加回复。如果未提供回复，将使用当前用户的ID和当前时间。

**`example`**
```javascript
const activeSheet = spread.getActiveSheet();
const threadedCommentManager = activeSheet.threadedComments;
const tc = threadedCommentManager.add(1, 1);
const reply = tc.add({ message: [{ type: GC.Spread.Sheets.ThreadedComments.ContentType.text, value: 'hello' }] });
console.log(reply);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `reply` | [`IReply`](../interfaces/GC.Spread.Sheets.ThreadedComments.IReply.md) | 要添加的回复。 |

#### Returns

``null`` \| [`IReply`](../interfaces/GC.Spread.Sheets.ThreadedComments.IReply.md)

___

### <a id="all" name="all"></a> all

▸ **all**(`replies?`): [`IReply`](../interfaces/GC.Spread.Sheets.ThreadedComments.IReply.md)[]

获取或设置所有回复；当提供数组时，将它们添加到当前评论中。

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

| Name | Type |
| :------ | :------ |
| `replies?` | [`IReply`](../interfaces/GC.Spread.Sheets.ThreadedComments.IReply.md)[] |

#### Returns

[`IReply`](../interfaces/GC.Spread.Sheets.ThreadedComments.IReply.md)[]

___

### <a id="col" name="col"></a> col

▸ **col**(): `number`

获取嵌套评论的列。

**`example`**
```javascript
const activeSheet = spread.getActiveSheet();
const threadedCommentManager = activeSheet.threadedComments;
const tc = threadedCommentManager.add(1, 1);
const col = tc.col();
console.log(col);
```

#### Returns

`number`

___

### <a id="get" name="get"></a> get

▸ **get**(`index`): `undefined` \| [`IReply`](../interfaces/GC.Spread.Sheets.ThreadedComments.IReply.md)

按索引获取回复。

**`example`**
```javascript
const activeSheet = spread.getActiveSheet();
const threadedCommentManager = activeSheet.threadedComments;
const tc = threadedCommentManager.add(1, 1);
tc.add({ message: [{ type: GC.Spread.Sheets.ThreadedComments.ContentType.text, value: 'hello' }] });
const reply = tc.get(0);
console.log(reply);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 回复索引的从零开始。 |

#### Returns

`undefined` \| [`IReply`](../interfaces/GC.Spread.Sheets.ThreadedComments.IReply.md)

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`index`): ``null`` \| [`IReply`](../interfaces/GC.Spread.Sheets.ThreadedComments.IReply.md)

按索引删除回复。

**`example`**
```javascript
const activeSheet = spread.getActiveSheet();
const threadedCommentManager = activeSheet.threadedComments;
const tc = threadedCommentManager.add(1, 1);
tc.add({ message: [{ type: GC.Spread.Sheets.ThreadedComments.ContentType.text, value: 'hello' }] });
tc.add({ message: [{ type: GC.Spread.Sheets.ThreadedComments.ContentType.text, value: 'world' }] });
tc.remove(0);
console.log(tc.get(0));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 回复索引。 |

#### Returns

``null`` \| [`IReply`](../interfaces/GC.Spread.Sheets.ThreadedComments.IReply.md)

___

### <a id="resolved" name="resolved"></a> resolved

▸ **resolved**(`resolved?`): `boolean`

获取或设置评论是否已解决。

**`example`**
```javascript
const activeSheet = spread.getActiveSheet();
const threadedCommentManager = activeSheet.threadedComments;
const tc = threadedCommentManager.add(1, 1);
tc.add({ message: [{ type: GC.Spread.Sheets.ThreadedComments.ContentType.text, value: 'hello' }] });
tc.resolved(true);
console.log(tc.resolved());
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `resolved?` | `boolean` |

#### Returns

`boolean`

___

### <a id="row" name="row"></a> row

▸ **row**(): `number`

获取 threaded comment 的行。

**`example`**
```javascript
const activeSheet = spread.getActiveSheet();
const threadedCommentManager = activeSheet.threadedComments;
const tc = threadedCommentManager.add(1, 1);
const row = tc.row();
console.log(row);
```

#### Returns

`number`

___

### <a id="set" name="set"></a> set

▸ **set**(`index`, `reply`): `void`

更新回复的内容和元数据。

**`example`**
```javascript
const activeSheet = spread.getActiveSheet();
const threadedCommentManager = activeSheet.threadedComments;
const tc = threadedCommentManager.add(1, 1);
tc.add({ message: [{ type: GC.Spread.Sheets.ThreadedComments.ContentType.text, value: 'hello' }] });
tc.set(0, { message: [{ type: GC.Spread.Sheets.ThreadedComments.ContentType.text, value: 'hello, world' }] });
console.log(tc.get(0));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 回复索引。 |
| `reply` | [`IReply`](../interfaces/GC.Spread.Sheets.ThreadedComments.IReply.md) | 新回复。 |

#### Returns

`void`
