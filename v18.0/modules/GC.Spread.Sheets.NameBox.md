# Namespace: NameBox

[Spread](GC.Spread.md).[Sheets](GC.Spread.Sheets.md).NameBox

## Table of contents

### Classes

- [NameBox](../classes/GC.Spread.Sheets.NameBox.NameBox.md)

### Interfaces

- [INameBoxOptions](../interfaces/GC.Spread.Sheets.NameBox.INameBoxOptions.md)

### Functions

- [findControl](GC.Spread.Sheets.NameBox.md#findcontrol)

## Functions

### <a id="findcontrol" name="findcontrol"></a> findControl

▸ **findControl**(`host`): [`NameBox`](../classes/GC.Spread.Sheets.NameBox.NameBox.md)

Gets the NameBox instance by the host element.

**`代码示例`**
``` javascript
var spread = new GC.Spread.Sheets.Workbook("ss");
var nameBox = new GC.Spread.Sheets.NameBox.NameBox('nameBox');
nameBox.bind(spread);
var nameBoxInstance = GC.Spread.Sheets.NameBox.findControl('nameBox');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `host` | `string` \| `HTMLElement` | 宿主元素或宿主元素id |

#### Returns

[`NameBox`](../classes/GC.Spread.Sheets.NameBox.NameBox.md)

The NameBox instance.
