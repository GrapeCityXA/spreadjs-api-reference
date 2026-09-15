# Class: DataChartManager

[Sheets](../modules/GC.Spread.Sheets.md).[DataCharts](../modules/GC.Spread.Sheets.DataCharts.md).DataChartManager

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.DataCharts.DataChartManager.md#constructor)

### Methods

- [add](GC.Spread.Sheets.DataCharts.DataChartManager.md#add)
- [all](GC.Spread.Sheets.DataCharts.DataChartManager.md#all)
- [clear](GC.Spread.Sheets.DataCharts.DataChartManager.md#clear)
- [get](GC.Spread.Sheets.DataCharts.DataChartManager.md#get)
- [remove](GC.Spread.Sheets.DataCharts.DataChartManager.md#remove)
- [zIndex](GC.Spread.Sheets.DataCharts.DataChartManager.md#zindex)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new DataChartManager**()

表示一个数据图表管理器，用于管理工作表中的所有数据图表。

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`name`, `x`, `y`, `width`, `height`, `type`): [`DataChart`](GC.Spread.Sheets.DataCharts.DataChart.md)

向工作表中添加数据图表。

**`example`**
```
//此示例展示如何添加数据图表。
var datachart = activeSheet.datacharts.add('datachart1', 250, 20, 480, 300, GC.Spread.Sheets.DataCharts.DataChartType.column);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要添加到工作表中的数据图表名称。 |
| `x` | `number` | 数据图表的x坐标位置。 |
| `y` | `number` | 数据图表的y坐标位置。 |
| `width` | `number` | 数据图表的宽度。 |
| `height` | `number` | 数据图表的高度。 |
| `type` | [`DataChartType`](../enums/GC.Spread.Sheets.DataCharts.DataChartType.md) | 数据图表的类型。 |

#### Returns

[`DataChart`](GC.Spread.Sheets.DataCharts.DataChart.md)

已添加到工作表中的数据图表。

___

### <a id="all" name="all"></a> all

▸ **all**(): [`DataChart`](GC.Spread.Sheets.DataCharts.DataChart.md)[]

获取所有数据图表。

**`example`**
```
activeSheet.datacharts.add('DataChart1', 0, 20, 480, 300, GC.Spread.Sheets.DataCharts.DataChartType.column);
activeSheet.datacharts.add('DataChart2', 500, 20, 480, 300, GC.Spread.Sheets.DataCharts.DataChartType.pie);
var dataCharts = activeSheet.datacharts.all();
for (var i = 0; i &lt; dataCharts.length; i++) {
    alert("Name of dataChart " + i + " is:  " + dataCharts[i].name())
}
```

#### Returns

[`DataChart`](GC.Spread.Sheets.DataCharts.DataChart.md)[]

获取所有数据图表。

___

### <a id="clear" name="clear"></a> clear

▸ **clear**(): `void`

移除所有数据图表。

#### Returns

`void`

___

### <a id="get" name="get"></a> get

▸ **get**(`name`): [`DataChart`](GC.Spread.Sheets.DataCharts.DataChart.md)

通过名称获取数据图表。

**`example`**
```
activeSheet.datacharts.add('DataChart1', 0, 20, 480, 300, GC.Spread.Sheets.DataCharts.DataChartType.column);
//button
$("#button1").click(function () {
 var dataChart = activeSheet.datacharts.get("DataChart1");
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 数据图表名称。 |

#### Returns

[`DataChart`](GC.Spread.Sheets.DataCharts.DataChart.md)

通过名称获取数据图表。

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`name`): `void`

通过名称移除数据图表。

**`example`**
```
activeSheet.datacharts.add('DataChart1', 0, 20, 480, 300, GC.Spread.Sheets.DataCharts.DataChartType.column);
//button
$("#button1").click(function () {
     activeSheet.resumePaint();
     activeSheet.datacharts.remove("DataChart1");
     activeSheet.repaint();
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 数据图表名称。 |

#### Returns

`void`

___

### <a id="zindex" name="zindex"></a> zIndex

▸ **zIndex**(`name`, `zIndex?`): `any`

获取或设置图表的z-index。

**`example`**
```
activeSheet.datacharts.add('DataChart1', 200, 20, 480, 300, GC.Spread.Sheets.DataCharts.DataChartType.column);
activeSheet.datacharts.add('DataChart2', 0, 20, 480, 300, GC.Spread.Sheets.DataCharts.DataChartType.pie);
activeSheet.datacharts.zIndex('DataChart1', 897);
activeSheet.datacharts.zIndex('DataChart2', 890);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 图表名称。 |
| `zIndex?` | `number` | 图表的z-index。 |

#### Returns

`any`

如果参数'zIndex'为null或undefined，则返回指定名称图表的z-index。
