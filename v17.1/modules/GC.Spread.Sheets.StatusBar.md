# Namespace: StatusBar

[Spread](GC.Spread.md).[Sheets](GC.Spread.Sheets.md).StatusBar

## Table of contents

### Namespaces

- [StatusItem](GC.Spread.Sheets.StatusBar.StatusItem.md)

### Classes

- [StatusBar](../classes/GC.Spread.Sheets.StatusBar.StatusBar.md)
- [StatusItem](../classes/GC.Spread.Sheets.StatusBar.StatusItem-1.md)

### Interfaces

- [IStatusBarOptions](../interfaces/GC.Spread.Sheets.StatusBar.IStatusBarOptions.md)

### Functions

- [findControl](GC.Spread.Sheets.StatusBar.md#findcontrol)

## Functions

### <a id="findcontrol" name="findcontrol"></a> findControl

▸ **findControl**(`host`): [`StatusBar`](../classes/GC.Spread.Sheets.StatusBar.StatusBar.md)

通过宿主元素获取状态栏实例

**`代码示例`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var spanItem = new GC.Spread.Sheets.StatusBar.StatusItem('spanItem', {menuContent: 'current span', value: 'span test'});
var statusBar = new GC.Spread.Sheets.StatusBar.StatusBar(
document.getElementById('statusBar'),
{ items: [spanItem] }
);
statusBar.bind(spread);
var statusBarInstance = GC.Spread.Sheets.StatusBar.findControl('statusBar');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `host` | `string` \| `HTMLElement` | 宿主元素或宿主元素id |

#### Returns

[`StatusBar`](../classes/GC.Spread.Sheets.StatusBar.StatusBar.md)

状态栏实例
