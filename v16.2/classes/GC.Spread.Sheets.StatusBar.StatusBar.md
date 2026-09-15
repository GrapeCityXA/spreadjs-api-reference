# Class: StatusBar

[Sheets](../modules/GC.Spread.Sheets.md).[StatusBar](../modules/GC.Spread.Sheets.StatusBar.md).StatusBar

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.StatusBar.StatusBar.md#constructor)

### Methods

- [add](GC.Spread.Sheets.StatusBar.StatusBar.md#add)
- [all](GC.Spread.Sheets.StatusBar.StatusBar.md#all)
- [bind](GC.Spread.Sheets.StatusBar.StatusBar.md#bind)
- [dispose](GC.Spread.Sheets.StatusBar.StatusBar.md#dispose)
- [get](GC.Spread.Sheets.StatusBar.StatusBar.md#get)
- [remove](GC.Spread.Sheets.StatusBar.StatusBar.md#remove)
- [unbind](GC.Spread.Sheets.StatusBar.StatusBar.md#unbind)
- [update](GC.Spread.Sheets.StatusBar.StatusBar.md#update)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new StatusBar**(`host`, `options?`)

状态栏

**`代码示例`**
```
let statusBar = new GC.Spread.Sheets.StatusBar.StatusBar(document.getElementById('statusBar'),
  {items: [new GC.Spread.Sheets.StatusBar.StatusItem('labelItem', {menuContent: 'label'})]});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `host` | `HTMLElement` | DOM元素 |
| `options?` | [`IStatusBarOptions`](../interfaces/GC.Spread.Sheets.StatusBar.IStatusBarOptions.md) | - |

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`item`, `position`): `boolean`

将项实例添加到StatusBar

**`代码示例`**
```
let StatusItem = GC.Spread.Sheets.StatusBar.StatusItem;
let spanItem = new StatusItem('spanItemName', {menuContent: 'span', value: 'spanValue'});
let spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
let statusBar = new GC.Spread.Sheets.StatusBar.StatusBar(document.getElementById('statusBar'));
statusBar.bind(spread);
statusBar.add(spanItem);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | [`StatusItem`](GC.Spread.Sheets.StatusBar.StatusItem.md) | StatusItem子级的实例 子级从StatusItem扩展 |
| `position` | `number` | 位置是所有项数组中的项索引 从0开始项显示位置也与对齐相关 如果位置无效或不确定,则默认放置它 |

#### Returns

`boolean`

添加项结果 如果添加成功,则返回true,否则失败

___

### <a id="all" name="all"></a> all

▸ **all**(): [`StatusItem`](GC.Spread.Sheets.StatusBar.StatusItem.md)[]

获取所有项列表

**`代码示例`**
```
let spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
let statusBar = new GC.Spread.Sheets.StatusBar.StatusBar(document.getElementById('statusBar'));
statusBar.bind(spread);
let itemList = statusBar.all();
statusBar.remove(itemList[0]);
```

#### Returns

[`StatusItem`](GC.Spread.Sheets.StatusBar.StatusItem.md)[]

状态栏上的项列表

___

### <a id="bind" name="bind"></a> bind

▸ **bind**(`context`): `void`

绑定StatusBar的上下文

**`代码示例`**
```
let spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
let statusBar = new GC.Spread.Sheets.StatusBar.StatusBar(document.getElementById('statusBar'));
statusBar.bind(spread);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context` | [`Workbook`](GC.Spread.Sheets.Workbook.md) | StatusBar的上下文 上下文可以触发StatusBar的状态更改 这里的上下文是GC.Spread.Sheets.Workbook的实例 |

#### Returns

`void`

___

### <a id="dispose" name="dispose"></a> dispose

▸ **dispose**(): `void`

处置StatusBar并解除所有事件的绑定

**`代码示例`**
```
let spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
let statusBar = new GC.Spread.Sheets.StatusBar.StatusBar(document.getElementById('statusBar'));
statusBar.bind(spread);
// 做一些事请
statusBar.dispose();
```

#### Returns

`void`

___

### <a id="get" name="get"></a> get

▸ **get**(`itemName`): [`StatusItem`](GC.Spread.Sheets.StatusBar.StatusItem.md)

通过项名称获取项

**`代码示例`**
```
let StatusItem = GC.Spread.Sheets.StatusBar.StatusItem;
let spanItemName = 'spanItemName';
let spanItem = new StatusItem(spanItemName, {menuContent: 'span', value: 'spanValue'});
let spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
let statusBar = new GC.Spread.Sheets.StatusBar.StatusBar(document.getElementById('statusBar'));
statusBar.bind(spread);
statusBar.add(spanItem);
let spanItemInstance = statusBar.get(spanItemName);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `itemName` | `string` |

#### Returns

[`StatusItem`](GC.Spread.Sheets.StatusBar.StatusItem.md)

指定itemName的StatusItem

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`itemName`): `boolean`

从状态栏中删除该项

**`代码示例`**
```
let StatusItem = GC.Spread.Sheets.StatusBar.StatusItem;
let spanItemName = 'spanItemName';
let spanItem = new StatusItem(spanItemName, {menuContent: 'span', value: 'spanValue'});
let spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
let statusBar = new GC.Spread.Sheets.StatusBar.StatusBar(document.getElementById('statusBar'));
statusBar.bind(spread);
statusBar.add(spanItem);
// 做一些事请
statusBar.remove(spanItemName);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `itemName` | `string` | StatusItem的名称 |

#### Returns

`boolean`

如果为true表示删除成功,否则为失败

___

### <a id="unbind" name="unbind"></a> unbind

▸ **unbind**(): `void`

取消绑定StatusBar的上下文

**`代码示例`**
```
let spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
let statusBar = new GC.Spread.Sheets.StatusBar.StatusBar(document.getElementById('statusBar'));
statusBar.bind(spread);
// 做一些事请
statusBar.unbind();
```

#### Returns

`void`

___

### <a id="update" name="update"></a> update

▸ **update**(): `void`

更新状态栏

**`代码示例`**
```
let spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
let statusBar = new GC.Spread.Sheets.StatusBar.StatusBar(document.getElementById('statusBar'));
statusBar.update();
```

#### Returns

`void`
