# Interface: IRowActionOptions

[Sheets](../modules/GC.Spread.Sheets.md).[TableSheet](../modules/GC.Spread.Sheets.TableSheet.md).IRowActionOptions

## Table of contents

### Properties

- [command](GC.Spread.Sheets.TableSheet.IRowActionOptions.md#command)
- [iconSize](GC.Spread.Sheets.TableSheet.IRowActionOptions.md#iconsize)
- [icons](GC.Spread.Sheets.TableSheet.IRowActionOptions.md#icons)
- [name](GC.Spread.Sheets.TableSheet.IRowActionOptions.md#name)
- [shortcutKey](GC.Spread.Sheets.TableSheet.IRowActionOptions.md#shortcutkey)
- [tooltip](GC.Spread.Sheets.TableSheet.IRowActionOptions.md#tooltip)

### Methods

- [iconSelector](GC.Spread.Sheets.TableSheet.IRowActionOptions.md#iconselector)

## Properties

### <a id="command" name="command"></a> command

• `Optional` **command**: `string`

___

### <a id="iconsize" name="iconsize"></a> iconSize

• `Optional` **iconSize**: `number` \| [`IImageSize`](GC.Spread.Sheets.IImageSize.md)

___

### <a id="icons" name="icons"></a> icons

• `Optional` **icons**: (`string` \| [`ButtonImageType`](../enums/GC.Spread.Sheets.ButtonImageType.md))[]

___

### <a id="name" name="name"></a> name

• `Optional` **name**: `string`

___

### <a id="shortcutkey" name="shortcutkey"></a> shortcutKey

• `Optional` **shortcutKey**: [`IShortcutKey`](GC.Spread.Sheets.TableSheet.IShortcutKey.md)

___

### <a id="tooltip" name="tooltip"></a> tooltip

• `Optional` **tooltip**: `string`

## Methods

### <a id="iconselector" name="iconselector"></a> iconSelector

▸ `Optional` **iconSelector**(`item`, `index`, `context`): `number` \| `boolean`

#### Parameters

| Name | Type |
| :------ | :------ |
| `item` | `any` |
| `index` | `number` |
| `context` | `any` |

#### Returns

`number` \| `boolean`
