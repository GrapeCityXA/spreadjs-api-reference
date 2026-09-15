# Class: CustomSlicerThemeManager

[Sheets](../modules/GC.Spread.Sheets.md).[Slicers](../modules/GC.Spread.Sheets.Slicers.md).CustomSlicerThemeManager

## Hierarchy

- [`CustomThemeManagerBase`](GC.Spread.Sheets.CustomThemeManagerBase.md)

  ↳ **`CustomSlicerThemeManager`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Slicers.CustomSlicerThemeManager.md#constructor)

### Methods

- [add](GC.Spread.Sheets.Slicers.CustomSlicerThemeManager.md#add)
- [all](GC.Spread.Sheets.Slicers.CustomSlicerThemeManager.md#all)
- [get](GC.Spread.Sheets.Slicers.CustomSlicerThemeManager.md#get)
- [remove](GC.Spread.Sheets.Slicers.CustomSlicerThemeManager.md#remove)
- [update](GC.Spread.Sheets.Slicers.CustomSlicerThemeManager.md#update)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new CustomSlicerThemeManager**(`workbook`)

代表一个自定义切片器主题管理器，可以管理所有自定义切片器主题。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workbook` | [`Workbook`](GC.Spread.Sheets.Workbook.md) | 工作簿 |

#### Overrides

[CustomThemeManagerBase](GC.Spread.Sheets.CustomThemeManagerBase.md).[constructor](GC.Spread.Sheets.CustomThemeManagerBase.md#constructor)

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`theme`): `undefined` \| [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

添加新的切片器主题。

**`example`**
```
// add a new slicer theme named "custom0"
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
let slicerStyle = spread.customSlicerThemes.add("custom0");
let wholeSlicerStyle = new GC.Spread.Sheets.Slicers.SlicerStyleInfo();
wholeSlicerStyle.backColor = "#0C66E4";
slicerStyle.wholeSlicerStyle(wholeSlicerStyle);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `theme` | `string` \| [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md) | 新的切片器主题或只是您要添加的新切片器主题名称 |

#### Returns

`undefined` \| [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

返回新添加的切片器主题，如果指定的切片器主题已存在，则添加切片器主题失败，返回undefined

___

### <a id="all" name="all"></a> all

▸ **all**(): [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)[]

获取切片器主题集合。

**`example`**
```
// get all slicer slicer themes
let slicerStylesCollection = spread.customSlicerThemes.all();
```

#### Returns

[`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)[]

Array<GC.Spread.Sheets.Slicers.SlicerStyle>

___

### <a id="get" name="get"></a> get

▸ **get**(`name`): `undefined` \| [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

按名称获取切片器主题。

**`example`**
```
// get slicer theme
slicerStyle = spread.customSlicerThemes.get("custom0");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 获取切片器主题的具体名称 |

#### Returns

`undefined` \| [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md)

如果找到对应的特定名称的切片器主题，则返回该主题；否则，返回未定义。

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`name`): `void`

按名称删除切片器主题。

**`example`**
```
// delete slicer theme
spread.customSlicerThemes.remove("custom0");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要删除的切片器主题的具体名称 |

#### Returns

`void`

___

### <a id="update" name="update"></a> update

▸ **update**(`oldThemeName`, `newTheme`): `void`

更新切片器主题。

**`example`**
```
// update slicer theme
slicerStyle = spread.customSlicerThemes.update("custom0", new GC.Spread.Sheets.Slicers.SlicerStyle());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `oldThemeName` | `string` | 旧的主题名称 |
| `newTheme` | [`SlicerStyle`](GC.Spread.Sheets.Slicers.SlicerStyle.md) | 新的主题 |

#### Returns

`void`
