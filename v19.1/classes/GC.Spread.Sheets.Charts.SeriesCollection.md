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

表示一个图表系列的集合。

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`series`): `void`

向系列集合中添加一个新系列。

**`example`**
```javascript
// 此示例展示如何添加一个新系列。
var dataRange = "A1:D4";
var chart = activeSheet.charts.add('Chart1', GC.Spread.Sheets.Charts.ChartType.columnClustered, 250, 20, 600, 400, dataRange);
chart.series().add({
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

| Name | Type | Description |
| :------ | :------ | :------ |
| `series` | [`ISeries`](../interfaces/GC.Spread.Sheets.Charts.ISeries.md) \| [`ISeries`](../interfaces/GC.Spread.Sheets.Charts.ISeries.md)[] | 图表系列。 |

#### Returns

`void`

___

### <a id="get" name="get"></a> get

▸ **get**(`index?`): `any`

获取系列集合中的所有系列或指定系列。

**`example`**
```javascript
// 此示例展示如何获取一个系列。
var dataRange = "A1:D4";
var chart = activeSheet.charts.add('Chart1', GC.Spread.Sheets.Charts.ChartType.columnClustered, 250, 20, 600, 400, dataRange);
var series1 = chart.series().get(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index?` | `number` | 系列索引。 |

#### Returns

`any`

图表系列。

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`index`): `void`

从系列集合中删除指定系列。

**`example`**
```javascript
// 此示例展示如何删除指定系列。
var dataRange = "A1:D4";
var chart = activeSheet.charts.add('Chart1', GC.Spread.Sheets.Charts.ChartType.columnClustered, 250, 20, 600, 400, dataRange);
chart.series().remove(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 系列索引。 |

#### Returns

`void`

___

### <a id="set" name="set"></a> set

▸ **set**(`index`, `series`): `void`

更新指定系列的属性。

**`example`**
```javascript
// 此示例展示如何更新系列的属性。
var dataRange = "A1:D4";
var chart = activeSheet.charts.add('Chart1', GC.Spread.Sheets.Charts.ChartType.columnClustered, 250, 20, 600, 400, dataRange);
var series1 = chart.series().get(0);
series1.backColor = "red";
chart.series().set(0, series1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 系列索引。 |
| `series` | [`ISeries`](../interfaces/GC.Spread.Sheets.Charts.ISeries.md) | 图表系列。 |

#### Returns

`void`
