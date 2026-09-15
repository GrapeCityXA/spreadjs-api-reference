# Class: ComboBox

[Sheets](../modules/GC.Spread.Sheets.md).[CellTypes](../modules/GC.Spread.Sheets.CellTypes.md).ComboBox

## Hierarchy

- [`Base`](GC.Spread.Sheets.CellTypes.Base.md)

  ↳ **`ComboBox`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.CellTypes.ComboBox.md#constructor)

### Properties

- [typeName](GC.Spread.Sheets.CellTypes.ComboBox.md#typename)

### Methods

- [activateEditor](GC.Spread.Sheets.CellTypes.ComboBox.md#activateeditor)
- [allowFloat](GC.Spread.Sheets.CellTypes.ComboBox.md#allowfloat)
- [createEditorElement](GC.Spread.Sheets.CellTypes.ComboBox.md#createeditorelement)
- [dataBinding](GC.Spread.Sheets.CellTypes.ComboBox.md#databinding)
- [deactivateEditor](GC.Spread.Sheets.CellTypes.ComboBox.md#deactivateeditor)
- [editable](GC.Spread.Sheets.CellTypes.ComboBox.md#editable)
- [editorValueType](GC.Spread.Sheets.CellTypes.ComboBox.md#editorvaluetype)
- [focus](GC.Spread.Sheets.CellTypes.ComboBox.md#focus)
- [format](GC.Spread.Sheets.CellTypes.ComboBox.md#format)
- [fromJSON](GC.Spread.Sheets.CellTypes.ComboBox.md#fromjson)
- [getAutoFitHeight](GC.Spread.Sheets.CellTypes.ComboBox.md#getautofitheight)
- [getAutoFitWidth](GC.Spread.Sheets.CellTypes.ComboBox.md#getautofitwidth)
- [getEditorValue](GC.Spread.Sheets.CellTypes.ComboBox.md#geteditorvalue)
- [getHitInfo](GC.Spread.Sheets.CellTypes.ComboBox.md#gethitinfo)
- [isEditingValueChanged](GC.Spread.Sheets.CellTypes.ComboBox.md#iseditingvaluechanged)
- [isImeAware](GC.Spread.Sheets.CellTypes.ComboBox.md#isimeaware)
- [isReservedKey](GC.Spread.Sheets.CellTypes.ComboBox.md#isreservedkey)
- [itemHeight](GC.Spread.Sheets.CellTypes.ComboBox.md#itemheight)
- [items](GC.Spread.Sheets.CellTypes.ComboBox.md#items)
- [maxDropDownItems](GC.Spread.Sheets.CellTypes.ComboBox.md#maxdropdownitems)
- [paint](GC.Spread.Sheets.CellTypes.ComboBox.md#paint)
- [paintContent](GC.Spread.Sheets.CellTypes.ComboBox.md#paintcontent)
- [parse](GC.Spread.Sheets.CellTypes.ComboBox.md#parse)
- [processKeyDown](GC.Spread.Sheets.CellTypes.ComboBox.md#processkeydown)
- [processKeyUp](GC.Spread.Sheets.CellTypes.ComboBox.md#processkeyup)
- [processMouseDown](GC.Spread.Sheets.CellTypes.ComboBox.md#processmousedown)
- [processMouseEnter](GC.Spread.Sheets.CellTypes.ComboBox.md#processmouseenter)
- [processMouseLeave](GC.Spread.Sheets.CellTypes.ComboBox.md#processmouseleave)
- [processMouseMove](GC.Spread.Sheets.CellTypes.ComboBox.md#processmousemove)
- [processMouseUp](GC.Spread.Sheets.CellTypes.ComboBox.md#processmouseup)
- [selectAll](GC.Spread.Sheets.CellTypes.ComboBox.md#selectall)
- [setEditorValue](GC.Spread.Sheets.CellTypes.ComboBox.md#seteditorvalue)
- [toJSON](GC.Spread.Sheets.CellTypes.ComboBox.md#tojson)
- [updateEditor](GC.Spread.Sheets.CellTypes.ComboBox.md#updateeditor)
- [updateEditorContainer](GC.Spread.Sheets.CellTypes.ComboBox.md#updateeditorcontainer)
- [updateImeMode](GC.Spread.Sheets.CellTypes.ComboBox.md#updateimemode)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new ComboBox**()

表示一个可编辑的组合框单元格。

**`example`**
```
// 此示例创建一个组合框单元格。
var cellType2 = new GC.Spread.Sheets.CellTypes.ComboBox();
cellType2.items(["a","b","c"]);
activeSheet.getCell(2, 2).cellType(cellType2);
```

#### Overrides

[Base](GC.Spread.Sheets.CellTypes.Base.md).[constructor](GC.Spread.Sheets.CellTypes.Base.md#constructor)

## Properties

### <a id="typename" name="typename"></a> typeName

• **typeName**: `string`

表示用于支持序列化的类型名称字符串。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[typeName](GC.Spread.Sheets.CellTypes.Base.md#typename)

## Methods

### <a id="activateeditor" name="activateeditor"></a> activateEditor

▸ **activateEditor**(`editorContext`, `cellStyle`, `cellRect`, `context?`): `void`

激活编辑器，包括设置编辑器的属性或属性以及绑定编辑器的事件。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由 createEditorElement 方法创建的 DOM 元素。 |
| `cellStyle` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际样式。 |
| `cellRect` | [`Rect`](GC.Spread.Sheets.Rect.md) | 单元格的布局信息。 |
| `context?` | `any` | 与单元格类型相关的上下文。 |

#### Returns

`void`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[activateEditor](GC.Spread.Sheets.CellTypes.Base.md#activateeditor)

___

### <a id="allowfloat" name="allowfloat"></a> allowFloat

▸ **allowFloat**(`value?`): `any`

获取或设置是否允许组合框的弹出菜单溢出Spread。

**`example`**
```
// 此示例设置allowFloat方法。
var items2 = ["a", "ab", "abc", "apple", "boy", "cat", "dog"];
var comboBoxCellType = new GC.Spread.Sheets.CellTypes.ComboBox().items(items2);
comboBoxCellType.allowFloat(false);
activeSheet.getCell(1, 3).cellType(comboBoxCellType);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置值，则返回复合框的弹出菜单是否允许溢出Spread；否则返回复合框单元格类型。

___

### <a id="createeditorelement" name="createeditorelement"></a> createEditorElement

▸ **createEditorElement**(`context?`): `HTMLElement`

创建一个 DOM 元素并返回它。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context?` | `any` | 与单元格类型相关的上下文。 |

#### Returns

`HTMLElement`

返回一个 DOM 元素。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[createEditorElement](GC.Spread.Sheets.CellTypes.Base.md#createeditorelement)

___

### <a id="databinding" name="databinding"></a> dataBinding

▸ **dataBinding**(`value?`): [`IDataBinding`](../interfaces/GC.Spread.Sheets.CellTypes.IDataBinding.md) \| [`ComboBox`](GC.Spread.Sheets.CellTypes.ComboBox.md)

获取或设置组合框单元格类型的数据绑定。

**`example`**
```
// 此示例显示将表名绑定到组合框单元格类型。
var tableName = { dataSource: "productName", text: "productName", value: "productId" };
var cellType = new GC.Spread.Sheets.CellTypes.ComboBox();
cellType.dataBinding(tableName);
activeSheet.getCell(1, 3).cellType(cellType);
```

**`example`**
```
// 此示例显示将公式绑定到组合框单元格类型。
var formula = { dataSource: '=SORT(UNIQUE(QUERY("Products", {"productName","productId"})))', text: 0, value: 1 };
var cellType2 = new GC.Spread.Sheets.CellTypes.ComboBox();
cellType2.dataBinding(formula);
activeSheet.getCell(10, 3).cellType(cellType2);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`IDataBinding`](../interfaces/GC.Spread.Sheets.CellTypes.IDataBinding.md) |

#### Returns

[`IDataBinding`](../interfaces/GC.Spread.Sheets.CellTypes.IDataBinding.md) \| [`ComboBox`](GC.Spread.Sheets.CellTypes.ComboBox.md)

如果未设置值，则返回复合框的数据绑定；否则返回复合框单元格类型。

___

### <a id="deactivateeditor" name="deactivateeditor"></a> deactivateEditor

▸ **deactivateEditor**(`editorContext`, `context?`): `void`

停用编辑器，例如取消绑定编辑器的事件。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由 createEditorElement 方法创建的 DOM 元素。 |
| `context?` | `any` | 与单元格类型相关的上下文。 |

#### Returns

`void`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[deactivateEditor](GC.Spread.Sheets.CellTypes.Base.md#deactivateeditor)

___

### <a id="editable" name="editable"></a> editable

▸ **editable**(`value?`): `any`

获取或设置是否可编辑组合框。

**`example`**
```
// 此示例设置editable方法。
var items2 = ["a", "ab", "abc", "apple", "boy", "cat", "dog"];
var eComboBoxCellType = new GC.Spread.Sheets.CellTypes.ComboBox().items(items2).editable(true);
activeSheet.getCell(1, 3).cellType(eComboBoxCellType);
activeSheet.setColumnWidth(0,120);
activeSheet.setColumnWidth(2,120);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否可编辑组合框。 |

#### Returns

`any`

如果未设置值，则返回复合框是否可编辑；否则返回复合框单元格类型。

___

### <a id="editorvaluetype" name="editorvaluetype"></a> editorValueType

▸ **editorValueType**(`value?`): `any`

获取或设置写入基础数据模型的值。

**`example`**
```
// 此示例获取类型。
var cellType2 = new GC.Spread.Sheets.CellTypes.ComboBox();
cellType2.items(["a","b","c"]);
activeSheet.getCell(2, 2).cellType(cellType2);
alert(cellType2.editorValueType());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`EditorValueType`](../enums/GC.Spread.Sheets.CellTypes.EditorValueType.md) | 编辑器的值类型。 |

#### Returns

`any`

如果未设置值，则返回复合框的值类型；否则返回复合框单元格类型。

___

### <a id="focus" name="focus"></a> focus

▸ **focus**(`editorContext`, `context?`): `void`

聚焦编辑器 DOM 元素。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由 createEditorElement 方法创建的 DOM 元素。 |
| `context?` | `any` | 与单元格类型相关的上下文。 |

#### Returns

`void`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[focus](GC.Spread.Sheets.CellTypes.Base.md#focus)

___

### <a id="format" name="format"></a> format

▸ **format**(`value`, `format`, `formattedData?`, `context?`): `string`

使用指定的格式格式化一个值。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 要格式化的对象值。 |
| `format` | `string` \| [`GeneralFormatter`](GC.Spread.Formatter.GeneralFormatter.md) | 格式。 |
| `formattedData?` | [`FormattedData`](../interfaces/GC.Spread.Sheets.FormattedData.md) | 格式化的数据。 |
| `context?` | `any` | 与单元格类型相关的上下文。 |

#### Returns

`string`

返回格式化的字符串。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[format](GC.Spread.Sheets.CellTypes.Base.md#format)

___

### <a id="fromjson" name="fromjson"></a> fromJSON

▸ **fromJSON**(`settings`): `void`

从指定的 JSON 字符串加载对象状态。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `settings` | `any` | 从反序列化获取的单元格类型数据。 |

#### Returns

`void`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[fromJSON](GC.Spread.Sheets.CellTypes.Base.md#fromjson)

___

### <a id="getautofitheight" name="getautofitheight"></a> getAutoFitHeight

▸ **getAutoFitHeight**(`value`, `text`, `cellStyle`, `zoomFactor`, `context?`): `number`

获取一个单元格的高度，可以用于处理行自动适应。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 单元格的值。 |
| `text` | `string` | 单元格的文本。 |
| `cellStyle` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际值。 |
| `zoomFactor` | `number` | 当前工作表的缩放因子。 |
| `context?` | `any` | 与单元格类型相关的上下文。 |

#### Returns

`number`

返回单元格的高度，可以用于处理行自动适应。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[getAutoFitHeight](GC.Spread.Sheets.CellTypes.Base.md#getautofitheight)

___

### <a id="getautofitwidth" name="getautofitwidth"></a> getAutoFitWidth

▸ **getAutoFitWidth**(`value`, `text`, `cellStyle`, `zoomFactor`, `context?`): `number`

获取一个单元格的宽度，可以用于处理列自动适应。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 单元格的值。 |
| `text` | `string` | 单元格的文本。 |
| `cellStyle` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际值。 |
| `zoomFactor` | `number` | 当前工作表的缩放因子。 |
| `context?` | `any` | 与单元格类型相关的上下文。 |

#### Returns

`number`

返回单元格的宽度，可以用于处理列自动适应。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[getAutoFitWidth](GC.Spread.Sheets.CellTypes.Base.md#getautofitwidth)

___

### <a id="geteditorvalue" name="geteditorvalue"></a> getEditorValue

▸ **getEditorValue**(`editorContext`, `context?`): `any`

获取编辑器的值。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由 createEditorElement 方法创建的 DOM 元素。 |
| `context?` | `any` | 与单元格类型相关的上下文。 |

#### Returns

`any`

返回编辑器的值。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[getEditorValue](GC.Spread.Sheets.CellTypes.Base.md#geteditorvalue)

___

### <a id="gethitinfo" name="gethitinfo"></a> getHitInfo

▸ **getHitInfo**(`x`, `y`, `cellStyle`, `cellRect`, `context?`): [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md)

获取单元格类型的命中信息。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | 指针当前位置相对于画布的 <i>x</i> 坐标。 |
| `y` | `number` | 指针当前位置相对于画布的 <i>y</i> 坐标。 |
| `cellStyle` | [`Style`](GC.Spread.Sheets.Style.md) | 当前单元格的实际样式。 |
| `cellRect` | [`Rect`](GC.Spread.Sheets.Rect.md) | 当前单元格的布局信息。 |
| `context?` | `any` | 与单元格类型相关的上下文。 |

#### Returns

[`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md)

返回一个包含 <i>x</i>, <i>y</i>, <i>row</i>, <i>col</i>, <i>cellRect</i> 和 <i>sheetArea</i> 参数的对象，以及一个指示 <i>isReservedLocation</i> 的值。
<i>isReservedLocation</i> 为 `true` 表示命中测试在单元格类型需要处理的特殊区域；否则为 `false`。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[getHitInfo](GC.Spread.Sheets.CellTypes.Base.md#gethitinfo)

___

### <a id="iseditingvaluechanged" name="iseditingvaluechanged"></a> isEditingValueChanged

▸ **isEditingValueChanged**(`oldValue`, `newValue`, `context?`): `boolean`

编辑值是否已更改。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `oldValue` | `any` | 旧的编辑值。 |
| `newValue` | `any` | 新的编辑值。 |
| `context?` | `any` | 与单元格类型相关的上下文。有关更多信息，请参阅备注。 |

#### Returns

`boolean`

如果 oldValue 等于 newValue，则返回 `true`；否则返回 `false`。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[isEditingValueChanged](GC.Spread.Sheets.CellTypes.Base.md#iseditingvaluechanged)

___

### <a id="isimeaware" name="isimeaware"></a> isImeAware

▸ **isImeAware**(`context?`): `boolean`

此单元格类型是否支持 IME。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context?` | `any` | 与单元格类型相关的上下文。有关更多信息，请参阅备注。 |

#### Returns

`boolean`

如果单元格类型支持 IME，则返回 `true`；否则返回 `false`。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[isImeAware](GC.Spread.Sheets.CellTypes.Base.md#isimeaware)

___

### <a id="isreservedkey" name="isreservedkey"></a> isReservedKey

▸ **isReservedKey**(`e`, `context?`): `boolean`

单元格类型是否自行处理键盘事件。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `e` | `KeyboardEvent` | 键盘事件。 |
| `context?` | `any` | 与单元格类型相关的上下文。有关更多信息，请参阅备注。 |

#### Returns

`boolean`

如果单元格类型自行处理键盘事件，则返回 `true`；否则返回 `false`。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[isReservedKey](GC.Spread.Sheets.CellTypes.Base.md#isreservedkey)

___

### <a id="itemheight" name="itemheight"></a> itemHeight

▸ **itemHeight**(`value?`): `any`

获取或设置每个项目的身高。

**`example`**
```
// 此示例设置itemHeight方法。
var cellType2 = new GC.Spread.Sheets.CellTypes.ComboBox();
cellType2.items(["a","b","c"]);
cellType2.itemHeight(30);
activeSheet.getCell(2, 2).cellType(cellType2);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 每个项目的身高。 |

#### Returns

`any`

如果未设置值，则返回复合框的每个项目的身高；否则返回复合框单元格类型。

___

### <a id="items" name="items"></a> items

▸ **items**(`items?`): `any`

获取或设置组合框下拉列表的项目。

**`example`**
```
// 此示例创建一个组合框单元格。
var cellType2 = new GC.Spread.Sheets.CellTypes.ComboBox();
cellType2.items(["a","b","c"]);
activeSheet.getCell(2, 2).cellType(cellType2);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `items?` | `any`[] | 组合框的项目。 |

#### Returns

`any`

如果未设置值，则返回项目数组；否则返回复合框单元格类型。

___

### <a id="maxdropdownitems" name="maxdropdownitems"></a> maxDropDownItems

▸ **maxDropDownItems**(`value?`): `any`

获取或设置每页下拉列表的最大项目数。

**`example`**
```
// 此示例显示一次显示三个项目。
var cellType2 = new GC.Spread.Sheets.CellTypes.ComboBox();
cellType2.items(["a", "b", "c", "d", "e", "f", "g", "h"]);
cellType2.maxDropDownItems(3);
activeSheet.getCell(2, 2).cellType(cellType2);
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 每页下拉列表的最大项目数。 |

#### Returns

`any`

如果未设置值，则返回复合框每页下拉列表的最大项目数；否则返回复合框单元格类型。

___

### <a id="paint" name="paint"></a> paint

▸ **paint**(`ctx`, `value`, `x`, `y`, `w`, `h`, `style`, `context?`): `void`

在画布上绘制单元格。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ctx` | `CanvasRenderingContext2D` | 画布的二维上下文。 |
| `value` | `any` | 单元格的值。 |
| `x` | `number` | 相对于画布的 <i>x</i> 坐标。 |
| `y` | `number` | 相对于画布的 <i>y</i> 坐标。 |
| `w` | `number` | 单元格的宽度。 |
| `h` | `number` | 单元格的高度。 |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际样式。 |
| `context?` | `any` | 与单元格类型相关的上下文。有关更多信息，请参阅备注。 |

#### Returns

`void`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[paint](GC.Spread.Sheets.CellTypes.Base.md#paint)

___

### <a id="paintcontent" name="paintcontent"></a> paintContent

▸ **paintContent**(`ctx`, `value`, `x`, `y`, `w`, `h`, `style`, `context?`): `void`

在画布上绘制单元格内容区域。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ctx` | `CanvasRenderingContext2D` | 画布的二维上下文。 |
| `value` | `any` | 单元格的值。 |
| `x` | `number` | 相对于画布的 <i>x</i> 坐标。 |
| `y` | `number` | 相对于画布的 <i>y</i> 坐标。 |
| `w` | `number` | 单元格内容区域的宽度。 |
| `h` | `number` | 单元格内容区域的高度。 |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际样式。 |
| `context?` | `any` | 与单元格类型相关的上下文。有关更多信息，请参阅备注。 |

#### Returns

`void`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[paintContent](GC.Spread.Sheets.CellTypes.Base.md#paintcontent)

___

### <a id="parse" name="parse"></a> parse

▸ **parse**(`text`, `formatStr`, `context?`): `any`

使用指定的格式字符串将文本解析为对象。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `text` | `string` | 要解析的文本字符串。 |
| `formatStr` | `string` | 解析格式字符串。 |
| `context?` | `any` | 与单元格类型相关的上下文。有关更多信息，请参阅备注。 |

#### Returns

`any`

解析后的对象。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[parse](GC.Spread.Sheets.CellTypes.Base.md#parse)

___

### <a id="processkeydown" name="processkeydown"></a> processKeyDown

▸ **processKeyDown**(`event`, `context?`): `boolean`

在显示模式下处理按键按下事件。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `event` | `KeyboardEvent` | 键盘事件。 |
| `context?` | `any` | 与单元格类型相关的上下文。有关更多信息，请参阅备注。 |

#### Returns

`boolean`

如果处理成功则返回 `true`；否则返回 `false`。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[processKeyDown](GC.Spread.Sheets.CellTypes.Base.md#processkeydown)

___

### <a id="processkeyup" name="processkeyup"></a> processKeyUp

▸ **processKeyUp**(`event`, `context?`): `boolean`

在显示模式下处理按键释放事件。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `event` | `KeyboardEvent` | 键盘事件。 |
| `context?` | `any` | 与单元格类型相关的上下文。有关更多信息，请参阅备注。 |

#### Returns

`boolean`

如果处理成功则返回 `true`；否则返回 `false`。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[processKeyUp](GC.Spread.Sheets.CellTypes.Base.md#processkeyup)

___

### <a id="processmousedown" name="processmousedown"></a> processMouseDown

▸ **processMouseDown**(`hitInfo`): `boolean`

在显示模式下处理鼠标按下事件。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitInfo` | [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md) | 由 getHitInfo 方法返回的命中测试信息。有关更多信息，请参阅备注。 |

#### Returns

`boolean`

如果处理成功则返回 `true`；否则返回 `false`。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[processMouseDown](GC.Spread.Sheets.CellTypes.Base.md#processmousedown)

___

### <a id="processmouseenter" name="processmouseenter"></a> processMouseEnter

▸ **processMouseEnter**(`hitInfo`): `boolean`

在显示模式下处理鼠标进入事件。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitInfo` | [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md) | 由 getHitInfo 方法返回的命中测试信息。有关更多信息，请参阅备注。 |

#### Returns

`boolean`

如果处理成功则返回 `true`；否则返回 `false`。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[processMouseEnter](GC.Spread.Sheets.CellTypes.Base.md#processmouseenter)

___

### <a id="processmouseleave" name="processmouseleave"></a> processMouseLeave

▸ **processMouseLeave**(`hitInfo`): `boolean`

在显示模式下处理鼠标离开事件。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitInfo` | [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md) | 由 getHitInfo 方法返回的命中测试信息。有关更多信息，请参阅备注。 |

#### Returns

`boolean`

如果处理成功则返回 `true`；否则返回 `false`。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[processMouseLeave](GC.Spread.Sheets.CellTypes.Base.md#processmouseleave)

___

### <a id="processmousemove" name="processmousemove"></a> processMouseMove

▸ **processMouseMove**(`hitInfo`): `boolean`

在显示模式下处理鼠标移动事件。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitInfo` | [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md) | 由 getHitInfo 方法返回的命中测试信息。有关更多信息，请参阅备注。 |

#### Returns

`boolean`

如果处理成功则返回 `true`；否则返回 `false`。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[processMouseMove](GC.Spread.Sheets.CellTypes.Base.md#processmousemove)

___

### <a id="processmouseup" name="processmouseup"></a> processMouseUp

▸ **processMouseUp**(`hitInfo`): `boolean`

在显示模式下处理鼠标释放事件。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitInfo` | [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md) | 由 getHitInfo 方法返回的命中测试信息。有关更多信息，请参阅备注。 |

#### Returns

`boolean`

如果处理成功则返回 `true`；否则返回 `false`。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[processMouseUp](GC.Spread.Sheets.CellTypes.Base.md#processmouseup)

___

### <a id="selectall" name="selectall"></a> selectAll

▸ **selectAll**(`editorContext`, `context?`): `void`

选择编辑器 DOM 元素中的所有文本。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由 createEditorElement 方法创建的 DOM 元素。 |
| `context?` | `any` | 与单元格类型相关的上下文。有关更多信息，请参阅备注。 |

#### Returns

`void`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[selectAll](GC.Spread.Sheets.CellTypes.Base.md#selectall)

___

### <a id="seteditorvalue" name="seteditorvalue"></a> setEditorValue

▸ **setEditorValue**(`editorContext`, `value`, `context?`): `void`

设置编辑器的值。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由 createEditorElement 方法创建的 DOM 元素。 |
| `value` | `any` | 由活动单元格返回的值。 |
| `context?` | `any` | 与单元格类型相关的上下文。有关更多信息，请参阅备注。 |

#### Returns

`void`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[setEditorValue](GC.Spread.Sheets.CellTypes.Base.md#seteditorvalue)

___

### <a id="tojson" name="tojson"></a> toJSON

▸ **toJSON**(): `any`

将对象状态保存为 JSON 字符串。

#### Returns

`any`

单元格类型数据。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[toJSON](GC.Spread.Sheets.CellTypes.Base.md#tojson)

___

### <a id="updateeditor" name="updateeditor"></a> updateEditor

▸ **updateEditor**(`editorContext`, `cellStyle`, `cellRect`, `context?`): [`Rect`](GC.Spread.Sheets.Rect.md)

更新编辑器的大小。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由 createEditorElement 方法创建的 DOM 元素。 |
| `cellStyle` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际样式。 |
| `cellRect` | [`Rect`](GC.Spread.Sheets.Rect.md) | 单元格的布局信息。 |
| `context?` | `any` | 与单元格类型相关的上下文。有关更多信息，请参阅备注。 |

#### Returns

[`Rect`](GC.Spread.Sheets.Rect.md)

返回单元格包装元素的新大小，它应包含 'width' 和 'height' 两个属性。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[updateEditor](GC.Spread.Sheets.CellTypes.Base.md#updateeditor)

___

### <a id="updateeditorcontainer" name="updateeditorcontainer"></a> updateEditorContainer

▸ **updateEditorContainer**(`editorContext`, `editorBounds`, `cellStyle`): `void`

更新单元格包装元素的大小。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由 createEditorElement 方法创建的 DOM 元素。 |
| `editorBounds` | [`Rect`](GC.Spread.Sheets.Rect.md) | 单元格包装元素的新大小。 |
| `cellStyle` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际样式。 |

#### Returns

`void`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[updateEditorContainer](GC.Spread.Sheets.CellTypes.Base.md#updateeditorcontainer)

___

### <a id="updateimemode" name="updateimemode"></a> updateImeMode

▸ **updateImeMode**(`editorContext`, `imeMode`, `context?`): `void`

更新编辑器的输入法模式。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由 createEditorElement 方法创建的 DOM 元素。 |
| `imeMode` | [`ImeMode`](../enums/GC.Spread.Sheets.ImeMode.md) | 来自单元格实际样式的输入法模式。 |
| `context?` | `any` | 与单元格类型相关的上下文。有关更多信息，请参阅备注。 |

#### Returns

`void`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[updateImeMode](GC.Spread.Sheets.CellTypes.Base.md#updateimemode)
