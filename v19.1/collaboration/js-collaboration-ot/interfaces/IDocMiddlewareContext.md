# Interface: IDocMiddlewareContext<S, T\>

定义文档中间件操作的上下文。

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
- [readOp](IDocMiddlewareContext.md#readop)
- [readSnapshots](IDocMiddlewareContext.md#readsnapshots)
- [receive](IDocMiddlewareContext.md#receive)
- [reply](IDocMiddlewareContext.md#reply)
- [submit](IDocMiddlewareContext.md#submit)

## Properties

### <a id="afterwrite" name="afterwrite"></a> afterWrite

• **afterWrite**: [`IDocSubmitMiddlewareContext`](IDocSubmitMiddlewareContext.md)<`S`, `T`\>

当操作成功写入数据库后的上下文。

___

### <a id="apply" name="apply"></a> apply

• **apply**: [`IDocSubmitMiddlewareContext`](IDocSubmitMiddlewareContext.md)<`S`, `T`\>

当将操作应用到快照时的上下文。

___

### <a id="commit" name="commit"></a> commit

• **commit**: [`IDocSubmitMiddlewareContext`](IDocSubmitMiddlewareContext.md)<`S`, `T`\>

当准备将操作提交到数据库时的上下文。

___

### <a id="readop" name="readop"></a> readOp

• **readOp**: [`IDocReadOpMiddlewareContext`](IDocReadOpMiddlewareContext.md)<`T`\>

当从数据库加载操作时的上下文。

___

### <a id="readsnapshots" name="readsnapshots"></a> readSnapshots

• **readSnapshots**: [`IDocReadSnapshotsMiddlewareContext`](IDocReadSnapshotsMiddlewareContext.md)<`S`\>

当从数据库加载一个或多个快照用于 fetch 或 subscribe 操作时的上下文。

___

### <a id="receive" name="receive"></a> receive

• **receive**: [`IDocReceiveMiddlewareContext`](IDocReceiveMiddlewareContext.md)<`T`\>

当文档收到来自客户端的消息时的上下文。

___

### <a id="reply" name="reply"></a> reply

• **reply**: [`IDocReplyMiddlewareContext`](IDocReplyMiddlewareContext.md)<`S`, `T`\>

当文档即将发送非错误回复到客户端消息时的上下文。

___

### <a id="submit" name="submit"></a> submit

• **submit**: [`IDocSubmitMiddlewareContext`](IDocSubmitMiddlewareContext.md)<`S`, `T`\>

当发起提交操作时的上下文。
