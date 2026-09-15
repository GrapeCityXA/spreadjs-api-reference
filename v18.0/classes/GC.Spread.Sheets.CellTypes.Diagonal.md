# Class: Diagonal

[Sheets](../modules/GC.Spread.Sheets.md).[CellTypes](../modules/GC.Spread.Sheets.CellTypes.md).Diagonal

## Hierarchy

- [`Text`](GC.Spread.Sheets.CellTypes.Text.md)

  ↳ **`Diagonal`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.CellTypes.Diagonal.md#constructor)

### Properties

- [typeName](GC.Spread.Sheets.CellTypes.Diagonal.md#typename)

### Methods

- [activateEditor](GC.Spread.Sheets.CellTypes.Diagonal.md#activateeditor)
- [createEditorElement](GC.Spread.Sheets.CellTypes.Diagonal.md#createeditorelement)
- [deactivateEditor](GC.Spread.Sheets.CellTypes.Diagonal.md#deactivateeditor)
- [divergeDirection](GC.Spread.Sheets.CellTypes.Diagonal.md#divergedirection)
- [focus](GC.Spread.Sheets.CellTypes.Diagonal.md#focus)
- [format](GC.Spread.Sheets.CellTypes.Diagonal.md#format)
- [fromJSON](GC.Spread.Sheets.CellTypes.Diagonal.md#fromjson)
- [getAutoFitHeight](GC.Spread.Sheets.CellTypes.Diagonal.md#getautofitheight)
- [getAutoFitWidth](GC.Spread.Sheets.CellTypes.Diagonal.md#getautofitwidth)
- [getEditorValue](GC.Spread.Sheets.CellTypes.Diagonal.md#geteditorvalue)
- [getHitInfo](GC.Spread.Sheets.CellTypes.Diagonal.md#gethitinfo)
- [isEditingValueChanged](GC.Spread.Sheets.CellTypes.Diagonal.md#iseditingvaluechanged)
- [isImeAware](GC.Spread.Sheets.CellTypes.Diagonal.md#isimeaware)
- [isReservedKey](GC.Spread.Sheets.CellTypes.Diagonal.md#isreservedkey)
- [lineBorder](GC.Spread.Sheets.CellTypes.Diagonal.md#lineborder)
- [paint](GC.Spread.Sheets.CellTypes.Diagonal.md#paint)
- [paintContent](GC.Spread.Sheets.CellTypes.Diagonal.md#paintcontent)
- [parse](GC.Spread.Sheets.CellTypes.Diagonal.md#parse)
- [processKeyDown](GC.Spread.Sheets.CellTypes.Diagonal.md#processkeydown)
- [processKeyUp](GC.Spread.Sheets.CellTypes.Diagonal.md#processkeyup)
- [processMouseDown](GC.Spread.Sheets.CellTypes.Diagonal.md#processmousedown)
- [processMouseEnter](GC.Spread.Sheets.CellTypes.Diagonal.md#processmouseenter)
- [processMouseLeave](GC.Spread.Sheets.CellTypes.Diagonal.md#processmouseleave)
- [processMouseMove](GC.Spread.Sheets.CellTypes.Diagonal.md#processmousemove)
- [processMouseUp](GC.Spread.Sheets.CellTypes.Diagonal.md#processmouseup)
- [selectAll](GC.Spread.Sheets.CellTypes.Diagonal.md#selectall)
- [setEditorValue](GC.Spread.Sheets.CellTypes.Diagonal.md#seteditorvalue)
- [toJSON](GC.Spread.Sheets.CellTypes.Diagonal.md#tojson)
- [updateEditor](GC.Spread.Sheets.CellTypes.Diagonal.md#updateeditor)
- [updateEditorContainer](GC.Spread.Sheets.CellTypes.Diagonal.md#updateeditorcontainer)
- [updateImeMode](GC.Spread.Sheets.CellTypes.Diagonal.md#updateimemode)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Diagonal**()

表示一个带对角线的单元格。

**`example`**
```
//This example creates a diagonal cell.
var diagonalCellType = new GC.Spread.Sheets.CellTypes.Diagonal();
activeSheet.getCell(2, 2).cellType(diagonalCellType).value('Year,Product,Region');
```

#### Overrides

[Text](GC.Spread.Sheets.CellTypes.Text.md).[constructor](GC.Spread.Sheets.CellTypes.Text.md#constructor)

## Properties

### <a id="typename" name="typename"></a> typeName

• **typeName**: `string`

表示用于支持序列化的类型名称字符串。

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[typeName](GC.Spread.Sheets.CellTypes.Text.md#typename)

## Methods

### <a id="activateeditor" name="activateeditor"></a> activateEditor

▸ **activateEditor**(`editorContext`, `cellStyle`, `cellRect`, `context?`): `void`

激活编辑器，包括为编辑器设置属性或特性，并为编辑器绑定事件。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由 createEditorElement 方法创建的 DOM 元素。 |
| `cellStyle` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际样式。 |
| `cellRect` | [`Rect`](GC.Spread.Sheets.Rect.md) | 单元格的布局信息。 |
| `context?` | `any` | 与单元格类型相关联的上下文。更多信息请参阅 “备注”。 |

#### Returns

`void`

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[activateEditor](GC.Spread.Sheets.CellTypes.Text.md#activateeditor)

___

### <a id="createeditorelement" name="createeditorelement"></a> createEditorElement

▸ **createEditorElement**(`context?`): `HTMLElement`

创建一个 DOM 元素，然后返回它。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context?` | `any` | 与单元格类型相关联的上下文。更多信息请参阅 “备注”。 |

#### Returns

`HTMLElement`

返回一个 DOM 元素。

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[createEditorElement](GC.Spread.Sheets.CellTypes.Text.md#createeditorelement)

___

### <a id="deactivateeditor" name="deactivateeditor"></a> deactivateEditor

▸ **deactivateEditor**(`editorContext`, `context?`): `void`

停用编辑器，例如解除编辑器的事件绑定。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由 createEditorElement 方法创建的 DOM 元素。 |
| `context?` | `any` | 与单元格类型相关联的上下文。更多信息请参阅 “备注”。 |

#### Returns

`void`

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[deactivateEditor](GC.Spread.Sheets.CellTypes.Text.md#deactivateeditor)

___

### <a id="divergedirection" name="divergedirection"></a> divergeDirection

▸ **divergeDirection**(`value?`): [`Diagonal`](GC.Spread.Sheets.CellTypes.Diagonal.md) \| [`DivergeDirection`](../enums/GC.Spread.Sheets.CellTypes.DivergeDirection.md)

获取或设置对角线单元格类型的发散方向。

**`example`**
```
//This example gets the diverge direction type.
var cellType = new GC.Spread.Sheets.CellTypes.Diagonal();
activeSheet.getCell(2, 2).cellType(cellType);
alert(cellType.divergeDirection());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`DivergeDirection`](../enums/GC.Spread.Sheets.CellTypes.DivergeDirection.md) | 发散方向的类型。 |

#### Returns

[`Diagonal`](GC.Spread.Sheets.CellTypes.Diagonal.md) \| [`DivergeDirection`](../enums/GC.Spread.Sheets.CellTypes.DivergeDirection.md)

如果未设置值，则返回发散方向的类型；否则，返回对角线单元格类型。

___

### <a id="focus" name="focus"></a> focus

▸ **focus**(`editorContext`, `context?`): `void`

聚焦编辑器的 DOM 元素。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由 createEditorElement 方法创建的 DOM 元素。 |
| `context?` | `any` | 与单元格类型相关联的上下文。更多信息请参阅 “备注”。 |

#### Returns

`void`

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[focus](GC.Spread.Sheets.CellTypes.Text.md#focus)

___

### <a id="format" name="format"></a> format

▸ **format**(`value`, `format`, `formattedData?`, `context?`): `string`

使用指定格式将值格式化为字符串。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 要格式化的对象值。 |
| `format` | `string` \| [`GeneralFormatter`](GC.Spread.Formatter.GeneralFormatter.md) | 格式。 |
| `formattedData?` | [`FormattedData`](../interfaces/GC.Spread.Sheets.FormattedData.md) | 格式化后的数据。 |
| `context?` | `any` | 与单元格类型相关联的上下文。更多信息请参阅 “备注”。 |

#### Returns

`string`

返回格式化后的字符串。

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[format](GC.Spread.Sheets.CellTypes.Text.md#format)

___

### <a id="fromjson" name="fromjson"></a> fromJSON

▸ **fromJSON**(`settings`): `void`

从指定的 JSON 字符串加载对象状态。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `settings` | `any` | 反序列化得到的单元格类型数据。 |

#### Returns

`void`

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[fromJSON](GC.Spread.Sheets.CellTypes.Text.md#fromjson)

___

### <a id="getautofitheight" name="getautofitheight"></a> getAutoFitHeight

▸ **getAutoFitHeight**(`value`, `text`, `cellStyle`, `zoomFactor`, `context?`): `number`

获取可用于处理行自动调整的单元格高度。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 单元格的值。 |
| `text` | `string` | 单元格的文本。 |
| `cellStyle` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际值。 |
| `zoomFactor` | `number` | 当前工作表的缩放因子。 |
| `context?` | `any` | 与单元格类型相关联的上下文。更多信息请参阅 “备注”。 |

#### Returns

`number`

返回可用于处理行自动调整的单元格高度。

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[getAutoFitHeight](GC.Spread.Sheets.CellTypes.Text.md#getautofitheight)

___

### <a id="getautofitwidth" name="getautofitwidth"></a> getAutoFitWidth

▸ **getAutoFitWidth**(`value`, `text`, `cellStyle`, `zoomFactor`, `context?`): `number`

获取可用于处理列自动调整的单元格宽度。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 单元格的值。|
| `text` | `string` | 单元格的文本。 |
| `cellStyle` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际值。 |
| `zoomFactor` | `number` | 当前工作表的缩放因子。 |
| `context?` | `any` | 与单元格类型相关联的上下文。更多信息请参阅 “备注”。 |

#### Returns

`number`

返回可用于处理列自动调整的单元格宽度。

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[getAutoFitWidth](GC.Spread.Sheets.CellTypes.Text.md#getautofitwidth)

___

### <a id="geteditorvalue" name="geteditorvalue"></a> getEditorValue

▸ **getEditorValue**(`editorContext`, `context?`): `any`

获取编辑器的值。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由 createEditorElement 方法创建的 DOM 元素。 |
| `context?` | `any` | 与单元格类型相关联的上下文。更多信息请参阅 “备注”。 |

#### Returns

`any`

返回编辑器的值。

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[getEditorValue](GC.Spread.Sheets.CellTypes.Text.md#geteditorvalue)

___

### <a id="gethitinfo" name="gethitinfo"></a> getHitInfo

▸ **getHitInfo**(`x`, `y`, `cellStyle`, `cellRect`, `context?`): [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md)

获取单元格类型的命中信息。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | 指针当前位置相对于画布的 x 坐标。|
| `y` | `number` | 指针当前位置相对于画布的 y 坐标。 |
| `cellStyle` | [`Style`](GC.Spread.Sheets.Style.md) | 当前单元格的实际样式。 |
| `cellRect` | [`Rect`](GC.Spread.Sheets.Rect.md) | 当前单元格的布局信息。 |
| `context?` | `any` | 与单元格类型相关联的上下文。更多信息请参阅 “备注”。 |

#### Returns

[`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md)

返回一个对象，该对象包含 x、y、row、col、cellRect 和 sheetArea 参数，以及一个指示 isReservedLocation 的值。
如果命中测试位于单元格类型需要处理的特殊区域，则 isReservedLocation 为`true`；否则为`false`。

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[getHitInfo](GC.Spread.Sheets.CellTypes.Text.md#gethitinfo)

___

### <a id="iseditingvaluechanged" name="iseditingvaluechanged"></a> isEditingValueChanged

▸ **isEditingValueChanged**(`oldValue`, `newValue`, `context?`): `boolean`

编辑值是否已更改。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `oldValue` | `any` | 旧的编辑值。 |
| `newValue` | `any` | 新的编辑值。 |
| `context?` | `any` | 与单元格类型相关联的上下文。更多信息请参阅 “备注”。 |

#### Returns

`boolean`

如果 oldValue 等于 newValue，则为`true`；否则为`false`。

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[isEditingValueChanged](GC.Spread.Sheets.CellTypes.Text.md#iseditingvaluechanged)

___

### <a id="isimeaware" name="isimeaware"></a> isImeAware

▸ **isImeAware**(`context?`): `boolean`

此单元格类型是否支持输入法编辑器（IME）。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context?` | `any` | 与单元格类型相关联的上下文。更多信息请参阅 “备注”。 |

#### Returns

`boolean`

如果单元格类型支持 IME，则为`true`；否则为`false`。

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[isImeAware](GC.Spread.Sheets.CellTypes.Text.md#isimeaware)

___

### <a id="isreservedkey" name="isreservedkey"></a> isReservedKey

▸ **isReservedKey**(`e`, `context?`): `boolean`

单元格类型是否自行处理键盘事件。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `e` | `KeyboardEvent` | 键盘事件。 |
| `context?` | `any` | 与单元格类型相关联的上下文。更多信息请参阅 “备注”。 |

#### Returns

`boolean`

如果单元格类型自行处理键盘事件，则返回`true`；否则返回`false`。

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[isReservedKey](GC.Spread.Sheets.CellTypes.Text.md#isreservedkey)

___

### <a id="lineborder" name="lineborder"></a> lineBorder

▸ **lineBorder**(`value?`): [`LineBorder`](GC.Spread.Sheets.LineBorder.md) \| [`Diagonal`](GC.Spread.Sheets.CellTypes.Diagonal.md)

获取或设置对角线单元格类型的线条边框。

**`example`**
```
//This example gets the diverge direction type.
var cellType = new GC.Spread.Sheets.CellTypes.Diagonal();
activeSheet.getCell(2, 2).cellType(cellType);
alert(cellType.lineBorder());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`LineBorder`](GC.Spread.Sheets.LineBorder.md) | 线条边框的类型。 |

#### Returns

[`LineBorder`](GC.Spread.Sheets.LineBorder.md) \| [`Diagonal`](GC.Spread.Sheets.CellTypes.Diagonal.md)

如果未设置值，则返回线条边框的类型；否则，返回对角线单元格类型。

___

### <a id="paint" name="paint"></a> paint

▸ **paint**(`ctx`, `value`, `x`, `y`, `w`, `h`, `style`, `context?`): `void`

在画布上绘制一个单元格。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ctx` | `CanvasRenderingContext2D` | 画布的二维上下文。 |
| `value` | `any` | 单元格的值。 |
| `x` | `number` | 相对于画布的 x 坐标。 |
| `y` | `number` | 相对于画布的 y 坐标。 |
| `w` | `number` | 单元格的宽度。 |
| `h` | `number` | 单元格的高度。 |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际样式。 |
| `context?` | `any` | 与单元格类型相关联的上下文。更多信息请参阅 “备注”。 |

#### Returns

`void`

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[paint](GC.Spread.Sheets.CellTypes.Text.md#paint)

___

### <a id="paintcontent" name="paintcontent"></a> paintContent

▸ **paintContent**(`ctx`, `value`, `x`, `y`, `w`, `h`, `style`, `context?`): `void`

在画布上绘制单元格内容区域。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ctx` | `CanvasRenderingContext2D` | 画布的二维上下文。 |
| `value` | `any` | 单元格的值。 |
| `x` | `number` | 相对于画布的 x 坐标。 |
| `y` | `number` | 相对于画布的 y 坐标。 |
| `w` | `number` | 单元格内容区域的宽度。 |
| `h` | `number` | 单元格内容区域的高度。 |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际样式。 |
| `context?` | `any` | 与单元格类型相关联的上下文。更多信息请参阅 “备注”。 |

#### Returns

`void`

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[paintContent](GC.Spread.Sheets.CellTypes.Text.md#paintcontent)

___

### <a id="parse" name="parse"></a> parse

▸ **parse**(`text`, `formatStr`, `context?`): `any`

使用指定的格式字符串将文本解析为一个对象。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `text` | `string` | 要解析的文本字符串。 |
| `formatStr` | `string` | 解析格式字符串。 |
| `context?` | `any` | 与单元格类型相关联的上下文。更多信息请参阅 “备注”。 |

#### Returns

`any`

解析后的对象。

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[parse](GC.Spread.Sheets.CellTypes.Text.md#parse)

___

### <a id="processkeydown" name="processkeydown"></a> processKeyDown

▸ **processKeyDown**(`event`, `context?`): `boolean`

在显示模式下处理按键按下事件。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `event` | `KeyboardEvent` | 键盘事件。 |
| `context?` | `any` | 与单元格类型相关联的上下文。更多信息请参阅 “备注”。 |

#### Returns

`boolean`

如果处理成功，则返回`true`；否则返回`false`。

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[processKeyDown](GC.Spread.Sheets.CellTypes.Text.md#processkeydown)

___

### <a id="processkeyup" name="processkeyup"></a> processKeyUp

▸ **processKeyUp**(`event`, `context?`): `boolean`

在显示模式下处理按键松开事件。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `event` | `KeyboardEvent` | 键盘事件。 |
| `context?` | `any` | 与单元格类型相关联的上下文。更多信息请参阅 “备注”。 |

#### Returns

`boolean`

如果处理成功，则返回`true`；否则返回`false`。

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[processKeyUp](GC.Spread.Sheets.CellTypes.Text.md#processkeyup)

___

### <a id="processmousedown" name="processmousedown"></a> processMouseDown

▸ **processMouseDown**(`hitInfo`): `boolean`

在显示模式下处理鼠标按下事件。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitInfo` | [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md) | 由 getHitInfo 方法返回的命中测试信息。更多信息请参阅 “备注”。 |

#### Returns

`boolean`

如果处理成功，则返回`true`；否则返回`false`。

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[processMouseDown](GC.Spread.Sheets.CellTypes.Text.md#processmousedown)

___

### <a id="processmouseenter" name="processmouseenter"></a> processMouseEnter

▸ **processMouseEnter**(`hitInfo`): `boolean`

在显示模式下处理鼠标进入事件。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitInfo` | [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md) | 由 getHitInfo 方法返回的命中测试信息。更多信息请参阅 “备注”。 |

#### Returns

`boolean`

如果处理成功，则返回`true`；否则返回`false`。

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[processMouseEnter](GC.Spread.Sheets.CellTypes.Text.md#processmouseenter)

___

### <a id="processmouseleave" name="processmouseleave"></a> processMouseLeave

▸ **processMouseLeave**(`hitInfo`): `boolean`

在显示模式下处理鼠标离开事件。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitInfo` | [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md) | 由 getHitInfo 方法返回的命中测试信息。更多信息请参阅 “备注”。 |

#### Returns

`boolean`

如果处理成功，则返回`true`；否则返回`false`。

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[processMouseLeave](GC.Spread.Sheets.CellTypes.Text.md#processmouseleave)

___

### <a id="processmousemove" name="processmousemove"></a> processMouseMove

▸ **processMouseMove**(`hitInfo`): `boolean`

在显示模式下处理鼠标移动事件。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitInfo` | [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md) | 由 getHitInfo 方法返回的命中测试信息。更多信息请参阅 “备注”。 |

#### Returns

`boolean`

如果处理成功，则返回`true`；否则返回`false`。

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[processMouseMove](GC.Spread.Sheets.CellTypes.Text.md#processmousemove)

___

### <a id="processmouseup" name="processmouseup"></a> processMouseUp

▸ **processMouseUp**(`hitInfo`): `boolean`

在显示模式下处理鼠标松开事件。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitInfo` | [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md) | 由 getHitInfo 方法返回的命中测试信息。更多信息请参阅 “备注”。 |

#### Returns

`boolean`

如果处理成功，则返回`true`；否则返回`false`。

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[processMouseUp](GC.Spread.Sheets.CellTypes.Text.md#processmouseup)

___

### <a id="selectall" name="selectall"></a> selectAll

▸ **selectAll**(`editorContext`, `context?`): `void`

选中编辑器 DOM 元素中的所有文本。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由 createEditorElement 方法创建的 DOM 元素。 |
| `context?` | `any` | 与单元格类型相关联的上下文。更多信息请参阅 “备注”。 |

#### Returns

`void`

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[selectAll](GC.Spread.Sheets.CellTypes.Text.md#selectall)

___

### <a id="seteditorvalue" name="seteditorvalue"></a> setEditorValue

▸ **setEditorValue**(`editorContext`, `value`, `context?`): `void`

设置编辑器的值。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由 createEditorElement 方法创建的 DOM 元素。 |
| `value` | `any` | 从活动单元格返回的值。 |
| `context?` | `any` | 与单元格类型相关联的上下文。更多信息请参阅 “备注”。 |

#### Returns

`void`

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[setEditorValue](GC.Spread.Sheets.CellTypes.Text.md#seteditorvalue)

___

### <a id="tojson" name="tojson"></a> toJSON

▸ **toJSON**(): `any`

将对象状态保存为 JSON 字符串。

#### Returns

`any`

单元格类型数据。

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[toJSON](GC.Spread.Sheets.CellTypes.Text.md#tojson)

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
| `context?` | `any` | 与单元格类型相关联的上下文。更多信息请参阅 “备注”。 |

#### Returns

[`Rect`](GC.Spread.Sheets.Rect.md)

返回单元格包装元素的新大小，它应包含 “width” 和 “height” 两个属性。

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[updateEditor](GC.Spread.Sheets.CellTypes.Text.md#updateeditor)

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

[Text](GC.Spread.Sheets.CellTypes.Text.md).[updateEditorContainer](GC.Spread.Sheets.CellTypes.Text.md#updateeditorcontainer)

___

### <a id="updateimemode" name="updateimemode"></a> updateImeMode

▸ **updateImeMode**(`editorContext`, `imeMode`, `context?`): `void`

更新编辑器的输入法模式。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由 createEditorElement 方法创建的 DOM 元素。 |
| `imeMode` | [`ImeMode`](../enums/GC.Spread.Sheets.ImeMode.md) | 来自单元格实际样式的输入法模式。 |
| `context?` | `any` | 与单元格类型相关联的上下文。更多信息请参阅 “备注”。 |

#### Returns

`void`

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[updateImeMode](GC.Spread.Sheets.CellTypes.Text.md#updateimemode)
