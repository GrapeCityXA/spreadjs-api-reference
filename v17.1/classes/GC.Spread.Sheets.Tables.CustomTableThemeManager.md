# Class: CustomTableThemeManager

[Sheets](../modules/GC.Spread.Sheets.md).[Tables](../modules/GC.Spread.Sheets.Tables.md).CustomTableThemeManager

## Hierarchy

- [`CustomThemeManagerBase`](GC.Spread.Sheets.CustomThemeManagerBase.md)

  ↳ **`CustomTableThemeManager`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Tables.CustomTableThemeManager.md#constructor)

### Methods

- [add](GC.Spread.Sheets.Tables.CustomTableThemeManager.md#add)
- [all](GC.Spread.Sheets.Tables.CustomTableThemeManager.md#all)
- [get](GC.Spread.Sheets.Tables.CustomTableThemeManager.md#get)
- [remove](GC.Spread.Sheets.Tables.CustomTableThemeManager.md#remove)
- [update](GC.Spread.Sheets.Tables.CustomTableThemeManager.md#update)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new CustomTableThemeManager**(`workbook`)

代表一个自定义表格主题管理器，可以管理所有自定义表格主题。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workbook` | [`Workbook`](GC.Spread.Sheets.Workbook.md) | 工作簿 |

#### Overrides

[CustomThemeManagerBase](GC.Spread.Sheets.CustomThemeManagerBase.md).[constructor](GC.Spread.Sheets.CustomThemeManagerBase.md#constructor)

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`theme`): `undefined` \| [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md)

添加新的表格主题。

**`example`**
```
// add a new table theme named "custom0"
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
let tableStyle = spread.customTableThemes.add("custom0");
let firstColumnStripStyle = new GC.Spread.Sheets.Tables.TableStyle();
firstColumnStripStyle.backColor = "#0C66E4";
tableStyle.firstColumnStripStyle(firstColumnStripStyle);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `theme` | `string` \| [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md) | 新的表格主题或只是您要添加的新表格主题名称 |

#### Returns

`undefined` \| [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md)

返回新添加的表格主题，如果指定的表格主题已存在，则添加表格主题失败，返回undefined

___

### <a id="all" name="all"></a> all

▸ **all**(): [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md)[]

获取表格主题集合。

**`example`**
```
// get all table table themes
let tableStylesCollection = spread.customTableThemes.all();
```

#### Returns

[`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md)[]

Array<GC.Spread.Sheets.Tables.TableTheme>

___

### <a id="get" name="get"></a> get

▸ **get**(`name`): `undefined` \| [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md)

按名称获取表格主题。

**`example`**
```
// get table theme
tableStyle = spread.customTableThemes.get("custom0");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 获取的表主题的具体名称 |

#### Returns

`undefined` \| [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md)

如果找到对应的特定名称的表主题，则返回该主题；否则，返回未定义。

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`name`): `void`

按名称删除表格主题。

**`example`**
```
// delete table theme
spread.customTableThemes.remove("custom0");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要删除的表主题的具体名称 |

#### Returns

`void`

___

### <a id="update" name="update"></a> update

▸ **update**(`oldThemeName`, `newTheme`): `void`

更新表格主题。

**`example`**
```
// update table theme
tableStyle = spread.customTableThemes.update("custom0", new GC.Spread.Sheets.Tables.TableTheme());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `oldThemeName` | `string` | 旧主题名称 |
| `newTheme` | [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md) | 新主题 |

#### Returns

`void`
