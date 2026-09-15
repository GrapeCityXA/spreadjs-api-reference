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

表示一个可以管理所有自定义时间轴切片器主题的自定义时间轴切片器主题管理器。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workbook` | [`Workbook`](GC.Spread.Sheets.Workbook.md) | 工作簿。 |

#### Overrides

[CustomThemeManagerBase](GC.Spread.Sheets.CustomThemeManagerBase.md).[constructor](GC.Spread.Sheets.CustomThemeManagerBase.md#constructor)

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`theme`): `undefined` \| [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

添加新的时间轴主题。

**`example`**
```
// 添加一个名为"custom0"的新时间轴主题
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
let timeLineStyle = spread.customTimelineThemes.add("custom0");
let wholeTimelineStyle = new GC.Spread.Sheets.Slicers.TimelineStyleInfo();
wholeTimelineStyle.backColor = "#0C66E4";
timeLineStyle.wholeTimelineStyle(wholeTimelineStyle);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `theme` | `string` \| [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md) | 要添加的新时间轴主题或仅是新时间轴主题名称。 |

#### Returns

`undefined` \| [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

返回新添加的时间轴主题，如果已存在同名时间轴主题，则添加失败并返回undefined

___

### <a id="all" name="all"></a> all

▸ **all**(): [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)[]

获取时间轴主题集合。

**`example`**
```
// 获取所有时间轴主题
let timeLineStylesCollection = spread.customTimelineThemes.all();
```

#### Returns

[`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)[]

Array<GC.Spread.Sheets.Slicers.TimelineStyle>

___

### <a id="get" name="get"></a> get

▸ **get**(`name`): `undefined` \| [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

通过名称获取时间轴主题。

**`example`**
```
// 获取时间轴主题
timeLineStyle = spread.customTimelineThemes.get("custom0");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要获取的时间轴主题的特定名称 |

#### Returns

`undefined` \| [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md)

如果找到指定名称的时间轴主题，则返回该主题；否则返回undefined

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`name`): `void`

通过名称删除时间轴主题。

**`example`**
```
// 删除时间轴主题
spread.customTimelineThemes.remove("custom0");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要删除的时间轴主题的特定名称 |

#### Returns

`void`

___

### <a id="update" name="update"></a> update

▸ **update**(`oldThemeName`, `newTheme`): `void`

更新时间轴切片器主题。

**`example`**
```
// 更新时间轴切片器主题
timelineStyle = spread.customTimelineThemes.update("custom0", new GC.Spread.Sheets.Slicers.TimelineStyle());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `oldThemeName` | `string` | 要更新的时间轴切片器主题的特定名称 |
| `newTheme` | [`TimelineStyle`](GC.Spread.Sheets.Slicers.TimelineStyle.md) | 要更新的时间轴切片器主题 |

#### Returns

`void`
