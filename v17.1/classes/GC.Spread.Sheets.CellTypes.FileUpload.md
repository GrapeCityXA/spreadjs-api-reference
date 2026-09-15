# Class: FileUpload

[Sheets](../modules/GC.Spread.Sheets.md).[CellTypes](../modules/GC.Spread.Sheets.CellTypes.md).FileUpload

## Hierarchy

- [`Base`](GC.Spread.Sheets.CellTypes.Base.md)

  ↳ **`FileUpload`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.CellTypes.FileUpload.md#constructor)

### Properties

- [previewCommand](GC.Spread.Sheets.CellTypes.FileUpload.md#previewcommand)
- [typeName](GC.Spread.Sheets.CellTypes.FileUpload.md#typename)

### Methods

- [accept](GC.Spread.Sheets.CellTypes.FileUpload.md#accept)
- [activateEditor](GC.Spread.Sheets.CellTypes.FileUpload.md#activateeditor)
- [createEditorElement](GC.Spread.Sheets.CellTypes.FileUpload.md#createeditorelement)
- [deactivateEditor](GC.Spread.Sheets.CellTypes.FileUpload.md#deactivateeditor)
- [focus](GC.Spread.Sheets.CellTypes.FileUpload.md#focus)
- [format](GC.Spread.Sheets.CellTypes.FileUpload.md#format)
- [fromJSON](GC.Spread.Sheets.CellTypes.FileUpload.md#fromjson)
- [getAutoFitHeight](GC.Spread.Sheets.CellTypes.FileUpload.md#getautofitheight)
- [getAutoFitWidth](GC.Spread.Sheets.CellTypes.FileUpload.md#getautofitwidth)
- [getEditorValue](GC.Spread.Sheets.CellTypes.FileUpload.md#geteditorvalue)
- [getHitInfo](GC.Spread.Sheets.CellTypes.FileUpload.md#gethitinfo)
- [isClearEnabled](GC.Spread.Sheets.CellTypes.FileUpload.md#isclearenabled)
- [isDownloadEnabled](GC.Spread.Sheets.CellTypes.FileUpload.md#isdownloadenabled)
- [isEditingValueChanged](GC.Spread.Sheets.CellTypes.FileUpload.md#iseditingvaluechanged)
- [isImeAware](GC.Spread.Sheets.CellTypes.FileUpload.md#isimeaware)
- [isPreviewEnabled](GC.Spread.Sheets.CellTypes.FileUpload.md#ispreviewenabled)
- [isReservedKey](GC.Spread.Sheets.CellTypes.FileUpload.md#isreservedkey)
- [marginBottom](GC.Spread.Sheets.CellTypes.FileUpload.md#marginbottom)
- [marginLeft](GC.Spread.Sheets.CellTypes.FileUpload.md#marginleft)
- [marginRight](GC.Spread.Sheets.CellTypes.FileUpload.md#marginright)
- [marginTop](GC.Spread.Sheets.CellTypes.FileUpload.md#margintop)
- [maxSize](GC.Spread.Sheets.CellTypes.FileUpload.md#maxsize)
- [paint](GC.Spread.Sheets.CellTypes.FileUpload.md#paint)
- [paintContent](GC.Spread.Sheets.CellTypes.FileUpload.md#paintcontent)
- [parse](GC.Spread.Sheets.CellTypes.FileUpload.md#parse)
- [processKeyDown](GC.Spread.Sheets.CellTypes.FileUpload.md#processkeydown)
- [processKeyUp](GC.Spread.Sheets.CellTypes.FileUpload.md#processkeyup)
- [processMouseDown](GC.Spread.Sheets.CellTypes.FileUpload.md#processmousedown)
- [processMouseEnter](GC.Spread.Sheets.CellTypes.FileUpload.md#processmouseenter)
- [processMouseLeave](GC.Spread.Sheets.CellTypes.FileUpload.md#processmouseleave)
- [processMouseMove](GC.Spread.Sheets.CellTypes.FileUpload.md#processmousemove)
- [processMouseUp](GC.Spread.Sheets.CellTypes.FileUpload.md#processmouseup)
- [selectAll](GC.Spread.Sheets.CellTypes.FileUpload.md#selectall)
- [setEditorValue](GC.Spread.Sheets.CellTypes.FileUpload.md#seteditorvalue)
- [toJSON](GC.Spread.Sheets.CellTypes.FileUpload.md#tojson)
- [updateEditor](GC.Spread.Sheets.CellTypes.FileUpload.md#updateeditor)
- [updateEditorContainer](GC.Spread.Sheets.CellTypes.FileUpload.md#updateeditorcontainer)
- [updateImeMode](GC.Spread.Sheets.CellTypes.FileUpload.md#updateimemode)
- [valuePath](GC.Spread.Sheets.CellTypes.FileUpload.md#valuepath)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new FileUpload**()

代表文件上传单元格类型

**`example`**
```
// set a FileUpload celltype
const cellType1 = new GC.Spread.Sheets.CellTypes.FileUpload();
sheet.setCellType(1, 1, cellType1);
// FileUpload support the valuePath property, will parse the cell value with valuePath to GC.Spread.Sheets.CellTypes.IFileInfo
sheet.getCellType(1, 1).valuePath("blob");
sheet.setValue(1, 1, blob); // value path is "blob"
sheet.getCellType(2, 2).valuePath("dataUrl");
sheet.setValue(2, 2, dataUrl); // value path is "dataUrl"
sheet.getCellType(3, 3).valuePath(undefined);
sheet.setValue(3, 3, { name: 'test1.png', blob: blob }); // value path is undefined
sheet.setValue(3, 3, { name: 'test2.txt', dataUrl: dataUrl }); // value path is undefined
```

#### Overrides

[Base](GC.Spread.Sheets.CellTypes.Base.md).[constructor](GC.Spread.Sheets.CellTypes.Base.md#constructor)

## Properties

### <a id="previewcommand" name="previewcommand"></a> previewCommand

• `Optional` **previewCommand**: `string` \| (`file`: [`IFilePreviewInfo`](../interfaces/GC.Spread.Sheets.CellTypes.IFilePreviewInfo.md)) => `void`

通过设置点击预览按钮后的事件回调或命令，自定义个性化预览逻辑和UI显示。

**`returns`**

**`example`**
```
// This example creates a file upload cell.
// Customize your preview function.
fileUpload.previewCommand = function (fileInfo) {
   // Custom preview logic
}

// Customize your preview command.
fileUpload.previewCommand = 'openPreviewDialog';

activeSheet.getCell(1, 1).cellType(fileUpload);
```

___

### <a id="typename" name="typename"></a> typeName

• **typeName**: `string`

表示用于支持序列化的类型名称字符串。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[typeName](GC.Spread.Sheets.CellTypes.Base.md#typename)

## Methods

### <a id="accept" name="accept"></a> accept

▸ **accept**(`value?`): `string`

获取或设置可以上传的文件类型。

**`example`**
```
// This example creates a file upload cell.
const fileUpload = new GC.Spread.Sheets.CellTypes.FileUpload();
fileUpload.accept('image/*');
activeSheet.getCell(1, 1).cellType(fileUpload);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 可以上传的文件类型 |

#### Returns

`string`

返回可以上传的文件类型。

___

### <a id="activateeditor" name="activateeditor"></a> activateEditor

▸ **activateEditor**(`editorContext`, `cellStyle`, `cellRect`, `context?`): `void`

激活编辑器，包括设置编辑器的属性或绑定编辑器的事件。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由 createEditorElement 方法创建的 DOM 元素 |
| `cellStyle` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际样式 |
| `cellRect` | [`Rect`](GC.Spread.Sheets.Rect.md) | 单元格的布局信息 |
| `context?` | `any` | 与单元格类型相关的上下文。请参阅备注了解更多信息 |

#### Returns

`void`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[activateEditor](GC.Spread.Sheets.CellTypes.Base.md#activateeditor)

___

### <a id="createeditorelement" name="createeditorelement"></a> createEditorElement

▸ **createEditorElement**(`context?`): `HTMLElement`

创建一个 DOM 元素然后返回它。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context?` | `any` | 与单元格类型相关的上下文。请参阅备注了解更多信息 |

#### Returns

`HTMLElement`

Returns a DOM element.

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[createEditorElement](GC.Spread.Sheets.CellTypes.Base.md#createeditorelement)

___

### <a id="deactivateeditor" name="deactivateeditor"></a> deactivateEditor

▸ **deactivateEditor**(`editorContext`, `context?`): `void`

停用编辑器，例如取消编辑器的绑定事件

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由 createEditorElement 方法创建的 DOM 元素 |
| `context?` | `any` | 与单元格类型相关的上下文。请参阅备注了解更多信息 |

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
| `editorContext` | `HTMLElement` | 由 createEditorElement 方法创建的 DOM 元素 |
| `context?` | `any` | 与单元格类型相关的上下文。请参阅备注了解更多信息 |

#### Returns

`void`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[focus](GC.Spread.Sheets.CellTypes.Base.md#focus)

___

### <a id="format" name="format"></a> format

▸ **format**(`value`, `format`, `formattedData?`, `context?`): `string`

将具有指定格式的值格式化为字符串

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | The object value to format. |
| `format` | `string` \| [`GeneralFormatter`](GC.Spread.Formatter.GeneralFormatter.md) | 格式 |
| `formattedData?` | [`FormattedData`](../interfaces/GC.Spread.Sheets.FormattedData.md) | 格式化的数据 |
| `context?` | `any` | 与单元格类型相关的上下文。请参阅备注了解更多信息 |

#### Returns

`string`

返回格式化的字符串

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[format](GC.Spread.Sheets.CellTypes.Base.md#format)

___

### <a id="fromjson" name="fromjson"></a> fromJSON

▸ **fromJSON**(`settings`): `void`

从指定的 JSON 字符串加载对象状态

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `settings` | `any` | 来自反序列化的单元格类型数据 |

#### Returns

`void`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[fromJSON](GC.Spread.Sheets.CellTypes.Base.md#fromjson)

___

### <a id="getautofitheight" name="getautofitheight"></a> getAutoFitHeight

▸ **getAutoFitHeight**(`value`, `text`, `cellStyle`, `zoomFactor`, `context?`): `number`

获取可用于处理行自动调整的单元格高度

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | The cell's value. |
| `text` | `string` | The cell's text. |
| `cellStyle` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际值 |
| `zoomFactor` | `number` | 当前工作表的缩放系数 |
| `context?` | `any` | 与单元格类型相关的上下文。请参阅备注了解更多信息 |

#### Returns

`number`

返回可用于处理行自动调整的单元格高度

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[getAutoFitHeight](GC.Spread.Sheets.CellTypes.Base.md#getautofitheight)

___

### <a id="getautofitwidth" name="getautofitwidth"></a> getAutoFitWidth

▸ **getAutoFitWidth**(`value`, `text`, `cellStyle`, `zoomFactor`, `context?`): `number`

获取可用于处理列自动调整的单元格宽度

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `any` | 单元格的值 |
| `text` | `string` | 单元格的文本 |
| `cellStyle` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际值 |
| `zoomFactor` | `number` | 当前工作表的缩放系数 |
| `context?` | `any` | 与单元格类型相关的上下文。请参阅备注了解更多信息 |

#### Returns

`number`

返回可用于处理列自动调整的单元格宽度

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[getAutoFitWidth](GC.Spread.Sheets.CellTypes.Base.md#getautofitwidth)

___

### <a id="geteditorvalue" name="geteditorvalue"></a> getEditorValue

▸ **getEditorValue**(`editorContext`, `context?`): `any`

获取编辑器的值

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由 createEditorElement 方法创建的 DOM 元素 |
| `context?` | `any` | 与单元格类型相关的上下文。请参阅备注了解更多信息 |

#### Returns

`any`

返回编辑器的值

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[getEditorValue](GC.Spread.Sheets.CellTypes.Base.md#geteditorvalue)

___

### <a id="gethitinfo" name="gethitinfo"></a> getHitInfo

▸ **getHitInfo**(`x`, `y`, `cellStyle`, `cellRect`, `context?`): [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md)

获取单元格类型的命中信息

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | <i>x</i> -指针当前位置相对于画布的坐标 |
| `y` | `number` | <i>y</i>-指针当前位置相对于画布的坐标 |
| `cellStyle` | [`Style`](GC.Spread.Sheets.Style.md) | 当前单元格的实际样式 |
| `cellRect` | [`Rect`](GC.Spread.Sheets.Rect.md) | 当前单元格的布局信息 |
| `context?` | `any` | 与单元格类型相关的上下文。请参阅备注了解更多信息 |

#### Returns

[`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md)

返回一个包含 <i>x</i>、<i>y</i>、<i>row</i>、<i>col</i>、<i>cellRect</i> 的对象和 <i>sheetArea</i> 参数，以及指示 <i>isReservedLocation</i> 的值。
如果命中测试位于单元类型需要处理的特殊区域，则 <i>isReservedLocation</i> 为“true”；否则，“false”。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[getHitInfo](GC.Spread.Sheets.CellTypes.Base.md#gethitinfo)

___

### <a id="isclearenabled" name="isclearenabled"></a> isClearEnabled

▸ **isClearEnabled**(`value?`): `boolean`

获取或设置是否显示文件清除按钮。

**`example`**
```
// This example creates a file upload cell.
const fileUpload = new GC.Spread.Sheets.CellTypes.FileUpload();
fileUpload.isClearEnabled(false);
activeSheet.getCell(1, 1).cellType(fileUpload);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否显示文件清除按钮 |

#### Returns

`boolean`

返回当前显示的文件清除按钮。

___

### <a id="isdownloadenabled" name="isdownloadenabled"></a> isDownloadEnabled

▸ **isDownloadEnabled**(`value?`): `boolean`

获取或设置是否显示文件下载按钮

**`example`**
```
// This example creates a file upload cell.
const fileUpload = new GC.Spread.Sheets.CellTypes.FileUpload();
fileUpload.isDownloadEnabled(false);
activeSheet.getCell(1, 1).cellType(fileUpload);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否显示文件下载按钮 |

#### Returns

`boolean`

返回当前显示的文件下载按钮

___

### <a id="iseditingvaluechanged" name="iseditingvaluechanged"></a> isEditingValueChanged

▸ **isEditingValueChanged**(`oldValue`, `newValue`, `context?`): `boolean`

编辑值是否改变

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `oldValue` | `any` | 旧的编辑值 |
| `newValue` | `any` | 新的编辑值 |
| `context?` | `any` | 与单元格类型相关的上下文。请参阅备注了解更多信息 |

#### Returns

`boolean`

如果旧值等于新值则为“true”；否则，“false”。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[isEditingValueChanged](GC.Spread.Sheets.CellTypes.Base.md#iseditingvaluechanged)

___

### <a id="isimeaware" name="isimeaware"></a> isImeAware

▸ **isImeAware**(`context?`): `boolean`

该单元格类型是否识别 IME。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context?` | `any` | 与单元格类型相关的上下文。请参阅备注了解更多信息 |

#### Returns

`boolean`

如果单元格类型支持 IME，则为“true”；否则，“false”。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[isImeAware](GC.Spread.Sheets.CellTypes.Base.md#isimeaware)

___

### <a id="ispreviewenabled" name="ispreviewenabled"></a> isPreviewEnabled

▸ **isPreviewEnabled**(`value?`): `boolean`

获取或设置是否显示文件预览按钮

**`example`**
```
// This example creates a file upload cell.
const fileUpload = new GC.Spread.Sheets.CellTypes.FileUpload();
fileUpload.isPreviewEnabled(false);
activeSheet.getCell(1, 1).cellType(fileUpload);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否显示文件预览按钮 |

#### Returns

`boolean`

返回当前显示的文件预览按钮

___

### <a id="isreservedkey" name="isreservedkey"></a> isReservedKey

▸ **isReservedKey**(`e`, `context?`): `boolean`

单元格类型本身是否处理键盘事件

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `e` | `KeyboardEvent` | 键盘事件 |
| `context?` | `any` | 与单元格类型相关的上下文。请参阅备注了解更多信息 |

#### Returns

`boolean`

如果单元格类型本身处理键盘事件，则返回“true”；否则，“false”。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[isReservedKey](GC.Spread.Sheets.CellTypes.Base.md#isreservedkey)

___

### <a id="marginbottom" name="marginbottom"></a> marginBottom

▸ **marginBottom**(`value?`): `number`

获取或设置底部边距值。

**`example`**
```
// This example creates a file upload cell.
const fileUpload = new GC.Spread.Sheets.CellTypes.FileUpload();
fileUpload.marginBottom(10);
activeSheet.getCell(1, 1).cellType(fileUpload);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 底部边距值 |

#### Returns

`number`

如果没有设置值，则返回当前底部边距

___

### <a id="marginleft" name="marginleft"></a> marginLeft

▸ **marginLeft**(`value?`): `number`

获取或设置左部边距值

**`example`**
```
// This example creates a file upload cell.
const fileUpload = new GC.Spread.Sheets.CellTypes.FileUpload();
fileUpload.marginLeft(10);
activeSheet.getCell(1, 1).cellType(fileUpload);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 左部边距值 |

#### Returns

`number`

如果没有设置值，则返回当前左部边距

___

### <a id="marginright" name="marginright"></a> marginRight

▸ **marginRight**(`value?`): `number`

获取或设置右部边距值

**`example`**
```
// This example creates a file upload cell.
const fileUpload = new GC.Spread.Sheets.CellTypes.FileUpload();
fileUpload.marginRight(10);
activeSheet.getCell(1, 1).cellType(fileUpload);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 右部边距值 |

#### Returns

`number`

如果没有设置值，则返回当前右部边距

___

### <a id="margintop" name="margintop"></a> marginTop

▸ **marginTop**(`value?`): `number`

获取或设置顶部边距值

**`example`**
```
// This example creates a file upload cell.
const fileUpload = new GC.Spread.Sheets.CellTypes.FileUpload();
fileUpload.marginTop(10);
activeSheet.getCell(1, 1).cellType(fileUpload);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 顶部边距值 |

#### Returns

`number`

如果没有设置值，则返回当前顶部边距

___

### <a id="maxsize" name="maxsize"></a> maxSize

▸ **maxSize**(`value?`): `number`

获取或设置可以上传的最大文件大小

**`example`**
```
// This example creates a file upload cell.
const fileUpload = new GC.Spread.Sheets.CellTypes.FileUpload();
fileUpload.maxSize(10000);
activeSheet.getCell(1, 1).cellType(fileUpload);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 可以上传的最大文件大小 |

#### Returns

`number`

返回可以上传的最大文件大小。

___

### <a id="paint" name="paint"></a> paint

▸ **paint**(`ctx`, `value`, `x`, `y`, `w`, `h`, `style`, `context?`): `void`

在画布上绘制一个单元格。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ctx` | `CanvasRenderingContext2D` | 画布的二维环境 |
| `value` | `any` | 单元格的值 |
| `x` | `number` | <i>x</i>-相对于画布的坐标 |
| `y` | `number` | <i>y</i>-相对于画布的坐标 |
| `w` | `number` | 单元格的宽度 |
| `h` | `number` | 单元格的高度|
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际样式 |
| `context?` | `any` | 与单元格类型相关的上下文。请参阅备注以获取更多信息 |

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
| `ctx` | `CanvasRenderingContext2D` | 画布的二维环境 |
| `value` | `any` | 单元格的值 |
| `x` | `number` | <i>x</i>-相对于画布的坐标 |
| `y` | `number` | <i>y</i>-相对于画布的坐标 |
| `w` | `number` | 单元格内容区域的宽度 |
| `h` | `number` | 单元格内容区域的高度 |
| `style` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际样式 |
| `context?` | `any` | 与单元格类型相关的上下文。请参阅备注以获取更多信息 |


#### Returns

`void`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[paintContent](GC.Spread.Sheets.CellTypes.Base.md#paintcontent)

___

### <a id="parse" name="parse"></a> parse

▸ **parse**(`text`, `formatStr`, `context?`): `any`

将具有指定格式字符串的文本解析为对象

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `text` | `string` | 解析文本字符串 |
| `formatStr` | `string` | 解析格式字符串 |
| `context?` | `any` | 与单元格类型相关的上下文。请参阅备注以获取更多信息 |

#### Returns

`any`

The parsed object.

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[parse](GC.Spread.Sheets.CellTypes.Base.md#parse)

___

### <a id="processkeydown" name="processkeydown"></a> processKeyDown

▸ **processKeyDown**(`event`, `context?`): `boolean`

在显示模式下处理按键按下。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `event` | `KeyboardEvent` | 键盘事件 |
| `context?` | `any` | 与单元格类型相关的上下文。请参阅备注以获取更多信息 |

#### Returns

`boolean`

如果过程成功则返回“true”；否则，“false”。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[processKeyDown](GC.Spread.Sheets.CellTypes.Base.md#processkeydown)

___

### <a id="processkeyup" name="processkeyup"></a> processKeyUp

▸ **processKeyUp**(`event`, `context?`): `boolean`

在显示模式下处理按键

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `event` | `KeyboardEvent` | 键盘事件 |
| `context?` | `any` | 与单元格类型相关的上下文。请参阅备注以获取更多信息 |

#### Returns

`boolean`

如果过程成功则返回“true”；否则，“false”。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[processKeyUp](GC.Spread.Sheets.CellTypes.Base.md#processkeyup)

___

### <a id="processmousedown" name="processmousedown"></a> processMouseDown

▸ **processMouseDown**(`hitInfo`): `boolean`

在显示模式下处理鼠标按下。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitInfo` | [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md) | getHitInfo 方法返回的命中测试信息。请参阅备注以获取更多信息。 |

#### Returns

`boolean`

如果过程成功则返回“true”；否则，“false”。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[processMouseDown](GC.Spread.Sheets.CellTypes.Base.md#processmousedown)

___

### <a id="processmouseenter" name="processmouseenter"></a> processMouseEnter

▸ **processMouseEnter**(`hitInfo`): `boolean`

在显示模式下处理鼠标输入。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitInfo` | [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md) | getHitInfo 方法返回的命中测试信息。请参阅备注以获取更多信息 |

#### Returns

`boolean`

如果过程成功则返回“true”；否则，“false”。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[processMouseEnter](GC.Spread.Sheets.CellTypes.Base.md#processmouseenter)

___

### <a id="processmouseleave" name="processmouseleave"></a> processMouseLeave

▸ **processMouseLeave**(`hitInfo`): `boolean`

处理鼠标离开显示模式。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitInfo` | [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md) | getHitInfo 方法返回的命中测试信息。请参阅备注以获取更多信息 |

#### Returns

`boolean`

如果过程成功则返回“true”；否则，“false”。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[processMouseLeave](GC.Spread.Sheets.CellTypes.Base.md#processmouseleave)

___

### <a id="processmousemove" name="processmousemove"></a> processMouseMove

▸ **processMouseMove**(`hitInfo`): `boolean`

在显示模式下处理鼠标移动。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitInfo` | [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md) | getHitInfo 方法返回的命中测试信息。请参阅备注以获取更多信息 |

#### Returns

`boolean`

如果过程成功则返回“true”；否则，“false”。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[processMouseMove](GC.Spread.Sheets.CellTypes.Base.md#processmousemove)

___

### <a id="processmouseup" name="processmouseup"></a> processMouseUp

▸ **processMouseUp**(`hitInfo`): `boolean`

在显示模式下处理鼠标松开。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `hitInfo` | [`IHitTestCellTypeHitInfo`](../interfaces/GC.Spread.Sheets.IHitTestCellTypeHitInfo.md) | getHitInfo 方法返回的命中测试信息。请参阅备注以获取更多信息 |

#### Returns

`boolean`

如果过程成功则返回“true”；否则，“false”。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[processMouseUp](GC.Spread.Sheets.CellTypes.Base.md#processmouseup)

___

### <a id="selectall" name="selectall"></a> selectAll

▸ **selectAll**(`editorContext`, `context?`): `void`

选择编辑器 DOM 元素中的所有文本。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由 createEditorElement 方法创建的 DOM 元素 |
| `context?` | `any` | 与单元格类型相关的上下文。请参阅备注以获取更多信息 |

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
| `editorContext` | `HTMLElement` | 由 createEditorElement 方法创建的 DOM 元素 |
| `value` | `any` | 从活动单元格返回的值 |
| `context?` | `any` | 与单元格类型相关的上下文。请参阅备注以获取更多信息 |

#### Returns

`void`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[setEditorValue](GC.Spread.Sheets.CellTypes.Base.md#seteditorvalue)

___

### <a id="tojson" name="tojson"></a> toJSON

▸ **toJSON**(): `any`

将对象状态保存到 JSON 字符串

#### Returns

`any`

单元格类型数据

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[toJSON](GC.Spread.Sheets.CellTypes.Base.md#tojson)

___

### <a id="updateeditor" name="updateeditor"></a> updateEditor

▸ **updateEditor**(`editorContext`, `cellStyle`, `cellRect`, `context?`): [`Rect`](GC.Spread.Sheets.Rect.md)

更新编辑器的大小。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由 createEditorElement 方法创建的 DOM 元素 |
| `cellStyle` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际样式 |
| `cellRect` | [`Rect`](GC.Spread.Sheets.Rect.md) | 单元格的布局信息 |
| `context?` | `any` | 与单元格类型相关的上下文。请参阅备注以获取更多信息 |

#### Returns

[`Rect`](GC.Spread.Sheets.Rect.md)

返回单元格包装元素的新大小，它应该包含两个属性“宽度”和“高度”。

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[updateEditor](GC.Spread.Sheets.CellTypes.Base.md#updateeditor)

___

### <a id="updateeditorcontainer" name="updateeditorcontainer"></a> updateEditorContainer

▸ **updateEditorContainer**(`editorContext`, `editorBounds`, `cellStyle`): `void`

更新单元格包装元素大小。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由 createEditorElement 方法创建的 DOM 元素 |
| `editorBounds` | [`Rect`](GC.Spread.Sheets.Rect.md) | 单元格包装元素的新大小 |
| `cellStyle` | [`Style`](GC.Spread.Sheets.Style.md) | 单元格的实际样式 |

#### Returns

`void`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[updateEditorContainer](GC.Spread.Sheets.CellTypes.Base.md#updateeditorcontainer)

___

### <a id="updateimemode" name="updateimemode"></a> updateImeMode

▸ **updateImeMode**(`editorContext`, `imeMode`, `context?`): `void`

更新编辑器的 ime 模式。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `editorContext` | `HTMLElement` | 由 createEditorElement 方法创建的 DOM 元素 |
| `imeMode` | [`ImeMode`](../enums/GC.Spread.Sheets.ImeMode.md) | 来自单元格实际样式的 ime 模式 |
| `context?` | `any` | 与单元格类型相关的上下文。请参阅备注以获取更多信息 |

#### Returns

`void`

#### Inherited from

[Base](GC.Spread.Sheets.CellTypes.Base.md).[updateImeMode](GC.Spread.Sheets.CellTypes.Base.md#updateimemode)

___

### <a id="valuepath" name="valuepath"></a> valuePath

▸ **valuePath**(`value?`): `string`

获取或设置 FileUpload 单元格类型的值路径，单元格将通过 fileInfo 中的 valuePath 获取值。

**`example`**
```
// This example creates a file upload cell and setValue with dataUrl.
const fileUpload = new GC.Spread.Sheets.CellTypes.FileUpload();
fileUpload.valuePath("dataUrl"); // set valuePath dataUrl, default is dataUrl
activeSheet.getCell(1, 1).cellType(fileUpload);
activeSheet.setValue(1, 1, 'data:text/plain;base64,MQ==')
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 值路径值 |

#### Returns

`string`

如果没有设置值，则返回当前值路径，默认值路径为 dataUrl。
