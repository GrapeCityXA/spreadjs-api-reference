# Class: StatusItem

[Sheets](../modules/GC.Spread.Sheets.md).[StatusBar](../modules/GC.Spread.Sheets.StatusBar.md).StatusItem

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.StatusBar.StatusItem-1.md#constructor)

### Methods

- [onBind](GC.Spread.Sheets.StatusBar.StatusItem-1.md#onbind)
- [onCreateItemView](GC.Spread.Sheets.StatusBar.StatusItem-1.md#oncreateitemview)
- [onDispose](GC.Spread.Sheets.StatusBar.StatusItem-1.md#ondispose)
- [onUnbind](GC.Spread.Sheets.StatusBar.StatusItem-1.md#onunbind)
- [onUpdate](GC.Spread.Sheets.StatusBar.StatusItem-1.md#onupdate)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new StatusItem**(`name`, `options?`)

状态项的基础类，提供基本的值显示和相关的上下文菜单项功能。

**`example`**
```
let StatusItem = GC.Spread.Sheets.StatusBar.StatusItem;
let labelItem = new StatusItem('labelItem', {menuContent: 'label', value: 'text'});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 名称是唯一标识符，在上下文菜单和状态栏中都需要。 |
| `options?` | [`IStatusItemOptions`](../interfaces/GC.Spread.Sheets.StatusBar.StatusItem.IStatusItemOptions.md) | - |

## Methods

### <a id="onbind" name="onbind"></a> onBind

▸ **onBind**(`context`): `void`

绑定上下文。可以重写以添加与上下文相关的事件监听器。

**`override`**

**`example`**
```
LabelItem.prototype.onBind = function (context) {
  // 处理上下文相关操作
}
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context` | [`Workbook`](GC.Spread.Sheets.Workbook.md) | 状态栏项的执行上下文。 |

#### Returns

`void`

___

### <a id="oncreateitemview" name="oncreateitemview"></a> onCreateItemView

▸ **onCreateItemView**(`container`): `void`

在状态栏上创建项目元素。可以重写以自定义项目。

**`override`**

**`example`**
```
let StatusItem = GC.Spread.Sheets.StatusBar.StatusItem;
function LabelItem (name, options) {
  StatusItem.call(this, name, options);
}
LabelItem.prototype = new StatusItem();
LabelItem.prototype.onCreateItemView = function (container) {
  let item = document.createElement('div');
  item.innerText = this.value;
  container.appendChild(item);
  // 为容器添加事件监听器
}
statusBar.add(new LabelItem('labelItem', {menuContent: 'label', value: 'options test'}));
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `container` | `HTMLElement` |

#### Returns

`void`

___

### <a id="ondispose" name="ondispose"></a> onDispose

▸ **onDispose**(): `void`

销毁状态栏以解绑上下文，移除所有监听器并销毁所有元素。

**`override`**

**`example`**
```
let StatusItem = GC.Spread.Sheets.StatusBar.StatusItem;
function LabelItem (name, options) {
  StatusItem.call(this, name, options);
}
LabelItem.prototype = new StatusItem();
LabelItem.prototype.onDispose = function () {
  // 销毁当前项目
  // 然后调用父类的dispose方法
  StatusItem.prototype.onDispose.call(this);
}
```

#### Returns

`void`

___

### <a id="onunbind" name="onunbind"></a> onUnbind

▸ **onUnbind**(): `void`

解绑上下文。可以重写以移除与上下文相关的事件监听器。

**`override`**

**`example`**
```
LabelItem.prototype.onUnbind = function () {
  // 移除与上下文相关的事件监听器
}
```

#### Returns

`void`

___

### <a id="onupdate" name="onupdate"></a> onUpdate

▸ **onUpdate**(`content?`): `void`

状态栏更新的回调函数。在状态栏绑定或更新函数时，或状态栏在上下文菜单中的选中状态改变时调用。
可以在其中实现更新相关的操作。当当前项目需要更新时，用户也应该调用onUpdate。
父类中的默认操作是根据visible属性更新当前项目。

**`override`**

**`example`**
```
let StatusItem = GC.Spread.Sheets.StatusBar.StatusItem;
function LabelItem (name, options) {
    StatusItem.call(this, name, options);
}
LabelItem.prototype = new StatusItem();
LabelItem.prototype.onUpdate = function () {
    StatusItem.prototype.onUpdate.call(this);
    // 更新项目。
}
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `content?` | `string` | 要在StatusItem上显示的字符串内容。 |

#### Returns

`void`
