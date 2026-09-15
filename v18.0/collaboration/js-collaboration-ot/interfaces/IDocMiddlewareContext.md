# Interface: IDocMiddlewareContext<S, T\>

文档中间件的上下文。

## Type parameters

| Name |
| :------ |
| `S` |
| `T` |

## Table of contents

### Properties

- [afterWrite](IDocMiddlewareContext.md#afterwrite)
- [apply](IDocMiddlewareContext.md#apply)
- [commit](IDocMiddlewareContext.md#commit)
- [commitSnapshot](IDocMiddlewareContext.md#commitsnapshot)
- [readOp](IDocMiddlewareContext.md#readop)
- [readSnapshots](IDocMiddlewareContext.md#readsnapshots)
- [receive](IDocMiddlewareContext.md#receive)
- [reply](IDocMiddlewareContext.md#reply)
- [submit](IDocMiddlewareContext.md#submit)
- [submitSnapshot](IDocMiddlewareContext.md#submitsnapshot)

## Properties

### <a id="afterwrite" name="afterwrite"></a> afterWrite

• **afterWrite**: [`IDocSubmitMiddlewareContext`](IDocSubmitMiddlewareContext.md)<`S`, `T`\>

一个操作已成功写入数据库。

___

### <a id="apply" name="apply"></a> apply

• **apply**: [`IDocSubmitSnapshotMiddlewareContext`](IDocSubmitSnapshotMiddlewareContext.md)<`S`, `T`\>

该操作即将应用到快照上。

___

### <a id="commit" name="commit"></a> commit

• **commit**: [`IDocSubmitMiddlewareContext`](IDocSubmitMiddlewareContext.md)<`S`, `T`\>

一个操作准备提交到数据库。

___

### <a id="commitsnapshot" name="commitsnapshot"></a> commitSnapshot

• **commitSnapshot**: [`IDocSubmitSnapshotMiddlewareContext`](IDocSubmitSnapshotMiddlewareContext.md)<`S`, `T`\>

一个快照准备提交到数据库。

___

### <a id="readop" name="readop"></a> readOp

• **readOp**: [`IDocReadOpMiddlewareContext`](IDocReadOpMiddlewareContext.md)<`T`\>

一个操作已从数据库加载。

___

### <a id="readsnapshots" name="readsnapshots"></a> readSnapshots

• **readSnapshots**: [`IDocReadSnapshotsMiddlewareContext`](IDocReadSnapshotsMiddlewareContext.md)<`S`\>

为了执行获取或订阅操作，已从数据库加载一个或多个快照。

___

### <a id="receive" name="receive"></a> receive

• **receive**: [`IDocReceiveMiddlewareContext`](IDocReceiveMiddlewareContext.md)<`T`\>

文档接收到来自客户端的消息。

___

### <a id="reply" name="reply"></a> reply

• **reply**: [`IDocReplyMiddlewareContext`](IDocReplyMiddlewareContext.md)<`S`, `T`\>

文档即将向客户端消息发送一个非错误回复。

___

### <a id="submit" name="submit"></a> submit

• **submit**: [`IDocSubmitMiddlewareContext`](IDocSubmitMiddlewareContext.md)<`S`, `T`\>

开始提交一个操作。

___

### <a id="submitsnapshot" name="submitsnapshot"></a> submitSnapshot

• **submitSnapshot**: [`IDocSubmitSnapshotMiddlewareContext`](IDocSubmitSnapshotMiddlewareContext.md)<`S`, `T`\>

开始提交快照。
