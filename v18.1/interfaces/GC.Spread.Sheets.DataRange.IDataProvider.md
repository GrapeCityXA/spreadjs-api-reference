# Interface: IDataProvider

[Sheets](../modules/GC.Spread.Sheets.md).[DataRange](../modules/GC.Spread.Sheets.DataRange.md).IDataProvider

## Table of contents

### Properties

- [host](GC.Spread.Sheets.DataRange.IDataProvider.md#host)

### Methods

- [fromJSON](GC.Spread.Sheets.DataRange.IDataProvider.md#fromjson)
- [getSpans](GC.Spread.Sheets.DataRange.IDataProvider.md#getspans)
- [getStyle](GC.Spread.Sheets.DataRange.IDataProvider.md#getstyle)
- [getValue](GC.Spread.Sheets.DataRange.IDataProvider.md#getvalue)
- [onClear](GC.Spread.Sheets.DataRange.IDataProvider.md#onclear)
- [onColumnChange](GC.Spread.Sheets.DataRange.IDataProvider.md#oncolumnchange)
- [onContextMenu](GC.Spread.Sheets.DataRange.IDataProvider.md#oncontextmenu)
- [onCopy](GC.Spread.Sheets.DataRange.IDataProvider.md#oncopy)
- [onDestroy](GC.Spread.Sheets.DataRange.IDataProvider.md#ondestroy)
- [onDoubleClick](GC.Spread.Sheets.DataRange.IDataProvider.md#ondoubleclick)
- [onKeyDown](GC.Spread.Sheets.DataRange.IDataProvider.md#onkeydown)
- [onKeyUp](GC.Spread.Sheets.DataRange.IDataProvider.md#onkeyup)
- [onMouseDown](GC.Spread.Sheets.DataRange.IDataProvider.md#onmousedown)
- [onMouseMove](GC.Spread.Sheets.DataRange.IDataProvider.md#onmousemove)
- [onMouseUp](GC.Spread.Sheets.DataRange.IDataProvider.md#onmouseup)
- [onMouseWheel](GC.Spread.Sheets.DataRange.IDataProvider.md#onmousewheel)
- [onRowChange](GC.Spread.Sheets.DataRange.IDataProvider.md#onrowchange)
- [setValue](GC.Spread.Sheets.DataRange.IDataProvider.md#setvalue)
- [toJSON](GC.Spread.Sheets.DataRange.IDataProvider.md#tojson)
- [undo](GC.Spread.Sheets.DataRange.IDataProvider.md#undo)

## Properties

### <a id="host" name="host"></a> host

• **host**: [`DataRange`](../classes/GC.Spread.Sheets.DataRange.DataRange.md)

数据提供者宿主

## Methods

### <a id="fromjson" name="fromjson"></a> fromJSON

▸ `Optional` **fromJSON**(`options`): `void`

实现此钩子以处理反序列化。

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | `Object` |
| `options.typeName` | `string` |

#### Returns

`void`

___

### <a id="getspans" name="getspans"></a> getSpans

▸ `Optional` **getSpans**(`row`, `col`, `rowCount`, `colCount`): [`Range`](../classes/GC.Spread.Sheets.Range.md)[]

实现此钩子以为数据范围单元格提供跨度。`row`、`col`、`rowCount`和`colCount`参数基于数据范围轴。

#### Parameters

| Name | Type |
| :------ | :------ |
| `row` | `number` |
| `col` | `number` |
| `rowCount` | `number` |
| `colCount` | `number` |

#### Returns

[`Range`](../classes/GC.Spread.Sheets.Range.md)[]

___

### <a id="getstyle" name="getstyle"></a> getStyle

▸ `Optional` **getStyle**(`row`, `col`): [`Style`](../classes/GC.Spread.Sheets.Style.md)

实现此钩子以为数据范围单元格提供样式。`row`和`col`参数基于数据范围轴。它应该返回`GC.Spread.Sheets.Style`类型的样式，否则表示无法从数据提供者获取样式，将继续从工作表模型获取样式。

#### Parameters

| Name | Type |
| :------ | :------ |
| `row` | `number` |
| `col` | `number` |

#### Returns

[`Style`](../classes/GC.Spread.Sheets.Style.md)

___

### <a id="getvalue" name="getvalue"></a> getValue

▸ `Optional` **getValue**(`row`, `col`): `unknown`

实现此钩子以为数据范围单元格提供值。`row`和`col`参数基于数据范围轴。如果返回`undefined`，表示无法从数据提供者获取值，将继续从工作表模型获取值。

#### Parameters

| Name | Type |
| :------ | :------ |
| `row` | `number` |
| `col` | `number` |

#### Returns

`unknown`

___

### <a id="onclear" name="onclear"></a> onClear

▸ `Optional` **onClear**(`row`, `col`, `rowCount`, `colCount`, `changes`): `boolean`

实现此钩子以处理清除内容操作。返回`true`表示阻止工作表的清除操作。返回`false`表示阻止清除数据范围内容。默认为`false`。

#### Parameters

| Name | Type |
| :------ | :------ |
| `row` | `number` |
| `col` | `number` |
| `rowCount` | `number` |
| `colCount` | `number` |
| `changes` | `any`[] |

#### Returns

`boolean`

___

### <a id="oncolumnchange" name="oncolumnchange"></a> onColumnChange

▸ `Optional` **onColumnChange**(`col`, `colCount`, `changeType`, `changes`): `void`

实现此钩子以接收更改的列信息。`col`和`colCount`参数基于数据范围轴。如果需要撤销/重做，请将更改发布到`changes`参数中。

#### Parameters

| Name | Type |
| :------ | :------ |
| `col` | `number` |
| `colCount` | `number` |
| `changeType` | ``"delete"`` \| ``"add"`` |
| `changes` | `any`[] |

#### Returns

`void`

___

### <a id="oncontextmenu" name="oncontextmenu"></a> onContextMenu

▸ `Optional` **onContextMenu**(`row`, `col`, `e`): `boolean`

实现此钩子以处理鼠标右键菜单操作。`row`和`col`参数基于数据范围轴。返回`true`表示阻止后续工作表操作。默认为false。

#### Parameters

| Name | Type |
| :------ | :------ |
| `row` | `number` |
| `col` | `number` |
| `e` | `MouseEvent` |

#### Returns

`boolean`

___

### <a id="oncopy" name="oncopy"></a> onCopy

▸ `Optional` **onCopy**(`name`): `boolean` \| { `dataProvider`: [`IDataProvider`](GC.Spread.Sheets.DataRange.IDataProvider.md) ; `name`: `string`  }

实现此钩子以处理复制操作。输入参数`name`是复制的数据范围名称，需要返回一个不同的新数据范围`name`和数据提供者实例。返回`true`表示阻止工作表的复制操作。返回`false`表示阻止复制数据范围。默认为`false`。

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |

#### Returns

`boolean` \| { `dataProvider`: [`IDataProvider`](GC.Spread.Sheets.DataRange.IDataProvider.md) ; `name`: `string`  }

___

### <a id="ondestroy" name="ondestroy"></a> onDestroy

▸ `Optional` **onDestroy**(): `void`

实现此钩子以处理销毁操作。

#### Returns

`void`

___

### <a id="ondoubleclick" name="ondoubleclick"></a> onDoubleClick

▸ `Optional` **onDoubleClick**(`row`, `col`, `e`): `boolean`

实现此钩子以处理鼠标双击操作。`row`和`col`参数基于数据范围轴。返回`true`表示阻止后续工作表操作。默认为false。

#### Parameters

| Name | Type |
| :------ | :------ |
| `row` | `number` |
| `col` | `number` |
| `e` | `MouseEvent` |

#### Returns

`boolean`

___

### <a id="onkeydown" name="onkeydown"></a> onKeyDown

▸ `Optional` **onKeyDown**(`row`, `col`, `e`): `boolean`

实现此钩子以处理按键按下操作。`row`和`col`参数基于数据范围轴。返回`true`表示阻止后续工作表操作。默认为false。

#### Parameters

| Name | Type |
| :------ | :------ |
| `row` | `number` |
| `col` | `number` |
| `e` | `KeyboardEvent` |

#### Returns

`boolean`

___

### <a id="onkeyup" name="onkeyup"></a> onKeyUp

▸ `Optional` **onKeyUp**(`row`, `col`, `e`): `boolean`

实现此钩子以处理按键释放操作。`row`和`col`参数基于数据范围轴。返回`true`表示阻止后续工作表操作。默认为false。

#### Parameters

| Name | Type |
| :------ | :------ |
| `row` | `number` |
| `col` | `number` |
| `e` | `KeyboardEvent` |

#### Returns

`boolean`

___

### <a id="onmousedown" name="onmousedown"></a> onMouseDown

▸ `Optional` **onMouseDown**(`row`, `col`, `e`): `boolean`

实现此钩子以处理鼠标按下操作。`row`和`col`参数基于数据范围轴。返回`true`表示阻止后续工作表操作。默认为false。

#### Parameters

| Name | Type |
| :------ | :------ |
| `row` | `number` |
| `col` | `number` |
| `e` | `MouseEvent` |

#### Returns

`boolean`

___

### <a id="onmousemove" name="onmousemove"></a> onMouseMove

▸ `Optional` **onMouseMove**(`row`, `col`, `e`): `boolean`

实现此钩子以处理鼠标移动操作。`row`和`col`参数基于数据范围轴。返回`true`表示阻止后续工作表操作。默认为false。

#### Parameters

| Name | Type |
| :------ | :------ |
| `row` | `number` |
| `col` | `number` |
| `e` | `MouseEvent` |

#### Returns

`boolean`

___

### <a id="onmouseup" name="onmouseup"></a> onMouseUp

▸ `Optional` **onMouseUp**(`row`, `col`, `e`): `boolean`

实现此钩子以处理鼠标释放操作。`row`和`col`参数基于数据范围轴。返回`true`表示阻止后续工作表操作。默认为false。

#### Parameters

| Name | Type |
| :------ | :------ |
| `row` | `number` |
| `col` | `number` |
| `e` | `MouseEvent` |

#### Returns

`boolean`

___

### <a id="onmousewheel" name="onmousewheel"></a> onMouseWheel

▸ `Optional` **onMouseWheel**(`deltaX`, `deltaY`, `e`): `boolean`

实现此钩子以处理鼠标滚轮操作。返回`true`表示阻止后续工作表操作。默认为false。

#### Parameters

| Name | Type |
| :------ | :------ |
| `deltaX` | `number` |
| `deltaY` | `number` |
| `e` | `MouseEvent` |

#### Returns

`boolean`

___

### <a id="onrowchange" name="onrowchange"></a> onRowChange

▸ `Optional` **onRowChange**(`row`, `rowCount`, `changeType`, `changes`): `void`

实现此钩子以接收更改的行信息。`row`和`rowCount`参数基于数据范围轴。如果需要撤销/重做，请将更改发布到`changes`参数中。

#### Parameters

| Name | Type |
| :------ | :------ |
| `row` | `number` |
| `rowCount` | `number` |
| `changeType` | ``"delete"`` \| ``"add"`` |
| `changes` | `any`[] |

#### Returns

`void`

___

### <a id="setvalue" name="setvalue"></a> setValue

▸ `Optional` **setValue**(`row`, `col`, `value`, `changes`): `boolean`

实现此钩子以接收来自数据范围的更改值。`row`和`col`参数基于数据范围轴。如果需要撤销/重做，请将更改发布到`changes`参数中。如果返回`true`，表示成功将值设置到数据提供者，将阻止将值设置到工作表模型。

#### Parameters

| Name | Type |
| :------ | :------ |
| `row` | `number` |
| `col` | `number` |
| `value` | `unknown` |
| `changes` | `any`[] |

#### Returns

`boolean`

___

### <a id="tojson" name="tojson"></a> toJSON

▸ `Optional` **toJSON**(): `Object`

实现此钩子以处理序列化。

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `typeName` | `string` |

___

### <a id="undo" name="undo"></a> undo

▸ `Optional` **undo**(`change`): `void`

实现此钩子以处理撤销操作。输入参数`change`是用户在相应钩子中创建的。

#### Parameters

| Name | Type |
| :------ | :------ |
| `change` | `any` |

#### Returns

`void`
