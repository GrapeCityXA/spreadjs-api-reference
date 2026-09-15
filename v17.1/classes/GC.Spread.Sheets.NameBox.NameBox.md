# Class: NameBox

[Sheets](../modules/GC.Spread.Sheets.md).[NameBox](../modules/GC.Spread.Sheets.NameBox.md).NameBox

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.NameBox.NameBox.md#constructor)

### Properties

- [options](GC.Spread.Sheets.NameBox.NameBox.md#options)

### Methods

- [dispose](GC.Spread.Sheets.NameBox.NameBox.md#dispose)
- [getHost](GC.Spread.Sheets.NameBox.NameBox.md#gethost)
- [refresh](GC.Spread.Sheets.NameBox.NameBox.md#refresh)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new NameBox**(`host`, `workbook`, `options?`)

名称框组件

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `host` | `string` \| `HTMLElement` | DOM 元素 |
| `workbook` | [`Workbook`](GC.Spread.Sheets.Workbook.md) | - |
| `options?` | [`INameBoxOptions`](../interfaces/GC.Spread.Sheets.NameBox.INameBoxOptions.md) | - |

## Properties

### <a id="options" name="options"></a> options

• **options**: [`INameBoxOptions`](../interfaces/GC.Spread.Sheets.NameBox.INameBoxOptions.md)

指示名称框的选项

**`property`** {boolean} [enableAddCustomName] 在输入选择器中不存在的名称时是否启用添加自定义名称

**`property`** {boolean} [enableNavigateToRange] 指示在输入名称或单击自定义列表项时启用导航到命名范围或绘图项

**`property`** {boolean} [showCustomNameList] 指示是否显示自定义名称列表下拉指示器

**`property`** {number} [dropDownMaxHeight] 指示下拉列表元素的最大高度

## Methods

### <a id="dispose" name="dispose"></a> dispose

▸ **dispose**(): `void`

销毁 NameBox，并解除所有事件的绑定

**`代码示例`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var nameBox = new GC.Spread.Sheets.NameBox.NameBox(document.getElementById('nameBox'), spread);
// do something
nameBox.dispose();
```

#### Returns

`void`

___

### <a id="gethost" name="gethost"></a> getHost

▸ **getHost**(): `HTMLElement`

获取名称框组件所在容器

**`代码示例`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var nameBox = new GC.Spread.Sheets.NameBox.NameBox(document.getElementById('nameBox'), spread);
var host = nameBox.getHost();
```

#### Returns

`HTMLElement`

___

### <a id="refresh" name="refresh"></a> refresh

▸ **refresh**(): `void`

刷新名称框，并将名称框值同步到工作表选择

**`代码示例`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var nameBox = new GC.Spread.Sheets.NameBox.NameBox(document.getElementById('nameBox'), spread);
var sheet = spread.getActiveSheet();
sheet.setSelection(0, 0, 3, 3);
nameBox.refresh();
```

#### Returns

`void`
