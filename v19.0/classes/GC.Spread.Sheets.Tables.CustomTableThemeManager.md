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

表示一个可以管理所有自定义表格主题的自定义表格主题管理器。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workbook` | [`Workbook`](GC.Spread.Sheets.Workbook.md) | 工作簿。 |

#### Overrides

[CustomThemeManagerBase](GC.Spread.Sheets.CustomThemeManagerBase.md).[constructor](GC.Spread.Sheets.CustomThemeManagerBase.md#constructor)

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`theme`): `undefined` \| [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md)

添加一个新的表格主题。

**`example`**
```
// 添加一个名为"custom0"的新表格主题
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
let tableStyle = spread.customTableThemes.add("custom0");
let firstColumnStripStyle = new GC.Spread.Sheets.Tables.TableStyle();
firstColumnStripStyle.backColor = "#0C66E4";
tableStyle.firstColumnStripStyle(firstColumnStripStyle);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `theme` | `string` \| [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md) | 要添加的新表格主题或新表格主题名称 |

#### Returns

`undefined` \| [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md)

返回新添加的表格主题，如果命名表格主题已存在，则添加失败并返回undefined

___

### <a id="all" name="all"></a> all

▸ **all**(): [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md)[]

获取表格主题集合。

**`example`**
```
// 获取所有表格主题
let tableStylesCollection = spread.customTableThemes.all();
```

#### Returns

[`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md)[]

Array<GC.Spread.Sheets.Tables.TableTheme>

___

### <a id="get" name="get"></a> get

▸ **get**(`name`): `undefined` \| [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md)

通过名称获取表格主题。

**`example`**
```
// 获取表格主题
tableStyle = spread.customTableThemes.get("custom0");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要获取的特定表格主题名称 |

#### Returns

`undefined` \| [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md)

如果找到具有特定名称的对应表格主题，则返回该主题；否则返回undefined。

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`name`): `void`

通过名称移除表格主题。

**`example`**
```
// 删除表格主题
spread.customTableThemes.remove("custom0");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要移除的特定表格主题名称 |

#### Returns

`void`

___

### <a id="update" name="update"></a> update

▸ **update**(`oldThemeName`, `newTheme`): `void`

更新表格主题。

**`example`**
```
// 更新表格主题
tableStyle = spread.customTableThemes.update("custom0", new GC.Spread.Sheets.Tables.TableTheme());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `oldThemeName` | `string` | 要更新的特定表格主题名称 |
| `newTheme` | [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md) | 要更新的特定表格主题 |

#### Returns

`void`
