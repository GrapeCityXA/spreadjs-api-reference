# Class: CustomPivotTableThemeManager

[Spread](../modules/GC.Spread.md).[Pivot](../modules/GC.Spread.Pivot.md).CustomPivotTableThemeManager

## Hierarchy

- [`CustomThemeManagerBase`](GC.Spread.Sheets.CustomThemeManagerBase.md)

  ↳ **`CustomPivotTableThemeManager`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Pivot.CustomPivotTableThemeManager.md#constructor)

### Methods

- [add](GC.Spread.Pivot.CustomPivotTableThemeManager.md#add)
- [all](GC.Spread.Pivot.CustomPivotTableThemeManager.md#all)
- [get](GC.Spread.Pivot.CustomPivotTableThemeManager.md#get)
- [remove](GC.Spread.Pivot.CustomPivotTableThemeManager.md#remove)
- [update](GC.Spread.Pivot.CustomPivotTableThemeManager.md#update)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new CustomPivotTableThemeManager**(`workbook`)

代表一个自定义数据透视表主题管理器，可以管理所有自定义数据透视表主题。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workbook` | [`Workbook`](GC.Spread.Sheets.Workbook.md) | 工作簿 |

#### Overrides

[CustomThemeManagerBase](GC.Spread.Sheets.CustomThemeManagerBase.md).[constructor](GC.Spread.Sheets.CustomThemeManagerBase.md#constructor)

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`theme`): `undefined` \| [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md)

添加新的数据透视表主题。

**`代码示例`**
```
// add a new pivot table theme named "custom0"
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
let pivotTableStyle = spread.customPivotTableThemes.add("custom0");
let wholeTableStyle = new GC.Spread.Pivot.PivotTableStyle();
wholeTableStyle.backColor = "#0C66E4";
tableStyle.wholeTableStyle(wholeTableStyle);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `theme` | `string` \| [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md) | 新的数据透视表主题或只是您要添加的新数据透视表主题名称 |

#### Returns

`undefined` \| [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md)

返回新添加的数据透视表主题，如果指定的数据透视表主题已存在，则添加数据透视表主题失败，返回undefined

___

### <a id="all" name="all"></a> all

▸ **all**(): [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md)[]

获取数据透视表主题集合。

**`代码示例`**
```
// get all pivot table themes
let tableStylesCollection = spread.customPivotTableThemes.all();
```

#### Returns

[`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md)[]

Array<GC.Spread.Pivot.PivotTableTheme>

___

### <a id="get" name="get"></a> get

▸ **get**(`name`): `undefined` \| [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md)

按名称获取数据透视表主题。

**`代码示例`**
```
// get pivot table theme
pivotTableStyle = spread.customPivotTableThemes.get("custom0");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要获取的数据透视表主题的具体名称 |

#### Returns

`undefined` \| [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md)

如果找到对应的特定名称的数据透视表主题，则返回该主题；否则，返回未定义。

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`name`): `void`

按名称删除数据透视表主题。

**`代码示例`**
```
// delete pivot table theme
spread.customPivotTableThemes.remove("custom0");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要删除的数据透视表主题的具体名称 |

#### Returns

`void`

___

### <a id="update" name="update"></a> update

▸ **update**(`oldThemeName`, `newTheme`): `void`

更新数据透视表主题。

**`代码示例`**
```
// update pivot table theme
tableStyle = spread.customPivotTableThemes.update("custom0", new GC.Spread.Pivot.PivotTableTheme());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `oldThemeName` | `string` | 要更新的数据透视表主题的具体名称 |
| `newTheme` | [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md) | 要更新的数据透视表主题的具体名称 |

#### Returns

`void`
