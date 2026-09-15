# Class: SparklineEx

[Sheets](../modules/GC.Spread.Sheets.md).[Sparklines](../modules/GC.Spread.Sheets.Sparklines.md).SparklineEx

## Hierarchy

- **`SparklineEx`**

  ↳ [`Codabar`](GC.Spread.Sheets.Barcode.Codabar.md)

  ↳ [`Code128`](GC.Spread.Sheets.Barcode.Code128.md)

  ↳ [`Code39`](GC.Spread.Sheets.Barcode.Code39.md)

  ↳ [`Code49`](GC.Spread.Sheets.Barcode.Code49.md)

  ↳ [`Code93`](GC.Spread.Sheets.Barcode.Code93.md)

  ↳ [`DataMatrix`](GC.Spread.Sheets.Barcode.DataMatrix.md)

  ↳ [`EAN13`](GC.Spread.Sheets.Barcode.EAN13.md)

  ↳ [`EAN8`](GC.Spread.Sheets.Barcode.EAN8.md)

  ↳ [`GS1_128`](GC.Spread.Sheets.Barcode.GS1_128.md)

  ↳ [`PDF417`](GC.Spread.Sheets.Barcode.PDF417.md)

  ↳ [`QRCode`](GC.Spread.Sheets.Barcode.QRCode.md)

  ↳ [`AreaSparkline`](GC.Spread.Sheets.Sparklines.AreaSparkline.md)

  ↳ [`BoxPlotSparkline`](GC.Spread.Sheets.Sparklines.BoxPlotSparkline.md)

  ↳ [`BulletSparkline`](GC.Spread.Sheets.Sparklines.BulletSparkline.md)

  ↳ [`CascadeSparkline`](GC.Spread.Sheets.Sparklines.CascadeSparkline.md)

  ↳ [`ColumnSparkline`](GC.Spread.Sheets.Sparklines.ColumnSparkline.md)

  ↳ [`GaugeKPISparkline`](GC.Spread.Sheets.Sparklines.GaugeKPISparkline.md)

  ↳ [`HBarSparkline`](GC.Spread.Sheets.Sparklines.HBarSparkline.md)

  ↳ [`HistogramSparkline`](GC.Spread.Sheets.Sparklines.HistogramSparkline.md)

  ↳ [`ImageSparkline`](GC.Spread.Sheets.Sparklines.ImageSparkline.md)

  ↳ [`LineSparkline`](GC.Spread.Sheets.Sparklines.LineSparkline.md)

  ↳ [`LollipopVariSparkline`](GC.Spread.Sheets.Sparklines.LollipopVariSparkline.md)

  ↳ [`MonthSparkline`](GC.Spread.Sheets.Sparklines.MonthSparkline.md)

  ↳ [`ParetoSparkline`](GC.Spread.Sheets.Sparklines.ParetoSparkline.md)

  ↳ [`PieSparkline`](GC.Spread.Sheets.Sparklines.PieSparkline.md)

  ↳ [`RangeBlockSparkline`](GC.Spread.Sheets.Sparklines.RangeBlockSparkline.md)

  ↳ [`ScatterSparkline`](GC.Spread.Sheets.Sparklines.ScatterSparkline.md)

  ↳ [`SpreadSparkline`](GC.Spread.Sheets.Sparklines.SpreadSparkline.md)

  ↳ [`StackedSparkline`](GC.Spread.Sheets.Sparklines.StackedSparkline.md)

  ↳ [`VariSparkline`](GC.Spread.Sheets.Sparklines.VariSparkline.md)

  ↳ [`VBarSparkline`](GC.Spread.Sheets.Sparklines.VBarSparkline.md)

  ↳ [`WinlossSparkline`](GC.Spread.Sheets.Sparklines.WinlossSparkline.md)

  ↳ [`YearSparkline`](GC.Spread.Sheets.Sparklines.YearSparkline.md)

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Sparklines.SparklineEx.md#constructor)

### Properties

