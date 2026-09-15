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

表示名称框。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `host` | `string` \| `HTMLElement` | DOM元素。 |
| `workbook` | [`Workbook`](GC.Spread.Sheets.Workbook.md) | - |
| `options?` | [`INameBoxOptions`](../interfaces/GC.Spread.Sheets.NameBox.INameBoxOptions.md) | - |

## Properties

### <a id="options" name="options"></a> options

• **options**: [`INameBoxOptions`](../interfaces/GC.Spread.Sheets.NameBox.INameBoxOptions.md)

表示名称框的选项。

**`property`** {boolean} [enableAddCustomName] 表示是否允许在输入不存在的名称时添加到选择器中。

**`property`** {boolean} [enableNavigateToRange] 表示是否允许在输入名称或点击自定义列表项时导航到命名范围或绘图项。

**`property`** {boolean} [showCustomNameList] 表示是否显示自定义名称列表下拉指示器。

**`property`** {number} [dropDownMaxHeight] 表示下拉列表元素的最大高度。

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var div = document.createElement('div');
div.id = 'nameBox';
div.style.width = '300px';
div.style.height = '50px';
document.getElementById('panel').appendChild(div);

var nameBox = new GC.Spread.Sheets.NameBox.NameBox(document.getElementById('nameBox'), spread);
nameBox.options.enableAddCustomName = false; // 现在不能在名称框输入框中输入添加自定义名称。
nameBox.options.enableNavigateToRange = false; // 现在不能将选定范围交换为名称框输入框的值。
nameBox.options.showCustomNameList = false; // 现在不能通过右侧的下拉箭头按钮打开自定义名称列表，并且该按钮将被隐藏。
nameBox.options.dropDownMaxHeight = 100; // 现在自定义名称列表宿主DOM元素的高度不会超过100px。

```

## Methods

### <a id="dispose" name="dispose"></a> dispose

▸ **dispose**(): `void`

释放名称框并解绑所有事件。

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var nameBox = new GC.Spread.Sheets.NameBox.NameBox(document.getElementById('nameBox'), spread);
// 执行某些操作
nameBox.dispose();
```

#### Returns

`void`

___

### <a id="gethost" name="gethost"></a> getHost

▸ **getHost**(): `HTMLElement`

获取名称框的宿主元素。

**`example`**
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

刷新名称框并将名称框的值同步到工作表选择。

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var nameBox = new GC.Spread.Sheets.NameBox.NameBox(document.getElementById('nameBox'), spread);
var sheet = spread.getActiveSheet();
sheet.setSelection(0, 0, 3, 3);
nameBox.refresh();
```

#### Returns

`void`
