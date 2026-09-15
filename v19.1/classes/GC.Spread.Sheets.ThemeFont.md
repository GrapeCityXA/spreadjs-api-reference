# Class: ThemeFont

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).ThemeFont

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.ThemeFont.md#constructor)

### Methods

- [bodyEastAsianFont](GC.Spread.Sheets.ThemeFont.md#bodyeastasianfont)
- [bodyFont](GC.Spread.Sheets.ThemeFont.md#bodyfont)
- [bodyFontScriptTypeface](GC.Spread.Sheets.ThemeFont.md#bodyfontscripttypeface)
- [headingEastAsianFont](GC.Spread.Sheets.ThemeFont.md#headingeastasianfont)
- [headingFont](GC.Spread.Sheets.ThemeFont.md#headingfont)
- [headingFontScriptTypeface](GC.Spread.Sheets.ThemeFont.md#headingfontscripttypeface)
- [name](GC.Spread.Sheets.ThemeFont.md#name)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new ThemeFont**(`name`, `headingFont`, `bodyFont`, `headingEastAsianFont?`, `bodyEastAsianFont?`)

表示主题字体。

**`example`**
```javascript
//此示例创建一个新的SpreadTheme对象。
var custom = new GC.Spread.Sheets.Theme("Custom");
custom.font().bodyEastAsianFont("SimSum");
sheet.currentTheme(custom);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 主题字体的名称。 |
| `headingFont` | `string` | 拉丁文本标题字体的名称。 |
| `bodyFont` | `string` | 拉丁文本正文字体的名称。 |
| `headingEastAsianFont?` | `string` | 东亚文本标题字体的名称。 |
| `bodyEastAsianFont?` | `string` | 东亚文本正文字体的名称。 |

## Methods

### <a id="bodyeastasianfont" name="bodyeastasianfont"></a> bodyEastAsianFont

▸ **bodyEastAsianFont**(`value?`): `any`

获取或设置东亚文本主题字体的正文字体。

**`example`**
```javascript
var custom = new GC.Spread.Sheets.Theme("Custom", null, "Cambria", "Calibri");
custom.font().bodyEastAsianFont("SimSum");
sheet.currentTheme(custom);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 东亚文本主题字体的正文字体。 |

#### Returns

`any`

如果未设置值，则返回主题字体的名称；否则返回主题字体。

___

### <a id="bodyfont" name="bodyfont"></a> bodyFont

▸ **bodyFont**(`value?`): `any`

获取或设置拉丁文本主题字体的正文字体。

**`example`**
```javascript
var custom = new GC.Spread.Sheets.Theme("Custom", null, "Cambria", "Calibri");
custom.font().bodyFont("Calibri");
sheet.currentTheme(custom);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 拉丁文本主题字体的正文字体。 |

#### Returns

`any`

如果未设置值，则返回主题字体的名称；否则返回主题字体。

___

### <a id="bodyfontscripttypeface" name="bodyfontscripttypeface"></a> bodyFontScriptTypeface

▸ **bodyFontScriptTypeface**(`script`, `typeface?`): `any`

根据字体脚本获取或设置字体。

**`example`**
```javascript
var custom = new GC.Spread.Sheets.Theme("Custom");
// 根据字体脚本获取字体
var typeface = custom.bodyFontScriptTypeface('Hans');
// 根据字体脚本设置字体
custom.bodyFontScriptTypeface('Hans', 'SimSum');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `script` | `string` | 字体脚本代码。 |
| `typeface?` | `string` | 字体。 |

#### Returns

`any`

如果只设置了脚本，则返回字体；否则设置字体。

___

### <a id="headingeastasianfont" name="headingeastasianfont"></a> headingEastAsianFont

▸ **headingEastAsianFont**(`value?`): `any`

获取或设置东亚文本主题字体的标题字体。

**`example`**
```javascript
var custom = new GC.Spread.Sheets.Theme("Custom", null, "Cambria", "Calibri");
custom.font().headingEastAsianFont("SimSum");
sheet.currentTheme(custom);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 东亚文本主题字体的标题字体。 |

#### Returns

`any`

如果未设置值，则返回主题字体的名称；否则返回主题字体。

___

### <a id="headingfont" name="headingfont"></a> headingFont

▸ **headingFont**(`value?`): `any`

获取或设置拉丁文本主题字体的标题字体。

**`example`**
```javascript
var custom = new GC.Spread.Sheets.Theme("Custom", null, "Cambria", "Calibri");
custom.font().headingFont("Calibri");
sheet.currentTheme(custom);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 拉丁文本主题字体的标题字体。 |

#### Returns

`any`

如果未设置值，则返回主题字体的名称；否则返回主题字体。

___

### <a id="headingfontscripttypeface" name="headingfontscripttypeface"></a> headingFontScriptTypeface

▸ **headingFontScriptTypeface**(`script`, `typeface?`): `any`

根据字体脚本获取或设置字体。

**`example`**
```javascript
var custom = new GC.Spread.Sheets.Theme("Custom");
// 根据字体脚本获取字体
var typeface = custom.headingFontScriptTypeface('Hans');
// 根据字体脚本设置字体
custom.headingFontScriptTypeface('Hans', 'SimSum');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `script` | `string` | 字体脚本代码。 |
| `typeface?` | `string` | 字体。 |

#### Returns

`any`

如果只设置了脚本，则返回字体；否则设置字体。

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置主题字体的名称。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 主题字体的名称。 |

#### Returns

`any`

如果未设置值，则返回主题字体的名称；否则返回主题字体。
