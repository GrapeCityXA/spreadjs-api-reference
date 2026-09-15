# Class: TableSheetPanel

[Sheets](../modules/GC.Spread.Sheets.md).[TableSheet](../modules/GC.Spread.Sheets.TableSheet.md).TableSheetPanel

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.TableSheet.TableSheetPanel.md#constructor)

### Methods

- [attach](GC.Spread.Sheets.TableSheet.TableSheetPanel.md#attach)
- [destroy](GC.Spread.Sheets.TableSheet.TableSheetPanel.md#destroy)
- [detach](GC.Spread.Sheets.TableSheet.TableSheetPanel.md#detach)
- [findControl](GC.Spread.Sheets.TableSheet.TableSheetPanel.md#findcontrol)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new TableSheetPanel**(`name`, `tableSheet`, `host`, `options?`)

具有指定名称、集算表、宿主元素和选项设置的集算表面板

**`代码示例`**
```
//本示例创建了一个TableSheetPanel
var host = document.getElementById("panel");
var panel = new GC.Spread.Sheets.TableSheet.TableSheetPanel("myPanel", tableSheet, host);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 集算表面板名称 |
| `tableSheet` | [`TableSheet`](GC.Spread.Sheets.TableSheet.TableSheet.md) | 集算表 |
| `host` | `HTMLElement` | 宿主元素 |
| `options?` | [`IPanelOption`](../interfaces/GC.Spread.Sheets.TableSheet.IPanelOption.md) | - |

## Methods

### <a id="attach" name="attach"></a> attach

▸ **attach**(`tableSheet`): `void`

将集算表关联在当前集算表面板上

**`代码示例`**
```
//本示例子关联了一个集算表
panel.attach(tableSheet);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tableSheet` | [`TableSheet`](GC.Spread.Sheets.TableSheet.TableSheet.md) | 集算表 |

#### Returns

`void`

___

### <a id="destroy" name="destroy"></a> destroy

▸ **destroy**(): `void`

销毁当前的集算表面板

**`代码示例`**
```
//本示例销毁当前的集算表面板
panel.destroy();
```

#### Returns

`void`

___

### <a id="detach" name="detach"></a> detach

▸ **detach**(): `void`

从当前集算表面板上分离集算表

**`代码示例`**
```
//本示例分离了一个集算表
panel.detach();
```

#### Returns

`void`

___

### <a id="findcontrol" name="findcontrol"></a> findControl

▸ `Static` **findControl**(`host`): [`TableSheetPanel`](GC.Spread.Sheets.TableSheet.TableSheetPanel.md)

通过DOM元素查找集算表面板

**`代码示例`**
```
//本示例展示通过DOM元素查找集算表面板
GC.Spread.Sheets.TableSheet.TableSheetPanel.findControl(document.getElementById("sampleDiv"));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `host` | `string` \| `HTMLElement` | 宿主元素 |

#### Returns

[`TableSheetPanel`](GC.Spread.Sheets.TableSheet.TableSheetPanel.md)
