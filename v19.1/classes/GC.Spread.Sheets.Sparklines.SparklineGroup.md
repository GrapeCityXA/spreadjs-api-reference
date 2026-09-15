# Class: SparklineGroup

[Sheets](../modules/GC.Spread.Sheets.md).[Sparklines](../modules/GC.Spread.Sheets.Sparklines.md).SparklineGroup

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Sparklines.SparklineGroup.md#constructor)

### Properties

- [setting](GC.Spread.Sheets.Sparklines.SparklineGroup.md#setting)
- [sparklineType](GC.Spread.Sheets.Sparklines.SparklineGroup.md#sparklinetype)

### Methods

- [add](GC.Spread.Sheets.Sparklines.SparklineGroup.md#add)
- [clone](GC.Spread.Sheets.Sparklines.SparklineGroup.md#clone)
- [contains](GC.Spread.Sheets.Sparklines.SparklineGroup.md#contains)
- [count](GC.Spread.Sheets.Sparklines.SparklineGroup.md#count)
- [dateAxisData](GC.Spread.Sheets.Sparklines.SparklineGroup.md#dateaxisdata)
- [dateAxisOrientation](GC.Spread.Sheets.Sparklines.SparklineGroup.md#dateaxisorientation)
- [remove](GC.Spread.Sheets.Sparklines.SparklineGroup.md#remove)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new SparklineGroup**(`type`, `setting`)

表示一个迷你图组。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | [`SparklineType`](../enums/GC.Spread.Sheets.Sparklines.SparklineType.md) | 迷你图的类型。 |
| `setting` | [`SparklineSetting`](GC.Spread.Sheets.Sparklines.SparklineSetting.md) | 迷你图组的设置。 |

## Properties

### <a id="setting" name="setting"></a> setting

• **setting**: [`SparklineSetting`](GC.Spread.Sheets.Sparklines.SparklineSetting.md)

表示迷你图设置。

___

### <a id="sparklinetype" name="sparklinetype"></a> sparklineType

• **sparklineType**: [`SparklineType`](../enums/GC.Spread.Sheets.Sparklines.SparklineType.md)

表示迷你图类型。

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`item`): `void`

向组中添加一个迷你图。

**`example`**
```javascript
let sheet = spread.getActiveSheet();
sheet.setArray(0, 0, [1,2,3,4,3,2,3,5]);
let dataRange = new GC.Spread.Sheets.Range(0, 0, 8, 1);
let setting = new GC.Spread.Sheets.Sparklines.SparklineSetting();
let sparkline1 = sheet.setSparkline(11, 0, dataRange, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
let sparkline2 = sheet.setSparkline(11, 3, dataRange, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
let sparkline3 = sheet.setSparkline(11, 6, dataRange, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.column, setting);
let sparklineGroup = sheet.groupSparkline([sparkline1,sparkline2]);
// 向迷你图组添加一个迷你图
sparklineGroup.add(sparkline3);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | [`Sparkline`](GC.Spread.Sheets.Sparklines.Sparkline.md) | 迷你图项。 |

#### Returns

`void`

___

### <a id="clone" name="clone"></a> clone

▸ **clone**(): [`SparklineGroup`](GC.Spread.Sheets.Sparklines.SparklineGroup.md)

克隆当前的迷你图组。

**`example`**
```javascript
let sheet = spread.getActiveSheet();
sheet.setArray(0, 0, [1,2,3,4,3,2,3,5]);
let dataRange = new GC.Spread.Sheets.Range(0, 0, 8, 1);
let setting = new GC.Spread.Sheets.Sparklines.SparklineSetting();
let sparkline1 = sheet.setSparkline(11, 0, dataRange, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
let sparkline2 = sheet.setSparkline(11, 3, dataRange, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
let sparklineGroup = sheet.groupSparkline([sparkline1,sparkline2]

let sparklineGroup2 = sparklineGroup.clone();
```

#### Returns

[`SparklineGroup`](GC.Spread.Sheets.Sparklines.SparklineGroup.md)

克隆的迷你图组。

___

### <a id="contains" name="contains"></a> contains

▸ **contains**(`item`): `boolean`

确定组中是否包含特定值。

**`example`**
```javascript
let sheet = spread.getActiveSheet();
sheet.setArray(0, 0, [1,2,3,4,3,2,3,5]);
let dataRange = new GC.Spread.Sheets.Range(0, 0, 8, 1);
let setting = new GC.Spread.Sheets.Sparklines.SparklineSetting();
let sparkline1 = sheet.setSparkline(11, 0, dataRange, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
let sparkline2 = sheet.setSparkline(11, 3, dataRange, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
let sparkline3 = sheet.setSparkline(11, 6, dataRange, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
let sparklineGroup = sheet.groupSparkline([sparkline1,sparkline2]);

console.log(sparklineGroup.contains(sparkline1)); // true
console.log(sparklineGroup.contains(sparkline3)); // false
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | [`Sparkline`](GC.Spread.Sheets.Sparklines.Sparkline.md) | 要在组中定位的对象。 |

#### Returns

`boolean`

如果在组中找到该项，则为 `true`；否则为 `false`。

___

### <a id="count" name="count"></a> count

▸ **count**(): `number`

表示迷你图组内部列表的数量。

**`example`**
```javascript
let sheet = spread.getActiveSheet();
sheet.setArray(0, 0, [1,2,3,4,3,2,3,5]);
let dataRange = new GC.Spread.Sheets.Range(0, 0, 8, 1);
let setting = new GC.Spread.Sheets.Sparklines.SparklineSetting();
let sparkline1 = sheet.setSparkline(11, 0, dataRange, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
let sparkline2 = sheet.setSparkline(11, 3, dataRange, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
let sparklineGroup = sheet.groupSparkline([sparkline1,sparkline2]);

console.log(sparklineGroup.count()); // 2
```

#### Returns

`number`

组中的迷你图数量。

___

### <a id="dateaxisdata" name="dateaxisdata"></a> dateAxisData

▸ **dateAxisData**(`value?`): `any`

表示日期轴数据。

**`example`**
```javascript
let sheet = spread.getActiveSheet();
sheet.setArray(0, 0, [-1,2,3,4,3,2,3,5]);
let dataRange = new GC.Spread.Sheets.Range(0, 0, 8, 1);
let setting = new GC.Spread.Sheets.Sparklines.SparklineSetting();
let sparkline1 = sheet.setSparkline(11, 0, dataRange, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
let sparkline2 = sheet.setSparkline(11, 3, dataRange, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
let sparklineGroup = sheet.groupSparkline([sparkline1,sparkline2]);

sheet.setArray(0, 1, [1,4,6,5,3,6,10,2]);
sparklineGroup.dateAxisData(new GC.Spread.Sheets.Range(0, 1, 8, 1));
console.log(sparklineGroup.dateAxisData());
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`Range`](GC.Spread.Sheets.Range.md) | 日期轴数据。 |

#### Returns

`any`

如果未设置值，则返回日期轴数据；否则返回 undefined。

___

### <a id="dateaxisorientation" name="dateaxisorientation"></a> dateAxisOrientation

▸ **dateAxisOrientation**(`value`): `any`

表示日期轴方向。

**`example`**
```javascript
let sheet = spread.getActiveSheet();
sheet.setArray(0, 0, [-1,2,3,4,3,2,3,5]);
let dataRange = new GC.Spread.Sheets.Range(0, 0, 8, 1);
let setting = new GC.Spread.Sheets.Sparklines.SparklineSetting();
let sparkline1 = sheet.setSparkline(11, 0, dataRange, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
let sparkline2 = sheet.setSparkline(11, 3, dataRange, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
let sparklineGroup = sheet.groupSparkline([sparkline1,sparkline2]);

sheet.setArray(0, 1, [1,4,6,5,3,6,10,2]);
sparklineGroup.dateAxisData(new GC.Spread.Sheets.Range(0, 1, 8, 1));
sparklineGroup.dateAxisOrientation(GC.Spread.Sheets.Sparklines.DataOrientation.Vertical);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value` | [`DataOrientation`](../enums/GC.Spread.Sheets.Sparklines.DataOrientation.md) |

#### Returns

`any`

如果未设置值，则返回日期轴方向；否则返回 undefined。

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`item`): [`Sparkline`](GC.Spread.Sheets.Sparklines.Sparkline.md)[]

从组中删除第一个出现的特定对象。

**`example`**
```javascript
let sheet = spread.getActiveSheet();
sheet.setArray(0, 0, [-1,2,3,4,3,2,3,5]);
let dataRange = new GC.Spread.Sheets.Range(0, 0, 8, 1);
let setting = new GC.Spread.Sheets.Sparklines.SparklineSetting();
let sparkline1 = sheet.setSparkline(11, 0, dataRange, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
let sparkline2 = sheet.setSparkline(11, 3, dataRange, GC.Spread.Sheets.Sparklines.DataOrientation.Vertical, GC.Spread.Sheets.Sparklines.SparklineType.line, setting);
let sparklineGroup = sheet.groupSparkline([sparkline1,sparkline2]);

console.log(sparklineGroup.count()) // 2
sparklineGroup.remove(sparkline1);
console.log(sparklineGroup.count()) // 1
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | [`Sparkline`](GC.Spread.Sheets.Sparklines.Sparkline.md) | 迷你图项。 |

#### Returns

[`Sparkline`](GC.Spread.Sheets.Sparklines.Sparkline.md)[]

迷你图数组。
