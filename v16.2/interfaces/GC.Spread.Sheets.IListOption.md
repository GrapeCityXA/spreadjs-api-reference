# Interface: IListOption

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).IListOption

## Table of contents

### Properties

- [items](GC.Spread.Sheets.IListOption.md#items)
- [layout](GC.Spread.Sheets.IListOption.md#layout)
- [multiSelect](GC.Spread.Sheets.IListOption.md#multiselect)
- [text](GC.Spread.Sheets.IListOption.md#text)
- [valueType](GC.Spread.Sheets.IListOption.md#valuetype)

### Methods

- [onItemSelected](GC.Spread.Sheets.IListOption.md#onitemselected)

## Properties

### <a id="items" name="items"></a> items

• **items**: [`IListItem`](GC.Spread.Sheets.IListItem.md)[] \| [`IListOption`](GC.Spread.Sheets.IListOption.md)[] \| () => `HTMLElement`

a function returns a DOM element

___

### <a id="layout" name="layout"></a> layout

• `Optional` **layout**: [`IListLayout`](GC.Spread.Sheets.IListLayout.md)

___

### <a id="multiselect" name="multiselect"></a> multiSelect

• `Optional` **multiSelect**: `boolean`

___

### <a id="text" name="text"></a> text

• `Optional` **text**: `string`

___

### <a id="valuetype" name="valuetype"></a> valueType

• `Optional` **valueType**: [`DropdownListValue`](../enums/GC.Spread.Sheets.DropdownListValue.md)

## Methods

### <a id="onitemselected" name="onitemselected"></a> onItemSelected

▸ `Optional` **onItemSelected**(`e`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `e` | `MouseEvent` |

#### Returns

`string`
