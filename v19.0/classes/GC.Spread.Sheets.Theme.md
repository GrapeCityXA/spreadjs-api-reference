# Class: Theme

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).Theme

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Theme.md#constructor)

### Methods

- [bodyFont](GC.Spread.Sheets.Theme.md#bodyfont)
- [colors](GC.Spread.Sheets.Theme.md#colors)
- [font](GC.Spread.Sheets.Theme.md#font)
- [headingFont](GC.Spread.Sheets.Theme.md#headingfont)
- [name](GC.Spread.Sheets.Theme.md#name)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Theme**(`name`, `colorScheme`, `headingFont`, `bodyFont`)

表示一个配色方案。

**`example`**
```
//此示例创建一个新的SpreadTheme对象。
sheet.getCell(0, 0).backColor("accent 1");
sheet.getCell(1, 0).backColor("accent 6");
$("#btn").click(function () {
    var custom = new GC.Spread.Sheets.Theme("Custom");
    custom.colors().accent1("red");
    custom.colors().accent6("green");
    sheet.currentTheme(custom);
})
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 主题名称。 |
| `colorScheme` | [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md) | 主题颜色的基础颜色。 |
| `headingFont` | `string` | 标题字体名称。 |
| `bodyFont` | `string` | 正文字体名称。 |

## Methods

### <a id="bodyfont" name="bodyfont"></a> bodyFont

▸ **bodyFont**(`value?`): `any`

根据文化获取或设置主题的正文字体。

**`example`**
```
var custom = new GC.Spread.Sheets.Theme("Custom");
custom.bodyFont('cursive');
sheet.currentTheme(custom);
sheet.setValue(0, 0, 'hello world!'); // 单元格的字体将为'cursive'。
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置值，则返回正文字体；否则返回主题。

___

### <a id="colors" name="colors"></a> colors

▸ **colors**(`value?`): `any`

获取或设置主题的基础颜色。

**`example`**
```
var custom = new GC.Spread.Sheets.Theme("Custom");
custom.colors().accent1("red");
custom.colors().accent6("green");
sheet.currentTheme(custom);
sheet.getCell(0, 0).backColor("accent 1"); // 单元格的背景色将为红色。
sheet.getCell(0, 1).backColor("accent 6"); // 单元格的背景色将为绿色。
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md) |

#### Returns

`any`

如果未设置值，则返回主题的基础颜色；否则返回主题。

___

### <a id="font" name="font"></a> font

▸ **font**(`value?`): `any`

获取或设置主题的字体。

**`example`**
```
var custom = new GC.Spread.Sheets.Theme("Custom");
custom.font().bodyFont("cursive");
sheet.currentTheme(custom);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`ThemeFont`](GC.Spread.Sheets.ThemeFont.md) |

#### Returns

`any`

如果未设置值，则返回主题的字体；否则返回主题。

___

### <a id="headingfont" name="headingfont"></a> headingFont

▸ **headingFont**(`value?`): `any`

根据文化获取或设置主题的标题字体。

**`example`**
```
var custom = new GC.Spread.Sheets.Theme("Custom");
custom.headingFont('cursive');
sheet.currentTheme(custom);
sheet.getCell(0, 0).themeFont('Headings');
sheet.setValue(0, 0, 'hello world!'); // 单元格的字体将为'cursive'。
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置值，则返回标题字体；否则返回主题。

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置主题的名称。

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置值，则返回主题名称；否则返回主题。
