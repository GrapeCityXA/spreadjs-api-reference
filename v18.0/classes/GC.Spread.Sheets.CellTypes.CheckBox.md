# Class: CheckBox

[Sheets](../modules/GC.Spread.Sheets.md).[CellTypes](../modules/GC.Spread.Sheets.CellTypes.md).CheckBox

## Hierarchy

- [`Base`](GC.Spread.Sheets.CellTypes.Base.md)

  ↳ **`CheckBox`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.CellTypes.CheckBox.md#constructor)

### Properties

- [typeName](GC.Spread.Sheets.CellTypes.CheckBox.md#typename)

### Methods

- [activateEditor](GC.Spread.Sheets.CellTypes.CheckBox.md#activateeditor)
- [boxSize](GC.Spread.Sheets.CellTypes.CheckBox.md#boxsize)
- [caption](GC.Spread.Sheets.CellTypes.CheckBox.md#caption)
- [createEditorElement](GC.Spread.Sheets.CellTypes.CheckBox.md#createeditorelement)
- [deactivateEditor](GC.Spread.Sheets.CellTypes.CheckBox.md#deactivateeditor)
- [focus](GC.Spread.Sheets.CellTypes.CheckBox.md#focus)
- [format](GC.Spread.Sheets.CellTypes.CheckBox.md#format)
- [fromJSON](GC.Spread.Sheets.CellTypes.CheckBox.md#fromjson)
- [getAutoFitHeight](GC.Spread.Sheets.CellTypes.CheckBox.md#getautofitheight)
- [getAutoFitWidth](GC.Spread.Sheets.CellTypes.CheckBox.md#getautofitwidth)
- [getEditorValue](GC.Spread.Sheets.CellTypes.CheckBox.md#geteditorvalue)
- [getHitInfo](GC.Spread.Sheets.CellTypes.CheckBox.md#gethitinfo)
- [isEditingValueChanged](GC.Spread.Sheets.CellTypes.CheckBox.md#iseditingvaluechanged)
- [isImeAware](GC.Spread.Sheets.CellTypes.CheckBox.md#isimeaware)
- [isReservedKey](GC.Spread.Sheets.CellTypes.CheckBox.md#isreservedkey)
- [isThreeState](GC.Spread.Sheets.CellTypes.CheckBox.md#isthreestate)
- [paint](GC.Spread.Sheets.CellTypes.CheckBox.md#paint)
- [paintContent](GC.Spread.Sheets.CellTypes.CheckBox.md#paintcontent)
- [parse](GC.Spread.Sheets.CellTypes.CheckBox.md#parse)
- [processKeyDown](GC.Spread.Sheets.CellTypes.CheckBox.md#processkeydown)
- [processKeyUp](GC.Spread.Sheets.CellTypes.CheckBox.md#processkeyup)
- [processMouseDown](GC.Spread.Sheets.CellTypes.CheckBox.md#processmousedown)
- [processMouseEnter](GC.Spread.Sheets.CellTypes.CheckBox.md#processmouseenter)
- [processMouseLeave](GC.Spread.Sheets.CellTypes.CheckBox.md#processmouseleave)
- [processMouseMove](GC.Spread.Sheets.CellTypes.CheckBox.md#processmousemove)
- [processMouseUp](GC.Spread.Sheets.CellTypes.CheckBox.md#processmouseup)
- [selectAll](GC.Spread.Sheets.CellTypes.CheckBox.md#selectall)
- [setEditorValue](GC.Spread.Sheets.CellTypes.CheckBox.md#seteditorvalue)
- [textAlign](GC.Spread.Sheets.CellTypes.CheckBox.md#textalign)
- [textFalse](GC.Spread.Sheets.CellTypes.CheckBox.md#textfalse)
- [textIndeterminate](GC.Spread.Sheets.CellTypes.CheckBox.md#textindeterminate)
- [textTrue](GC.Spread.Sheets.CellTypes.CheckBox.md#texttrue)
- [toJSON](GC.Spread.Sheets.CellTypes.CheckBox.md#tojson)
- [updateEditor](GC.Spread.Sheets.CellTypes.CheckBox.md#updateeditor)
- [updateEditorContainer](GC.Spread.Sheets.CellTypes.CheckBox.md#updateeditorcontainer)
- [updateImeMode](GC.Spread.Sheets.CellTypes.CheckBox.md#updateimemode)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new CheckBox**()

一个复选框单元格

**`代码示例`**
``` javascript
//本示例创建一个复选框单元格
var cellType1 = new GC.Spread.Sheets.CellTypes.CheckBox();
cellType1.caption("caption");
cellType1.textTrue("true");
cellType1.textFalse("false");
cellType1.textIndeterminate("indeterminate");
cellType1.textAlign(GC.Spread.Sheets.CellTypes.CheckBoxTextAlign.bottom);
cellType1.isThreeState(true);
cellType1.boxSize(20);
activeSheet.getCell(1, 1).cellType(cellType1);
```

#### Overrides

[Base](GC.Spread.Sheets.CellTypes.Base.md).[constructor](GC.Spread.Sheets.CellTypes.Base.md#constructor)

## Properties

### <a id="typename" name="typename"></a> typeName

• **typeName**: `string`

支持序列化的类型名称字符串

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[typeName](GC.Spread.Sheets.CellTypes.Base.md#typename)

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

[Base](GC.Spread.Sheets.CellTypes.Base.md).[activateEditor](GC.Spread.Sheets.CellTypes.Base.md#activateeditor)

___

### <a id="boxsize" name="boxsize"></a> boxSize

▸ **boxSize**(`value?`): `any`

获取或设置复选框大小的值

**`example`**
```
// This example creates a check box cell.
var cellType1 = new GC.Spread.Sheets.CellTypes.CheckBox();
cellType1.caption("caption");
cellType1.textTrue("true");
cellType1.textFalse("false");
cellType1.textIndeterminate("indeterminate");
cellType1.textAlign(GC.Spread.Sheets.CellTypes.CheckBoxTextAlign.bottom);
cellType1.isThreeState(true);
cellType1.boxSize(20);
activeSheet.getCell(1, 1).cellType(cellType1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` \| `number` | 复选框的大小。此值支持数字和“auto” |

#### Returns

`any`

如果未设置值，返回复选框的大小

___

### <a id="caption" name="caption"></a> caption

▸ **caption**(`value?`): `any`

获取或设置单元格类型的标题

**`example`**
```
//This example creates a check box cell.
var cellType1 = new GC.Spread.Sheets.CellTypes.CheckBox();
cellType1.caption("caption");
cellType1.textTrue("true");
cellType1.textFalse("false");
cellType1.textIndeterminate("indeterminate");
cellType1.textAlign(GC.Spread.Sheets.CellTypes.CheckBoxTextAlign.bottom);
cellType1.isThreeState(true);
cellType1.boxSize(20);
activeSheet.getCell(1, 1).cellType(cellType1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 单元格类型的标题 |

#### Returns

`any`

如果未设置值，返回标题；否则，返回复选框单元类型

___

### <a id="createeditorelement" name="createeditorelement"></a> createEditorElement

▸ **createEditorElement**(`context?`): `HTMLElement`

创建一个DOM元素然后返回它

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context?` | `any` | 与单元格类型相关的上下文 |

#### Returns

`HTMLElement`

DOM 容器

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[createEditorElement](GC.Spread.Sheets.CellTypes.Base.md#createeditorelement)

___

### <a id="deactivateeditor" name="deactivateeditor"></a> deactivateEditor

▸ **deactivateEditor**(`editorContext`, `context?`): `void`

停用编辑器，例如编辑器的事件解绑

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由CreateEdoditorelement方法创建的DOM元素 |
| `context?` | `any` | 与单元格类型相关的上下文 |

#### Returns

`void`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[deactivateEditor](GC.Spread.Sheets.CellTypes.Base.md#deactivateeditor)

___

### <a id="focus" name="focus"></a> focus

▸ **focus**(`editorContext`, `context?`): `void`

聚焦编辑器 DOM 元素

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由CreateEdoditorelement方法创建的DOM元素 |
| `context?` | `any` | 与单元格类型相关的上下文 |

#### Returns

`void`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[focus](GC.Spread.Sheets.CellTypes.Base.md#focus)

___

### <a id="format" name="format"></a> format

▸ **format**(`value`, `format`, `formattedData?`, `context?`): `string`

格式为带有指定格式的值为字符串

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | The object value to format. |
| `format` | `string` \| [`GeneralFormatter`](GC.Spread.Formatter.GeneralFormatter.md) | 格式 |
| `formattedData?` | [`FormattedData`](../interfaces/GC.Spread.Sheets.FormattedData.md) | 待格式化的数据 |
| `context?` | `any` | 与单元格类型相关的上下文 |

#### Returns

`string`

格式化后的字符串

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[format](GC.Spread.Sheets.CellTypes.Base.md#format)

___

### <a id="fromjson" name="fromjson"></a> fromJSON

▸ **fromJSON**(`settings`): `void`

从指定的 JSON 字符串加载对象状态

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `settings` | `any` | 反序列化后的设置 |

#### Returns

`void`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[fromJSON](GC.Spread.Sheets.CellTypes.Base.md#fromjson)

___

### <a id="getautofitheight" name="getautofitheight"></a> getAutoFitHeight

▸ **getAutoFitHeight**(`value`, `text`, `cellStyle`, `zoomFactor`, `context?`): `number`

获取可用于处理行的自动高度

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 值 |
| `text` | `string` | 文本 |
| `cellStyle` | [`Style`](GC.Spread.Sheets.Style.md) | 实际值 |
| `zoomFactor` | `number` | 当前工作表缩放比例 |
| `context?` | `any` | 与单元格类型相关的上下文 |

#### Returns

`number`

处理行的自动高度

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[getAutoFitHeight](GC.Spread.Sheets.CellTypes.Base.md#getautofitheight)

___

### <a id="getautofitwidth" name="getautofitwidth"></a> getAutoFitWidth

▸ **getAutoFitWidth**(`value`, `text`, `cellStyle`, `zoomFactor`, `context?`): `number`

获取可用于处理列的自动宽度

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 值 |
| `text` | `string` | 文本 |
| `cellStyle` | [`Style`](GC.Spread.Sheets.Style.md) | 实际值 |
| `zoomFactor` | `number` | 当前工作表缩放比例 |
| `context?` | `any` | 与单元格类型相关的上下文 |

#### Returns

`number`

处理列的自动宽度

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[getAutoFitWidth](GC.Spread.Sheets.CellTypes.Base.md#getautofitwidth)

___

### <a id="geteditorvalue" name="geteditorvalue"></a> getEditorValue

▸ **getEditorValue**(`editorContext`, `context?`): `any`

返回编辑器的值

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由CreateEdoditorelement方法创建的DOM元素 |
| `context?` | `any` | 与单元格类型相关的上下文 |

#### Returns

`any`

编辑器的值

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[getEditorValue](GC.Spread.Sheets.CellTypes.Base.md#geteditorvalue)

___

### <a id="gethitinfo" name="gethitinfo"></a> getHitInfo

▸ **getHitInfo**(`x`, `y`, `cellStyle`, `cellRect`, `context?`): [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md)

获取单元格类型的 HitTest 信息

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | <i>x</i>-指针相对于画布的当前位置的坐标 |
| `y` | `number` | <i>y</i>-指针相对于画布的当前位置的坐标 |
| `cellStyle` | [`Style`](GC.Spread.Sheets.Style.md) | 当前单元格实际样式 |
| `cellRect` | [`Rect`](GC.Spread.Sheets.Rect.md) | 当前单元格布局 |
| `context?` | `any` | 与单元格类型相关的上下文 |

#### Returns

[`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md)

返回一个包含以下参数的对象：`x`、`y`、`row`、`col`、`cellRect` 和 `sheetArea`，以及指示 `isReservedLocation` 的值
如果击中测试在单元格类型需要处理的特殊区域内，则 `isReservedLocation` 为 `true`；否则为 `false`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[getHitInfo](GC.Spread.Sheets.CellTypes.Base.md#gethitinfo)

___

### <a id="iseditingvaluechanged" name="iseditingvaluechanged"></a> isEditingValueChanged

▸ **isEditingValueChanged**(`oldValue`, `newValue`, `context?`): `boolean`

编辑值是否已更改

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `oldValue` | `any` | 旧值 |
| `newValue` | `any` | 新值 |
| `context?` | `any` | 与单元格类型相关的上下文 |

#### Returns

`boolean`

`true` 如果 oldvalue 等于 newValue；否则，`false`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[isEditingValueChanged](GC.Spread.Sheets.CellTypes.Base.md#iseditingvaluechanged)

___

### <a id="isimeaware" name="isimeaware"></a> isImeAware

▸ **isImeAware**(`context?`): `boolean`

该单元格类型是否响应 IME

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context?` | `any` | 与单元格类型相关的上下文 |

#### Returns

`boolean`

`true` 如果单元格类型响应 IME；否则，`false`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[isImeAware](GC.Spread.Sheets.CellTypes.Base.md#isimeaware)

___

### <a id="isreservedkey" name="isreservedkey"></a> isReservedKey

▸ **isReservedKey**(`e`, `context?`): `boolean`

单元类型是否处理键盘事件本身

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `e` | `KeyboardEvent` | 键盘事件 |
| `context?` | `any` | 与单元格类型相关的上下文 |

#### Returns

`boolean`

如果单元格类型处理键盘事件本身，则返回`true`；否则，`false`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[isReservedKey](GC.Spread.Sheets.CellTypes.Base.md#isreservedkey)

___

### <a id="isthreestate" name="isthreestate"></a> isThreeState

▸ **isThreeState**(`value?`): `any`

获取或设置一个指示复选框是否支持三个状态的值

**`example`**
```
//This example creates a check box cell.
var cellType1 = new GC.Spread.Sheets.CellTypes.CheckBox();
cellType1.caption("caption");
cellType1.textTrue("true");
cellType1.textFalse("false");
cellType1.textIndeterminate("indeterminate");
cellType1.textAlign(GC.Spread.Sheets.CellTypes.CheckBoxTextAlign.bottom);
cellType1.isThreeState(true);
cellType1.boxSize(20);
activeSheet.getCell(1, 1).cellType(cellType1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 复选框是否支持三个状态 |

#### Returns

`any`

如果未设置值，则返回复选框是否支持三个状态；否则，返回复选框单元类型

___

### <a id="paint" name="paint"></a> paint

▸ **paint**(`ctx`, `value`, `x`, `y`, `w`, `h`, `style`, `context?`): `void`

在画布上绘制单元格

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ctx` | `CanvasRenderingContext2D` | 画布上下文 |
| `value` | `any` | 单元格值 |
| `x` | `number` | <i>x</i>-相对画布的坐标 |
| `y` | `number` | <i>y</i>-相对画布的坐标 |
| `w` | `number` | 宽度 |
| `h` | `number` | 高度 |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 实际样式 |
| `context?` | `any` | 与单元格类型相关的上下文 |

#### Returns

`void`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[paint](GC.Spread.Sheets.CellTypes.Base.md#paint)

___

### <a id="paintcontent" name="paintcontent"></a> paintContent

▸ **paintContent**(`ctx`, `value`, `x`, `y`, `w`, `h`, `style`, `context?`): `void`

在画布上绘制单元格内容

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ctx` | `CanvasRenderingContext2D` | 画布上下文 |
| `value` | `any` | 单元格值 |
| `x` | `number` | <i>x</i>-相对画布的坐标 |
| `y` | `number` | <i>y</i>-相对画布的坐标 |
| `w` | `number` | 宽度 |
| `h` | `number` | 高度 |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 实际样式 |
| `context?` | `any` | 与单元格类型相关的上下文 |

#### Returns

`void`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[paintContent](GC.Spread.Sheets.CellTypes.Base.md#paintcontent)

___

### <a id="parse" name="parse"></a> parse

▸ **parse**(`text`, `formatStr`, `context?`): `any`

根据指定的字符串格式化

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `text` | `string` | 解析字符串 |
| `formatStr` | `string` | 格式字符串 |
| `context?` | `any` | 与单元格类型相关的上下文 |

#### Returns

`any`

格式化后的对象

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[parse](GC.Spread.Sheets.CellTypes.Base.md#parse)

___

### <a id="processkeydown" name="processkeydown"></a> processKeyDown

▸ **processKeyDown**(`event`, `context?`): `boolean`

绘制模式下处理 KeyDown 事件

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `event` | `KeyboardEvent` | 键盘事件 |
| `context?` | `any` | 与单元格类型相关的上下文 |

#### Returns

`boolean`

如果该过程成功，则返回`true`；否则，`false`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[processKeyDown](GC.Spread.Sheets.CellTypes.Base.md#processkeydown)

___

### <a id="processkeyup" name="processkeyup"></a> processKeyUp

▸ **processKeyUp**(`event`, `context?`): `boolean`

绘制模式下处理 KeyUp 事件

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `event` | `KeyboardEvent` | 键盘事件 |
| `context?` | `any` | 与单元格类型相关的上下文 |

#### Returns

`boolean`

如果该过程成功，则返回`true`；否则，`false`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[processKeyUp](GC.Spread.Sheets.CellTypes.Base.md#processkeyup)

___

### <a id="processmousedown" name="processmousedown"></a> processMouseDown

▸ **processMouseDown**(`hitInfo`): `boolean`

绘制模式下处理 MouseDown 事件

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitInfo` | [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md) |  返回 HitTest 信息 |

#### Returns

`boolean`

如果该过程成功，则返回`true`；否则，`false`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[processMouseDown](GC.Spread.Sheets.CellTypes.Base.md#processmousedown)

___

### <a id="processmouseenter" name="processmouseenter"></a> processMouseEnter

▸ **processMouseEnter**(`hitInfo`): `boolean`

绘制模式下处理 MouseEnter 事件

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitInfo` | [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md) | 返回 HitTest 信息 |

#### Returns

`boolean`

如果该过程成功，则返回`true`；否则，`false`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[processMouseEnter](GC.Spread.Sheets.CellTypes.Base.md#processmouseenter)

___

### <a id="processmouseleave" name="processmouseleave"></a> processMouseLeave

▸ **processMouseLeave**(`hitInfo`): `boolean`

绘制模式下处理 MouseLeave 事件

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitInfo` | [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md) | 返回 HitTest 信息 |

#### Returns

`boolean`

如果该过程成功，则返回`true`；否则，`false`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[processMouseLeave](GC.Spread.Sheets.CellTypes.Base.md#processmouseleave)

___

### <a id="processmousemove" name="processmousemove"></a> processMouseMove

▸ **processMouseMove**(`hitInfo`): `boolean`

绘制模式下处理 MouseMove 事件

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitInfo` | [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md) | 返回 HitTest 信息 |

#### Returns

`boolean`

如果该过程成功，则返回`true`；否则，`false`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[processMouseMove](GC.Spread.Sheets.CellTypes.Base.md#processmousemove)

___

### <a id="processmouseup" name="processmouseup"></a> processMouseUp

▸ **processMouseUp**(`hitInfo`): `boolean`

绘制模式下处理 MouseUp 事件

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitInfo` | [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md) | 返回 HitTest 信息 |

#### Returns

`boolean`

如果该过程成功，则返回`true`；否则，`false`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[processMouseUp](GC.Spread.Sheets.CellTypes.Base.md#processmouseup)

___

### <a id="selectall" name="selectall"></a> selectAll

▸ **selectAll**(`editorContext`, `context?`): `void`

选择编辑器DOM元素中的所有文本

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由CreateEdoditorelement方法创建的DOM元素 |
| `context?` | `any` | 与单元格类型相关的上下文 |

#### Returns

`void`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[selectAll](GC.Spread.Sheets.CellTypes.Base.md#selectall)

___

### <a id="seteditorvalue" name="seteditorvalue"></a> setEditorValue

▸ **setEditorValue**(`editorContext`, `value`, `context?`): `void`

设置编辑器值

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由CreateEdoditorelement方法创建的DOM元素 |
| `value` | `any` | 活动单元格的值 |
| `context?` | `any` | 与单元格类型相关的上下文 |

#### Returns

`void`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[setEditorValue](GC.Spread.Sheets.CellTypes.Base.md#seteditorvalue)

___

### <a id="textalign" name="textalign"></a> textAlign

▸ **textAlign**(`value?`): `any`

获取或设置与复选框相对于复选框的文本对齐

**`example`**
```
//This example creates a check box cell.
var cellType1 = new GC.Spread.Sheets.CellTypes.CheckBox();
cellType1.caption("caption");
cellType1.textTrue("true");
cellType1.textFalse("false");
cellType1.textIndeterminate("indeterminate");
cellType1.textAlign(GC.Spread.Sheets.CellTypes.CheckBoxTextAlign.bottom);
cellType1.isThreeState(true);
cellType1.boxSize(20);
activeSheet.getCell(1, 1).cellType(cellType1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`CheckBoxTextAlign`](../enums/GC.Spread.Sheets.CellTypes.CheckBoxTextAlign.md) | 相对于复选框的文本对齐 |

#### Returns

`any`

如果未设置值，请返回与复选框相对于复选框的文本对齐；否则，返回复选框单元类型

___

### <a id="textfalse" name="textfalse"></a> textFalse

▸ **textFalse**(`value?`): `any`

当单元格值为`false`时，获取或设置单元格中的文本

**`example`**
```
//This example creates a check box cell.
var cellType1 = new GC.Spread.Sheets.CellTypes.CheckBox();
cellType1.caption("caption");
cellType1.textTrue("true");
cellType1.textFalse("false");
cellType1.textIndeterminate("indeterminate");
cellType1.textAlign(GC.Spread.Sheets.CellTypes.CheckBoxTextAlign.bottom);
cellType1.isThreeState(true);
cellType1.boxSize(20);
activeSheet.getCell(1, 1).cellType(cellType1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 当单元格值为`false`时，返回单元格中的文本 |

#### Returns

`any`

如果未设置值，请在单元格值为` false`时返回单元格中的文本。如果设置了值，请返回复选框单元格

___

### <a id="textindeterminate" name="textindeterminate"></a> textIndeterminate

▸ **textIndeterminate**(`value?`): `any`

当单元格值不确定时，获取或设置了单元格中的文本（`true`和`false`）

**`example`**
```
//This example creates a check box cell.
var cellType1 = new GC.Spread.Sheets.CellTypes.CheckBox();
cellType1.caption("caption");
cellType1.textTrue("true");
cellType1.textFalse("false");
cellType1.textIndeterminate("indeterminate");
cellType1.textAlign(GC.Spread.Sheets.CellTypes.CheckBoxTextAlign.bottom);
cellType1.isThreeState(true);
cellType1.boxSize(20);
activeSheet.getCell(1, 1).cellType(cellType1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 当单元格值不确定时，返回单元格中的文本 |

#### Returns

`any`

如果未设置值，请在单元格值不确定时返回单元格中的文本。如果设置了值，请返回复选框单元格

___

### <a id="texttrue" name="texttrue"></a> textTrue

▸ **textTrue**(`value?`): `any`

当单元格值为`true`时获取或设置单元格中的文本

**`example`**
```
//This example creates a check box cell.
var cellType1 = new GC.Spread.Sheets.CellTypes.CheckBox();
cellType1.caption("caption");
cellType1.textTrue("true");
cellType1.textFalse("false");
cellType1.textIndeterminate("indeterminate");
cellType1.textAlign(GC.Spread.Sheets.CellTypes.CheckBoxTextAlign.bottom);
cellType1.isThreeState(true);
cellType1.boxSize(20);
activeSheet.getCell(1, 1).cellType(cellType1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 单元格值为`true`时的文本 |

#### Returns

`any`

如果未设置值，请在单元格值为`true`时返回文本。如果设置了值，请返回复选框单元格

___

### <a id="tojson" name="tojson"></a> toJSON

▸ **toJSON**(): `any`

将对象状态保存为JSON字符串

#### Returns

`any`

单元格类型数据

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[toJSON](GC.Spread.Sheets.CellTypes.Base.md#tojson)

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

[Base](GC.Spread.Sheets.CellTypes.Base.md).[updateEditor](GC.Spread.Sheets.CellTypes.Base.md#updateeditor)

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

[Base](GC.Spread.Sheets.CellTypes.Base.md).[updateEditorContainer](GC.Spread.Sheets.CellTypes.Base.md#updateeditorcontainer)

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

[Base](GC.Spread.Sheets.CellTypes.Base.md).[updateImeMode](GC.Spread.Sheets.CellTypes.Base.md#updateimemode)
