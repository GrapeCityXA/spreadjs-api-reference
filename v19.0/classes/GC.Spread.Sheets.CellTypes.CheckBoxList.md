# Class: CheckBoxList

[Sheets](../modules/GC.Spread.Sheets.md).[CellTypes](../modules/GC.Spread.Sheets.CellTypes.md).CheckBoxList

## Hierarchy

- [`Base`](GC.Spread.Sheets.CellTypes.Base.md)

  ↳ **`CheckBoxList`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.CellTypes.CheckBoxList.md#constructor)

### Properties

- [typeName](GC.Spread.Sheets.CellTypes.CheckBoxList.md#typename)

### Methods

- [activateEditor](GC.Spread.Sheets.CellTypes.CheckBoxList.md#activateeditor)
- [boxSize](GC.Spread.Sheets.CellTypes.CheckBoxList.md#boxsize)
- [createEditorElement](GC.Spread.Sheets.CellTypes.CheckBoxList.md#createeditorelement)
- [deactivateEditor](GC.Spread.Sheets.CellTypes.CheckBoxList.md#deactivateeditor)
- [direction](GC.Spread.Sheets.CellTypes.CheckBoxList.md#direction)
- [focus](GC.Spread.Sheets.CellTypes.CheckBoxList.md#focus)
- [format](GC.Spread.Sheets.CellTypes.CheckBoxList.md#format)
- [fromJSON](GC.Spread.Sheets.CellTypes.CheckBoxList.md#fromjson)
- [getAutoFitHeight](GC.Spread.Sheets.CellTypes.CheckBoxList.md#getautofitheight)
- [getAutoFitWidth](GC.Spread.Sheets.CellTypes.CheckBoxList.md#getautofitwidth)
- [getEditorValue](GC.Spread.Sheets.CellTypes.CheckBoxList.md#geteditorvalue)
- [getHitInfo](GC.Spread.Sheets.CellTypes.CheckBoxList.md#gethitinfo)
- [isEditingValueChanged](GC.Spread.Sheets.CellTypes.CheckBoxList.md#iseditingvaluechanged)
- [isFlowLayout](GC.Spread.Sheets.CellTypes.CheckBoxList.md#isflowlayout)
- [isImeAware](GC.Spread.Sheets.CellTypes.CheckBoxList.md#isimeaware)
- [isReservedKey](GC.Spread.Sheets.CellTypes.CheckBoxList.md#isreservedkey)
- [itemSpacing](GC.Spread.Sheets.CellTypes.CheckBoxList.md#itemspacing)
- [items](GC.Spread.Sheets.CellTypes.CheckBoxList.md#items)
- [maxColumnCount](GC.Spread.Sheets.CellTypes.CheckBoxList.md#maxcolumncount)
- [maxRowCount](GC.Spread.Sheets.CellTypes.CheckBoxList.md#maxrowcount)
- [mode](GC.Spread.Sheets.CellTypes.CheckBoxList.md#mode)
- [paint](GC.Spread.Sheets.CellTypes.CheckBoxList.md#paint)
- [paintContent](GC.Spread.Sheets.CellTypes.CheckBoxList.md#paintcontent)
- [parse](GC.Spread.Sheets.CellTypes.CheckBoxList.md#parse)
- [processKeyDown](GC.Spread.Sheets.CellTypes.CheckBoxList.md#processkeydown)
- [processKeyUp](GC.Spread.Sheets.CellTypes.CheckBoxList.md#processkeyup)
- [processMouseDown](GC.Spread.Sheets.CellTypes.CheckBoxList.md#processmousedown)
- [processMouseEnter](GC.Spread.Sheets.CellTypes.CheckBoxList.md#processmouseenter)
- [processMouseLeave](GC.Spread.Sheets.CellTypes.CheckBoxList.md#processmouseleave)
- [processMouseMove](GC.Spread.Sheets.CellTypes.CheckBoxList.md#processmousemove)
- [processMouseUp](GC.Spread.Sheets.CellTypes.CheckBoxList.md#processmouseup)
- [selectAll](GC.Spread.Sheets.CellTypes.CheckBoxList.md#selectall)
- [setEditorValue](GC.Spread.Sheets.CellTypes.CheckBoxList.md#seteditorvalue)
- [textAlign](GC.Spread.Sheets.CellTypes.CheckBoxList.md#textalign)
- [toJSON](GC.Spread.Sheets.CellTypes.CheckBoxList.md#tojson)
- [toggleOptions](GC.Spread.Sheets.CellTypes.CheckBoxList.md#toggleoptions)
- [updateEditor](GC.Spread.Sheets.CellTypes.CheckBoxList.md#updateeditor)
- [updateEditorContainer](GC.Spread.Sheets.CellTypes.CheckBoxList.md#updateeditorcontainer)
- [updateImeMode](GC.Spread.Sheets.CellTypes.CheckBoxList.md#updateimemode)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new CheckBoxList**()

表示一个可编辑的复选框列表单元格。

**`example`**
```
//此示例创建一个复选框列表单元格。
var cellType2 = new GC.Spread.Sheets.CellTypes.CheckBoxList();
cellType2.items([{text:"a",value:1},{text:"b",value:2},{text:"c",value:3}]);
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

### <a id="boxsize" name="boxsize"></a> boxSize

▸ **boxSize**(`value?`): `any`

获取或设置复选框的大小，只支持数字和“auto”。如果使用非法值，大小不会改变。

**`example`**
```
// 此示例创建一个复选框列表单元格。
var cellType2 = new GC.Spread.Sheets.CellTypes.CheckBoxList();
cellType2.items([{text:"a",value:1},{text:"b",value:2},{text:"c",value:3}]);
cellType2.boxSize(20);
activeSheet.getCell(2, 2).cellType(cellType2);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` \| `number` | 复选框的大小。如果值为“auto”，则复选框的大小将随字体大小变化。 |

#### Returns

`any`

如果未设置值，则返回复选框的大小；否则返回复选框列表单元格类型。

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

### <a id="direction" name="direction"></a> direction

▸ **direction**(`value?`): `any`

获取或设置复选框列表的顺序。

**`example`**
```
// 此示例创建一个复选框列表单元格。
var cellType2 = new GC.Spread.Sheets.CellTypes.CheckBoxList();
cellType2.items([{text:"a",value:1},{text:"b",value:2},{text:"c",value:3}]);
cellType2.direction(GC.Spread.Sheets.CellTypes.Direction.vertical);
activeSheet.getCell(2, 2).cellType(cellType2);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`Direction`](../enums/GC.Spread.Sheets.CellTypes.Direction.md) | 是否垂直。 |

#### Returns

`any`

如果未设置值，则返回复选框列表的顺序是否垂直；否则返回复选框列表单元格类型。

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

### <a id="isflowlayout" name="isflowlayout"></a> isFlowLayout

▸ **isFlowLayout**(`value?`): `any`

获取或设置复选框列表的布局是否自动适应。

**`example`**
```
// 此示例创建一个复选框列表单元格。
var cellType2 = new GC.Spread.Sheets.CellTypes.CheckBoxList();
cellType2.items([{text:"a",value:1},{text:"b",value:2},{text:"c",value:3}]);
cellType2.isFlowLayout(true);
activeSheet.getCell(2, 2).cellType(cellType2);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否自动适应。 |

#### Returns

`any`

如果未设置值，则返回是否自动适应；否则返回复选框列表单元格类型。

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

### <a id="itemspacing" name="itemspacing"></a> itemSpacing

▸ **itemSpacing**(`value?`): `any`

获取或设置复选框列表中两个项目之间的间距。

**`example`**
```
// 此示例创建一个复选框列表单元格。
var cellType2 = new GC.Spread.Sheets.CellTypes.CheckBoxList();
cellType2.items([{text:"a",value:1},{text:"b",value:2},{text:"c",value:3}]);
cellType2.itemSpacing({
     horizontal:80,
     vertical:20
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`IItemSpacing`](../interfaces/GC.Spread.Sheets.CellTypes.IItemSpacing.md) | 复选框列表中两个项目之间的间距。 |

#### Returns

`any`

如果未设置值，则返回复选框列表中两个项目之间的间距；否则返回复选框列表单元格类型。

___

### <a id="items" name="items"></a> items

▸ **items**(`items?`): `any`

获取或设置复选框列表的项目。

**`example`**
```
// 此示例创建一个复选框列表单元格。
var cellType2 = new GC.Spread.Sheets.CellTypes.CheckBoxList();
cellType2.items([{text:"a",value:1},{text:"b",value:2},{text:"c",value:3}]);
activeSheet.getCell(2, 2).cellType(cellType2);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `items?` | `string`[] \| [`ICelltypeItemOption`](../interfaces/GC.Spread.Sheets.CellTypes.ICelltypeItemOption.md)[] | 复选框列表的项目。 |

#### Returns

`any`

如果未设置值，则返回项目数组；否则返回复选框列表单元格类型。

___

### <a id="maxcolumncount" name="maxcolumncount"></a> maxColumnCount

▸ **maxColumnCount**(`value?`): `any`

获取或设置复选框列表的列数。

**`example`**
```
// 此示例创建一个复选框列表单元格。
var cellType2 = new GC.Spread.Sheets.CellTypes.CheckBoxList();
cellType2.items([{text:"a",value:1},{text:"b",value:2},{text:"c",value:3}]);
cellType2.maxColumnCount(2);
activeSheet.getCell(2, 2).cellType(cellType2);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 复选框列表的列数。 |

#### Returns

`any`

如果未设置值，则返回列数；否则返回复选框列表单元格类型。

___

### <a id="maxrowcount" name="maxrowcount"></a> maxRowCount

▸ **maxRowCount**(`value?`): `any`

获取或设置复选框列表的行数。

**`example`**
```
// 此示例创建一个复选框列表单元格。
var cellType2 = new GC.Spread.Sheets.CellTypes.CheckBoxList();
cellType2.items([{text:"a",value:1},{text:"b",value:2},{text:"c",value:3}]);
cellType2.maxRowCount(2);
activeSheet.getCell(2, 2).cellType(cellType2);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 复选框列表的行数。 |

#### Returns

`any`

如果未设置值，则返回行数；否则返回复选框列表单元格类型。

___

### <a id="mode" name="mode"></a> mode

▸ **mode**(`value?`): `any`

获取或设置一个值，该值指示复选框列表单元格类型的模式。

**`example`**
```
// 此示例创建一个复选框列表单元格。
var cellType = new GC.Spread.Sheets.CellTypes.CheckBoxList();
cellType.items([{text:"a",value:1},{text:"b",value:2},{text:"c",value:3}]);
cellType.mode("toggle");
activeSheet.getCell(2, 2).cellType(cellType);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | ``"checkbox"`` \| ``"toggle"`` | 复选框列表单元格类型的模式。 |

#### Returns

`any`

如果未设置值，则返回复选框列表单元格类型的模式。

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

### <a id="textalign" name="textalign"></a> textAlign

▸ **textAlign**(`value?`): `any`

获取或设置复选框的位置文本，只支持“left”和“right”。

**`example`**
```
// 此示例创建一个复选框列表单元格。
var cellType2 = new GC.Spread.Sheets.CellTypes.CheckBoxList();
cellType2.items([{text:"a",value:1},{text:"b",value:2},{text:"c",value:3}]);
cellType2.textAlign(GC.Spread.Sheets.CellTypes.TextAlign.left);
activeSheet.getCell(2, 2).cellType(cellType2);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`TextAlign`](../enums/GC.Spread.Sheets.CellTypes.TextAlign.md) | 复选框的位置文本。 |

#### Returns

`any`

如果未设置值，则返回复选框的位置文本；否则返回复选框列表单元格类型。

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

### <a id="toggleoptions" name="toggleoptions"></a> toggleOptions

▸ **toggleOptions**(`value?`): `any`

获取或设置一个值，该值指示切换选项

**`example`**
```
// 此示例创建一个复选框列表单元格。
var cellType = new GC.Spread.Sheets.CellTypes.CheckBoxList();
cellType.items([{text:"a",value:1},{text:"b",value:2},{text:"c",value:3}]);
cellType.mode("toggle");
cellType.toggleOptions({
    width: 60,
    height: 30,
    trackColorOn: '#4CAF50',
    trackColorOff: '#767577',
    sliderColorOn: '#ffffff',
    sliderColorOff: '#ffffff',
    sliderMargin: 2,
    animationDuration: 100,
    trackRadius: 8,
    sliderRadius: 4
});
activeSheet.getCell(2, 2).cellType(cellType);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`IToggleOptions`](../interfaces/GC.Spread.Sheets.CellTypes.IToggleOptions.md) | 切换选项。 |

#### Returns

`any`

如果未设置值，则返回切换选项。

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
