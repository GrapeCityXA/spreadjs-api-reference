# Class: Chart

[Sheets](../modules/GC.Spread.Sheets.md).[Charts](../modules/GC.Spread.Sheets.Charts.md).Chart

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Charts.Chart.md#constructor)

### Properties

- [typeName](GC.Spread.Sheets.Charts.Chart.md#typename)

### Methods

- [allowMove](GC.Spread.Sheets.Charts.Chart.md#allowmove)
- [allowResize](GC.Spread.Sheets.Charts.Chart.md#allowresize)
- [alt](GC.Spread.Sheets.Charts.Chart.md#alt)
- [axes](GC.Spread.Sheets.Charts.Chart.md#axes)
- [canPrint](GC.Spread.Sheets.Charts.Chart.md#canprint)
- [chartArea](GC.Spread.Sheets.Charts.Chart.md#chartarea)
- [chartType](GC.Spread.Sheets.Charts.Chart.md#charttype)
- [cloneContent](GC.Spread.Sheets.Charts.Chart.md#clonecontent)
- [colorScheme](GC.Spread.Sheets.Charts.Chart.md#colorscheme)
- [content](GC.Spread.Sheets.Charts.Chart.md#content)
- [dataLabels](GC.Spread.Sheets.Charts.Chart.md#datalabels)
- [dataRange](GC.Spread.Sheets.Charts.Chart.md#datarange)
- [displayBlanksAs](GC.Spread.Sheets.Charts.Chart.md#displayblanksas)
- [displayNaAsBlank](GC.Spread.Sheets.Charts.Chart.md#displaynaasblank)
- [dynamicMove](GC.Spread.Sheets.Charts.Chart.md#dynamicmove)
- [dynamicSize](GC.Spread.Sheets.Charts.Chart.md#dynamicsize)
- [endColumn](GC.Spread.Sheets.Charts.Chart.md#endcolumn)
- [endColumnOffset](GC.Spread.Sheets.Charts.Chart.md#endcolumnoffset)
- [endRow](GC.Spread.Sheets.Charts.Chart.md#endrow)
- [endRowOffset](GC.Spread.Sheets.Charts.Chart.md#endrowoffset)
- [fixedPosition](GC.Spread.Sheets.Charts.Chart.md#fixedposition)
- [formatOvers](GC.Spread.Sheets.Charts.Chart.md#formatovers)
- [getFormula](GC.Spread.Sheets.Charts.Chart.md#getformula)
- [getHost](GC.Spread.Sheets.Charts.Chart.md#gethost)
- [height](GC.Spread.Sheets.Charts.Chart.md#height)
- [hoverStyle](GC.Spread.Sheets.Charts.Chart.md#hoverstyle)
- [ignoreHidden](GC.Spread.Sheets.Charts.Chart.md#ignorehidden)
- [isLocked](GC.Spread.Sheets.Charts.Chart.md#islocked)
- [isSelected](GC.Spread.Sheets.Charts.Chart.md#isselected)
- [isVisible](GC.Spread.Sheets.Charts.Chart.md#isvisible)
- [legend](GC.Spread.Sheets.Charts.Chart.md#legend)
- [name](GC.Spread.Sheets.Charts.Chart.md#name)
- [refreshContent](GC.Spread.Sheets.Charts.Chart.md#refreshcontent)
- [series](GC.Spread.Sheets.Charts.Chart.md#series)
- [setFormula](GC.Spread.Sheets.Charts.Chart.md#setformula)
- [startColumn](GC.Spread.Sheets.Charts.Chart.md#startcolumn)
- [startColumnOffset](GC.Spread.Sheets.Charts.Chart.md#startcolumnoffset)
- [startRow](GC.Spread.Sheets.Charts.Chart.md#startrow)
- [startRowOffset](GC.Spread.Sheets.Charts.Chart.md#startrowoffset)
- [switchDataOrientation](GC.Spread.Sheets.Charts.Chart.md#switchdataorientation)
- [title](GC.Spread.Sheets.Charts.Chart.md#title)
- [toImageSrc](GC.Spread.Sheets.Charts.Chart.md#toimagesrc)
- [toImageSrcAsync](GC.Spread.Sheets.Charts.Chart.md#toimagesrcasync)
- [useAnimation](GC.Spread.Sheets.Charts.Chart.md#useanimation)
- [width](GC.Spread.Sheets.Charts.Chart.md#width)
- [x](GC.Spread.Sheets.Charts.Chart.md#x)
- [y](GC.Spread.Sheets.Charts.Chart.md#y)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Chart**(`sheet`, `name`, `chartType`, `x`, `y`, `width`, `height`, `dataRange?`, `dataOrientation?`, `colorScheme?`)

表示一个图表。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheet` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 图表所在的工作表。 |
| `name` | `string` | 图表的名称。 |
| `chartType` | [`ChartType`](../enums/GC.Spread.Sheets.Charts.ChartType.md) | 图表的类型。 |
| `x` | `number` | 图表的 <i>x</i> 坐标位置。 |
| `y` | `number` | 图表的 <i>y</i> 坐标位置。 |
| `width` | `number` | 图表的宽度。 |
| `height` | `number` | 图表的高度。 |
| `dataRange?` | `string` | - |
| `dataOrientation?` | [`RowCol`](../enums/GC.Spread.Sheets.Charts.RowCol.md) | - |
| `colorScheme?` | [`ColorScheme`](../modules/GC.Spread.Sheets.Charts.md#colorscheme) | - |

## Properties

### <a id="typename" name="typename"></a> typeName

• **typeName**: `string`

表示用于支持序列化的类型名称字符串。

## Methods

### <a id="allowmove" name="allowmove"></a> allowMove

▸ **allowMove**(`value?`): `any`

获取或设置是否禁用移动图表。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否禁用移动图表的设置。 |

#### Returns

`any`

如果未设置值，则返回是否禁用移动图表的设置；否则返回图表。

___

### <a id="allowresize" name="allowresize"></a> allowResize

▸ **allowResize**(`value?`): `any`

获取或设置是否禁用调整图表大小。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否禁用调整图表大小的设置。 |

#### Returns

`any`

如果未设置值，则返回是否禁用调整图表大小的设置；否则返回图表。

___

### <a id="alt" name="alt"></a> alt

▸ **alt**(`value?`): `any`

获取或设置图表的替代文本，用于屏幕阅读器。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 图表的替代文本。 |

#### Returns

`any`

图表的替代文本。

___

### <a id="axes" name="axes"></a> axes

▸ **axes**(`value?`): `any`

获取或设置图表的坐标轴。

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`IAxes`](../interfaces/GC.Spread.Sheets.Charts.IAxes.md) |

#### Returns

`any`

如果未设置值，则返回图表的坐标轴；否则返回图表。

___

### <a id="canprint" name="canprint"></a> canPrint

▸ **canPrint**(`value?`): `any`

获取或设置此图表是否可打印。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 表示此图表是否可打印的值。 |

#### Returns

`any`

如果未设置值，则返回此图表是否可打印。

___

### <a id="chartarea" name="chartarea"></a> chartArea

▸ **chartArea**(`value?`): `any`

获取或设置图表的图表区域样式。

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`IChartArea`](../interfaces/GC.Spread.Sheets.Charts.IChartArea.md) |

#### Returns

`any`

如果未设置值，则返回图表的图表区域样式；否则返回图表。

___

### <a id="charttype" name="charttype"></a> chartType

▸ **chartType**(`value?`): `any`

获取或设置图表的类型。

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`ChartType`](../enums/GC.Spread.Sheets.Charts.ChartType.md) |

#### Returns

`any`

如果未设置值，则返回图表的类型；否则返回图表。

___

### <a id="clonecontent" name="clonecontent"></a> cloneContent

▸ **cloneContent**(): `HTMLElement`

获取实例当前内容的副本。

**`deprecated`** since version 17.0.0, 此方法在 charts 插件中不可用，要使用此方法，请使用 legacy-charts 插件。

#### Returns

`HTMLElement`

实例当前内容的副本。

___

### <a id="colorscheme" name="colorscheme"></a> colorScheme

▸ **colorScheme**(`value?`): [`ColorScheme`](../modules/GC.Spread.Sheets.Charts.md#colorscheme) \| [`Chart`](GC.Spread.Sheets.Charts.Chart.md)

获取或设置图表颜色。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`ColorScheme`](../modules/GC.Spread.Sheets.Charts.md#colorscheme) | 表示图表颜色样式的值。 |

#### Returns

[`ColorScheme`](../modules/GC.Spread.Sheets.Charts.md#colorscheme) \| [`Chart`](GC.Spread.Sheets.Charts.Chart.md)

如果未设置值，则返回当前图表颜色样式；否则返回图表。

___

### <a id="content" name="content"></a> content

▸ **content**(`value?`): `any`

获取或设置自定义图表的内容。

**`deprecated`** since version 17.0.0, 此方法在 charts 插件中不可用，要使用此方法，请使用 legacy-charts 插件。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `HTMLElement` | 自定义图表的内容。 |

#### Returns

`any`

如果未设置值，则返回自定义图表的内容；否则返回图表。

___

### <a id="datalabels" name="datalabels"></a> dataLabels

▸ **dataLabels**(`value?`): `any`

获取或设置图表的数据标签样式。

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`IDataLabels`](../interfaces/GC.Spread.Sheets.Charts.IDataLabels.md) |

#### Returns

`any`

如果未设置值，则返回图表的数据标签样式；否则返回图表。

___

### <a id="datarange" name="datarange"></a> dataRange

▸ **dataRange**(`value?`): `any`

获取或设置图表的整个数据范围（以公式字符串形式）。

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置值，则返回图表整个数据范围的公式字符串；否则返回图表。

___

### <a id="displayblanksas" name="displayblanksas"></a> displayBlanksAs

▸ **displayBlanksAs**(`value?`): `any`

获取或设置图表显示空白数据的方式。

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`DisplayBlanksAs`](../enums/GC.Spread.Sheets.Charts.DisplayBlanksAs.md) |

#### Returns

`any`

如果未设置值，则返回图表显示空白数据的方式；否则返回图表。

___

### <a id="displaynaasblank" name="displaynaasblank"></a> displayNaAsBlank

▸ **displayNaAsBlank**(`value?`): `boolean` \| [`Chart`](GC.Spread.Sheets.Charts.Chart.md)

获取或设置是否将 #N/A 单元格显示为空白单元格。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否将 #N/A 单元格显示为空白单元格的值。 |

#### Returns

`boolean` \| [`Chart`](GC.Spread.Sheets.Charts.Chart.md)

如果未设置值，则返回是否将 #N/A 单元格显示为空白单元格；否则返回图表。

___

### <a id="dynamicmove" name="dynamicmove"></a> dynamicMove

▸ **dynamicMove**(`value?`): `any`

获取或设置对象在隐藏或显示、调整大小或移动行或列时是否移动。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 表示对象在隐藏或显示、调整大小或移动行或列时是否移动的值。 |

#### Returns

`any`

如果未设置值，则返回此图表是否动态移动；否则返回图表。

___

### <a id="dynamicsize" name="dynamicsize"></a> dynamicSize

▸ **dynamicSize**(`value?`): `any`

获取或设置图表位置是否固定。当 fixedPosition 为 true 时，dynamicMove 和 dynamicSize 将被禁用。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 表示图表位置是否固定的值。 |

#### Returns

`any`

如果未设置值，则返回图表位置是否固定；否则返回图表。

___

### <a id="endcolumn" name="endcolumn"></a> endColumn

▸ **endColumn**(`value?`): `any`

获取或设置图表位置的结束列索引。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 图表位置的结束列索引。 |

#### Returns

`any`

如果未设置值，则返回图表位置的结束列索引；否则返回图表。

___

### <a id="endcolumnoffset" name="endcolumnoffset"></a> endColumnOffset

▸ **endColumnOffset**(`value?`): `any`

获取或设置相对于图表结束列的偏移量。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 相对于图表结束列的偏移量。 |

#### Returns

`any`

如果未设置值，则返回相对于图表结束列的偏移量；否则返回图表。

___

### <a id="endrow" name="endrow"></a> endRow

▸ **endRow**(`value?`): `any`

获取或设置图表位置的结束行索引。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 图表位置的结束行索引。 |

#### Returns

`any`

如果未设置值，则返回图表位置的结束行索引；否则返回图表。

___

### <a id="endrowoffset" name="endrowoffset"></a> endRowOffset

▸ **endRowOffset**(`value?`): `any`

获取或设置相对于图表结束行的偏移量。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 相对于图表结束行的偏移量。 |

#### Returns

`any`

如果未设置值，则返回相对于图表结束行的偏移量；否则返回图表。

___

### <a id="fixedposition" name="fixedposition"></a> fixedPosition

▸ **fixedPosition**(`value`): `any`

获取或设置对象在隐藏或显示、调整大小或移动行或列时是否改变大小。

**`deprecated`** 自版本 17.0.0 起，此方法在图表插件中不可用，要使用此方法，请使用 legacy-charts 插件。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `boolean` | 表示对象在隐藏或显示、调整大小或移动行或列时是否改变大小的值。 |

#### Returns

`any`

如果未设置值，则返回此图表是否动态改变大小；否则返回图表。

___

### <a id="formatovers" name="formatovers"></a> formatOvers

▸ **formatOvers**(`value?`): [`IFormatOvers`](../interfaces/GC.Spread.Sheets.Charts.IFormatOvers.md) \| [`Chart`](GC.Spread.Sheets.Charts.Chart.md)

获取或设置瀑布图不同点的集合样式。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`IFormatOvers`](../interfaces/GC.Spread.Sheets.Charts.IFormatOvers.md) | 瀑布图特定数据点的集合样式。 |

#### Returns

[`IFormatOvers`](../interfaces/GC.Spread.Sheets.Charts.IFormatOvers.md) \| [`Chart`](GC.Spread.Sheets.Charts.Chart.md)

如果未设置值，则返回瀑布图不同点的集合样式。

___

### <a id="getformula" name="getformula"></a> getFormula

▸ **getFormula**(`path`): `string`

通过路径获取图表的公式字符串。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `path` | `string` | 可以接受公式字符串的路径，可以是 "x"、"y"、"width"、"height" 之一。 |

#### Returns

`string`

通过路径返回图表的公式字符串。

___

### <a id="gethost" name="gethost"></a> getHost

▸ **getHost**(): `HTMLElement`[]

获取自定义内容的 DOM 宿主。

**`deprecated`** 自版本 17.0.0 起，此方法在图表插件中不可用，要使用此方法，请使用 legacy-charts 插件。

#### Returns

`HTMLElement`[]

___

### <a id="height" name="height"></a> height

▸ **height**(`value?`): `any`

获取或设置图表的高度。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 图表的高度。 |

#### Returns

`any`

如果未设置值，则返回图表的高度；否则返回图表。

___

### <a id="hoverstyle" name="hoverstyle"></a> hoverStyle

▸ **hoverStyle**(`value?`): `any`

获取或设置用户悬停在数据点上时的样式。

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`IHoverStyle`](../interfaces/GC.Spread.Sheets.Charts.IHoverStyle.md) |

#### Returns

`any`

如果未设置值，则返回图表的当前悬停样式；否则返回图表。

___

### <a id="ignorehidden" name="ignorehidden"></a> ignoreHidden

▸ **ignoreHidden**(`value?`): `boolean` \| [`Chart`](GC.Spread.Sheets.Charts.Chart.md)

获取或设置图表是否显示隐藏行和列的数据。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 表示图表是否显示隐藏行和列数据的值。 |

#### Returns

`boolean` \| [`Chart`](GC.Spread.Sheets.Charts.Chart.md)

如果未设置值，则返回图表是否显示隐藏行和列数据；否则返回图表。

___

### <a id="islocked" name="islocked"></a> isLocked

▸ **isLocked**(`value?`): `any`

获取或设置此图表是否被锁定。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 表示此图表是否被锁定的值。 |

#### Returns

`any`

如果未设置值，则返回此图表是否被锁定；否则返回图表。

___

### <a id="isselected" name="isselected"></a> isSelected

▸ **isSelected**(`value?`): `any`

获取或设置此图表是否被选中。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 表示此图表是否被选中的值。 |

#### Returns

`any`

如果未设置值，则返回此图表是否被选中；否则返回图表。

___

### <a id="isvisible" name="isvisible"></a> isVisible

▸ **isVisible**(`value?`): `any`

获取或设置此图表是否可见。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 表示此图表是否可见的值。 |

#### Returns

`any`

如果未设置值，则返回此图表是否可见；否则返回图表。

___

### <a id="legend" name="legend"></a> legend

▸ **legend**(`value?`): `any`

获取或设置图表的图例。

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`IChartLegend`](../interfaces/GC.Spread.Sheets.Charts.IChartLegend.md) |

#### Returns

`any`

如果未设置值，则返回图表的图例；否则返回图表。

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取图表的名称。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 图表的名称。 |

#### Returns

`any`

如果未设置值，则返回图表的名称；否则返回图表。

___

### <a id="refreshcontent" name="refreshcontent"></a> refreshContent

▸ **refreshContent**(): `void`

刷新图表，在大多数情况下不需要调用此方法。

#### Returns

`void`

___

### <a id="series" name="series"></a> series

▸ **series**(): [`SeriesCollection`](GC.Spread.Sheets.Charts.SeriesCollection.md)

获取图表的系列集合。

#### Returns

[`SeriesCollection`](GC.Spread.Sheets.Charts.SeriesCollection.md)

返回图表的系列集合。

___

### <a id="setformula" name="setformula"></a> setFormula

▸ **setFormula**(`path`, `formula`): `void`

通过路径设置图表的公式字符串。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `path` | `string` | 可以接受公式字符串的路径，可以是 "x"、"y"、"width"、"height" 之一。 |
| `formula` | `string` | 公式字符串。 |

#### Returns

`void`

___

### <a id="startcolumn" name="startcolumn"></a> startColumn

▸ **startColumn**(`value?`): `any`

获取或设置图表位置的起始列索引。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 图表位置的起始列索引。 |

#### Returns

`any`

如果未设置值，则返回图表位置的起始列索引；否则返回图表。

___

### <a id="startcolumnoffset" name="startcolumnoffset"></a> startColumnOffset

▸ **startColumnOffset**(`value?`): `any`

获取或设置相对于图表起始列的偏移量。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 相对于图表起始列的偏移量。 |

#### Returns

`any`

如果未设置值，则返回相对于图表起始列的偏移量；否则返回图表。

___

### <a id="startrow" name="startrow"></a> startRow

▸ **startRow**(`value?`): `any`

获取或设置图表位置的起始行索引。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 图表位置的起始行索引。 |

#### Returns

`any`

如果未设置值，则返回图表位置的起始行索引；否则返回图表。

___

### <a id="startrowoffset" name="startrowoffset"></a> startRowOffset

▸ **startRowOffset**(`value?`): `any`

获取或设置相对于图表起始行的偏移量。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 相对于图表起始行的偏移量。 |

#### Returns

`any`

如果未设置值，则返回相对于图表起始行的偏移量；否则返回图表。

___

### <a id="switchdataorientation" name="switchdataorientation"></a> switchDataOrientation

▸ **switchDataOrientation**(): `boolean`

在行和列之间切换数据方向。

#### Returns

`boolean`

当数据方向可更改且成功切换时返回 true；否则返回 false。

___

### <a id="title" name="title"></a> title

▸ **title**(`value?`): `any`

获取或设置图表的标题。

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`IChartTitle`](../interfaces/GC.Spread.Sheets.Charts.IChartTitle.md) |

#### Returns

`any`

如果未设置值，则返回图表的标题；否则返回图表。

___

### <a id="toimagesrc" name="toimagesrc"></a> toImageSrc

▸ **toImageSrc**(): `string`

获取图表的 Base64 字符串类型的图片源。

**`example`**
```
let chartImageSrc = sheet.charts.all()[0].toImageSrc();
```

#### Returns

`string`

返回图表的 Base64 图片源字符串。

___

### <a id="toimagesrcasync" name="toimagesrcasync"></a> toImageSrcAsync

▸ **toImageSrcAsync**(): `Promise`<`string`\>

获取图表的 Base64 字符串类型的图片源。

**`example`**
```
let chartImageSrc = await sheet.charts.all()[0].toImageSrcAsync();
```

#### Returns

`Promise`<`string`\>

返回图表的 Base64 图片源字符串。

___

### <a id="useanimation" name="useanimation"></a> useAnimation

▸ **useAnimation**(`value?`): `any`

获取或设置是否对图表应用动画。

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置值，则返回是否对图表应用动画；否则返回图表。

___

### <a id="width" name="width"></a> width

▸ **width**(`value?`): `any`

获取或设置图表的宽度。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 图表的宽度。 |

#### Returns

`any`

如果未设置值，则返回图表的宽度；否则返回图表。

___

### <a id="x" name="x"></a> x

▸ **x**(`value?`): `any`

获取或设置图表的水平位置。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 图表的水平位置。 |

#### Returns

`any`

如果未设置值，则返回图表的水平位置；否则返回图表。

___

### <a id="y" name="y"></a> y

▸ **y**(`value?`): `any`

获取或设置图表的垂直位置。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 图表的垂直位置。 |

#### Returns

`any`

如果未设置值，则返回图表的垂直位置；否则返回图表。
