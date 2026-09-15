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

表示一个 PDF 字体管理器。

## Methods

### <a id="fallbackfont" name="fallbackfont"></a> fallbackFont

▸ `Static` **fallbackFont**(`font`): `any`

为特定字体提供备用字体。

**`static`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `font` | `string` | CSS 字体字符串。 |

#### Returns

`any`

以 base64 字符串或 ArrayBuffer 格式的字体文件。

___

### <a id="registerfont" name="registerfont"></a> registerFont

▸ `Static` **registerFont**(`name`, `font`): `void`

注册用于导出 PDF 的字体。

**`static`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 字体名称。 |
| `font` | `Object` | - |

#### Returns

`void`
