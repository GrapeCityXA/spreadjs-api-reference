# Interface: IButtonComboEditorOption

[Sheets](../modules/GC.Spread.Sheets.md).[Designer](../modules/GC.Spread.Sheets.Designer.md).IButtonComboEditorOption

## Hierarchy

- [`IBindingComponentBaseOption`](GC.Spread.Sheets.Designer.IBindingComponentBaseOption.md)

  ↳ **`IButtonComboEditorOption`**

## Table of contents

### Properties

- [bindingPath](GC.Spread.Sheets.Designer.IButtonComboEditorOption.md#bindingpath)
- [buttonClassName](GC.Spread.Sheets.Designer.IButtonComboEditorOption.md#buttonclassname)
- [className](GC.Spread.Sheets.Designer.IButtonComboEditorOption.md#classname)
- [enableWhen](GC.Spread.Sheets.Designer.IButtonComboEditorOption.md#enablewhen)
- [id](GC.Spread.Sheets.Designer.IButtonComboEditorOption.md#id)
- [margin](GC.Spread.Sheets.Designer.IButtonComboEditorOption.md#margin)
- [mutexWith](GC.Spread.Sheets.Designer.IButtonComboEditorOption.md#mutexwith)
- [popupWidth](GC.Spread.Sheets.Designer.IButtonComboEditorOption.md#popupwidth)
- [type](GC.Spread.Sheets.Designer.IButtonComboEditorOption.md#type)
- [visibleWhen](GC.Spread.Sheets.Designer.IButtonComboEditorOption.md#visiblewhen)

### Methods

- [generateItemsFunc](GC.Spread.Sheets.Designer.IButtonComboEditorOption.md#generateitemsfunc)
- [getValueFunc](GC.Spread.Sheets.Designer.IButtonComboEditorOption.md#getvaluefunc)
- [setValueFunc](GC.Spread.Sheets.Designer.IButtonComboEditorOption.md#setvaluefunc)

## Properties

### <a id="bindingpath" name="bindingpath"></a> bindingPath

• `Optional` **bindingPath**: `string`

#### Inherited from

[IBindingComponentBaseOption](GC.Spread.Sheets.Designer.IBindingComponentBaseOption.md).[bindingPath](GC.Spread.Sheets.Designer.IBindingComponentBaseOption.md#bindingpath)

___

### <a id="buttonclassname" name="buttonclassname"></a> buttonClassName

• **buttonClassName**: `string`

___

### <a id="classname" name="classname"></a> className

• `Optional` **className**: `string`

#### Inherited from

[IBindingComponentBaseOption](GC.Spread.Sheets.Designer.IBindingComponentBaseOption.md).[className](GC.Spread.Sheets.Designer.IBindingComponentBaseOption.md#classname)

___

### <a id="enablewhen" name="enablewhen"></a> enableWhen

• `Optional` **enableWhen**: `string`

#### Inherited from

[IBindingComponentBaseOption](GC.Spread.Sheets.Designer.IBindingComponentBaseOption.md).[enableWhen](GC.Spread.Sheets.Designer.IBindingComponentBaseOption.md#enablewhen)

___

### <a id="id" name="id"></a> id

• `Optional` **id**: `string`

#### Inherited from

[IBindingComponentBaseOption](GC.Spread.Sheets.Designer.IBindingComponentBaseOption.md).[id](GC.Spread.Sheets.Designer.IBindingComponentBaseOption.md#id)

___

### <a id="margin" name="margin"></a> margin

• `Optional` **margin**: `string`

#### Inherited from

[IBindingComponentBaseOption](GC.Spread.Sheets.Designer.IBindingComponentBaseOption.md).[margin](GC.Spread.Sheets.Designer.IBindingComponentBaseOption.md#margin)

___

### <a id="mutexwith" name="mutexwith"></a> mutexWith

• `Optional` **mutexWith**: `string`

#### Inherited from

[IBindingComponentBaseOption](GC.Spread.Sheets.Designer.IBindingComponentBaseOption.md).[mutexWith](GC.Spread.Sheets.Designer.IBindingComponentBaseOption.md#mutexwith)

___

### <a id="popupwidth" name="popupwidth"></a> popupWidth

• **popupWidth**: `number`

___

### <a id="type" name="type"></a> type

• **type**: ``"ButtonComboEditor"``

___

### <a id="visiblewhen" name="visiblewhen"></a> visibleWhen

• `Optional` **visibleWhen**: `string`

#### Inherited from

[IBindingComponentBaseOption](GC.Spread.Sheets.Designer.IBindingComponentBaseOption.md).[visibleWhen](GC.Spread.Sheets.Designer.IBindingComponentBaseOption.md#visiblewhen)

## Methods

### <a id="generateitemsfunc" name="generateitemsfunc"></a> generateItemsFunc

▸ **generateItemsFunc**(`v`): [`IListGroupItemData`](GC.Spread.Sheets.Designer.IListGroupItemData.md)[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `v` | `any` |

#### Returns

[`IListGroupItemData`](GC.Spread.Sheets.Designer.IListGroupItemData.md)[]

___

### <a id="getvaluefunc" name="getvaluefunc"></a> getValueFunc

▸ `Optional` **getValueFunc**(`instance`): `any`

#### Parameters

| Name | Type |
| :------ | :------ |
| `instance` | `any` |

#### Returns

`any`

___

### <a id="setvaluefunc" name="setvaluefunc"></a> setValueFunc

▸ `Optional` **setValueFunc**(`instance`, `v`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `instance` | `any` |
| `v` | `any` |

#### Returns

`void`
