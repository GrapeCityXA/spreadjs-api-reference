# Class: Range

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).Range

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Range.md#constructor)

### Properties

- [col](GC.Spread.Sheets.Range.md#col)
- [colCount](GC.Spread.Sheets.Range.md#colcount)
- [row](GC.Spread.Sheets.Range.md#row)
- [rowCount](GC.Spread.Sheets.Range.md#rowcount)

### Methods

- [contains](GC.Spread.Sheets.Range.md#contains)
- [containsRange](GC.Spread.Sheets.Range.md#containsrange)
- [equals](GC.Spread.Sheets.Range.md#equals)
- [getIntersect](GC.Spread.Sheets.Range.md#getintersect)
- [intersect](GC.Spread.Sheets.Range.md#intersect)
- [offset](GC.Spread.Sheets.Range.md#offset)
- [union](GC.Spread.Sheets.Range.md#union)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Range**(`r`, `c`, `rc`, `cc`)

区域，该区域由行索引、列索引、行数和列数组成

**`代码示例`**
```
var style = new GC.Spread.Sheets.Style();
style.backColor = "red";
var rule = new GC.Spread.Sheets.ConditionalFormatting.NormalConditionRule();
rule.ruleType(GC.Spread.Sheets.ConditionalFormatting.RuleType.cellValueRule);
rule.ranges([new GC.Spread.Sheets.Range(0,0,5,1)]);
rule.operator(GC.Spread.Sheets.ConditionalFormatting.ComparisonOperators.between);
rule.style(style);
rule.value1(2);
rule.value2(100);
activeSheet.conditionalFormats.addRule(rule);
activeSheet.setValue(0,0,1,3);
activeSheet.setValue(1,0,45,3);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `r` | `number` | 行索引 |
| `c` | `number` | 列索引 |
| `rc` | `number` | 行数 |
| `cc` | `number` | 列数 |

## Properties

### <a id="col" name="col"></a> col

• **col**: `number`

列索引

**`代码示例`**
```
var cellrange = new GC.Spread.Sheets.Range();
cellrange.col = 0;
cellrange.row = 1;
cellrange.colCount = 1;
cellrange.rowCount = 8;
activeSheet.setValue(1, 0, 1);
activeSheet.setValue(2, 0, -2);
activeSheet.setValue(3, 0, -1);
activeSheet.setValue(4, 0, 6);
activeSheet.setValue(5, 0, 4);
activeSheet.setValue(6, 0, -4);
activeSheet.setValue(7, 0, 3);
activeSheet.setValue(8, 0, 8);
var setting = new GC.Spread.Sheets.Sparklines.SparklineSetting();
setting.options.showMarkers = true;
activeSheet.setSparkline(13, 0, cellrange, GC.Spread.Sheets.Sparklines.DataOrientation.vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
```

___

### <a id="colcount" name="colcount"></a> colCount

• **colCount**: `number`

列数

**`代码示例`**
```
var cellrange = new GC.Spread.Sheets.Range();
cellrange.col = 0;
cellrange.row = 1;
cellrange.colCount = 1;
cellrange.rowCount = 8;
activeSheet.setValue(1, 0, 1);
activeSheet.setValue(2, 0, -2);
activeSheet.setValue(3, 0, -1);
activeSheet.setValue(4, 0, 6);
activeSheet.setValue(5, 0, 4);
activeSheet.setValue(6, 0, -4);
activeSheet.setValue(7, 0, 3);
activeSheet.setValue(8, 0, 8);
var setting = new GC.Spread.Sheets.Sparklines.SparklineSetting();
setting.options.showMarkers = true;
activeSheet.setSparkline(13, 0, cellrange, GC.Spread.Sheets.Sparklines.DataOrientation.vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
```

___

### <a id="row" name="row"></a> row

• **row**: `number`

行索引

**`代码示例`**
```
var cellrange = new GC.Spread.Sheets.Range();
cellrange.col = 0;
cellrange.row = 1;
cellrange.colCount = 1;
cellrange.rowCount = 8;
activeSheet.setValue(1, 0, 1);
activeSheet.setValue(2, 0, -2);
activeSheet.setValue(3, 0, -1);
activeSheet.setValue(4, 0, 6);
activeSheet.setValue(5, 0, 4);
activeSheet.setValue(6, 0, -4);
activeSheet.setValue(7, 0, 3);
activeSheet.setValue(8, 0, 8);
var setting = new GC.Spread.Sheets.Sparklines.SparklineSetting();
setting.options.showMarkers = true;
activeSheet.setSparkline(13, 0, cellrange, GC.Spread.Sheets.Sparklines.DataOrientation.vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
```

___

### <a id="rowcount" name="rowcount"></a> rowCount

• **rowCount**: `number`

行数

**`代码示例`**
```
var cellrange = new GC.Spread.Sheets.Range();
cellrange.col = 0;
cellrange.row = 1;
cellrange.colCount = 1;
cellrange.rowCount = 8;
activeSheet.setValue(1, 0, 1);
activeSheet.setValue(2, 0, -2);
activeSheet.setValue(3, 0, -1);
activeSheet.setValue(4, 0, 6);
activeSheet.setValue(5, 0, 4);
activeSheet.setValue(6, 0, -4);
activeSheet.setValue(7, 0, 3);
activeSheet.setValue(8, 0, 8);
var setting = new GC.Spread.Sheets.Sparklines.SparklineSetting();
setting.options.showMarkers = true;
activeSheet.setSparkline(13, 0, cellrange, GC.Spread.Sheets.Sparklines.DataOrientation.vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
```

## Methods

### <a id="contains" name="contains"></a> contains

▸ **contains**(`row`, `col`, `rowCount?`, `colCount?`): `boolean`

获取当前区域是否包含指定的单元格

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |
| `col` | `number` | 列索引 |
| `rowCount?` | `number` | 行数 |
| `colCount?` | `number` | 列数 |

#### Returns

`boolean`

为`true`时，区域包含单元格；若为`false`则不包含

___

### <a id="containsrange" name="containsrange"></a> containsRange

▸ **containsRange**(`range`): `boolean`

获取当前区域是否包含指定区域

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](GC.Spread.Sheets.Range.md) | 单元格区域 |

#### Returns

`boolean`

为`true`时，当前区域包含指定的单元格区域；若为`false`则不包含

___

### <a id="equals" name="equals"></a> equals

▸ **equals**(`range`): `boolean`

获取当前区域是否等于指定区域

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](GC.Spread.Sheets.Range.md) | 要比较的区域 |

#### Returns

`boolean`

为`true`时，当前区域等于指定的区域;;若为`false`则不等于

___

### <a id="getintersect" name="getintersect"></a> getIntersect

▸ **getIntersect**(`range`, `maxRowCount`, `maxColumnCount`): [`Range`](GC.Spread.Sheets.Range.md)

获取两个单元格区域的交集

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](GC.Spread.Sheets.Range.md) | 单元格区域 |
| `maxRowCount` | `number` | 最大行数 |
| `maxColumnCount` | `number` | 最大列数 |

#### Returns

[`Range`](GC.Spread.Sheets.Range.md)

如果没有交集或交集的单元格区域，则返回null

___

### <a id="intersect" name="intersect"></a> intersect

▸ **intersect**(`row`, `col`, `rowCount`, `colCount`): `boolean`

获取当前区域是否与行和列索引以及行和列计数指定的区域相交

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |
| `col` | `number` | 列索引 |
| `rowCount` | `number` | 行数 |
| `colCount` | `number` | 列数 |

#### Returns

`boolean`

为`true`时，指定区域与当前区域相交；若为`false`则不相交

___

### <a id="offset" name="offset"></a> offset

▸ **offset**(`x`, `y`): [`Range`](GC.Spread.Sheets.Range.md)

按指定的坐标偏移区域的位置

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `x` | `number` | 沿<i>x</i>轴的偏移量 |
| `y` | `number` | 沿<i>y</i>轴的偏移量 |

#### Returns

[`Range`](GC.Spread.Sheets.Range.md)

新位置

___

### <a id="union" name="union"></a> union

▸ **union**(`range`): [`Range`](GC.Spread.Sheets.Range.md)

将此区域与指定的区域连接为一个联合

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](GC.Spread.Sheets.Range.md) | 目标区域 |

#### Returns

[`Range`](GC.Spread.Sheets.Range.md)

返回区域的并集
