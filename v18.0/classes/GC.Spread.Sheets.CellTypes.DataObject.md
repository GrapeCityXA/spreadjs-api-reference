# Class: DataObject

[Sheets](../modules/GC.Spread.Sheets.md).[CellTypes](../modules/GC.Spread.Sheets.CellTypes.md).DataObject

## Hierarchy

- [`Text`](GC.Spread.Sheets.CellTypes.Text.md)

  ↳ **`DataObject`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.CellTypes.DataObject.md#constructor)

### Properties

- [typeName](GC.Spread.Sheets.CellTypes.DataObject.md#typename)

### Methods

- [activateEditor](GC.Spread.Sheets.CellTypes.DataObject.md#activateeditor)
- [createEditorElement](GC.Spread.Sheets.CellTypes.DataObject.md#createeditorelement)
- [deactivateEditor](GC.Spread.Sheets.CellTypes.DataObject.md#deactivateeditor)
- [focus](GC.Spread.Sheets.CellTypes.DataObject.md#focus)
- [format](GC.Spread.Sheets.CellTypes.DataObject.md#format)
- [fromJSON](GC.Spread.Sheets.CellTypes.DataObject.md#fromjson)
- [getAutoFitHeight](GC.Spread.Sheets.CellTypes.DataObject.md#getautofitheight)
- [getAutoFitWidth](GC.Spread.Sheets.CellTypes.DataObject.md#getautofitwidth)
- [getEditorValue](GC.Spread.Sheets.CellTypes.DataObject.md#geteditorvalue)
- [getHitInfo](GC.Spread.Sheets.CellTypes.DataObject.md#gethitinfo)
- [isEditingValueChanged](GC.Spread.Sheets.CellTypes.DataObject.md#iseditingvaluechanged)
- [isImeAware](GC.Spread.Sheets.CellTypes.DataObject.md#isimeaware)
- [isReservedKey](GC.Spread.Sheets.CellTypes.DataObject.md#isreservedkey)
- [paint](GC.Spread.Sheets.CellTypes.DataObject.md#paint)
- [paintContent](GC.Spread.Sheets.CellTypes.DataObject.md#paintcontent)
- [parse](GC.Spread.Sheets.CellTypes.DataObject.md#parse)
- [processKeyDown](GC.Spread.Sheets.CellTypes.DataObject.md#processkeydown)
- [processKeyUp](GC.Spread.Sheets.CellTypes.DataObject.md#processkeyup)
- [processMouseDown](GC.Spread.Sheets.CellTypes.DataObject.md#processmousedown)
- [processMouseEnter](GC.Spread.Sheets.CellTypes.DataObject.md#processmouseenter)
- [processMouseLeave](GC.Spread.Sheets.CellTypes.DataObject.md#processmouseleave)
- [processMouseMove](GC.Spread.Sheets.CellTypes.DataObject.md#processmousemove)
- [processMouseUp](GC.Spread.Sheets.CellTypes.DataObject.md#processmouseup)
- [selectAll](GC.Spread.Sheets.CellTypes.DataObject.md#selectall)
- [setEditorValue](GC.Spread.Sheets.CellTypes.DataObject.md#seteditorvalue)
- [toJSON](GC.Spread.Sheets.CellTypes.DataObject.md#tojson)
- [updateEditor](GC.Spread.Sheets.CellTypes.DataObject.md#updateeditor)
- [updateEditorContainer](GC.Spread.Sheets.CellTypes.DataObject.md#updateeditorcontainer)
- [updateImeMode](GC.Spread.Sheets.CellTypes.DataObject.md#updateimemode)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new DataObject**()

Represents a data object cell type.

**`example`**
```
//set a DataObject celltype which uses WEBSERVICE function to provide data
sheet.setFormula(1, 1, '=FILTERJSON(WEBSERVICE("https://demodata.mescius.io/northwind/api/v1/Products/1"))');
var cellType1 = new GC.Spread.Sheets.CellTypes.DataObject('=@.productName & " " & @.unitPrice');
sheet.setCellType(1, 1, cellType1);
```

#### Overrides

[Text](GC.Spread.Sheets.CellTypes.Text.md).[constructor](GC.Spread.Sheets.CellTypes.Text.md#constructor)

## Properties

### <a id="typename" name="typename"></a> typeName

• **typeName**: `string`

支持序列化的类型名称字符串

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[typeName](GC.Spread.Sheets.CellTypes.Text.md#typename)

## Methods

### <a id="activateeditor" name="activateeditor"></a> activateEditor

▸ **activateEditor**(`editorContext`, `cellStyle`, `cellRect`, `context?`): `void`

激活编辑器，包括为编辑器设置属性或属性以及为编辑器绑定事件

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由createEditorElement方法创建的DOM元素 |
| `cellStyle` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际样式 |
| `cellRect` | [`Rect`](GC.Spread.Sheets.Rect.md) | 单元格的布局信息 |
| `context?` | `any` | 与单元格类型关联的上下文 |

#### Returns

`void`

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[activateEditor](GC.Spread.Sheets.CellTypes.Text.md#activateeditor)

___

### <a id="createeditorelement" name="createeditorelement"></a> createEditorElement

▸ **createEditorElement**(`context?`): `HTMLElement`

创建一个DOM元素，然后返回

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context?` | `any` | 与单元格类型关联的上下文 |

#### Returns

`HTMLElement`

创建一个DOM元素，然后返回

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[createEditorElement](GC.Spread.Sheets.CellTypes.Text.md#createeditorelement)

___

### <a id="deactivateeditor" name="deactivateeditor"></a> deactivateEditor

▸ **deactivateEditor**(`editorContext`, `context?`): `void`

停用编辑器，例如解除绑定编辑器事件

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由createEditorElement方法创建的DOM元素 |
| `context?` | `any` | 与单元格类型关联的上下文 |

#### Returns

`void`

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[deactivateEditor](GC.Spread.Sheets.CellTypes.Text.md#deactivateeditor)

___

### <a id="focus" name="focus"></a> focus

▸ **focus**(`editorContext`, `context?`): `void`

关注编辑器DOM元素

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由createEditorElement方法创建的DOM元素 |
| `context?` | `any` | 与单元格类型关联的上下文 |

#### Returns

`void`

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[focus](GC.Spread.Sheets.CellTypes.Text.md#focus)

___

### <a id="format" name="format"></a> format

▸ **format**(`value`, `format`, `formattedData?`, `context?`): `string`

将具有指定格式的值格式化为字符串

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 要格式化的对象值 |
| `format` | `string` \| [`GeneralFormatter`](GC.Spread.Formatter.GeneralFormatter.md) | 格式化 |
| `formattedData?` | [`FormattedData`](../interfaces/GC.Spread.Sheets.FormattedData.md) | 格式化的数据 |
| `context?` | `any` | 与单元格类型关联的上下文 |

#### Returns

`string`

返回格式化的字符串

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[format](GC.Spread.Sheets.CellTypes.Text.md#format)

___

### <a id="fromjson" name="fromjson"></a> fromJSON

▸ **fromJSON**(`settings`): `void`

从指定的JSON字符串加载对象状态

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `settings` | `any` | 反序列化的单元格类型数据 |

#### Returns

`void`

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[fromJSON](GC.Spread.Sheets.CellTypes.Text.md#fromjson)

___

### <a id="getautofitheight" name="getautofitheight"></a> getAutoFitHeight

▸ **getAutoFitHeight**(`value`, `text`, `cellStyle`, `zoomFactor`, `context?`): `number`

获取单元格的高度，该高度可用于处理该行的自适应

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 单元格的值 |
| `text` | `string` | 单元格的文本 |
| `cellStyle` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际值 |
| `zoomFactor` | `number` | 当前工作表的缩放系数 |
| `context?` | `any` | 与单元格类型关联的上下文 |

#### Returns

`number`

返回单元格的高度，该高度可用于处理行的自适应

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[getAutoFitHeight](GC.Spread.Sheets.CellTypes.Text.md#getautofitheight)

___

### <a id="getautofitwidth" name="getautofitwidth"></a> getAutoFitWidth

▸ **getAutoFitWidth**(`value`, `text`, `cellStyle`, `zoomFactor`, `context?`): `number`

获取可用于处理列的自适应的单元格宽度

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 单元格的值 |
| `text` | `string` | 单元格的文本 |
| `cellStyle` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际值 |
| `zoomFactor` | `number` | 当前工作表的缩放系数 |
| `context?` | `any` | 与单元格类型关联的上下文 |

#### Returns

`number`

返回单元格的高度，该高度可用于处理列的自适应

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[getAutoFitWidth](GC.Spread.Sheets.CellTypes.Text.md#getautofitwidth)

___

### <a id="geteditorvalue" name="geteditorvalue"></a> getEditorValue

▸ **getEditorValue**(`editorContext`, `context?`): `any`

获取编辑器的值

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由createEditorElement方法创建的DOM元素 |
| `context?` | `any` | 与单元格类型关联的上下文 |

#### Returns

`any`

返回编辑器的值

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[getEditorValue](GC.Spread.Sheets.CellTypes.Text.md#geteditorvalue)

___

### <a id="gethitinfo" name="gethitinfo"></a> getHitInfo

▸ **getHitInfo**(`x`, `y`, `cellStyle`, `cellRect`, `context?`): [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md)

获取单元格类型的匹配信息

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | 指针相对于画布的当前位置的<i> x </i>坐标 |
| `y` | `number` | 指针相对于画布的当前位置的<i> y </i>坐标 |
| `cellStyle` | [`Style`](GC.Spread.Sheets.Style.md) | 当前单元格的实际样式 |
| `cellRect` | [`Rect`](GC.Spread.Sheets.Rect.md) | 当前单元格的布局信息 |
| `context?` | `any` | 与单元格类型关联的上下文 |

#### Returns

[`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md)

返回包含<i> x </i>,<i> y </i>,<i> row </i>,<i> col </i>,<i> cellRect </i>的对象 ,以及<i> sheetArea </i>参数，以及一个表示<i> isReservedLocation </i>的值
如果命中测试位于单元格类型需要处理的特殊区域中，则<i> isReservedLocation </i>为` true ` 否则为` false `

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[getHitInfo](GC.Spread.Sheets.CellTypes.Text.md#gethitinfo)

___

### <a id="iseditingvaluechanged" name="iseditingvaluechanged"></a> isEditingValueChanged

▸ **isEditingValueChanged**(`oldValue`, `newValue`, `context?`): `boolean`

编辑值是否已更改

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `oldValue` | `any` | 旧的编辑值 |
| `newValue` | `any` | 新的编辑值 |
| `context?` | `any` | 与单元格类型关联的上下文 |

#### Returns

`boolean`

如果oldValue等于newValue,为`true`;否则为`false`

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[isEditingValueChanged](GC.Spread.Sheets.CellTypes.Text.md#iseditingvaluechanged)

___

### <a id="isimeaware" name="isimeaware"></a> isImeAware

▸ **isImeAware**(`context?`): `boolean`

此单元格类型是否存在IME

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context?` | `any` | 与单元格类型关联的上下文 |

#### Returns

`boolean`

如果单元格类型存在IME,为`true`;否则为`false`

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[isImeAware](GC.Spread.Sheets.CellTypes.Text.md#isimeaware)

___

### <a id="isreservedkey" name="isreservedkey"></a> isReservedKey

▸ **isReservedKey**(`e`, `context?`): `boolean`

单元格类型是否处理键盘事件本身

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `e` | `KeyboardEvent` | 键盘事件 |
| `context?` | `any` | 与单元格类型关联的上下文 |

#### Returns

`boolean`

如果单元格类型处理键盘事件本身，则返回`true`;否则，返回false 否则为`false`

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[isReservedKey](GC.Spread.Sheets.CellTypes.Text.md#isreservedkey)

___

### <a id="paint" name="paint"></a> paint

▸ **paint**(`ctx`, `value`, `x`, `y`, `w`, `h`, `style`, `context?`): `void`

在画布上绘制一个单元格

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ctx` | `CanvasRenderingContext2D` | 画布的二维上下文 |
| `value` | `any` | 单元格的值 |
| `x` | `number` | <i> x </i>相对于画布的坐标 |
| `y` | `number` | 相对于画布的<i> y </i>坐标 |
| `w` | `number` | 单元格的宽度 |
| `h` | `number` | 单元格的高度 |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际样式 |
| `context?` | `any` | 与单元格类型关联的上下文 |

#### Returns

`void`

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[paint](GC.Spread.Sheets.CellTypes.Text.md#paint)

___

### <a id="paintcontent" name="paintcontent"></a> paintContent

▸ **paintContent**(`ctx`, `value`, `x`, `y`, `w`, `h`, `style`, `context?`): `void`

在画布上绘制单元格内容区域

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ctx` | `CanvasRenderingContext2D` | 画布的二维上下文 |
| `value` | `any` | 单元格的值 |
| `x` | `number` | <i> x </i>相对于画布的坐标 |
| `y` | `number` | 相对于画布的<i> y </i>坐标 |
| `w` | `number` | 单元格内容区域的宽度 |
| `h` | `number` | 单元格内容区域的高度 |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际样式 |
| `context?` | `any` | 与单元格类型关联的上下文 |

#### Returns

`void`

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[paintContent](GC.Spread.Sheets.CellTypes.Text.md#paintcontent)

___

### <a id="parse" name="parse"></a> parse

▸ **parse**(`text`, `formatStr`, `context?`): `any`

将具有指定格式字符串的文本解析为对象

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `text` | `string` | 解析文本字符串 |
| `formatStr` | `string` | 解析格式字符串 |
| `context?` | `any` | 与单元格类型关联的上下文 |

#### Returns

`any`

解析对象

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[parse](GC.Spread.Sheets.CellTypes.Text.md#parse)

___

### <a id="processkeydown" name="processkeydown"></a> processKeyDown

▸ **processKeyDown**(`event`, `context?`): `boolean`

在显示模式下处理按键

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `event` | `KeyboardEvent` | 键盘事件 |
| `context?` | `any` | 与单元格类型关联的上下文 |

#### Returns

`boolean`

如果过程成功，则返回` true `;否则为` false `

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[processKeyDown](GC.Spread.Sheets.CellTypes.Text.md#processkeydown)

___

### <a id="processkeyup" name="processkeyup"></a> processKeyUp

▸ **processKeyUp**(`event`, `context?`): `boolean`

在显示模式下处理按键

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `event` | `KeyboardEvent` | 键盘事件 |
| `context?` | `any` | 与单元格类型关联的上下文 |

#### Returns

`boolean`

如果过程成功，则返回` true `;否则为` false `

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[processKeyUp](GC.Spread.Sheets.CellTypes.Text.md#processkeyup)

___

### <a id="processmousedown" name="processmousedown"></a> processMouseDown

▸ **processMouseDown**(`hitInfo`): `boolean`

在显示模式下向下处理鼠标

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitInfo` | [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md) | getHitInfo方法返回的命中测试信息 |

#### Returns

`boolean`

如果过程成功，则返回` true `;否则为` false `

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[processMouseDown](GC.Spread.Sheets.CellTypes.Text.md#processmousedown)

___

### <a id="processmouseenter" name="processmouseenter"></a> processMouseEnter

▸ **processMouseEnter**(`hitInfo`): `boolean`

在显示模式下处理鼠标的输入

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitInfo` | [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md) | getHitInfo方法返回的命中测试信息 |

#### Returns

`boolean`

如果过程成功，则返回` true `;否则为` false `

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[processMouseEnter](GC.Spread.Sheets.CellTypes.Text.md#processmouseenter)

___

### <a id="processmouseleave" name="processmouseleave"></a> processMouseLeave

▸ **processMouseLeave**(`hitInfo`): `boolean`

在显示模式下处理鼠标离开

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitInfo` | [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md) | getHitInfo方法返回的命中测试信息 |

#### Returns

`boolean`

如果过程成功，则返回` true `;否则为` false `

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[processMouseLeave](GC.Spread.Sheets.CellTypes.Text.md#processmouseleave)

___

### <a id="processmousemove" name="processmousemove"></a> processMouseMove

▸ **processMouseMove**(`hitInfo`): `boolean`

在显示模式下处理鼠标移动

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitInfo` | [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md) | getHitInfo方法返回的命中测试信息 |

#### Returns

`boolean`

如果过程成功，则返回` true `;否则为` false `

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[processMouseMove](GC.Spread.Sheets.CellTypes.Text.md#processmousemove)

___

### <a id="processmouseup" name="processmouseup"></a> processMouseUp

▸ **processMouseUp**(`hitInfo`): `boolean`

在显示模式下处理鼠标抬起

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitInfo` | [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md) | getHitInfo方法返回的命中测试信息 |

#### Returns

`boolean`

如果过程成功，则返回` true `;否则为` false `

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[processMouseUp](GC.Spread.Sheets.CellTypes.Text.md#processmouseup)

___

### <a id="selectall" name="selectall"></a> selectAll

▸ **selectAll**(`editorContext`, `context?`): `void`

选择编辑器DOM元素中的所有文本

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由createEditorElement方法创建的DOM元素 |
| `context?` | `any` | 与单元格类型关联的上下文 |

#### Returns

`void`

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[selectAll](GC.Spread.Sheets.CellTypes.Text.md#selectall)

___

### <a id="seteditorvalue" name="seteditorvalue"></a> setEditorValue

▸ **setEditorValue**(`editorContext`, `value`, `context?`): `void`

设置编辑器的值

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由createEditorElement方法创建的DOM元素 |
| `value` | `any` | 从活动单元格返回的值 |
| `context?` | `any` | 与单元格类型关联的上下文 |

#### Returns

`void`

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[setEditorValue](GC.Spread.Sheets.CellTypes.Text.md#seteditorvalue)

___

### <a id="tojson" name="tojson"></a> toJSON

▸ **toJSON**(): `any`

将对象状态保存为JSON字符串

#### Returns

`any`

单元格类型数据

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[toJSON](GC.Spread.Sheets.CellTypes.Text.md#tojson)

___

### <a id="updateeditor" name="updateeditor"></a> updateEditor

▸ **updateEditor**(`editorContext`, `cellStyle`, `cellRect`, `context?`): [`Rect`](GC.Spread.Sheets.Rect.md)

更新编辑器的大小

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由createEditorElement方法创建的DOM元素 |
| `cellStyle` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际样式 |
| `cellRect` | [`Rect`](GC.Spread.Sheets.Rect.md) | 单元格的布局信息 |
| `context?` | `any` | 与单元格类型关联的上下文 |

#### Returns

[`Rect`](GC.Spread.Sheets.Rect.md)

返回单元格包装器元素的新大小，它应包含两个属性"width"和 "height"

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[updateEditor](GC.Spread.Sheets.CellTypes.Text.md#updateeditor)

___

### <a id="updateeditorcontainer" name="updateeditorcontainer"></a> updateEditorContainer

▸ **updateEditorContainer**(`editorContext`, `editorBounds`, `cellStyle`): `void`

更新单元格wrapper元素的大小

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由createEditorElement方法创建的DOM元素 |
| `editorBounds` | [`Rect`](GC.Spread.Sheets.Rect.md) | 单元格wrapper元素的新大小 |
| `cellStyle` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际样式 |

#### Returns

`void`

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[updateEditorContainer](GC.Spread.Sheets.CellTypes.Text.md#updateeditorcontainer)

___

### <a id="updateimemode" name="updateimemode"></a> updateImeMode

▸ **updateImeMode**(`editorContext`, `imeMode`, `context?`): `void`

更新编辑器的ime模式

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由createEditorElement方法创建的DOM元素 |
| `imeMode` | [`ImeMode`](../enums/GC.Spread.Sheets.ImeMode.md) | 单元格实际样式中的ime模式 |
| `context?` | `any` | 与单元格类型关联的上下文 |

#### Returns

`void`

#### Inherited from

[Text](GC.Spread.Sheets.CellTypes.Text.md).[updateImeMode](GC.Spread.Sheets.CellTypes.Text.md#updateimemode)
