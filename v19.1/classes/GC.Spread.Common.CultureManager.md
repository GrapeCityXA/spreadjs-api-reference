# Class: CultureManager

[Spread](../modules/GC.Spread.md).[Common](../modules/GC.Spread.Common.md).CultureManager

## Table of contents

### Constructors

- [constructor](GC.Spread.Common.CultureManager.md#constructor)

### Methods

- [addCultureInfo](GC.Spread.Common.CultureManager.md#addcultureinfo)
- [culture](GC.Spread.Common.CultureManager.md#culture)
- [getCultureInfo](GC.Spread.Common.CultureManager.md#getcultureinfo)
- [getLanguage](GC.Spread.Common.CultureManager.md#getlanguage)
- [getResources](GC.Spread.Common.CultureManager.md#getresources)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new CultureManager**()

表示文化管理器。

## Methods

### <a id="addcultureinfo" name="addcultureinfo"></a> addCultureInfo

▸ `Static` **addCultureInfo**(`cultureName`, `culture`, `language?`): `void`

将cultureInfo或自定义语言添加到文化管理器中。

**`static`**

**`example`**
```javascript
var myCulture = new GC.Spread.Common.CultureInfo();
myCulture.NumberFormat.currencySymbol = "\u20ac"
myCulture.NumberFormat.numberDecimalSeparator = ",";
myCulture.NumberFormat.numberGroupSeparator = ".";
myCulture.NumberFormat.arrayGroupSeparator = ";";
myCulture.NumberFormat.arrayListSeparator = "\\";
myCulture.NumberFormat.listSeparator = ";";
//添加一个区域性
GC.Spread.Common.CultureManager.addCultureInfo("de-DE", myCulture);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cultureName` | `string` | 要设置的文化名称。 |
| `culture` | [`CultureInfo`](GC.Spread.Common.CultureInfo.md) | - |
| `language?` | `object` | 要设置到文化的自定义语言。如果已设置，将覆盖旧语言。 |

#### Returns

`void`

___

### <a id="culture" name="culture"></a> culture

▸ `Static` **culture**(`cultureName?`, `force?`): `string`

获取或设置Sheets的文化。

**`static`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cultureName?` | `string` | 要获取的文化名称。 |
| `force?` | `boolean` | 可选参数。如果为 `true`，则强制重新应用区域性设置。 |

#### Returns

`string`

Sheets的当前文化名称。

___

### <a id="getcultureinfo" name="getcultureinfo"></a> getCultureInfo

▸ `Static` **getCultureInfo**(`cultureName?`): [`CultureInfo`](GC.Spread.Common.CultureInfo.md)

获取指定的cultureInfo。如果没有文化名称，则获取当前cultureInfo。

**`static`**

**`example`**
```javascript
GC.Spread.Common.CultureManager.getCultureInfo(); // return the current culture info.
GC.Spread.Common.CultureManager.getCultureInfo(1033); // return the culture info of culture id 1033, it's en culture.
GC.Spread.Common.CultureManager.getCultureInfo('en-us'); // return the culture info of en.
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cultureName?` | `string` \| `number` | 文化名称或文化ID |

#### Returns

[`CultureInfo`](GC.Spread.Common.CultureInfo.md)

指定的cultureInfo对象。

___

### <a id="getlanguage" name="getlanguage"></a> getLanguage

▸ `Static` **getLanguage**(`cultureName`): `object`

获取指定的自定义语言。

**`static`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cultureName` | `string` | 要获取的文化名称。 |

#### Returns

`object`

指定的对象。如果未定义语言则为null。

___

### <a id="getresources" name="getresources"></a> getResources

▸ `Static` **getResources**(`cultureName?`): `object`

获取指定的或当前的工作资源。

**`static`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cultureName?` | `string` | 要获取的文化名称。如果cultureName为null，将返回当前工作资源。 |

#### Returns

`object`

指定的或当前的工作资源。如果未定义语言则为null。