- [typeName](GC.Spread.Sheets.Sparklines.SparklineEx.md#typename)

### Methods

- [createFunction](GC.Spread.Sheets.Sparklines.SparklineEx.md#createfunction)
- [fromJSON](GC.Spread.Sheets.Sparklines.SparklineEx.md#fromjson)
- [name](GC.Spread.Sheets.Sparklines.SparklineEx.md#name)
- [paint](GC.Spread.Sheets.Sparklines.SparklineEx.md#paint)
- [toJSON](GC.Spread.Sheets.Sparklines.SparklineEx.md#tojson)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new SparklineEx**()

表示其他SparklineEx类的基类。

## Properties

### <a id="typename" name="typename"></a> typeName

• **typeName**: `string`

表示用于支持序列化的类型名称字符串。

## Methods

### <a id="createfunction" name="createfunction"></a> createFunction

▸ **createFunction**(): [`Function`](GC.Spread.CalcEngine.Functions.Function.md)

创建一个自定义函数，用于为SparklineEx提供数据和设置。

#### Returns

[`Function`](GC.Spread.CalcEngine.Functions.Function.md)

创建的自定义函数。

___

### <a id="fromjson" name="fromjson"></a> fromJSON

▸ **fromJSON**(`settings`): `void`

从指定的JSON字符串加载对象状态。

**`example`**
```javascript
window.MySparklineEx = function(color) {
    GC.Spread.Sheets.Sparklines.SparklineEx.apply(this, arguments);
    this.typeName = 'MySparklineEx';
    this.color = color;
}
MySparklineEx.prototype = new GC.Spread.Sheets.Sparklines.SparklineEx();
MySparklineEx.prototype.createFunction = function () {
    var func = new GC.Spread.CalcEngine.Functions.Function('CIRCLE', 0, 0);
    func.evaluate = function (args) {
          return {};
    };
    return func;
 };
MySparklineEx.prototype.paint = function (context, value, x, y, width, height) {
     context.beginPath();
     context.arc(x + width / 2, y + height / 2, (Math.min(width, height) - 6) / 2, 0, Math.PI * 2);
     context.strokeStyle = this.color;
     context.stroke();
};
let sparkline = new MySparklineEx("green");
sparkline.fromJSON({ color: "red", typeName: "MySparklineEx" });
spread.addSparklineEx(sparkline);
sheet.setFormula(3,3,"=CIRCLE()");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `settings` | `Object` | 来自反序列化的sparklineEx数据。 |

#### Returns

`void`

___

### <a id="name" name="name"></a> name

▸ **name**(): `string`

获取SparklineEx的名称。

**`example`**
```javascript
window.MySparklineEx = function(color) {
    GC.Spread.Sheets.Sparklines.SparklineEx.apply(this, arguments);
    this.typeName = 'MySparklineEx';
    this.color = color;
}
MySparklineEx.prototype = new GC.Spread.Sheets.Sparklines.SparklineEx();
MySparklineEx.prototype.createFunction = function () {
    var func = new GC.Spread.CalcEngine.Functions.Function('CIRCLE', 0, 0);
    func.evaluate = function (args) {
          return {};
    };
    return func;
 };
MySparklineEx.prototype.paint = function (context, value, x, y, width, height) {
     context.beginPath();
     context.arc(x + width / 2, y + height / 2, (Math.min(width, height) - 6) / 2, 0, Math.PI * 2);
     context.strokeStyle = this.color;
     context.stroke();
};
let sparkline = new MySparklineEx('green');
console.log(sparkline.name());
```

#### Returns

`string`

SparklineEx的名称。

___

### <a id="paint" name="paint"></a> paint

▸ **paint**(`context`, `value`, `x`, `y`, `width`, `height`): `void`

在画布上绘制SparklineEx。

**`example`**
```javascript
window.MySparklineEx = function(color) {
    GC.Spread.Sheets.Sparklines.SparklineEx.apply(this, arguments);
    this.typeName = 'MySparklineEx';
    this.color = color;
}
MySparklineEx.prototype = new GC.Spread.Sheets.Sparklines.SparklineEx();
MySparklineEx.prototype.createFunction = function () {
    var func = new GC.Spread.CalcEngine.Functions.Function('CIRCLE', 0, 0);
    func.evaluate = function (args) {
          return {};
    };
    return func;
 };
MySparklineEx.prototype.paint = function (context, value, x, y, width, height) {
     context.beginPath();
     context.arc(x + width / 2, y + height / 2, (Math.min(width, height) - 6) / 2, 0, Math.PI * 2);
     context.strokeStyle = this.color;
     context.stroke();
};
let sparkline = new MySparklineEx('green');
spread.addSparklineEx(sparkline);
let sheet = spread.getActiveSheet();
sheet.setFormula(3,3,"=CIRCLE()");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `context` | `CanvasRenderingContext2D` | 画布的二维上下文。 |
| `value` | `any` | 由自定义函数计算的值。 |
| `x` | `number` | 相对于画布的<i>x</i>坐标。 |
| `y` | `number` | 相对于画布的<i>y</i>坐标。 |
| `width` | `number` | 单元格的宽度。 |
| `height` | `number` | 单元格的高度。 |

#### Returns

`void`

___

### <a id="tojson" name="tojson"></a> toJSON

▸ **toJSON**(): `Object`

将对象状态保存为JSON字符串。

**`example`**
```javascript
window.MySparklineEx = function(color) {
    GC.Spread.Sheets.Sparklines.SparklineEx.apply(this, arguments);
    this.typeName = 'MySparklineEx';
    this.color = color;
}
MySparklineEx.prototype = new GC.Spread.Sheets.Sparklines.SparklineEx();
MySparklineEx.prototype.createFunction = function () {
    var func = new GC.Spread.CalcEngine.Functions.Function('CIRCLE', 0, 0);
    func.evaluate = function (args) {
          return {};
    };
    return func;
 };
MySparklineEx.prototype.paint = function (context, value, x, y, width, height) {
     context.beginPath();
     context.arc(x + width / 2, y + height / 2, (Math.min(width, height) - 6) / 2, 0, Math.PI * 2);
     context.strokeStyle = this.color;
     context.stroke();
};
let sparkline = new MySparklineEx('green');
console.log(sparkline.toJSON()); // { color: "green", typeName: "MySparklineEx", _name: "CIRCLE" }
```

#### Returns

`Object`

sparklineEx数据。
