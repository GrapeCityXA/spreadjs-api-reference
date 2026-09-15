# Class: CellStateManager

[Sheets](../modules/GC.Spread.Sheets.md).[CellState](../modules/GC.Spread.Sheets.CellState.md).CellStateManager

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.CellState.CellStateManager.md#constructor)

### Methods

- [add](GC.Spread.Sheets.CellState.CellStateManager.md#add)
- [clear](GC.Spread.Sheets.CellState.CellStateManager.md#clear)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new CellStateManager**(`sheet`)

表示一个可以管理工作表中所有单元格状态的单元格状态管理器。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheet` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 工作表。 |

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`range`, `state`, `style`, `sheetArea?`): `void`

**`description`** 为范围添加单元格状态实例，当范围单元格的状态匹配时将应用单元格状态的样式。

**`example`**
```
var style = new  GC.Spread.Sheets.Style();
style.backColor = 'blue';
style.foreColor = 'red';
var range = new GC.Spread.Sheets.Range(1,2,3,3);
sheet.cellStates.add(range,GC.Spread.Sheets.CellStatesType.hover,style,101);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](GC.Spread.Sheets.Range.md) | 将应用单元格状态样式的范围。 |
| `state` | [`CellStatesType`](../enums/GC.Spread.Sheets.CellStatesType.md) | 将使用样式的状态。 |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 状态匹配时要应用的样式。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | 工作表区域。如果未提供此参数，则默认为 `viewport`。 |

#### Returns

`void`

___

### <a id="clear" name="clear"></a> clear

▸ **clear**(`range`, `sheetArea`): `void`

**`description`** 按范围清除所有样式，清除后当单元格状态匹配时将不会应用任何样式。

**`example`**
```
var range = new GC.Spread.Sheets.Range(1,2,3,3);
sheet.cellStates.clear(range, GC.Spread.Sheets.SheetArea.viewport);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](GC.Spread.Sheets.Range.md) | 要清除的范围。 |
| `sheetArea` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | 工作表区域。如果未提供此参数，则默认为 `viewport`。 |

#### Returns

`void`
