# Class: Theme

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).Theme

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Theme.md#constructor)

### Methods

- [bodyFont](GC.Spread.Sheets.Theme.md#bodyfont)
- [colors](GC.Spread.Sheets.Theme.md#colors)
- [headerFont](GC.Spread.Sheets.Theme.md#headerfont)
- [name](GC.Spread.Sheets.Theme.md#name)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Theme**(`name`, `colorScheme`, `headerFont`, `bodyFont`)

配色方案

**`代码示例`**
```
//本示例创建了一个新的SpreadTheme对象
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
| `name` | `string` | 主题的名称 |
| `colorScheme` | [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md) | 主题颜色的基本颜色 |
| `headerFont` | `string` | 标题字体的名称 |
| `bodyFont` | `string` | 正文字体的名称 |

## Methods

### <a id="bodyfont" name="bodyfont"></a> bodyFont

▸ **bodyFont**(`value?`): `any`

获取或设置主题的正文字体

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 正文字体 |

#### Returns

`any`

如果没有设置值,返回正文字体;否则,返回主题

___

### <a id="colors" name="colors"></a> colors

▸ **colors**(`value?`): `any`

获取或设置主题的基本颜色

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`ColorScheme`](GC.Spread.Sheets.ColorScheme.md) | 主题的基本颜色 |

#### Returns

`any`

如果没有设置值,返回主题的基本颜色;否则,返回主题

___

### <a id="headerfont" name="headerfont"></a> headerFont

▸ **headerFont**(`value?`): `any`

获取或设置主题的标题字体

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 标题字体 |

#### Returns

`any`

如果没有设置值,返回标题字体;否则,返回主题

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置主题的名称

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 主题名称 |

#### Returns

`any`

如果没有设置值,返回主题名称;否则,返回主题
