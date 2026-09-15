# Class: DataChart

[Sheets](../modules/GC.Spread.Sheets.md).[DataCharts](../modules/GC.Spread.Sheets.DataCharts.md).DataChart

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.DataCharts.DataChart.md#constructor)

### Methods

- [allowMove](GC.Spread.Sheets.DataCharts.DataChart.md#allowmove)
- [allowResize](GC.Spread.Sheets.DataCharts.DataChart.md#allowresize)
- [alt](GC.Spread.Sheets.DataCharts.DataChart.md#alt)
- [canPrint](GC.Spread.Sheets.DataCharts.DataChart.md#canprint)
- [dynamicMove](GC.Spread.Sheets.DataCharts.DataChart.md#dynamicmove)
- [dynamicSize](GC.Spread.Sheets.DataCharts.DataChart.md#dynamicsize)
- [endColumn](GC.Spread.Sheets.DataCharts.DataChart.md#endcolumn)
- [endColumnOffset](GC.Spread.Sheets.DataCharts.DataChart.md#endcolumnoffset)
- [endRow](GC.Spread.Sheets.DataCharts.DataChart.md#endrow)
- [endRowOffset](GC.Spread.Sheets.DataCharts.DataChart.md#endrowoffset)
- [getChartConfig](GC.Spread.Sheets.DataCharts.DataChart.md#getchartconfig)
- [height](GC.Spread.Sheets.DataCharts.DataChart.md#height)
- [isLocked](GC.Spread.Sheets.DataCharts.DataChart.md#islocked)
- [isSelected](GC.Spread.Sheets.DataCharts.DataChart.md#isselected)
- [isVisible](GC.Spread.Sheets.DataCharts.DataChart.md#isvisible)
- [name](GC.Spread.Sheets.DataCharts.DataChart.md#name)
- [setChartConfig](GC.Spread.Sheets.DataCharts.DataChart.md#setchartconfig)
- [startColumn](GC.Spread.Sheets.DataCharts.DataChart.md#startcolumn)
- [startColumnOffset](GC.Spread.Sheets.DataCharts.DataChart.md#startcolumnoffset)
- [startRow](GC.Spread.Sheets.DataCharts.DataChart.md#startrow)
- [startRowOffset](GC.Spread.Sheets.DataCharts.DataChart.md#startrowoffset)
- [width](GC.Spread.Sheets.DataCharts.DataChart.md#width)
- [x](GC.Spread.Sheets.DataCharts.DataChart.md#x)
- [y](GC.Spread.Sheets.DataCharts.DataChart.md#y)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new DataChart**(`sheet`, `name`, `x`, `y`, `width`, `height`, `type`)

表示一个数据图表。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheet` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 数据图表所在的工作表。 |
| `name` | `string` | 数据图表的名称。 |
| `x` | `number` | 数据图表的 <i>x</i> 坐标位置。 |
| `y` | `number` | 数据图表的 <i>y</i> 坐标位置。 |
| `width` | `number` | 数据图表的宽度。 |
| `height` | `number` | 数据图表的高度。 |
| `type` | [`DataChartType`](../enums/GC.Spread.Sheets.DataCharts.DataChartType.md) | 数据图表的类型。 |

## Methods

### <a id="allowmove" name="allowmove"></a> allowMove

▸ **allowMove**(`value?`): `any`

获取或设置是否禁用移动数据图表。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否禁用移动数据图表的设置。 |

#### Returns

`any`

如果未设置值，则返回是否禁用移动数据图表的设置；否则返回数据图表。

___

### <a id="allowresize" name="allowresize"></a> allowResize

▸ **allowResize**(`value?`): `any`

获取或设置是否禁用调整数据图表大小。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否禁用调整数据图表大小的设置。 |

#### Returns

`any`

如果未设置值，则返回是否禁用调整数据图表大小的设置；否则返回数据图表。

___

### <a id="alt" name="alt"></a> alt

▸ **alt**(`value?`): `any`

获取或设置数据图表的替代文本（用于屏幕阅读器）。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 数据图表的替代文本。 |

#### Returns

`any`

数据图表的替代文本。

___

### <a id="canprint" name="canprint"></a> canPrint

▸ **canPrint**(`value?`): `any`

获取或设置此数据图表是否可打印。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 指示此数据图表是否可打印的值。 |

#### Returns

`any`

如果未设置值，则返回此数据图表是否可打印。

___

### <a id="dynamicmove" name="dynamicmove"></a> dynamicMove

▸ **dynamicMove**(`value?`): `any`

获取或设置当隐藏或显示、调整大小或移动行或列时，对象是否移动。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 指示当隐藏或显示、调整大小或移动行或列时，对象是否移动的值。 |

#### Returns

`any`

如果未设置值，则返回此数据图表是否动态移动；否则返回数据图表。

___

### <a id="dynamicsize" name="dynamicsize"></a> dynamicSize

▸ **dynamicSize**(`value?`): `any`

获取或设置数据图表的位置是否固定。当 fixedPosition 为 true 时，dynamicMove 和 dynamicSize 将被禁用。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 指示数据图表位置是否固定的值。 |

#### Returns

`any`

如果未设置值，则返回数据图表的位置是否固定；否则返回数据图表。

___

### <a id="endcolumn" name="endcolumn"></a> endColumn

▸ **endColumn**(`value?`): `any`

获取或设置数据图表位置的结束列索引。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 数据图表位置的结束列索引。 |

#### Returns

`any`

如果未设置值，则返回数据图表位置的结束列索引；否则返回数据图表。

___

### <a id="endcolumnoffset" name="endcolumnoffset"></a> endColumnOffset

▸ **endColumnOffset**(`value?`): `any`

获取或设置相对于数据图表结束列的偏移量。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 相对于数据图表结束列的偏移量。 |

#### Returns

`any`

如果未设置值，则返回相对于数据图表结束列的偏移量；否则返回数据图表。

___

### <a id="endrow" name="endrow"></a> endRow

▸ **endRow**(`value?`): `any`

获取或设置数据图表位置的结束行索引。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 数据图表位置的结束行索引。 |

#### Returns

`any`

如果未设置值，则返回数据图表位置的结束行索引；否则返回数据图表。

___

### <a id="endrowoffset" name="endrowoffset"></a> endRowOffset

▸ **endRowOffset**(`value?`): `any`

获取或设置相对于数据图表结束行的偏移量。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 相对于数据图表结束行的偏移量。 |

#### Returns

`any`

如果未设置值，则返回相对于数据图表结束行的偏移量；否则返回数据图表。

___

### <a id="getchartconfig" name="getchartconfig"></a> getChartConfig

▸ **getChartConfig**(): [`IDataChartConfig`](../interfaces/GC.Spread.Sheets.DataCharts.IDataChartConfig.md)

获取数据图表配置。

**`example`**
```javascript
var datachart = activeSheet.datacharts.add('datachart1', 250, 20, 480, 300, GC.Spread.Sheets.DataCharts.DataChartType.column);
console.log(datachart.getChartConfig());
```

#### Returns

[`IDataChartConfig`](../interfaces/GC.Spread.Sheets.DataCharts.IDataChartConfig.md)

数据图表的配置。

___

### <a id="height" name="height"></a> height

▸ **height**(`value?`): `any`

获取或设置数据图表的高度。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 数据图表的高度。 |

#### Returns

`any`

如果未设置值，则返回数据图表的高度；否则返回数据图表。

___

### <a id="islocked" name="islocked"></a> isLocked

▸ **isLocked**(`value?`): `any`

获取或设置此数据图表是否被锁定。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 指示此数据图表是否被锁定的值。 |

#### Returns

`any`

如果未设置值，则返回此数据图表是否被锁定；否则返回数据图表。

___

### <a id="isselected" name="isselected"></a> isSelected

▸ **isSelected**(`value?`): `any`

获取或设置此数据图表是否被选中。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 指示此数据图表是否被选中的值。 |

#### Returns

`any`

如果未设置值，则返回此数据图表是否被选中；否则返回数据图表。

___

### <a id="isvisible" name="isvisible"></a> isVisible

▸ **isVisible**(`value?`): `any`

获取或设置此数据图表是否可见。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 指示此数据图表是否可见的值。 |

#### Returns

`any`

如果未设置值，则返回此数据图表是否可见；否则返回数据图表。

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取数据图表的名称。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 数据图表的名称。 |

#### Returns

`any`

如果未设置值，则返回数据图表的名称；否则返回数据图表。

___

### <a id="setchartconfig" name="setchartconfig"></a> setChartConfig

▸ **setChartConfig**(`config`): `void`

设置数据图表配置。

**`example`**
```javascript
var datachart = activeSheet.datacharts.add('datachart1', 250, 20, 480, 300, GC.Spread.Sheets.DataCharts.DataChartType.column);
var config = datachart.getChartConfig();
config.plots[0].type = GC.Spread.Sheets.DataCharts.DataChartType.line;
datachart.setChartConfig(config);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `config` | [`IDataChartConfig`](../interfaces/GC.Spread.Sheets.DataCharts.IDataChartConfig.md) | 数据图表的配置。 |

#### Returns

`void`

___

### <a id="startcolumn" name="startcolumn"></a> startColumn

▸ **startColumn**(`value?`): `any`

获取或设置数据图表位置的起始列索引。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 数据图表位置的起始列索引。 |

#### Returns

`any`

如果未设置值，则返回数据图表位置的起始列索引；否则返回数据图表。

___

### <a id="startcolumnoffset" name="startcolumnoffset"></a> startColumnOffset

▸ **startColumnOffset**(`value?`): `any`

获取或设置相对于数据图表起始列的偏移量。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 相对于数据图表起始列的偏移量。 |

#### Returns

`any`

如果未设置值，则返回相对于数据图表起始列的偏移量；否则返回数据图表。

___

### <a id="startrow" name="startrow"></a> startRow

▸ **startRow**(`value?`): `any`

获取或设置数据图表位置的起始行索引。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 数据图表位置的起始行索引。 |

#### Returns

`any`

如果未设置值，则返回数据图表位置的起始行索引；否则返回数据图表。

___

### <a id="startrowoffset" name="startrowoffset"></a> startRowOffset

▸ **startRowOffset**(`value?`): `any`

获取或设置相对于数据图表起始行的偏移量。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 相对于数据图表起始行的偏移量。 |

#### Returns

`any`

如果未设置值，则返回相对于数据图表起始行的偏移量；否则返回数据图表。

___

### <a id="width" name="width"></a> width

▸ **width**(`value?`): `any`

获取或设置数据图表的宽度。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 数据图表的宽度。 |

#### Returns

`any`

如果未设置值，则返回数据图表的宽度；否则返回数据图表。

___

### <a id="x" name="x"></a> x

▸ **x**(`value?`): `any`

获取或设置数据图表的水平位置。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 数据图表的水平位置。 |

#### Returns

`any`

如果未设置值，则返回数据图表的水平位置；否则返回数据图表。

___

### <a id="y" name="y"></a> y

▸ **y**(`value?`): `any`

获取或设置数据图表的垂直位置。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 数据图表的垂直位置。 |

#### Returns

`any`

如果未设置值，则返回数据图表的垂直位置；否则返回数据图表。
