# Interface: ISnapshotFragmentsRequest<S\>

## Type parameters

| Name | Type |
| :------ | :------ |
| `S` | `unknown` |

## Table of contents

### Methods

- [createFragment](ISnapshotFragmentsRequest.md#createfragment)
- [deleteFragment](ISnapshotFragmentsRequest.md#deletefragment)
- [getFragment](ISnapshotFragmentsRequest.md#getfragment)
- [updateFragment](ISnapshotFragmentsRequest.md#updatefragment)

## Methods

### <a id="createfragment" name="createfragment"></a> createFragment

▸ **createFragment**(`id`, `data`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `data` | `S` |

#### Returns

`Promise`<`void`\>

___

### <a id="deletefragment" name="deletefragment"></a> deleteFragment

▸ **deleteFragment**(`id`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |

#### Returns

`Promise`<`void`\>

___

### <a id="getfragment" name="getfragment"></a> getFragment

▸ **getFragment**(`id`): `Promise`<``null`` \| `S`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |

#### Returns

`Promise`<``null`` \| `S`\>

___

### <a id="updatefragment" name="updatefragment"></a> updateFragment

▸ **updateFragment**(`id`, `data`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `data` | `S` |

#### Returns

`Promise`<`void`\>
