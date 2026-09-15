# Class: PDFFontsManager

[Sheets](../modules/GC.Spread.Sheets.md).[PDF](../modules/GC.Spread.Sheets.PDF.md).PDFFontsManager

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.PDF.PDFFontsManager.md#constructor)

### Methods

- [fallbackFont](GC.Spread.Sheets.PDF.PDFFontsManager.md#fallbackfont)
- [registerFont](GC.Spread.Sheets.PDF.PDFFontsManager.md#registerfont)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new PDFFontsManager**()

Represent a pdf fonts manager.

## Methods

### <a id="fallbackfont" name="fallbackfont"></a> fallbackFont

▸ `Static` **fallbackFont**(`font`): `any`

提供特定字体的备选字体

**`static`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `font` | `string` | CSS字体字符串 |

#### Returns

`any`

字体文件为base64字符串或ArrayBuffer

___

### <a id="registerfont" name="registerfont"></a> registerFont

▸ `Static` **registerFont**(`name`, `font`): `void`

注册用于导出PDF的字体

**`static`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 字体名称 |
| `font` | `Object` | - |

#### Returns

`void`
