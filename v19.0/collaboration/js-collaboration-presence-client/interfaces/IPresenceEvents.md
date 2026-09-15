# Interface: IPresenceEvents<P\>

## Type parameters

| Name |
| :------ |
| `P` |

## Table of contents

### Methods

- [add](IPresenceEvents.md#add)
- [remove](IPresenceEvents.md#remove)
- [update](IPresenceEvents.md#update)

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`addedPresences`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `addedPresences` | [`IPresences`](IPresences.md)<`P`\> |

#### Returns

`void`

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`removedPresencesIds`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `removedPresencesIds` | `string`[] |

#### Returns

`void`

___

### <a id="update" name="update"></a> update

▸ **update**(`updatedPresences`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `updatedPresences` | [`IPresences`](IPresences.md)<`P`\> |

#### Returns

`void`
