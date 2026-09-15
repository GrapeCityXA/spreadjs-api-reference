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

可以管理工作表中所有单元格状态的单元格管理器

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheet` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 工作表 |

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`range`, `state`, `style`, `sheetArea?`): `void`

**`description`** 为range添加单元格状态实例，当区域单元格的状态匹配时，将应用cellState的样式

**`代码示例`**
``` javascript
var style = new  GC.Spread.Sheets.Style();
style.backColor = 'blue';
style.foreColor = 'red';
var range = new GC.Spread.Sheets.Range(1,2,3,3);
sheet.cellStates.add(range,GC.Spread.Sheets.CellStatesType.hover,style,101);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](GC.Spread.Sheets.Range.md) | 作用域区域将应用cellState的样式 |
| `state` | [`CellStatesType`](../enums/GC.Spread.Sheets.CellStatesType.md) | 哪个状态将使用样式 |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 状态匹配时的样式 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | 工作表区域如果未提供此参数，则默认为<b> viewport </b> |

#### Returns

`void`

___

### <a id="clear" name="clear"></a> clear

▸ **clear**(`range`, `sheetArea`): `void`

**`description`** 按区域清除所有样式，清除后，当单元格状态匹配时将不应用任何样式

**`代码示例`**
``` javascript
var range = new GC.Spread.Sheets.Range(1,2,3,3);
sheet.cellStates.clear(range, GC.Spread.Sheets.SheetArea.viewport);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](GC.Spread.Sheets.Range.md) | 区域区域明确 |
| `sheetArea` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | 工作表区域如果未提供此参数，则默认为<b> viewport </b> |

#### Returns

`void`
