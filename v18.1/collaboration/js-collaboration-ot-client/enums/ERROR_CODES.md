# Enumeration: ERROR\_CODES

OT 错误的错误代码。

## Table of contents

### Enumeration members

- [ERR\_DOC\_ALREADY\_CREATED](ERROR_CODES.md#err_doc_already_created)
- [ERR\_DOC\_DOES\_NOT\_EXIST](ERROR_CODES.md#err_doc_does_not_exist)
- [ERR\_DOC\_TYPE\_NOT\_RECOGNIZED](ERROR_CODES.md#err_doc_type_not_recognized)
- [ERR\_DOC\_WAS\_DELETED](ERROR_CODES.md#err_doc_was_deleted)
- [ERR\_HARD\_ROLLBACK\_FETCH\_FAILED](ERROR_CODES.md#err_hard_rollback_fetch_failed)
- [ERR\_HISTORY\_SNAPSHOT\_NOT\_FOUND](ERROR_CODES.md#err_history_snapshot_not_found)
- [ERR\_MAX\_SUBMIT\_RETRIES\_EXCEEDED](ERROR_CODES.md#err_max_submit_retries_exceeded)
- [ERR\_MAX\_SUBMIT\_SNAPSHOT\_RETRIES\_EXCEEDED](ERROR_CODES.md#err_max_submit_snapshot_retries_exceeded)
- [ERR\_MESSAGE\_BADLY\_FORMED](ERROR_CODES.md#err_message_badly_formed)
- [ERR\_OP\_ALREADY\_SUBMITTED](ERROR_CODES.md#err_op_already_submitted)
- [ERR\_OT\_OP\_NOT\_APPLIED](ERROR_CODES.md#err_ot_op_not_applied)
- [ERR\_OT\_OP\_TRANSFORM\_FAILED](ERROR_CODES.md#err_ot_op_transform_failed)
- [ERR\_SNAPSHOT\_READS\_REJECTED](ERROR_CODES.md#err_snapshot_reads_rejected)
- [ERR\_SUBMIT\_TRANSFORM\_OPS\_NOT\_FOUND](ERROR_CODES.md#err_submit_transform_ops_not_found)
- [ERR\_UNKNOWN\_ERROR](ERROR_CODES.md#err_unknown_error)

## Enumeration members

### <a id="err_doc_already_created" name="err_doc_already_created"></a> ERR\_DOC\_ALREADY\_CREATED

• **ERR\_DOC\_ALREADY\_CREATED**

___

### <a id="err_doc_does_not_exist" name="err_doc_does_not_exist"></a> ERR\_DOC\_DOES\_NOT\_EXIST

• **ERR\_DOC\_DOES\_NOT\_EXIST**

___

### <a id="err_doc_type_not_recognized" name="err_doc_type_not_recognized"></a> ERR\_DOC\_TYPE\_NOT\_RECOGNIZED

• **ERR\_DOC\_TYPE\_NOT\_RECOGNIZED**

___

### <a id="err_doc_was_deleted" name="err_doc_was_deleted"></a> ERR\_DOC\_WAS\_DELETED

• **ERR\_DOC\_WAS\_DELETED**

___

### <a id="err_hard_rollback_fetch_failed" name="err_hard_rollback_fetch_failed"></a> ERR\_HARD\_ROLLBACK\_FETCH\_FAILED

• **ERR\_HARD\_ROLLBACK\_FETCH\_FAILED**

___

### <a id="err_history_snapshot_not_found" name="err_history_snapshot_not_found"></a> ERR\_HISTORY\_SNAPSHOT\_NOT\_FOUND

• **ERR\_HISTORY\_SNAPSHOT\_NOT\_FOUND**

___

### <a id="err_max_submit_retries_exceeded" name="err_max_submit_retries_exceeded"></a> ERR\_MAX\_SUBMIT\_RETRIES\_EXCEEDED

• **ERR\_MAX\_SUBMIT\_RETRIES\_EXCEEDED**

___

### <a id="err_max_submit_snapshot_retries_exceeded" name="err_max_submit_snapshot_retries_exceeded"></a> ERR\_MAX\_SUBMIT\_SNAPSHOT\_RETRIES\_EXCEEDED

• **ERR\_MAX\_SUBMIT\_SNAPSHOT\_RETRIES\_EXCEEDED**

___

### <a id="err_message_badly_formed" name="err_message_badly_formed"></a> ERR\_MESSAGE\_BADLY\_FORMED

• **ERR\_MESSAGE\_BADLY\_FORMED**

___

### <a id="err_op_already_submitted" name="err_op_already_submitted"></a> ERR\_OP\_ALREADY\_SUBMITTED

• **ERR\_OP\_ALREADY\_SUBMITTED**

___

### <a id="err_ot_op_not_applied" name="err_ot_op_not_applied"></a> ERR\_OT\_OP\_NOT\_APPLIED

• **ERR\_OT\_OP\_NOT\_APPLIED**

___

### <a id="err_ot_op_transform_failed" name="err_ot_op_transform_failed"></a> ERR\_OT\_OP\_TRANSFORM\_FAILED

• **ERR\_OT\_OP\_TRANSFORM\_FAILED**

___

### <a id="err_snapshot_reads_rejected" name="err_snapshot_reads_rejected"></a> ERR\_SNAPSHOT\_READS\_REJECTED

• **ERR\_SNAPSHOT\_READS\_REJECTED**

"readSnapshots" 中间件拒绝了特定快照的读取。

此错误代码主要用于服务器使用，通常不会在客户端遇到。
相反，每个遇到错误的特定文档将收到其特定的错误。

一个例外是查询，其中对特定快照的 "readSnapshots" 拒绝将导致客户端收到整个查询的此错误，
因为查询不支持文档特定的错误。

___

### <a id="err_submit_transform_ops_not_found" name="err_submit_transform_ops_not_found"></a> ERR\_SUBMIT\_TRANSFORM\_OPS\_NOT\_FOUND

• **ERR\_SUBMIT\_TRANSFORM\_OPS\_NOT\_FOUND**

___

### <a id="err_unknown_error" name="err_unknown_error"></a> ERR\_UNKNOWN\_ERROR

• **ERR\_UNKNOWN\_ERROR**
