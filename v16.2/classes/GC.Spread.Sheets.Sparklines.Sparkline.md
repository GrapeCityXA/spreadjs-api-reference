# Class: Sparkline

[Sheets](../modules/GC.Spread.Sheets.md).[Sparklines](../modules/GC.Spread.Sheets.Sparklines.md).Sparkline

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Sparklines.Sparkline.md#constructor)

### Properties

- [column](GC.Spread.Sheets.Sparklines.Sparkline.md#column)
- [row](GC.Spread.Sheets.Sparklines.Sparkline.md#row)

### Methods

- [clone](GC.Spread.Sheets.Sparklines.Sparkline.md#clone)
- [data](GC.Spread.Sheets.Sparklines.Sparkline.md#data)
- [dataOrientation](GC.Spread.Sheets.Sparklines.Sparkline.md#dataorientation)
- [dateAxisData](GC.Spread.Sheets.Sparklines.Sparkline.md#dateaxisdata)
- [dateAxisOrientation](GC.Spread.Sheets.Sparklines.Sparkline.md#dateaxisorientation)
- [displayDateAxis](GC.Spread.Sheets.Sparklines.Sparkline.md#displaydateaxis)
- [group](GC.Spread.Sheets.Sparklines.Sparkline.md#group)
- [paintSparkline](GC.Spread.Sheets.Sparklines.Sparkline.md#paintsparkline)
- [setting](GC.Spread.Sheets.Sparklines.Sparkline.md#setting)
- [sparklineType](GC.Spread.Sheets.Sparklines.Sparkline.md#sparklinetype)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Sparkline**(`row?`, `column?`, `dataReference?`, `dataOrientation?`, `type?`, `setting?`)

迷你图类

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row?` | `number` | 行索引 |
| `column?` | `number` | 列索引 |
| `dataReference?` | [`Range`](GC.Spread.Sheets.Range.md) | 迷你图所引用的数据区域 |
| `dataOrientation?` | [`DataOrientation`](../enums/GC.Spread.Sheets.Sparklines.DataOrientation.md) | 数据区域的方向 |
| `type?` | [`SparklineType`](../enums/GC.Spread.Sheets.Sparklines.SparklineType.md) | 迷你图的类型 |
| `setting?` | [`SparklineSetting`](GC.Spread.Sheets.Sparklines.SparklineSetting.md) | 迷你图的设置 |

## Properties

### <a id="column" name="column"></a> column

• **column**: `number`

获取列索引

___

### <a id="row" name="row"></a> row

• **row**: `number`

获取行索引

## Methods

### <a id="clone" name="clone"></a> clone

▸ **clone**(): [`Sparkline`](GC.Spread.Sheets.Sparklines.Sparkline.md)

克隆迷你图

#### Returns

[`Sparkline`](GC.Spread.Sheets.Sparklines.Sparkline.md)

克隆的迷你图

___

### <a id="data" name="data"></a> data

▸ **data**(`value?`): `any`

获取或设置数据对象

**`代码示例`**
```
//本示例使用data方法
activeSheet.suspendPaint();
activeSheet.setValue(1, 0, 10);
activeSheet.setValue(2, 0, 0);
activeSheet.setValue(3, 0, -3);
activeSheet.setValue(4, 0, -5);
activeSheet.setValue(0, 0, 1);
activeSheet.setValue(0, 1, 2);
activeSheet.setValue(0, 2, 4);
activeSheet.setValue(0, 3, 8);
activeSheet.setValue(0, 4, 6);
activeSheet.setValue(0, 5, new Date(2014, 1, 1));
activeSheet.setValue(1, 5, new Date(2014, 9, 1));
activeSheet.setValue(2, 5, new Date(2014, 7, 1));
activeSheet.setValue(3, 5, new Date(2014, 5, 1));
activeSheet.setValue(4, 5, new Date(2014, 3, 1));
var sparkline = activeSheet.setSparkline(5, 0, new GC.Spread.Sheets.Range(0, 0, 5, 5), GC.Spread.Sheets.Sparklines.DataOrientation.horizontal, GC.Spread.Sheets.Sparklines.SparklineType.line, new GC.Spread.Sheets.Sparklines.SparklineSetting(), new GC.Spread.Sheets.Range(0, 5, 5, 1), GC.Spread.Sheets.Sparklines.DataOrientation.vertical);
sparkline.data(new GC.Spread.Sheets.Range(0, 0, 5, 5));
sparkline.sparklineType(GC.Spread.Sheets.Sparklines.SparklineType.line);
sparkline.setting(new GC.Spread.Sheets.Sparklines.SparklineSetting());
sparkline.dateAxisData(new GC.Spread.Sheets.Range(0, 5, 5, 1));
sparkline.dataOrientation(GC.Spread.Sheets.Sparklines.DataOrientation.vertical);
sparkline.dateAxisOrientation(GC.Spread.Sheets.Sparklines.DataOrientation.vertical);
sparkline.row = 5;
sparkline.column = 0;
sparkline.displayDateAxis(true);
activeSheet.resumePaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`Range`](GC.Spread.Sheets.Range.md) | 迷你图数据 |

#### Returns

`any`

如果未设置任何值,则返回数据对象;否则,返回迷你图

___

### <a id="dataorientation" name="dataorientation"></a> dataOrientation

▸ **dataOrientation**(`value?`): `any`

获取或设置数据方向

**`代码示例`**
```
//本示例使用垂直数据和日期区域创建迷你图
var setting = new GC.Spread.Sheets.Sparklines.SparklineSetting();
setting.options.showMarkers = true;
setting.options.displayXAxis = true;
activeSheet.suspendPaint();
activeSheet.setValue(1, 0, 10);
activeSheet.setValue(2, 0, 0);
activeSheet.setValue(3, 0, -3);
activeSheet.setValue(4, 0, -5);
activeSheet.setValue(0, 0, 1);
activeSheet.setValue(0, 1, 2);
activeSheet.setValue(0, 2, 4);
activeSheet.setValue(0, 3, 8);
activeSheet.setValue(0, 4, 6);
activeSheet.setValue(0, 5, new Date(2014, 1, 1));
activeSheet.setValue(1, 5, new Date(2014, 9, 1));
activeSheet.setValue(2, 5, new Date(2014, 7, 1));
activeSheet.setValue(3, 5, new Date(2014, 5, 1));
activeSheet.setValue(4, 5, new Date(2014, 3, 1));
var sparkline = activeSheet.setSparkline(5, 0, new GC.Spread.Sheets.Range(0, 0, 5, 5), GC.Spread.Sheets.Sparklines.DataOrientation.horizontal, GC.Spread.Sheets.Sparklines.SparklineType.line, setting, new GC.Spread.Sheets.Range(0, 5, 5, 1), GC.Spread.Sheets.Sparklines.DataOrientation.vertical);
sparkline.dataOrientation(GC.Spread.Sheets.Sparklines.DataOrientation.vertical);
sparkline.displayDateAxis(true);
activeSheet.resumePaint();
activeSheet.addSpan(5, 0, 4, 3, null);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`DataOrientation`](../enums/GC.Spread.Sheets.Sparklines.DataOrientation.md) | 迷你图数据方向 |

#### Returns

`any`

如果未设置任何值,则返回迷你图数据方向 否则,返回迷你图

___

### <a id="dateaxisdata" name="dateaxisdata"></a> dateAxisData

▸ **dateAxisData**(`value?`): `any`

获取或设置日期轴数据对象

**`代码示例`**
```
//本示例使用dateAxisData方法
activeSheet.suspendPaint();
activeSheet.setValue(1, 0, 10);
activeSheet.setValue(2, 0, 0);
activeSheet.setValue(3, 0, -3);
activeSheet.setValue(4, 0, -5);
activeSheet.setValue(0, 0, 1);
activeSheet.setValue(0, 1, 2);
activeSheet.setValue(0, 2, 4);
activeSheet.setValue(0, 3, 8);
activeSheet.setValue(0, 4, 6);
activeSheet.setValue(0, 5, new Date(2014, 1, 1));
activeSheet.setValue(1, 5, new Date(2014, 9, 1));
activeSheet.setValue(2, 5, new Date(2014, 7, 1));
activeSheet.setValue(3, 5, new Date(2014, 5, 1));
activeSheet.setValue(4, 5, new Date(2014, 3, 1));
var sparkline = activeSheet.setSparkline(5, 0, new GC.Spread.Sheets.Range(0, 0, 5, 5), GC.Spread.Sheets.Sparklines.DataOrientation.horizontal, GC.Spread.Sheets.Sparklines.SparklineType.line, new GC.Spread.Sheets.Sparklines.SparklineSetting(), new GC.Spread.Sheets.Range(0, 5, 5, 1), GC.Spread.Sheets.Sparklines.DataOrientation.vertical);
sparkline.data(new GC.Spread.Sheets.Range(0, 0, 5, 5));
sparkline.sparklineType(GC.Spread.Sheets.Sparklines.SparklineType.line);
sparkline.setting(new GC.Spread.Sheets.Sparklines.SparklineSetting());
sparkline.dateAxisData(new GC.Spread.Sheets.Range(0, 5, 5, 1));
sparkline.dataOrientation(GC.Spread.Sheets.Sparklines.DataOrientation.vertical);
sparkline.dateAxisOrientation(GC.Spread.Sheets.Sparklines.DataOrientation.vertical);
sparkline.row = 5;
sparkline.column = 0;
sparkline.displayDateAxis(true);
activeSheet.resumePaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`Range`](GC.Spread.Sheets.Range.md) | 迷你图日期轴数据 |

#### Returns

`any`

如果未设置任何值,则返回迷你图日期轴数据 否则,返回迷你图

___

### <a id="dateaxisorientation" name="dateaxisorientation"></a> dateAxisOrientation

▸ **dateAxisOrientation**(`value?`): `any`

获取或设置日期轴方向

**`代码示例`**
```
//本示例使用带有水平日期的垂直数据来创建迷你图
var setting = new GC.Spread.Sheets.Sparklines.SparklineSetting();
setting.options.showMarkers = true;
setting.options.displayXAxis = true;
activeSheet.suspendPaint();
activeSheet.setValue(1, 0, 10);
activeSheet.setValue(2, 0, 0);
activeSheet.setValue(3, 0, -3);
activeSheet.setValue(4, 0, -5);
activeSheet.setValue(0, 0, 1);
activeSheet.setValue(0, 1, 2);
activeSheet.setValue(0, 2, 4);
activeSheet.setValue(0, 3, 8);
activeSheet.setValue(0, 4, 6);
activeSheet.setValue(0, 5, new Date(2014, 1, 1));
activeSheet.setValue(1, 5, new Date(2014, 9, 1));
activeSheet.setValue(2, 5, new Date(2014, 7, 1));
activeSheet.setValue(3, 5, new Date(2014, 5, 1));
activeSheet.setValue(4, 5, new Date(2014, 3, 1));
activeSheet.setValue(11, 0, new Date(2014, 1, 1));
activeSheet.setValue(11, 1, new Date(2014, 9, 1));
activeSheet.setValue(11, 2, new Date(2014, 7, 1));
activeSheet.setValue(11, 3, new Date(2014, 5, 1));
activeSheet.setValue(11, 4, new Date(2014, 3, 1));
var sparkline = activeSheet.setSparkline(5, 0, new GC.Spread.Sheets.Range(0, 0, 5, 5), GC.Spread.Sheets.Sparklines.DataOrientation.vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting, new GC.Spread.Sheets.Range(11, 0, 1, 5), GC.Spread.Sheets.Sparklines.DataOrientation.horizontal);
sparkline.dataOrientation(GC.Spread.Sheets.Sparklines.DataOrientation.vertical);
sparkline.dateAxisOrientation(GC.Spread.Sheets.Sparklines.DataOrientation.horizontal);
sparkline.displayDateAxis(true);
activeSheet.resumePaint();
activeSheet.addSpan(5, 0, 4, 3, null);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`DataOrientation`](../enums/GC.Spread.Sheets.Sparklines.DataOrientation.md) | 迷你图日期轴方向 |

#### Returns

`any`

如果未设置任何值,则返回迷你图日期轴的方向;否则,返回迷你图

___

### <a id="displaydateaxis" name="displaydateaxis"></a> displayDateAxis

▸ **displayDateAxis**(`value?`): `any`

获取或设置一个值,该值指示是否显示日期轴

**`代码示例`**
```
//本示例使用垂直数据和日期区域创建迷你图
var setting = new GC.Spread.Sheets.Sparklines.SparklineSetting();
setting.options.showMarkers = true;
setting.options.displayXAxis = true;
activeSheet.suspendPaint();
activeSheet.setValue(1, 0, 10);
activeSheet.setValue(2, 0, 0);
activeSheet.setValue(3, 0, -3);
activeSheet.setValue(4, 0, -5);
activeSheet.setValue(0, 0, 1);
activeSheet.setValue(0, 1, 2);
activeSheet.setValue(0, 2, 4);
activeSheet.setValue(0, 3, 8);
activeSheet.setValue(0, 4, 6);
activeSheet.setValue(0, 5, new Date(2014, 1, 1));
activeSheet.setValue(1, 5, new Date(2014, 9, 1));
activeSheet.setValue(2, 5, new Date(2014, 7, 1));
activeSheet.setValue(3, 5, new Date(2014, 5, 1));
activeSheet.setValue(4, 5, new Date(2014, 3, 1));
var sparkline = activeSheet.setSparkline(5, 0, new GC.Spread.Sheets.Range(0, 0, 5, 5), GC.Spread.Sheets.Sparklines.DataOrientation.horizontal, GC.Spread.Sheets.Sparklines.SparklineType.line, setting, new GC.Spread.Sheets.Range(0, 5, 5, 1), GC.Spread.Sheets.Sparklines.DataOrientation.vertical);
sparkline.dataOrientation(GC.Spread.Sheets.Sparklines.DataOrientation.vertical);
sparkline.displayDateAxis(true);
activeSheet.resumePaint();
activeSheet.addSpan(5, 0, 4, 3, null);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否显示日期轴 |

#### Returns

`any`

如果未设置任何值,则返回是否显示日期轴 否则,返回迷你图

___

### <a id="group" name="group"></a> group

▸ **group**(`value?`): `any`

获取或设置迷你图组

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SparklineGroup`](GC.Spread.Sheets.Sparklines.SparklineGroup.md) | 迷你图组 |

#### Returns

`any`

如果未设置任何值,则返回迷你图组 否则,返回迷你图

___

### <a id="paintsparkline" name="paintsparkline"></a> paintSparkline

▸ **paintSparkline**(`ctx`, `x`, `y`, `w`, `h`): `void`

在指定区域绘制迷你图

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ctx` | `CanvasRenderingContext2D` | 画布的二维上下文 |
| `x` | `number` | <i> x </i>相对于画布的坐标 |
| `y` | `number` | 相对于画布的<i> y </i>坐标 |
| `w` | `number` | 包含迷你图的单元格的宽度 |
| `h` | `number` | 包含迷你图的单元格的高度 |

#### Returns

`void`

___

### <a id="setting" name="setting"></a> setting

▸ **setting**(`value?`): `any`

获取或设置单元格的迷你图设置

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SparklineSetting`](GC.Spread.Sheets.Sparklines.SparklineSetting.md) | 迷你图设置 |

#### Returns

`any`

如果未设置任何值,则返回迷你图设置 否则,返回迷你图

___

### <a id="sparklinetype" name="sparklinetype"></a> sparklineType

▸ **sparklineType**(`value?`): `any`

获取或设置迷你图的类型

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`SparklineType`](../enums/GC.Spread.Sheets.Sparklines.SparklineType.md) | 迷你图的类型 |

#### Returns

`any`

如果未设置任何值,则返回迷你图类型 否则,返回迷你图
