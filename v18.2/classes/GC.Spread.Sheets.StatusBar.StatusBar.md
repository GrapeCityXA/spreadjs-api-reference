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

表示状态栏。

**`example`**
```
let statusBar = new GC.Spread.Sheets.StatusBar.StatusBar(document.getElementById('statusBar'),
  {items: [new GC.Spread.Sheets.StatusBar.StatusItem('labelItem', {menuContent: 'label'})]});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `host` | `HTMLElement` | DOM元素。 |
| `options?` | [`IStatusBarOptions`](../interfaces/GC.Spread.Sheets.StatusBar.IStatusBarOptions.md) | - |

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`item`, `position`): `boolean`

向状态栏添加项目实例。

**`example`**
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
| `item` | [`StatusItem`](GC.Spread.Sheets.StatusBar.StatusItem-1.md) | StatusItem子类的实例。子类继承自StatusItem。 |
| `position` | `number` | 项目在所有项目数组中的索引位置。从0开始。项目的显示位置也与对齐方式有关。如果位置无效或未定义，则按默认方式放置。 |

#### Returns

`boolean`

添加项目的结果。如果添加成功返回true，否则失败。

___

### <a id="all" name="all"></a> all

▸ **all**(): [`StatusItem`](GC.Spread.Sheets.StatusBar.StatusItem-1.md)[]

获取所有项目列表。

**`example`**
```
let spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
let statusBar = new GC.Spread.Sheets.StatusBar.StatusBar(document.getElementById('statusBar'));
statusBar.bind(spread);
let itemList = statusBar.all();
statusBar.remove(itemList[0]);
```

#### Returns

[`StatusItem`](GC.Spread.Sheets.StatusBar.StatusItem-1.md)[]

状态栏上的项目列表。

___

### <a id="bind" name="bind"></a> bind

▸ **bind**(`context`): `void`

绑定状态栏的上下文。

**`example`**
```
let spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
let statusBar = new GC.Spread.Sheets.StatusBar.StatusBar(document.getElementById('statusBar'));
statusBar.bind(spread);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context` | [`Workbook`](GC.Spread.Sheets.Workbook.md) | 状态栏的上下文。上下文可以触发状态栏的状态变化。这里的上下文是GC.Spread.Sheets.Workbook的实例。 |

#### Returns

`void`

___

### <a id="dispose" name="dispose"></a> dispose

▸ **dispose**(): `void`

释放状态栏并解绑所有事件。

**`example`**
```
let spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
let statusBar = new GC.Spread.Sheets.StatusBar.StatusBar(document.getElementById('statusBar'));
statusBar.bind(spread);
// do something
statusBar.dispose();
```

#### Returns

`void`

___

### <a id="get" name="get"></a> get

▸ **get**(`itemName`): [`StatusItem`](GC.Spread.Sheets.StatusBar.StatusItem-1.md)

通过项目名称获取项目。

**`example`**
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

| Name | Type | Description |
| :------ | :------ | :------ |
| `itemName` | `string` | 项目名称 |

#### Returns

[`StatusItem`](GC.Spread.Sheets.StatusBar.StatusItem-1.md)

指定名称的StatusItem实例

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`itemName`): `boolean`

从状态栏中移除项目。

**`example`**
```
let StatusItem = GC.Spread.Sheets.StatusBar.StatusItem;
let spanItemName = 'spanItemName';
let spanItem = new StatusItem(spanItemName, {menuContent: 'span', value: 'spanValue'});
let spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
let statusBar = new GC.Spread.Sheets.StatusBar.StatusBar(document.getElementById('statusBar'));
statusBar.bind(spread);
statusBar.add(spanItem);
// do something
statusBar.remove(spanItemName);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `itemName` | `string` | StatusItem的名称 |

#### Returns

`boolean`

如果为true表示移除成功，否则失败

___

### <a id="unbind" name="unbind"></a> unbind

▸ **unbind**(): `void`

解绑状态栏的上下文。

**`example`**
```
let spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
let statusBar = new GC.Spread.Sheets.StatusBar.StatusBar(document.getElementById('statusBar'));
statusBar.bind(spread);
// do something
statusBar.unbind();
```

#### Returns

`void`

___

### <a id="update" name="update"></a> update

▸ **update**(): `void`

更新状态栏。

**`example`**
```
let spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
let statusBar = new GC.Spread.Sheets.StatusBar.StatusBar(document.getElementById('statusBar'));
statusBar.update();
```

#### Returns

`void`
