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

本地化管理器

## Methods

### <a id="addcultureinfo" name="addcultureinfo"></a> addCultureInfo

▸ `Static` **addCultureInfo**(`cultureName`, `culture`, `language?`): `void`

将cultureInfo或自定义语言添加到本地化管理器中。

**`static`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cultureName` | `string` | 要设置的本地化名称 |
| `culture` | [`CultureInfo`](GC.Spread.Common.CultureInfo.md) | - |
| `language?` | `object` | 自定义语言设置本地化如果已经设置,它将覆盖旧的语言 |

#### Returns

`void`

___

### <a id="culture" name="culture"></a> culture

▸ `Static` **culture**(`cultureName?`): `string`

获取或设置表格本地化

**`static`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cultureName?` | `string` | 设置的本地化名称 |

#### Returns

`string`

. 表格的当前本地化名称

___

### <a id="getcultureinfo" name="getcultureinfo"></a> getCultureInfo

▸ `Static` **getCultureInfo**(`cultureName`): [`CultureInfo`](GC.Spread.Common.CultureInfo.md)

获取指定的cultureInfo 如果没有本地化名称,请获取当前的CultureInfo

**`static`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cultureName` | `string` \| `number` | 本地化名称或本地化ID |

#### Returns

[`CultureInfo`](GC.Spread.Common.CultureInfo.md)

指定的cultureInfo对象

___

### <a id="getlanguage" name="getlanguage"></a> getLanguage

▸ `Static` **getLanguage**(`cultureName`): `object`

获取指定的自定义语言

**`static`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cultureName` | `string` | 设置的本地化名称 |

#### Returns

`object`

指定的对象 如果未定义语言,则为Null

___

### <a id="getresources" name="getresources"></a> getResources

▸ `Static` **getResources**(`cultureName?`): `object`

获取指定的或当前的源

**`static`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `cultureName?` | `string` | 获取的文化名称如果cultureName为null,则将返回当前的源 |

#### Returns

`object`

指定的或当前的源如果未定义语言,则为Null
