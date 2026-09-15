# Class: HyperLink

[Sheets](../modules/GC.Spread.Sheets.md).[CellTypes](../modules/GC.Spread.Sheets.CellTypes.md).HyperLink

## Hierarchy

- [`Base`](GC.Spread.Sheets.CellTypes.Base.md)

  ↳ **`HyperLink`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.CellTypes.HyperLink.md#constructor)

### Properties

- [typeName](GC.Spread.Sheets.CellTypes.HyperLink.md#typename)

### Methods

- [activateEditor](GC.Spread.Sheets.CellTypes.HyperLink.md#activateeditor)
- [activeOnClick](GC.Spread.Sheets.CellTypes.HyperLink.md#activeonclick)
- [createEditorElement](GC.Spread.Sheets.CellTypes.HyperLink.md#createeditorelement)
- [deactivateEditor](GC.Spread.Sheets.CellTypes.HyperLink.md#deactivateeditor)
- [focus](GC.Spread.Sheets.CellTypes.HyperLink.md#focus)
- [format](GC.Spread.Sheets.CellTypes.HyperLink.md#format)
- [fromJSON](GC.Spread.Sheets.CellTypes.HyperLink.md#fromjson)
- [getAutoFitHeight](GC.Spread.Sheets.CellTypes.HyperLink.md#getautofitheight)
- [getAutoFitWidth](GC.Spread.Sheets.CellTypes.HyperLink.md#getautofitwidth)
- [getEditorValue](GC.Spread.Sheets.CellTypes.HyperLink.md#geteditorvalue)
- [getHitInfo](GC.Spread.Sheets.CellTypes.HyperLink.md#gethitinfo)
- [isEditingValueChanged](GC.Spread.Sheets.CellTypes.HyperLink.md#iseditingvaluechanged)
- [isImeAware](GC.Spread.Sheets.CellTypes.HyperLink.md#isimeaware)
- [isReservedKey](GC.Spread.Sheets.CellTypes.HyperLink.md#isreservedkey)
- [linkColor](GC.Spread.Sheets.CellTypes.HyperLink.md#linkcolor)
- [linkToolTip](GC.Spread.Sheets.CellTypes.HyperLink.md#linktooltip)
- [onClickAction](GC.Spread.Sheets.CellTypes.HyperLink.md#onclickaction)
- [paint](GC.Spread.Sheets.CellTypes.HyperLink.md#paint)
- [paintContent](GC.Spread.Sheets.CellTypes.HyperLink.md#paintcontent)
- [parse](GC.Spread.Sheets.CellTypes.HyperLink.md#parse)
- [processKeyDown](GC.Spread.Sheets.CellTypes.HyperLink.md#processkeydown)
- [processKeyUp](GC.Spread.Sheets.CellTypes.HyperLink.md#processkeyup)
- [processMouseDown](GC.Spread.Sheets.CellTypes.HyperLink.md#processmousedown)
- [processMouseEnter](GC.Spread.Sheets.CellTypes.HyperLink.md#processmouseenter)
- [processMouseLeave](GC.Spread.Sheets.CellTypes.HyperLink.md#processmouseleave)
- [processMouseMove](GC.Spread.Sheets.CellTypes.HyperLink.md#processmousemove)
- [processMouseUp](GC.Spread.Sheets.CellTypes.HyperLink.md#processmouseup)
- [selectAll](GC.Spread.Sheets.CellTypes.HyperLink.md#selectall)
- [setEditorValue](GC.Spread.Sheets.CellTypes.HyperLink.md#seteditorvalue)
- [target](GC.Spread.Sheets.CellTypes.HyperLink.md#target)
- [text](GC.Spread.Sheets.CellTypes.HyperLink.md#text)
- [toJSON](GC.Spread.Sheets.CellTypes.HyperLink.md#tojson)
- [updateEditor](GC.Spread.Sheets.CellTypes.HyperLink.md#updateeditor)
- [updateEditorContainer](GC.Spread.Sheets.CellTypes.HyperLink.md#updateeditorcontainer)
- [updateImeMode](GC.Spread.Sheets.CellTypes.HyperLink.md#updateimemode)
- [visitedLinkColor](GC.Spread.Sheets.CellTypes.HyperLink.md#visitedlinkcolor)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new HyperLink**()

表示超链接单元格。

**`example`**
```
var cellType = new GC.Spread.Sheets.CellTypes.HyperLink();
cellType.linkColor("blue");
cellType.visitedLinkColor("#FF2235");
cellType.text("SpreadJS");
cellType.linkToolTip("Company Web Site");
activeSheet.getCell(1, 1).cellType(cellType).value("http://www.spreadjs.com/");
activeSheet.getCell(1, -1).height(30);
```

**`example`**
```
var cellType = new GC.Spread.Sheets.CellTypes.HyperLink();
cellType.linkColor("blue");
cellType.visitedLinkColor("#FF2235");
cellType.text("SpreadJS");
cellType.linkToolTip("Company Web Site");
activeSheet.getCell(0, 2).cellType(cellType).value("formula.html");
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

### <a id="activeonclick" name="activeonclick"></a> activeOnClick

▸ **activeOnClick**(`value?`): `any`

获取或设置点击时是否移动到活动单元格。

**`example`**
```
//此示例使用activeOnClick方法。
var h1 = new GC.Spread.Sheets.CellTypes.HyperLink();
h1.text("SpreadsJS");
h1.linkToolTip("link to SpreadJS Web page");
h1.linkColor("rgb(0, 100, 200)");
h1.visitedLinkColor("rgb(0, 200, 100)");
h1.activeOnClick(true);
activeSheet.setCellType(1, 1, h1);
activeSheet.getCell(1, 1, GC.Spread.Sheets.SheetArea.viewport).value("http://www.spreadjs.com/").hAlign(GC.Spread.Sheets.HorizontalAlign.center);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 点击时是否移动到活动单元格。 |

#### Returns

`any`

如果未设置值，则返回一个表示是否移动到活动单元格的值；否则返回超链接单元格类型。

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

### <a id="linkcolor" name="linkcolor"></a> linkColor

▸ **linkColor**(`value?`): `any`

获取或设置超链接的颜色。

**`example`**
```
//此示例创建一个超链接单元格。
cellType = new GC.Spread.Sheets.CellTypes.HyperLink();
cellType.linkColor("blue");
cellType.visitedLinkColor("#FF2235");
cellType.text("SpreadJS");
cellType.linkToolTip("Company Web Site");
activeSheet.getCell(1, 1).cellType(cellType).value("http://www.spreadjs.com/");
activeSheet.getCell(1, -1).height(30);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 超链接颜色。 |

#### Returns

`any`

如果未设置值，则返回超链接颜色；否则返回超链接单元格类型。

___

### <a id="linktooltip" name="linktooltip"></a> linkToolTip

▸ **linkToolTip**(`value?`): `any`

获取或设置超链接的工具提示。

**`example`**
```
//此示例创建一个超链接单元格。
cellType = new GC.Spread.Sheets.CellTypes.HyperLink();
cellType.linkColor("blue");
cellType.visitedLinkColor("#FF2235");
cellType.text("SpreadJS");
cellType.linkToolTip("Company Web Site");
activeSheet.getCell(1, 1).cellType(cellType).value("http://www.spreadjs.com/");
activeSheet.getCell(1, -1).height(30);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 工具提示文本。 |

#### Returns

`any`

如果未设置值，则返回工具提示文本；否则返回超链接单元格类型。

___

### <a id="onclickaction" name="onclickaction"></a> onClickAction

▸ **onClickAction**(`value?`): `any`

获取或设置超链接的回调函数，如果执行该函数将表示回调的上下文。

**`example`**
```
//此示例在选择超链接时设置标签颜色。
var h2 = new GC.Spread.Sheets.CellTypes.HyperLink();
h2.text("set sheet tab style");
h2.linkToolTip("set sheet tab style");
h2.linkColor("blue");
h2.visitedLinkColor("#FF2235");
activeSheet.getCell(2, 1).cellType(h2).value("set sheet tab style").hAlign(GC.Spread.Sheets.HorizontalAlign.center);
h2.activeOnClick(true);
            h2.onClickAction(function () {
                var setSheetTabColor = {
                    canUndo: true,
                    execute: function (context, options, isUndo) {
                        activeSheet.name("Hyperlink");
                        activeSheet.options.sheetTabColor = "red";
                    }
                };
                var commandManager = spread.commandManager();
                var commandName = "setSheetTabStyle";
                commandManager.register(commandName, setSheetTabColor, null, false, false, false, false);
                commandManager.execute({cmd: commandName})
            });
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `Function` | 超链接的回调函数。 |

#### Returns

`any`

如果未设置值，则返回表示超链接回调的值；否则返回超链接单元格类型。

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

### <a id="target" name="target"></a> target

▸ **target**(`value?`): `any`

获取或设置超链接的目标类型。

**`example`**
```
//此示例创建一个超链接单元格。
var cellType = new GC.Spread.Sheets.CellTypes.HyperLink();
cellType.linkColor("blue");
cellType.visitedLinkColor("#FFFF00");
cellType.text("SpreadJS");
cellType.linkToolTip("Company Web Site");
cellType.target(GC.Spread.Sheets.CellTypes.HyperLinkTargetType.self);
activeSheet.getCell(0, 2).cellType(cellType).value("http://www.spreadjs.com/");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`HyperLinkTargetType`](../enums/GC.Spread.Sheets.CellTypes.HyperLinkTargetType.md) | 超链接的目标类型。 |

#### Returns

`any`

如果未设置值，则返回超链接的目标类型；否则返回超链接单元格类型。

___

### <a id="text" name="text"></a> text

▸ **text**(`value?`): `any`

获取或设置超链接的文本字符串。

**`example`**
```
//此示例创建一个超链接单元格。
var cellType = new GC.Spread.Sheets.CellTypes.HyperLink();
cellType.linkColor("blue");
cellType.visitedLinkColor("#FFFF00");
cellType.text("SpreadJS");
cellType.linkToolTip("Company Web Site");
cellType.target(GC.Spread.Sheets.CellTypes.HyperLinkTargetType.self);
activeSheet.getCell(0, 2).cellType(cellType).value("http://www.spreadjs.com/");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 超链接中显示的文本。 |

#### Returns

`any`

如果未设置值，则返回超链接中的文本；否则返回超链接单元格类型。

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

___

### <a id="visitedlinkcolor" name="visitedlinkcolor"></a> visitedLinkColor

▸ **visitedLinkColor**(`value?`): `any`

获取或设置已访问链接的颜色。

**`example`**
```
//此示例创建一个超链接单元格。
var cellType = new GC.Spread.Sheets.CellTypes.HyperLink();
cellType.linkColor("blue");
cellType.visitedLinkColor("#FFFF00");
cellType.text("SpreadJS");
cellType.linkToolTip("Company Web Site");
cellType.target(GC.Spread.Sheets.CellTypes.HyperLinkTargetType.self);
activeSheet.getCell(0, 2).cellType(cellType).value("http://www.spreadjs.com/");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 已访问链接的颜色。 |

#### Returns

`any`

如果未设置值，则返回已访问链接的颜色；否则返回超链接单元格类型。
