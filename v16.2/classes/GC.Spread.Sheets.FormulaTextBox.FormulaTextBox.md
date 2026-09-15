# Class: FormulaTextBox

[Sheets](../modules/GC.Spread.Sheets.md).[FormulaTextBox](../modules/GC.Spread.Sheets.FormulaTextBox.md).FormulaTextBox

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.FormulaTextBox.FormulaTextBox.md#constructor)

### Methods

- [add](GC.Spread.Sheets.FormulaTextBox.FormulaTextBox.md#add)
- [autoComplete](GC.Spread.Sheets.FormulaTextBox.FormulaTextBox.md#autocomplete)
- [destroy](GC.Spread.Sheets.FormulaTextBox.FormulaTextBox.md#destroy)
- [refresh](GC.Spread.Sheets.FormulaTextBox.FormulaTextBox.md#refresh)
- [remove](GC.Spread.Sheets.FormulaTextBox.FormulaTextBox.md#remove)
- [showHelp](GC.Spread.Sheets.FormulaTextBox.FormulaTextBox.md#showhelp)
- [text](GC.Spread.Sheets.FormulaTextBox.FormulaTextBox.md#text)
- [workbook](GC.Spread.Sheets.FormulaTextBox.FormulaTextBox.md#workbook)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new FormulaTextBox**(`host`, `options?`)

公式文本框

**`代码示例`**
```
window.onload = function(){
     var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"), { sheetCount: 1 });
     rangeSelector = new GC.Spread.Sheets.FormulaTextBox.FormulaTextBox(document.getElementById("ftb"), {rangeSelectMode: true});
     rangeSelector.workbook(spread);
}
function buttonClick(){
     alert(rangeSelector.text());
}
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `host` | `HTMLElement` | DOM元素 它可以是INPUT,TEXTAREA或可编辑的DIV |
| `options?` | [`IFormulaTextBoxOptions`](../interfaces/GC.Spread.Sheets.FormulaTextBox.IFormulaTextBoxOptions.md) | - |

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`functionDescription`): `void`

添加自定义功能描述

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `functionDescription` | [`IFunctionDescription`](../interfaces/GC.Spread.CalcEngine.Functions.IFunctionDescription.md) | 要添加的功能描述,可以是一个数组 |

#### Returns

`void`

___

### <a id="autocomplete" name="autocomplete"></a> autoComplete

▸ **autoComplete**(`value?`): `boolean`

获取或设置文本框是否使用自动完成

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 编辑时是否使用自动完成 |

#### Returns

`boolean`

如果未设置任何值,则返回文本框是否使用自动完成.否则,没有返回值

___

### <a id="destroy" name="destroy"></a> destroy

▸ **destroy**(): `void`

从公式文本框中删除宿主,并删除所有绑定事件

#### Returns

`void`

___

### <a id="refresh" name="refresh"></a> refresh

▸ **refresh**(`ignoreEditing?`): `void`

使用活动单元格刷新公式文本框

#### Parameters

| Name | Type |
| :------ | :------ |
| `ignoreEditing?` | `boolean` |

#### Returns

`void`

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`name`): `void`

删除自定义功能描述

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 自定义功能描述名称 |

#### Returns

`void`

___

### <a id="showhelp" name="showhelp"></a> showHelp

▸ **showHelp**(`value?`): `any`

获取或设置是否显示功能的帮助提示

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 编辑时是否显示功能的帮助提示 |

#### Returns

`any`

如果未设置任何值,则返回在编辑时文本框是否显示功能的帮助提示;否则,没有返回值

___

### <a id="text" name="text"></a> text

▸ **text**(`value?`): `string`

获取或设置文本

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 文本 |

#### Returns

`string`

如果未设置任何值,则返回文本 否则,没有返回值

___

### <a id="workbook" name="workbook"></a> workbook

▸ **workbook**(`value?`): [`Workbook`](GC.Spread.Sheets.Workbook.md)

获取或设置与公式文本框一起使用的工作簿

**`代码示例`**
```
window.onload = function(){
     var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
     var activeSheet = spread.getActiveSheet();
     activeSheet.setArray(0, 0, [1, 2, 3, 4, 5]);
     var fbx = new GC.Spread.Sheets.FormulaTextBox.FormulaTextBox(document.getElementById("formulaTextBox"));
     fbx.workbook(spread);
};
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`Workbook`](GC.Spread.Sheets.Workbook.md) | 工作簿 |

#### Returns

[`Workbook`](GC.Spread.Sheets.Workbook.md)

如果未设置任何值,则返回工作簿;否则,没有返回值
