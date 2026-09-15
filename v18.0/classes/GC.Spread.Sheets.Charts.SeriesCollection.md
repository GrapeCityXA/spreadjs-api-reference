# Class: SeriesCollection

[Sheets](../modules/GC.Spread.Sheets.md).[Charts](../modules/GC.Spread.Sheets.Charts.md).SeriesCollection

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Charts.SeriesCollection.md#constructor)

### Methods

- [add](GC.Spread.Sheets.Charts.SeriesCollection.md#add)
- [get](GC.Spread.Sheets.Charts.SeriesCollection.md#get)
- [remove](GC.Spread.Sheets.Charts.SeriesCollection.md#remove)
- [set](GC.Spread.Sheets.Charts.SeriesCollection.md#set)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new SeriesCollection**()

图表中的系列管理器

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`series`): `void`

Adds a new series to series collection.

**`代码示例`**
``` javascript
// 本示例展示如何添加新的系列
var dataRange = "A1:D4";
var chart = activeSheet.charts.add('Chart1', GC.Spread.Sheets.Charts.ChartType.columnClustered, 250, 20, 600, 400, dataRange);
chart.series.add({
    chartType: GC.Spread.Sheets.Charts.ChartType.columnClustered,
    axisGroup: GC.Spread.Sheets.Charts.AxisGroup.primary,
    backColor: {
        color: "lightblue",
        width: 2
    },
    xValues: "A2:A4",
    yValues: "B2:B4"
});
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `series` | [`ISeries`](../interfaces/GC.Spread.Sheets.Charts.ISeries.md) \| [`ISeries`](../interfaces/GC.Spread.Sheets.Charts.ISeries.md)[] |

#### Returns

`void`

___

### <a id="get" name="get"></a> get

▸ **get**(`index?`): `any`

从系列集合中获取所有系列或指定的系列

**`代码示例`**
``` javascript
// 本示例展示了如何设置一个系列
var dataRange = "A1:D4";
var chart = activeSheet.charts.add('Chart1', GC.Spread.Sheets.Charts.ChartType.columnClustered, 250, 20, 600, 400, dataRange);
var series1 = chart.series().get(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index?` | `number` | 系列的索引 |

#### Returns

`any`

图表系列

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`index`): `void`

从系列集合中删除指定的系列

**`代码示例`**
``` javascript
// 本示例说明如何删除指定的系列
var dataRange = "A1:D4";
var chart = activeSheet.charts.add('Chart1', GC.Spread.Sheets.Charts.ChartType.columnClustered, 250, 20, 600, 400, dataRange);
chart.series.remove(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 系列的索引 |

#### Returns

`void`

___

### <a id="set" name="set"></a> set

▸ **set**(`index`, `series`): `void`

Updates the specified series's property.

**`代码示例`**
``` javascript
// 本示例演示如何更新系列的属性
var dataRange = "A1:D4";
var chart = activeSheet.charts.add('Chart1', GC.Spread.Sheets.Charts.ChartType.columnClustered, 250, 20, 600, 400, dataRange);
var series1 = chart.series().get(0);
series1.backColor = "red";
chart.series().set(0, series1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 系列的索引 |
| `series` | [`ISeries`](../interfaces/GC.Spread.Sheets.Charts.ISeries.md) | - |

#### Returns

`void`
