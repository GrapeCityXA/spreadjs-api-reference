# Class: SubmitSnapshotRequest<S, T\>

## Type parameters

| Name |
| :------ |
| `S` |
| `T` |

## Table of contents

### Constructors

- [constructor](SubmitSnapshotRequest.md#constructor)

### Properties

- [context](SubmitSnapshotRequest.md#context)
- [doc](SubmitSnapshotRequest.md#doc)
- [document](SubmitSnapshotRequest.md#document)
- [extra](SubmitSnapshotRequest.md#extra)
- [fromVersion](SubmitSnapshotRequest.md#fromversion)
- [id](SubmitSnapshotRequest.md#id)
- [maxRetries](SubmitSnapshotRequest.md#maxretries)
- [ops](SubmitSnapshotRequest.md#ops)
- [retries](SubmitSnapshotRequest.md#retries)
- [saveMilestoneSnapshot](SubmitSnapshotRequest.md#savemilestonesnapshot)
- [saveSnapshot](SubmitSnapshotRequest.md#savesnapshot)
- [snapshot](SubmitSnapshotRequest.md#snapshot)
- [start](SubmitSnapshotRequest.md#start)
- [toVersion](SubmitSnapshotRequest.md#toversion)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new SubmitSnapshotRequest**<`S`, `T`\>()

#### Type parameters

| Name |
| :------ |
| `S` |
| `T` |

## Properties

### <a id="context" name="context"></a> context

• **context**: [`ISubmitSnapshotContext`](../interfaces/ISubmitSnapshotContext.md)<`T`\>

___

### <a id="doc" name="doc"></a> doc

• **doc**: [`DocumentServices`](DocumentServices.md)<`S`, `T`\>

___

### <a id="document" name="document"></a> document

• **document**: ``null`` \| [`IDocument`](../interfaces/IDocument.md)

___

### <a id="extra" name="extra"></a> extra

• **extra**: `unknown`

___

### <a id="fromversion" name="fromversion"></a> fromVersion

• **fromVersion**: `number`

___

### <a id="id" name="id"></a> id

• **id**: `string`

___

### <a id="maxretries" name="maxretries"></a> maxRetries

• `Optional` **maxRetries**: `number`

___

### <a id="ops" name="ops"></a> ops

• **ops**: ``null`` \| [`IOp`](../interfaces/IOp.md)<`T`\>[]

___

### <a id="retries" name="retries"></a> retries

• **retries**: `number`

___

### <a id="savemilestonesnapshot" name="savemilestonesnapshot"></a> saveMilestoneSnapshot

• **saveMilestoneSnapshot**: ``null`` \| `boolean`

___

### <a id="savesnapshot" name="savesnapshot"></a> saveSnapshot

• **saveSnapshot**: ``null`` \| `boolean`

___

### <a id="snapshot" name="snapshot"></a> snapshot

• **snapshot**: ``null`` \| [`ICommitSnapshot`](../interfaces/ICommitSnapshot.md)<`S`\>

___

### <a id="start" name="start"></a> start

• **start**: `number`

___

### <a id="toversion" name="toversion"></a> toVersion

• **toVersion**: `number`
