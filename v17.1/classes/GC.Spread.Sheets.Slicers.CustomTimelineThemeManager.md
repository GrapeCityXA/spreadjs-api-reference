# Class: CustomTimelineThemeManager

[Sheets](../modules/GC.Spread.Sheets.md).[Slicers](../modules/GC.Spread.Sheets.Slicers.md).CustomTimelineThemeManager

## Hierarchy

- [`CustomThemeManagerBase`](GC.Spread.Sheets.CustomThemeManagerBase.md)

  ↳ **`CustomTimelineThemeManager`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Slicers.CustomTimelineThemeManager.md#constructor)

### Methods

- [add](GC.Spread.Sheets.Slicers.CustomTimelineThemeManager.md#add)
- [all](GC.Spread.Sheets.Slicers.CustomTimelineThemeManager.md#all)
- [get](GC.Spread.Sheets.Slicers.CustomTimelineThemeManager.md#get)
- [remove](GC.Spread.Sheets.Slicers.CustomTimelineThemeManager.md#remove)
- [update](GC.Spread.Sheets.Slicers.CustomTimelineThemeManager.md#update)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new CustomTimelineThemeManager**(`workbook`)

表示自定义时间线切片器主题管理器，可以管理所有自定义时间线切片器主题。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workbook` | [`Workbook`](GC.Spread.Sheets.Workbook.md) | 工作簿 |

#### Overrides

[CustomThemeManagerBase](GC.Spread.Sheets.CustomThemeManagerBase.md).[constructor](GC.Spread.Sheets.CustomThemeManagerBase.md#constructor)

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`theme`): `undefined` \| [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

添加新的时间线主题。

**`example`**
```
// add a new timeLine theme named "custom0"
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
let timeLineStyle = spread.customTimelineThemes.add("custom0");
let wholeTimelineStyle = new GC.Spread.Sheets.Slicers.TimelineStyleInfo();
wholeTimelineStyle.backColor = "#0C66E4";
timeLineStyle.wholeTimelineStyle(wholeTimelineStyle);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `theme` | `string` \| [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md) | 新的时间线主题或只是您要添加的新时间线主题名称 |

#### Returns

`undefined` \| [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

返回新添加的timeLine主题，如果指定的timeLine主题已存在，则添加timeLine主题失败，返回undefined

___

### <a id="all" name="all"></a> all

▸ **all**(): [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)[]

获取时间线主题集合。

**`example`**
```
// get all timeLine timeLine themes
let timeLineStylesCollection = spread.customTimelineThemes.all();
```

#### Returns

[`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)[]

Array<GC.Spread.Sheets.Slicers.TimelineStyle>

___

### <a id="get" name="get"></a> get

▸ **get**(`name`): `undefined` \| [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

按名称获取时间线主题。

**`example`**
```
// get timeLine theme
timeLineStyle = spread.customTimelineThemes.get("custom0");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 获取的timeLine主题的具体名称 |

#### Returns

`undefined` \| [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

如果找到对应的特定名称的timeLine主题，则返回该主题；否则，返回未定义。

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`name`): `void`

按名称删除时间线主题。

**`example`**
```
// delete timeLine theme
spread.customTimelineThemes.remove("custom0");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要删除的时间线主题的具体名称 |

#### Returns

`void`

___

### <a id="update" name="update"></a> update

▸ **update**(`oldThemeName`, `newTheme`): `void`

更新时间线切片器主题。

**`example`**
```
// update timeline slicer theme
timelineStyle = spread.customTimelineThemes.update("custom0", new GC.Spread.Sheets.Slicers.TimelineStyle());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `oldThemeName` | `string` | 旧主题名称 |
| `newTheme` | [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md) | 新主题 |

#### Returns

`void`
