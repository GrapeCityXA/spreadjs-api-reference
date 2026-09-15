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

表示一个可以管理所有自定义数据透视表主题的管理器。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workbook` | [`Workbook`](GC.Spread.Sheets.Workbook.md) | 工作簿对象。 |

#### Overrides

[CustomThemeManagerBase](GC.Spread.Sheets.CustomThemeManagerBase.md).[constructor](GC.Spread.Sheets.CustomThemeManagerBase.md#constructor)

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`theme`): `undefined` \| [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md)

添加一个新的数据透视表主题。

**`example`**
```javascript
// 添加一个名为 "custom0" 的新数据透视表主题
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
let pivotTableStyle = spread.customPivotTableThemes.add("custom0");
let wholeTableStyle = new GC.Spread.Pivot.PivotTableStyle();
wholeTableStyle.backColor = "#0C66E4";
pivotTableStyle.wholeTableStyle(wholeTableStyle);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `theme` | `string` \| [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md) | 新的数据透视表主题或仅为要添加的新主题名称 |

#### Returns

`undefined` \| [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md)

返回新添加的数据透视表主题，如果同名主题已存在，则添加失败并返回 undefined

___

### <a id="all" name="all"></a> all

▸ **all**(): [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md)[]

获取数据透视表主题集合。

**`example`**
```javascript
// 获取所有数据透视表主题
let tableStylesCollection = spread.customPivotTableThemes.all();
```

#### Returns

[`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md)[]

Array<GC.Spread.Pivot.PivotTableTheme>

___

### <a id="get" name="get"></a> get

▸ **get**(`name`): `undefined` \| [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md)

按名称获取数据透视表主题。

**`example`**
```javascript
// 获取数据透视表主题
pivotTableStyle = spread.customPivotTableThemes.get("custom0");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要获取的数据透视表主题的特定名称 |

#### Returns

`undefined` \| [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md)

如果找到具有指定名称的对应主题，则返回该主题；否则返回 undefined

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`name`): `void`

按名称删除数据透视表主题。

**`example`**
```javascript
// 删除数据透视表主题
spread.customPivotTableThemes.remove("custom0");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要删除的数据透视表主题的特定名称 |

#### Returns

`void`

___

### <a id="update" name="update"></a> update

▸ **update**(`oldThemeName`, `newTheme`): `void`

更新数据透视表主题。

**`example`**
```javascript
// 更新数据透视表主题
tableStyle = spread.customPivotTableThemes.update("custom0", new GC.Spread.Pivot.PivotTableTheme());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `oldThemeName` | `string` | 要更新的数据透视表主题的特定名称 |
| `newTheme` | [`PivotTableTheme`](GC.Spread.Pivot.PivotTableTheme.md) | 新的数据透视表主题 |

#### Returns

`void`
