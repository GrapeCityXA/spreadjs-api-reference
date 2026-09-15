# Interface: IIncrementalLoadingOptions

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).IIncrementalLoadingOptions

## Table of contents

### Methods

- [loaded](GC.Spread.Sheets.IIncrementalLoadingOptions.md#loaded)
- [loading](GC.Spread.Sheets.IIncrementalLoadingOptions.md#loading)

## Methods

### <a id="loaded" name="loaded"></a> loaded

▸ `Optional` **loaded**(): `void`

增量加载完成时的回调函数。

#### Returns

`void`

___

### <a id="loading" name="loading"></a> loading

▸ `Optional` **loading**(`progress`, `args`): `void`

增量加载过程中的回调函数。

#### Parameters

| Name | Type |
| :------ | :------ |
| `progress` | `number` |
| `args` | `Object` |
| `args.sheet` | [`Worksheet`](../classes/GC.Spread.Sheets.Worksheet.md) |

#### Returns

`void`
