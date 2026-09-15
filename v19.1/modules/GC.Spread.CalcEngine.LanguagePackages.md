# Namespace: LanguagePackages

[Spread](GC.Spread.md).[CalcEngine](GC.Spread.CalcEngine.md).LanguagePackages

## Table of contents

### Functions

- [languagePackages](GC.Spread.CalcEngine.LanguagePackages.md#languagepackages)

## Functions

### <a id="languagepackages" name="languagepackages"></a> languagePackages

▸ **languagePackages**(`languageName?`): `any`

获取或设置计算引擎的语言包。

**`example`**
```javascript
GC.Spread.CalcEngine.LanguagePackages.languagePackages('fr');
GC.Spread.CalcEngine.LanguagePackages.languagePackages();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `languageName?` | `string` | 计算引擎语言名称字符串； |

#### Returns

`any`

如果未设置值，返回计算引擎语言名称字符串；
