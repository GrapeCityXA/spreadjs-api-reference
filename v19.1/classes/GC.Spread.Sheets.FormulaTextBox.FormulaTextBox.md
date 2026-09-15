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

表示公式文本框。

**`example`**
```javascript
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
| `host` | `HTMLElement` | DOM元素。可以是INPUT、TEXTAREA或可编辑的DIV。 |
| `options?` | [`IFormulaTextBoxOptions`](../interfaces/GC.Spread.Sheets.FormulaTextBox.IFormulaTextBoxOptions.md) | 选项。默认为 {rangeSelectMode: false, absoluteReference: false} |

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`functionDescription`): `void`

添加自定义函数描述。

**`example`**
```javascript
// 筛选函数描述
function filterFunctionDescription(functionDescription) {
    // 对函数描述进行筛选处理
    return functionDescription;
}

// 重写 add 方法
var originalAdd = GC.Spread.Sheets.FormulaTextBox.FormulaTextBox.prototype.add;
GC.Spread.Sheets.FormulaTextBox.FormulaTextBox.prototype.add = function (functionDescription) {
    // 先筛选函数描述，再调用原始方法
    originalAdd.call(this, filterFunctionDescription(functionDescription));
};
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `functionDescription` | [`IFunctionDescription`](../interfaces/GC.Spread.CalcEngine.Functions.IFunctionDescription.md) \| [`IFunctionDescription`](../interfaces/GC.Spread.CalcEngine.Functions.IFunctionDescription.md)[] | 要添加的函数描述，可传入单个对象或对象数组。有关详细信息，请参阅备注。 |

#### Returns

`void`

___

### <a id="autocomplete" name="autocomplete"></a> autoComplete

▸ **autoComplete**(`value?`): `boolean`

获取或设置文本框是否使用自动完成。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(_getElementById('ss'), { sheetCount: 2 });
var div = document.createElement('div');
div.id = 'fbx';
div.style.width = '300px';
div.style.height = '50px';
div.setAttribute('contentEditable', 'true');
document.getElementById('panel').appendChild(div);
var formulaTextBox = new GC.Spread.Sheets.FormulaTextBox.FormulaTextBox(div);
formulaTextBox.workbook(spread);
formulaTextBox.autoComplete(false);

// 在公式文本框输入元素中输入"=SUM"公式前缀，函数提示框将不会显示
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 编辑时是否使用自动完成。 |

#### Returns

`boolean`

如果未设置值，则返回文本框是否使用自动完成；否则没有返回值。

___

### <a id="destroy" name="destroy"></a> destroy

▸ **destroy**(): `void`

从公式文本框中移除宿主并移除所有绑定事件。

**`example`**
```javascript
var div = document.createElement('div');
div.id = 'fbx';
div.style.width = '300px';
div.style.height = '50px';
div.setAttribute('contentEditable', 'true');
document.body.appendChild(div);
var formulaTextBox = new GC.Spread.Sheets.FormulaTextBox.FormulaTextBox(div);
formulaTextBox.workbook(spread);

// 销毁公式文本框对象
formulaTextBox.destroy();
```

#### Returns

`void`

___

### <a id="refresh" name="refresh"></a> refresh

▸ **refresh**(`ignoreEditing?`): `void`

使用活动单元格刷新公式文本框。

**`example`**
```javascript
var div = document.createElement('div');
div.id = 'fbx';
div.style.width = '300px';
div.style.height = '50px';
div.style.position = 'absolute';
div.style.right = '100px';
div.style.top = '200px';
div.style.border = '3px solid red';
div.setAttribute('contentEditable', 'true');
document.body.appendChild(div);
var formulaTextBox = new GC.Spread.Sheets.FormulaTextBox.FormulaTextBox(div);
formulaTextBox.workbook(spread);

// 挂起事件并为活动单元格设置值。
spread.suspendEvent();
spread.getActiveSheet().setValue(0, 0, 100);
spread.resumeEvent();

// 刷新公式文本框
formulaTextBox.refresh();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ignoreEditing?` | `boolean` | 设置为true以避免公式文本框进入编辑模式。 |

#### Returns

`void`

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`name`): `void`

移除自定义函数描述。

**`example`**
```javascript
// 重写 add 方法
var originalAdd = GC.Spread.Sheets.FormulaTextBox.FormulaTextBox.prototype.add;
GC.Spread.Sheets.FormulaTextBox.FormulaTextBox.prototype.add = function (functionDescription) {
    originalAdd.call(this, functionDescription);
    this.remove('SUM');
};
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 自定义函数描述名称。 |

#### Returns

`void`

___

### <a id="showhelp" name="showhelp"></a> showHelp

▸ **showHelp**(`value?`): `any`

获取或设置是否显示函数的帮助提示。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(_getElementById('ss'), { sheetCount: 2 });
var div = document.createElement('div');
div.id = 'fbx';
div.style.width = '300px';
div.style.height = '50px';
div.setAttribute('contentEditable', 'true');
document.getElementById('panel').appendChild(div);
var formulaTextBox = new GC.Spread.Sheets.FormulaTextBox.FormulaTextBox(div);
formulaTextBox.workbook(spread);
formulaTextBox.showHelp(false);

// 在公式文本框输入元素中输入"=SUM"公式前缀，函数提示（自动完成）框将显示，但帮助函数不会显示
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 编辑时是否显示函数的帮助提示。 |

#### Returns

`any`

如果未设置值，则返回文本框在编辑时是否显示函数的帮助提示；否则没有返回值。

___

### <a id="text" name="text"></a> text

▸ **text**(`value?`): `string`

获取或设置文本。

**`example`**
```javascript
var spread = new GC.Spread.Sheets.Workbook(_getElementById('ss'), { sheetCount: 2 });
var div = document.createElement('div');
div.id = 'fbx';
div.style.width = '300px';
div.style.height = '50px';
div.setAttribute('contentEditable', 'true');
document.getElementById('panel').appendChild(div);
var formulaTextBox = new GC.Spread.Sheets.FormulaTextBox.FormulaTextBox(div);
formulaTextBox.workbook(spread);
formulaTextBox.text('this is text');
// 工作表将处于编辑状态，文本值将显示在公式文本框输入框中。
console.log(formulaTextBox.text()); // 'this is text'
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 文本。 |

#### Returns

`string`

如果未设置值，则返回文本；否则没有返回值。

___

### <a id="workbook" name="workbook"></a> workbook

▸ **workbook**(`value?`): [`Workbook`](GC.Spread.Sheets.Workbook.md)

获取或设置与公式文本框一起使用的Workbook组件。

**`example`**
```javascript
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
| `value?` | [`Workbook`](GC.Spread.Sheets.Workbook.md) | Workbook组件。 |

#### Returns

[`Workbook`](GC.Spread.Sheets.Workbook.md)

如果未设置值，则返回workbook组件；否则没有返回值。
