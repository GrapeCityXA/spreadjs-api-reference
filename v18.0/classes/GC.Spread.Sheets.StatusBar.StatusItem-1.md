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

状态项的基类提供基本值显示和相关的上下文菜单项功能

**`代码示例`**
``` javascript
let StatusItem = GC.Spread.Sheets.StatusBar.StatusItem;
let labelItem = new StatusItem('labelItem', {menuContent: 'label', value: 'text'});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 名称是唯一标识符，在上下文菜单和状态栏中需要 |
| `options?` | [`IStatusItemOptions`](../interfaces/GC.Spread.Sheets.StatusBar.StatusItem.IStatusItemOptions.md) | - |

## Methods

### <a id="onbind" name="onbind"></a> onBind

▸ **onBind**(`context`): `void`

绑定上下文。可以重写以添加与上下文相关的事件监听

**`override`**

**`代码示例`**
``` javascript
LabelItem.prototype.onBind = function (context) {
  // 关于上下文做一些事请
}
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context` | [`Workbook`](GC.Spread.Sheets.Workbook.md) | 执行上下文 |

#### Returns

`void`

___

### <a id="oncreateitemview" name="oncreateitemview"></a> onCreateItemView

▸ **onCreateItemView**(`container`): `void`

在状态栏上创建item元素。可以覆盖自定义项

**`override`**

**`代码示例`**
``` javascript
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

将状态栏部署为解除绑定上下文，删除所有监听并部署所有元素

**`override`**

**`代码示例`**
``` javascript
let StatusItem = GC.Spread.Sheets.StatusBar.StatusItem;
function LabelItem (name, options) {
  StatusItem.call(this, name, options);
}
LabelItem.prototype = new StatusItem();
LabelItem.prototype.onDispose = function () {
  // 部署当前项
  // 然后调用超级部署
  StatusItem.prototype.onDispose.call(this);
}
```

#### Returns

`void`

___

### <a id="onunbind" name="onunbind"></a> onUnbind

▸ **onUnbind**(): `void`

取消绑定上下文。可以重写以删除与上下文相关的事件监听

**`override`**

**`代码示例`**
``` javascript
LabelItem.prototype.onUnbind = function () {
  // 删除与上下文相关的事件监听
}
```

#### Returns

`void`

___

### <a id="onupdate" name="onupdate"></a> onUpdate

▸ **onUpdate**(`content?`): `void`

可以在其中实现与更新相关的操作当当前项需要更新时，用户应该调用onUpdate
可以在其中实现与更新相关的操作当当前项需要更新时，用户应该调用onUpdate
在超类中的默认操作是可见地更新当前项

**`override`**

**`代码示例`**
``` javascript
let StatusItem = GC.Spread.Sheets.StatusBar.StatusItem;
function LabelItem (name, options) {
  StatusItem.call(this, name, options);
}
LabelItem.prototype = new StatusItem();
LabelItem.prototype.onUpdate = function () {
  StatusItem.prototype.onUpdate.call(this);
  // 更新项
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `content?` | `string` | 要显示在 StatusItem 上的字符串内容 |

#### Returns

`void`
