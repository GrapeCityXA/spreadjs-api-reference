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

表示具有指定格式模式和格式字符串的格式化程序。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `format?` | `string` | 格式字符串（可选）。 |
| `cultureName?` | `string` | 区域性名称（可选）。 |

## Methods

### <a id="format" name="format"></a> format

▸ **format**(`obj`, `formattedData?`): `string`

使用格式化数据对象将指定对象格式化为字符串。

**`example`**
```javascript
// 此示例使用 format 方法。
var formatter = new GC.Spread.Formatter.GeneralFormatter("#,##0.00");
var result = formatter.format(123456.789);
console.log(result); // '123,456.79'
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `obj` | `Object` | 要格式化的单元格数据对象。 |
| `formattedData?` | `Object` | 包含格式化数据的对象（可选）。 |

#### Returns

`string`

格式化后的字符串。

___

### <a id="formatstring" name="formatstring"></a> formatString

▸ **formatString**(`value?`): `string` \| [`GeneralFormatter`](GC.Spread.Formatter.GeneralFormatter.md)

获取或设置此格式化程序的格式字符串。

**`example`**
```javascript
// 此示例获取格式字符串。
var formatter = new GC.Spread.Formatter.GeneralFormatter("#,##0.00");
var result = formatter.formatString();
console.log(result); // '#,##0.00'
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 此格式化程序的格式字符串。 |

#### Returns

`string` \| [`GeneralFormatter`](GC.Spread.Formatter.GeneralFormatter.md)

若无值设置，返回此格式化程序的格式字符串；否则返回格式化程序实例。

___

### <a id="parse" name="parse"></a> parse

▸ **parse**(`str`): `Object`

解析指定的文本。

**`example`**
```javascript
// 此示例使用 parse 方法。
var formatter = new GC.Spread.Formatter.GeneralFormatter("#,##0.00");
var result = formatter.parse("123,456.78");
console.log(result); // 123456.78
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `str` | `string` |

#### Returns

`Object`

解析后的对象。
