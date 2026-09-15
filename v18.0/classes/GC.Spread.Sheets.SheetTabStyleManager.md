# Class: SheetTabStyleManager

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).SheetTabStyleManager

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.SheetTabStyleManager.md#constructor)

### Methods

- [add](GC.Spread.Sheets.SheetTabStyleManager.md#add)
- [all](GC.Spread.Sheets.SheetTabStyleManager.md#all)
- [clear](GC.Spread.Sheets.SheetTabStyleManager.md#clear)
- [remove](GC.Spread.Sheets.SheetTabStyleManager.md#remove)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new SheetTabStyleManager**(`workbook`)

表示工作表选项卡样式管理器，它可以管理所有工作表选项卡的相关样式。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workbook` | [`Workbook`](GC.Spread.Sheets.Workbook.md) | 工作簿 |

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`state`, `style`, `sheetNames?`): `void`

在部分或全部工作表标签上添加状态样式

**`example`**
```
spread.sheetTabStyles.add(GC.Spread.Sheets.SheetTabState.active, {foreColor: "red"}, ["Sheet1", "Sheet2"]);
spread.sheetTabStyles.add(GC.Spread.Sheets.SheetTabState.hover, {foreColor: "red"});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `state` | [`SheetTabState`](../enums/GC.Spread.Sheets.SheetTabState.md) | 标签状态 |
| `style` | [`ISheetTabStyle`](../interfaces/GC.Spread.Sheets.ISheetTabStyle.md) | 标签样式 |
| `sheetNames?` | `string`[] | 应用标签样式的工作表名称数组 |

#### Returns

`void`

___

### <a id="all" name="all"></a> all

▸ **all**(`sheetNames?`): [`ISheetNameTabStyleMap`](../interfaces/GC.Spread.Sheets.ISheetNameTabStyleMap.md)

或者部分或者全部工作表标签的状态样式

**`example`**
```
spread.sheetTabStyles.all(["Sheet1", "Sheet2"]);
spread.sheetTabStyles.all();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheetNames?` | `string`[] | 查询状态样式的工作表名称数组 |

#### Returns

[`ISheetNameTabStyleMap`](../interfaces/GC.Spread.Sheets.ISheetNameTabStyleMap.md)

部分或者所有工作表标签的状态样式

___

### <a id="clear" name="clear"></a> clear

▸ **clear**(`sheetNames?`): `void`

清除状态样式

**`example`**
```
spread.sheetTabStyles.clear(["Sheet1", "Sheet2"]);
spread.sheetTabStyles.clear();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheetNames?` | `string`[] | 需要清除样式的工作表名称数组 |

#### Returns

`void`

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`state`, `sheetNames?`): `void`

删除部分或者全部状态样式

**`example`**
```
spread.sheetTabStyles.remove(GC.Spread.Sheets.SheetTabState.active, ["Sheet1", "Sheet2"]);
spread.sheetTabStyles.remove(GC.Spread.Sheets.SheetTabState.hover);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `state` | [`SheetTabState`](../enums/GC.Spread.Sheets.SheetTabState.md) | 标签状态 |
| `sheetNames?` | `string`[] | 需要删除样式的工作表名称数组  |

#### Returns

`void`
