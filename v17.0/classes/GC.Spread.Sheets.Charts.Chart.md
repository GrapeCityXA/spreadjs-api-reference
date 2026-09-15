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
- [useAnimation](GC.Spread.Sheets.Charts.Chart.md#useanimation)
- [width](GC.Spread.Sheets.Charts.Chart.md#width)
- [x](GC.Spread.Sheets.Charts.Chart.md#x)
- [y](GC.Spread.Sheets.Charts.Chart.md#y)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Chart**(`sheet`, `name`, `chartType`, `x`, `y`, `width`, `height`, `dataRange?`, `dataOrientation?`)

图表

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheet` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 图表的主表 |
| `name` | `string` | 图表名称 |
| `chartType` | [`ChartType`](../enums/GC.Spread.Sheets.Charts.ChartType.md) | 图表的类型 |
| `x` | `number` | 图表的<i> x </i>位置 |
| `y` | `number` | 图表的<i> y </i>位置 |
| `width` | `number` | 图表的宽度 |
| `height` | `number` | 图表的高度 |
| `dataRange?` | `string` | 图表数据区域的公式字符串 |
| `dataOrientation?` | [`RowCol`](../enums/GC.Spread.Sheets.Charts.RowCol.md) | 系列数据的方向 |

## Properties

### <a id="typename" name="typename"></a> typeName

• **typeName**: `string`

支持序列化的类型名称字符串

## Methods

### <a id="allowmove" name="allowmove"></a> allowMove

▸ **allowMove**(`value?`): `any`

获取或设置是否禁用移动浮动对象元素

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否禁用移动浮动对象元素的设置 |

#### Returns

`any`

如果未设置任何值，则返回是否禁用移动浮动对象元素的设置；否则，返回浮动对象元素

___

### <a id="allowresize" name="allowresize"></a> allowResize

▸ **allowResize**(`value?`): `any`

获取或设置是否禁用调整浮动对象的大小

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否禁用调整浮动对象大小的设置 |

#### Returns

`any`

如果未设置任何值，则返回是否禁用调整浮动对象大小的设置；否则，返回浮动对象

___

### <a id="alt" name="alt"></a> alt

▸ **alt**(`value?`): `any`

获取或设置浮动对象的可选文本

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 浮动对象的可选文本 |

#### Returns

`any`

浮动对象的可选文本

___

### <a id="axes" name="axes"></a> axes

▸ **axes**(`value?`): `any`

获取或设置图表的图表轴

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`IAxes`](../interfaces/GC.Spread.Sheets.Charts.IAxes.md) | 图表的图表轴 |

#### Returns

`any`

如果未设置值，返回图表的图表轴；否则，返回图表

majorGridLine和minorGridLine有相同的类型

___

### <a id="canprint" name="canprint"></a> canPrint

▸ **canPrint**(`value?`): `any`

获取或设置此图表是否可打印

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 指示此图表是否可打印 |

#### Returns

`any`

如果未设置值，则返回此图表是否可打印

___

### <a id="chartarea" name="chartarea"></a> chartArea

▸ **chartArea**(`value?`): `any`

获取或设置图表的图表区域样式

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`IChartArea`](../interfaces/GC.Spread.Sheets.Charts.IChartArea.md) | 图表的图表区域样式 |

#### Returns

`any`

如果未设置值，则返回图表的图表区样式；否则，返回图表

___

### <a id="charttype" name="charttype"></a> chartType

▸ **chartType**(`value?`): `any`

获取或设置图表的类型

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`ChartType`](../enums/GC.Spread.Sheets.Charts.ChartType.md) | 图表的类型 |

#### Returns

`any`

如果未设置任何值，则返回图表的类型；否则，返回图表

___

### <a id="clonecontent" name="clonecontent"></a> cloneContent

▸ **cloneContent**(): `HTMLElement`

获取当前实例的内容副本

#### Returns

`HTMLElement`

当前实例内容的副本

___

### <a id="content" name="content"></a> content

▸ **content**(`value?`): `any`

获取或设置自定义浮动对象元素的内容

**`deprecated`** 从 17.0.0 版本开始，该方法在图表插件中不可用，要使用该方法，请使用 legacy-charts 插件

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `HTMLElement` | 自定义浮动对象元素的内容 |

#### Returns

`any`

如果未设置任何值，则返回自定义浮动对象元素的内容；否则，返回浮动对象元素

___

### <a id="datalabels" name="datalabels"></a> dataLabels

▸ **dataLabels**(`value?`): `any`

Gets or sets the chart data labels style of the chart.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`IDataLabels`](../interfaces/GC.Spread.Sheets.Charts.IDataLabels.md) | The chart data labels style of the chart. |

#### Returns

`any`

If no value is set, returns the chart data labels style of the chart; otherwise, returns the chart.

___

### <a id="datarange" name="datarange"></a> dataRange

▸ **dataRange**(`value?`): `any`

获取或设置图表的整个数据区域作为公式字符串

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 图表数据区域的公式字符串 |

#### Returns

`any`

如果未设置任何值，则返回图表整个数据区域的公式字符串；否则，返回图表

___

### <a id="displayblanksas" name="displayblanksas"></a> displayBlanksAs

▸ **displayBlanksAs**(`value?`): `any`

获取或设置图表显示空白数据的方式

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`DisplayBlanksAs`](../enums/GC.Spread.Sheets.Charts.DisplayBlanksAs.md) | 图表显示空白数据的方式 |

#### Returns

`any`

如果未设置任何值，则返回图表显示空白数据的方式，否则返回图表

___

### <a id="displaynaasblank" name="displaynaasblank"></a> displayNaAsBlank

▸ **displayNaAsBlank**(`value?`): `boolean` \| [`Chart`](GC.Spread.Sheets.Charts.Chart.md)

获取或设置是否将＃N / A单元格显示为空白单元格

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否将＃N / A单元格显示为空白单元格 |

#### Returns

`boolean` \| [`Chart`](GC.Spread.Sheets.Charts.Chart.md)

如果未设置任何值，则返回是否将＃N / A单元格显示为空白单元格，否则，返回图表

___

### <a id="dynamicmove" name="dynamicmove"></a> dynamicMove

▸ **dynamicMove**(`value?`): `any`

获取或设置对象在隐藏或显示，调整大小或移动行或列时是否移动

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 该值指示对象在隐藏或显示，调整大小或移动行或列时是否移动 |

#### Returns

`any`

如果未设置任何值，则返回此浮动对象元素是否动态移动；否则，返回浮动对象元素

___

### <a id="dynamicsize" name="dynamicsize"></a> dynamicSize

▸ **dynamicSize**(`value?`): `any`

获取或设置在隐藏或显示，调整大小或移动行或列时对象的大小是否改变

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 该值指示在隐藏或显示，调整大小或移动行或列时对象的大小是否改变 |

#### Returns

`any`

如果未设置任何值，则返回此浮动对象元素是否动态更改大小；否则，返回浮动对象元素

___

### <a id="endcolumn" name="endcolumn"></a> endColumn

▸ **endColumn**(`value?`): `any`

获取或设置浮动对象元素位置的结束列索引

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 浮动对象元素位置的结束列索引 |

#### Returns

`any`

如果未设置任何值，则返回浮动对象元素位置的结束列索引；否则，返回浮动对象元素

___

### <a id="endcolumnoffset" name="endcolumnoffset"></a> endColumnOffset

▸ **endColumnOffset**(`value?`): `any`

获取或设置相对于浮动对象元素的结束列的偏移量

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 相对于浮动对象元素的结束列的偏移量 |

#### Returns

`any`

如果未设置任何值，则返回相对于浮动对象元素的结束列的偏移量；否则，返回浮动对象元素

___

### <a id="endrow" name="endrow"></a> endRow

▸ **endRow**(`value?`): `any`

获取或设置浮动对象元素位置的末行索引

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 浮动对象元素位置的末行索引 |

#### Returns

`any`

如果未设置任何值，则返回浮动对象元素位置的末端行索引；否则，返回浮动对象元素

___

### <a id="endrowoffset" name="endrowoffset"></a> endRowOffset

▸ **endRowOffset**(`value?`): `any`

获取或设置相对于浮动对象元素的最后一行的偏移量

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 相对于浮动对象元素的最后一行的偏移量 |

#### Returns

`any`

如果未设置任何值，则返回相对于浮动对象元素的最后一行的偏移量；否则，返回浮动对象元素

___

### <a id="fixedposition" name="fixedposition"></a> fixedPosition

▸ **fixedPosition**(`value`): `any`

获取或设置浮动对象元素的位置是否固定 当fixedPosition为true时,dynamicMove和dynamicSize被禁用

**`deprecated`** 从 17.0.0 版本开始，该方法在图表插件中不可用，要使用该方法，请使用 legacy-charts 插件

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `boolean` | 该值指示浮动对象元素的位置是否固定 |

#### Returns

`any`

如果未设置任何值，则返回浮动对象元素的位置是否固定 否则，返回浮动对象元素

___

### <a id="formatovers" name="formatovers"></a> formatOvers

▸ **formatOvers**(`value?`): [`Chart`](GC.Spread.Sheets.Charts.Chart.md) \| [`IFormatOvers`](../modules/GC.Spread.Sheets.Charts.md#iformatovers)

获取或设置瀑布图不同点收集样式

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`IFormatOvers`](../modules/GC.Spread.Sheets.Charts.md#iformatovers) | 瀑布图的特定数据点收集样式 |

#### Returns

[`Chart`](GC.Spread.Sheets.Charts.Chart.md) \| [`IFormatOvers`](../modules/GC.Spread.Sheets.Charts.md#iformatovers)

如果未设置值，则返回瀑布图不同点收集样式

___

### <a id="getformula" name="getformula"></a> getFormula

▸ **getFormula**(`path`): `string`

通过路径从图表中获取公式字符串

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `path` | `string` | 可以接受公式字符串的路径可以是“ x”，“ y”，“ width”，“height”之一 |

#### Returns

`string`

通过路径返回图表中的公式字符串

___

### <a id="gethost" name="gethost"></a> getHost

▸ **getHost**(): `HTMLElement`[]

获取自定义内容的dom宿主

**`deprecated`** 从 17.0.0 版本开始，该方法在图表插件中不可用，要使用该方法，请使用 legacy-charts 插件

#### Returns

`HTMLElement`[]

___

### <a id="height" name="height"></a> height

▸ **height**(`value?`): `any`

获取或设置浮动对象元素的高度

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 浮动对象元素的高度 |

#### Returns

`any`

如果未设置任何值，则返回一个浮动对象元素的高度；否则，返回浮动对象元素

___

### <a id="hoverstyle" name="hoverstyle"></a> hoverStyle

▸ **hoverStyle**(`value?`): `any`

获取或设置用户悬停在数据点上时的样式

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`IHoverStyle`](../interfaces/GC.Spread.Sheets.Charts.IHoverStyle.md) | 悬停的数据点的悬停样式 |

#### Returns

`any`

如果未设置值，则返回图表的当前悬停样式；否则，返回图表

___

### <a id="ignorehidden" name="ignorehidden"></a> ignoreHidden

▸ **ignoreHidden**(`value?`): `boolean` \| [`Chart`](GC.Spread.Sheets.Charts.Chart.md)

获取或设置图表显示隐藏的行和列数据的方式

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 图表显示隐藏的行和列数据时的值 |

#### Returns

`boolean` \| [`Chart`](GC.Spread.Sheets.Charts.Chart.md)

如果未设置任何值，则返回如果图表显示隐藏的行和列数据的值，否则返回该图表

___

### <a id="islocked" name="islocked"></a> isLocked

▸ **isLocked**(`value?`): `any`

获取或设置此浮动对象元素是否被锁定

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 该值指示此浮动对象元素是否被锁定 |

#### Returns

`any`

如果未设置任何值，则返回此浮动对象元素是否被锁定；否则，返回浮动对象元素

___

### <a id="isselected" name="isselected"></a> isSelected

▸ **isSelected**(`value?`): `any`

获取或设置是否选择此浮动对象元素

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 该值指示此浮动对象元素是否被选择 |

#### Returns

`any`

如果未设置任何值，则返回是否选择此浮动对象元素；否则，返回浮动对象元素

___

### <a id="isvisible" name="isvisible"></a> isVisible

▸ **isVisible**(`value?`): `any`

获取或设置此浮动对象元素是否可见

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 该值指示此浮动对象元素是否可见 |

#### Returns

`any`

如果未设置任何值，则返回此浮动对象元素是否可见；否则，返回浮动对象元素

___

### <a id="legend" name="legend"></a> legend

▸ **legend**(`value?`): `any`

获取或设置图表的图例

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`IChartLegend`](../interfaces/GC.Spread.Sheets.Charts.IChartLegend.md) | 图表的图例 |

#### Returns

`any`

如果未设置值，请返回图表的图例；否则，返回图表

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取浮动对象元素的名称

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 浮动对象元素的名称 |

#### Returns

`any`

如果未设置任何值，则返回浮动对象元素的名称；否则，返回浮动对象元素

___

### <a id="refreshcontent" name="refreshcontent"></a> refreshContent

▸ **refreshContent**(): `void`

刷新floatObject中的内容用户应重写此方法，以使其内容与floatObject同步

#### Returns

`void`

___

### <a id="series" name="series"></a> series

▸ **series**(): [`SeriesCollection`](GC.Spread.Sheets.Charts.SeriesCollection.md)

获取图表的系列集合

#### Returns

[`SeriesCollection`](GC.Spread.Sheets.Charts.SeriesCollection.md)

返回图表的系列集合

___

### <a id="setformula" name="setformula"></a> setFormula

▸ **setFormula**(`path`, `formula`): `void`

为图表通过路径将公式字符串设置

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `path` | `string` | 可以接受公式字符串的路径可以是“x”，“y”，“width”，“height”之一 |
| `formula` | `string` | 公式字符串 |

#### Returns

`void`

___

### <a id="startcolumn" name="startcolumn"></a> startColumn

▸ **startColumn**(`value?`): `any`

获取或设置浮动对象元素位置的起始列索引

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 浮动对象元素位置的起始列索引 |

#### Returns

`any`

如果未设置任何值，则返回浮动对象元素位置的起始列索引；否则，返回浮动对象元素

___

### <a id="startcolumnoffset" name="startcolumnoffset"></a> startColumnOffset

▸ **startColumnOffset**(`value?`): `any`

获取或设置相对于浮动对象元素的起始列的偏移量

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 相对于浮动对象元素的起始列的偏移量 |

#### Returns

`any`

如果未设置任何值，则返回相对于浮动对象元素的起始列的偏移量；否则，返回浮动对象元素

___

### <a id="startrow" name="startrow"></a> startRow

▸ **startRow**(`value?`): `any`

获取或设置浮动对象元素位置的起始行索引

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 动对象元素位置的起始行索引 |

#### Returns

`any`

如果未设置任何值，则返回浮动对象元素位置的起始行索引；否则，返回浮动对象

___

### <a id="startrowoffset" name="startrowoffset"></a> startRowOffset

▸ **startRowOffset**(`value?`): `any`

获取或设置相对于浮动对象元素的起始行的偏移量

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 相对于浮动对象元素的起始行的偏移量 |

#### Returns

`any`

如果未设置任何值，则返回相对于浮动对象元素起始行的偏移量；否则，返回浮动对象元素

___

### <a id="switchdataorientation" name="switchdataorientation"></a> switchDataOrientation

▸ **switchDataOrientation**(): `boolean`

在行和列之间切换数据方向

#### Returns

`boolean`

当数据方向可以更改并成功切换时，返回true;否则为假

___

### <a id="title" name="title"></a> title

▸ **title**(`value?`): `any`

获取或设置图表标题

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`IChartTitle`](../interfaces/GC.Spread.Sheets.Charts.IChartTitle.md) | 图表标题 |

#### Returns

`any`

如果未设置任何值，则返回图表标题；否则，返回图表

___

### <a id="useanimation" name="useanimation"></a> useAnimation

▸ **useAnimation**(`value?`): `any`

获取或设置是否将动画应用于图表

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否将动画应用于图表 |

#### Returns

`any`

如果未设置任何值，则返回是否将动画应用于图表；否则，返回图表

___

### <a id="width" name="width"></a> width

▸ **width**(`value?`): `any`

获取或设置浮动对象元素的宽度

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 浮动对象元素的宽度 |

#### Returns

`any`

如果未设置任何值，则返回一个浮动对象元素的宽度；否则，返回浮动对象元素

___

### <a id="x" name="x"></a> x

▸ **x**(`value?`): `any`

获取或设置浮动对象元素的水平位置

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 浮动对象元素的水平位置 |

#### Returns

`any`

如果未设置任何值，则返回浮动对象元素的水平位置；否则，返回浮动对象元素

___

### <a id="y" name="y"></a> y

▸ **y**(`value?`): `any`

获取或设置浮动对象元素的垂直位置

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 获取或设置浮动对象元素的垂直位置 |

#### Returns

`any`

如果未设置任何值，则返回浮动对象对象的垂直位置；否则，返回浮动对象元素
