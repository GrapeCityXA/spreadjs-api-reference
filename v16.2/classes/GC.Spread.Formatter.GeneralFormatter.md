# Class: GeneralFormatter

[Spread](../modules/GC.Spread.md).[Formatter](../modules/GC.Spread.Formatter.md).GeneralFormatter

## Table of contents

### Constructors

- [constructor](GC.Spread.Formatter.GeneralFormatter.md#constructor)

### Methods

- [format](GC.Spread.Formatter.GeneralFormatter.md#format)
- [formatString](GC.Spread.Formatter.GeneralFormatter.md#formatstring)
- [parse](GC.Spread.Formatter.GeneralFormatter.md#parse)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new GeneralFormatter**(`format?`, `cultureName?`)

具有指定模式和字符串的格式

#### Parameters

| Name | Type |
| :------ | :------ |
| `format?` | `string` |
| `cultureName?` | `string` |

## Methods

### <a id="format" name="format"></a> format

▸ **format**(`obj`, `formattedData?`): `string`

将指定对象格式化为具有格式化数据对象的字符串

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `obj` | `Object` | 要格式化单元格数据的对象 |
| `formattedData?` | `Object` | - |

#### Returns

`string`

格式化的字符串

___

### <a id="formatstring" name="formatstring"></a> formatString

▸ **formatString**(`value?`): `string` \| [`GeneralFormatter`](GC.Spread.Formatter.GeneralFormatter.md)

获取或设置此格式化的格式字符串

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 此格式化的格式字符串 |

#### Returns

`string` \| [`GeneralFormatter`](GC.Spread.Formatter.GeneralFormatter.md)

如果没有设置值,返回此格式化字符串;否则,返回格式

___

### <a id="parse" name="parse"></a> parse

▸ **parse**(`str`): `Object`

解析指定的文本

#### Parameters

| Name | Type |
| :------ | :------ |
| `str` | `string` |

#### Returns

`Object`

解析对象
