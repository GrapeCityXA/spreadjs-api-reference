# Class: ColorScheme

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).ColorScheme

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.ColorScheme.md#constructor)

### Methods

- [accent1](GC.Spread.Sheets.ColorScheme.md#accent1)
- [accent2](GC.Spread.Sheets.ColorScheme.md#accent2)
- [accent3](GC.Spread.Sheets.ColorScheme.md#accent3)
- [accent4](GC.Spread.Sheets.ColorScheme.md#accent4)
- [accent5](GC.Spread.Sheets.ColorScheme.md#accent5)
- [accent6](GC.Spread.Sheets.ColorScheme.md#accent6)
- [background1](GC.Spread.Sheets.ColorScheme.md#background1)
- [background2](GC.Spread.Sheets.ColorScheme.md#background2)
- [followedHyperlink](GC.Spread.Sheets.ColorScheme.md#followedhyperlink)
- [getColor](GC.Spread.Sheets.ColorScheme.md#getcolor)
- [hyperlink](GC.Spread.Sheets.ColorScheme.md#hyperlink)
- [name](GC.Spread.Sheets.ColorScheme.md#name)
- [textColor1](GC.Spread.Sheets.ColorScheme.md#textcolor1)
- [textColor2](GC.Spread.Sheets.ColorScheme.md#textcolor2)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new ColorScheme**(`name`, `background1`, `background2`, `text1`, `text2`, `accent1`, `accent2`, `accent3`, `accent4`, `accent5`, `accent6`, `link`, `followedLink`)

创建一个ColorScheme实例

**`classdesc`** 代表主题颜色

**`代码示例`**
```
//本示例为主题创建颜色
var ntheme = new GC.Spread.Sheets.Theme("customThemeColor");
ntheme.colors().accent1("lightgreen");
activeSheet.currentTheme(ntheme);
activeSheet.getCell(0, 0).backColor("accent 1");
activeSheet.getCell(1, 0).backColor("accent 1 30");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 包含命名变量的所有者 |
| `background1` | `string` | background1的主题颜色 |
| `background2` | `string` | background2的主题颜色 |
| `text1` | `string` | text1的主题颜色 |
| `text2` | `string` | text2的主题颜色 |
| `accent1` | `string` | accent1主题颜色 |
| `accent2` | `string` | accent2主题颜色 |
| `accent3` | `string` | accent3主题颜色 |
| `accent4` | `string` | accent4主题颜色 |
| `accent5` | `string` | accent5主题颜色 |
| `accent6` | `string` | accent6主题颜色 |
| `link` | `string` | 链接的颜色 |
| `followedLink` | `string` | 后续的链接颜色 |

## Methods

### <a id="accent1" name="accent1"></a> accent1

▸ **accent1**(`value?`): `any`

获取或设置配色方案的accent1主题颜色

**`代码示例`**
```
//本例设置了accent1颜色
var ntheme = new GC.Spread.Sheets.Theme("customThemeColor");
ntheme.colors().accent1("lightgreen");
activeSheet.currentTheme(ntheme);
activeSheet.getCell(0, 0).backColor("accent 1");
activeSheet.getCell(1, 0).backColor("accent 1 30");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | accent1主题颜色字符串 |

#### Returns

`any`

如果没有设置值,返回accent1主题颜色;否则,返回配色方案

___

### <a id="accent2" name="accent2"></a> accent2

▸ **accent2**(`value?`): `any`

获取或设置配色方案的accent2主题颜色

**`代码示例`**
```
//本示例设置了accent2颜色
var ntheme = new GC.Spread.Sheets.Theme("customThemeColor");
ntheme.colors().accent1("lightgreen");
ntheme.colors().accent2("red");
activeSheet.currentTheme(ntheme);
activeSheet.getCell(0, 0).backColor("accent 1");
activeSheet.getCell(1, 0).backColor("accent 2");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | accent2主题颜色字符串 |

#### Returns

`any`

如果没有设置值,返回accent2主题颜色;否则,返回配色方案

___

### <a id="accent3" name="accent3"></a> accent3

▸ **accent3**(`value?`): `any`

获取或设置配色方案的accent3主题颜色

**`代码示例`**
```
//本示例设置了accent3颜色
var ntheme = new GC.Spread.Sheets.Theme("customThemeColor");
ntheme.colors().accent1("lightgreen");
ntheme.colors().accent3("yellow");
activeSheet.currentTheme(ntheme);
activeSheet.getCell(0, 0).backColor("accent 1");
activeSheet.getCell(1, 0).backColor("accent 3");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | accent3主题颜色字符串 |

#### Returns

`any`

如果没有设置值,返回accent3主题颜色;否则,返回配色方案

___

### <a id="accent4" name="accent4"></a> accent4

▸ **accent4**(`value?`): `any`

获取或设置配色方案的accent4主题颜色

**`代码示例`**
```
//本例设置了accent4颜色
var ntheme = new GC.Spread.Sheets.Theme("customThemeColor");
ntheme.colors().accent1("lightgreen");
ntheme.colors().accent4("blue");
activeSheet.currentTheme(ntheme);
activeSheet.getCell(0, 0).backColor("accent 1");
activeSheet.getCell(1, 0).backColor("accent 4");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | accent4主题颜色字符串 |

#### Returns

`any`

如果没有设置值,返回accent4主题颜色;否则,返回配色方案

___

### <a id="accent5" name="accent5"></a> accent5

▸ **accent5**(`value?`): `any`

获取或设置配色方案的accent5主题颜色

**`代码示例`**
```
//本示例设置了accent5颜色
var ntheme = new GC.Spread.Sheets.Theme("customThemeColor");
ntheme.colors().accent1("lightgreen");
ntheme.colors().accent5("blue");
activeSheet.currentTheme(ntheme);
activeSheet.getCell(0, 0).backColor("accent 1");
activeSheet.getCell(1, 0).backColor("accent 5");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | accent5主题颜色字符串 |

#### Returns

`any`

如果没有设置值,返回accent5主题颜色;否则,返回配色方案

___

### <a id="accent6" name="accent6"></a> accent6

▸ **accent6**(`value?`): `any`

获取或设置配色方案的accent6主题颜色

**`代码示例`**
```
//本示例设置了accent6颜色
var ntheme = new GC.Spread.Sheets.Theme("customThemeColor");
ntheme.colors().accent1("lightgreen");
ntheme.colors().accent6("blue");
activeSheet.currentTheme(ntheme);
activeSheet.getCell(0, 0).backColor("accent 1");
activeSheet.getCell(1, 0).backColor("accent 6");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | accent6主题颜色字符串 |

#### Returns

`any`

如果没有设置值,返回accent6主题颜色;否则,返回配色方案

___

### <a id="background1" name="background1"></a> background1

▸ **background1**(`value?`): `any`

获取或设置配色方案的background1主题颜色

**`代码示例`**
```
//本示例设置了background1
var ntheme = new GC.Spread.Sheets.Theme("customThemeColor");
ntheme.colors().accent1("lightgreen");
ntheme.colors().background1("orange");
activeSheet.currentTheme(ntheme);
activeSheet.getCell(0, 0).backColor("accent 1");
activeSheet.getCell(1, 0).backColor("background 1");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | background1主题颜色字符串 |

#### Returns

`any`

如果没有设置值,返回background1主题颜色;否则,返回配色方案

___

### <a id="background2" name="background2"></a> background2

▸ **background2**(`value?`): `any`

 获取或设置配色方案的background2主题颜色

**`代码示例`**
```
//本示例设置background2颜色
var ntheme = new GC.Spread.Sheets.Theme("customThemeColor");
ntheme.colors().accent1("lightgreen");
ntheme.colors().background2("orange");
activeSheet.currentTheme(ntheme);
activeSheet.getCell(0, 0).backColor("accent 1");
activeSheet.getCell(1, 0).backColor("background 2");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | background2主题颜色字符串 |

#### Returns

`any`

如果未设置任何值,则返回background2主题颜色 否则,返回配色方案

___

### <a id="followedhyperlink" name="followedhyperlink"></a> followedHyperlink

▸ **followedHyperlink**(`value?`): `any`

获取或设置颜色方案遵循的超链接主题颜色

**`代码示例`**
```
//本示例设置followedHyperline颜色
var ntheme = new GC.Spread.Sheets.Theme("customThemeColor");
ntheme.colors().accent1("lightgreen");
ntheme.colors().followedHyperlink("orange");
ntheme.colors().hyperlink("red");
activeSheet.currentTheme(ntheme);
activeSheet.getCell(0, 0).backColor("accent 1");
activeSheet.getCell(1, 0).backColor("followedHyperlink");
activeSheet.getCell(2, 0).backColor("hyperlink");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 超链接主题颜色字符串 |

#### Returns

`any`

如果未设置任何值,则返回超链接主题颜色;否则,返回配色方案

___

### <a id="getcolor" name="getcolor"></a> getColor

▸ **getColor**(`name`): `string`

获取基于主题颜色的颜色

**`代码示例`**
```
//本示例获取主题颜色
var ntheme = new GC.Spread.Sheets.Theme("customThemeColor");
ntheme.colors().accent1("lightgreen");
ntheme.colors().followedHyperlink("orange");
ntheme.colors().hyperlink("red");
ntheme.colors().name("test");
activeSheet.currentTheme(ntheme);
activeSheet.getCell(0, 0).backColor("accent 1");
activeSheet.getCell(1, 0).backColor("followedHyperlink");
activeSheet.getCell(2, 0).backColor("hyperlink");
var cname = ntheme.getColor("accent 1");
alert(cname);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 主题颜色名称 |

#### Returns

`string`

主题颜色

___

### <a id="hyperlink" name="hyperlink"></a> hyperlink

▸ **hyperlink**(`value?`): `any`

获取或设置配色方案的超链接主题颜色

**`代码示例`**
```
//本示例设置超链接颜色
var ntheme = new GC.Spread.Sheets.Theme("customThemeColor");
ntheme.colors().accent1("lightgreen");
ntheme.colors().followedHyperlink("orange");
ntheme.colors().hyperlink("red");
activeSheet.currentTheme(ntheme);
activeSheet.getCell(0, 0).backColor("accent 1");
activeSheet.getCell(1, 0).backColor("followedHyperlink");
activeSheet.getCell(2, 0).backColor("hyperlink");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 超链接主题颜色字符串 |

#### Returns

`any`

如果未设置任何值,则返回超链接主题颜色;否则,返回配色方案

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置配色方案的名称

**`代码示例`**
```
//本示例设置主题名称
var ntheme = new GC.Spread.Sheets.Theme("customThemeColor");
ntheme.colors().accent1("lightgreen");
ntheme.colors().name("green theme");
activeSheet.currentTheme(ntheme);
activeSheet.getCell(0, 0).backColor("accent 1");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 名称 |

#### Returns

`any`

如果未设置任何值,则返回名称;否则,返回配色方案

___

### <a id="textcolor1" name="textcolor1"></a> textColor1

▸ **textColor1**(`value?`): `any`

获取或设置配色方案的textcolor1主题颜色

**`代码示例`**
```
//本示例设置textColor1颜色
var ntheme = new GC.Spread.Sheets.Theme("customThemeColor");
ntheme.colors().accent1("lightgreen");
ntheme.colors().textColor1("orange");
activeSheet.currentTheme(ntheme);
activeSheet.getCell(0, 0).backColor("accent 1");
activeSheet.getCell(1, 0).backColor("Text 1");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | textcolor1主题颜色字符串 |

#### Returns

`any`

如果未设置任何值,则返回textcolor1主题颜色;否则,返回配色方案

___

### <a id="textcolor2" name="textcolor2"></a> textColor2

▸ **textColor2**(`value?`): `any`

获取或设置配色方案的textcolor2主题颜色

**`代码示例`**
```
//本示例设置textColor2颜色
var ntheme = new GC.Spread.Sheets.Theme("customThemeColor");
ntheme.colors().accent1("lightgreen");
ntheme.colors().textColor2("orange");
activeSheet.currentTheme(ntheme);
activeSheet.getCell(0, 0).backColor("accent 1");
activeSheet.getCell(1, 0).backColor("Text 2");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | textcolor2主题颜色字符串 |

#### Returns

`any`

如果未设置任何值,则返回textcolor2主题颜色;否则,返回配色方案
