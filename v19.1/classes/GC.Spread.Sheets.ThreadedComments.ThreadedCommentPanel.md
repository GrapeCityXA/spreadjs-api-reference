# Class: ThreadedCommentPanel

[Sheets](../modules/GC.Spread.Sheets.md).[ThreadedComments](../modules/GC.Spread.Sheets.ThreadedComments.md).ThreadedCommentPanel

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.ThreadedComments.ThreadedCommentPanel.md#constructor)

### Methods

- [attach](GC.Spread.Sheets.ThreadedComments.ThreadedCommentPanel.md#attach)
- [destroy](GC.Spread.Sheets.ThreadedComments.ThreadedCommentPanel.md#destroy)
- [detach](GC.Spread.Sheets.ThreadedComments.ThreadedCommentPanel.md#detach)
- [findControl](GC.Spread.Sheets.ThreadedComments.ThreadedCommentPanel.md#findcontrol)
- [refresh](GC.Spread.Sheets.ThreadedComments.ThreadedCommentPanel.md#refresh)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new ThreadedCommentPanel**(`host`, `workbook`)

表示用于在工作簿中管理和导航评论的评论面板。

**`example`**
```javascript
const spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
const panelHost = document.getElementById("threadedCommentPanel");
const threadedCommentPanel = new GC.Spread.Sheets.ThreadedComments.ThreadedCommentPanel(panelHost, spread);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `host` | `string` \| `HTMLElement` | 表示将在其中渲染面板的容器元素或容器元素的ID。 |
| `workbook` | [`Workbook`](GC.Spread.Sheets.Workbook.md) | 表示评论面板所附加到的工作簿实例。 |

## Methods

### <a id="attach" name="attach"></a> attach

▸ **attach**(`workbook`): `void`

**`description`** 附加到工作簿以用于评论面板。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `workbook` | [`Workbook`](GC.Spread.Sheets.Workbook.md) | 表示被附加的工作簿。 |

#### Returns

`void`

void

___

### <a id="destroy" name="destroy"></a> destroy

▸ **destroy**(): `void`

**`description`** 销毁 PivotPanel。

#### Returns

`void`

___

### <a id="detach" name="detach"></a> detach

▸ **detach**(): `void`

**`description`** 分离工作簿以用于评论面板。

#### Returns

`void`

void

___

### <a id="findcontrol" name="findcontrol"></a> findControl

▸ **findControl**(`host`): [`ThreadedCommentPanel`](GC.Spread.Sheets.ThreadedComments.ThreadedCommentPanel.md)

通过宿主元素获取ThreadedCommentPanel实例。

**`example`**
```javascript
window.onload = function(){
     var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
     var threadedCommentPanel = new GC.Spread.Sheets.ThreadedComments.ThreadedCommentPanel(document.getElementById("threadedCommentPanel"));
     threadedCommentPanel.workbook(spread);
     var threadedCommentPanelInstance = GC.Spread.Sheets.ThreadedComments.ThreadedCommentPanel.findControl("threadedCommentPanel");
}
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `host` | `string` \| `HTMLElement` | 宿主元素或宿主元素id。 |

#### Returns

[`ThreadedCommentPanel`](GC.Spread.Sheets.ThreadedComments.ThreadedCommentPanel.md)

ThreadedCommentPanel实例。

___

### <a id="refresh" name="refresh"></a> refresh

▸ **refresh**(): `void`

刷新评论面板。

#### Returns

`void`
