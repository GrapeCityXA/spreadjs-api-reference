# Class: ChartCollection

[Sheets](../modules/GC.Spread.Sheets.md).[Charts](../modules/GC.Spread.Sheets.Charts.md).ChartCollection

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Charts.ChartCollection.md#constructor)

### Methods

- [add](GC.Spread.Sheets.Charts.ChartCollection.md#add)
- [all](GC.Spread.Sheets.Charts.ChartCollection.md#all)
- [clear](GC.Spread.Sheets.Charts.ChartCollection.md#clear)
- [get](GC.Spread.Sheets.Charts.ChartCollection.md#get)
- [preserveUnsupportedChart](GC.Spread.Sheets.Charts.ChartCollection.md#preserveunsupportedchart)
- [remove](GC.Spread.Sheets.Charts.ChartCollection.md#remove)
- [zIndex](GC.Spread.Sheets.Charts.ChartCollection.md#zindex)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new ChartCollection**()

表示一个图表管理器，用于管理工作表中的所有图表。

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`name`, `chartType`, `x`, `y`, `width`, `height`, `dataRange?`, `dataOrientation?`, `colorScheme?`): [`Chart`](GC.Spread.Sheets.Charts.Chart.md)

向工作表中添加图表。

**`example`**
```javascript
//此示例展示如何添加图表。
var dataRange = "A1:D4";
var chart = activeSheet.charts.add('Chart1', GC.Spread.Sheets.Charts.ChartType.columnClustered, 250, 20, 600, 400, dataRange);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要添加到工作表的图表名称。 |
| `chartType` | [`ChartType`](../enums/GC.Spread.Sheets.Charts.ChartType.md) | 图表类型。 |
| `x` | `number` | 图表的 x 坐标位置。 |
| `y` | `number` | 图表的 y 坐标位置。 |
| `width` | `number` | 图表的宽度。 |
| `height` | `number` | 图表的高度。 |
| `dataRange?` | `string` | 图表数据范围的公式字符串。 |
| `dataOrientation?` | [`RowCol`](../enums/GC.Spread.Sheets.Charts.RowCol.md) | 系列数据的排列方向。 |
| `colorScheme?` | [`ColorScheme`](../modules/GC.Spread.Sheets.Charts.md#colorscheme) | 图表的颜色样式。 |

#### Returns

[`Chart`](GC.Spread.Sheets.Charts.Chart.md)

已添加到工作表的图表。

___

### <a id="all" name="all"></a> all

▸ **all**(): [`Chart`](GC.Spread.Sheets.Charts.Chart.md)[]

获取工作表中的所有图表。

**`example`**
```javascript
var dataRange = "A1:D4";
activeSheet.charts.add('Chart1', GC.Spread.Sheets.Charts.ChartType.columnClustered, 250, 20, 600, 180, dataRange);
var dataRange2 = "A20:D24";
activeSheet.charts.add('Chart2', GC.Spread.Sheets.Charts.ChartType.columnClustered, 250, 220, 600, 180, dataRange2);
var charts = activeSheet.charts.all();
for (var i = 0; i &lt; charts.length; i++) {
    alert("Name of chart " + i + " is:  " + charts[i].name())
}
```

#### Returns

[`Chart`](GC.Spread.Sheets.Charts.Chart.md)[]

工作表中所有图表的集合。

___

### <a id="clear" name="clear"></a> clear

▸ **clear**(): `void`

删除工作表中的所有图表。

#### Returns

`void`

___

### <a id="get" name="get"></a> get

▸ **get**(`name`): [`Chart`](GC.Spread.Sheets.Charts.Chart.md)

根据指定名称获取工作表中的图表。

**`example`**
```javascript
var dataRange = "A1:D4";
activeSheet.charts.add('Chart1', GC.Spread.Sheets.Charts.ChartType.columnClustered, 250, 20, 600, 400, dataRange);
//button
$("#button1").click(function () {
 var chart = activeSheet.charts.get("f2");
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 图表名称。 |

#### Returns

[`Chart`](GC.Spread.Sheets.Charts.Chart.md)

工作表中指定名称的图表。

___

### <a id="preserveunsupportedchart" name="preserveunsupportedchart"></a> preserveUnsupportedChart

▸ **preserveUnsupportedChart**(`flag?`, `paintCallBack?`): `undefined` \| `boolean`

获取或设置导入时是否保留不支持的图表。

**`example`**
```javascript
sheet.charts.preserveUnsupportedChart(true, function(chart, ctx, width, height){
    ctx.textBaseline = 'middle';
    ctx.textAlign = 'center';
    ctx.fillStyle = '#000000';
    ctx.fillText("to be continue", width / 2, height / 2, width);
})
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `flag?` | `boolean` | 表示导入时是否保留不支持的图表，默认值为 false，如果设置为 true，将按照 paintCallBack 进行绘制。 |
| `paintCallBack?` | [`ILegacyChartPaintCallBack`](../interfaces/GC.Spread.Sheets.Charts.ILegacyChartPaintCallBack.md) \| [`IPaintCallBack`](../interfaces/GC.Spread.Sheets.Charts.IPaintCallBack.md) | 不支持的图表的显示内容函数。 |

#### Returns

`undefined` \| `boolean`

如果未设置值，则返回 flag 值，否则返回 undefined。

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`name`): `void`

根据指定名称从工作表中删除图表。

**`example`**
```javascript
var dataRange = "A1:D4";
activeSheet.charts.add('Chart1', GC.Spread.Sheets.Charts.ChartType.columnClustered, 250, 20, 600, 400, dataRange);
//button
$("#button1").click(function () {
     activeSheet.resumePaint();
     activeSheet.charts.remove("f2");
     activeSheet.repaint();
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 图表名称。 |

#### Returns

`void`

___

### <a id="zindex" name="zindex"></a> zIndex

▸ **zIndex**(`name`, `zIndex?`): `any`

获取或设置图表的 z-index。

**`example`**
```javascript
var dataRange = "A1:D4";
activeSheet.charts.add('Chart1', GC.Spread.Sheets.Charts.ChartType.columnClustered, 250, 20, 600, 180, dataRange);
var dataRange2 = "A20:D24";
activeSheet.charts.add('Chart2', GC.Spread.Sheets.Charts.ChartType.columnClustered, 250, 180, 600, 180, dataRange2);
activeSheet.charts.zIndex('Chart1', 897);
activeSheet.charts.zIndex('Chart2', 890);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 图表名称。 |
| `zIndex?` | `number` | 图表的 z-index。 |

#### Returns

`any`

如果参数 'zIndex' 为 null 或 undefined，则返回指定名称图表的 z-index。
