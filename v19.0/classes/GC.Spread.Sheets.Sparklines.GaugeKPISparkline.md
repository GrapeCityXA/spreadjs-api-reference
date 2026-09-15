# Class: GaugeKPISparkline

[Sheets](../modules/GC.Spread.Sheets.md).[Sparklines](../modules/GC.Spread.Sheets.Sparklines.md).GaugeKPISparkline

## Hierarchy

- [`SparklineEx`](GC.Spread.Sheets.Sparklines.SparklineEx.md)

  ↳ **`GaugeKPISparkline`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Sparklines.GaugeKPISparkline.md#constructor)

### Properties

- [typeName](GC.Spread.Sheets.Sparklines.GaugeKPISparkline.md#typename)

### Methods

- [createFunction](GC.Spread.Sheets.Sparklines.GaugeKPISparkline.md#createfunction)
- [fromJSON](GC.Spread.Sheets.Sparklines.GaugeKPISparkline.md#fromjson)
- [name](GC.Spread.Sheets.Sparklines.GaugeKPISparkline.md#name)
- [paint](GC.Spread.Sheets.Sparklines.GaugeKPISparkline.md#paint)
- [toJSON](GC.Spread.Sheets.Sparklines.GaugeKPISparkline.md#tojson)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new GaugeKPISparkline**()

表示仪表盘KPI迷你图的类。

#### Overrides

[SparklineEx](GC.Spread.Sheets.Sparklines.SparklineEx.md).[constructor](GC.Spread.Sheets.Sparklines.SparklineEx.md#constructor)

## Properties

### <a id="typename" name="typename"></a> typeName

• **typeName**: `string`

表示用于支持序列化的类型名称字符串。

#### Inherited from

[SparklineEx](GC.Spread.Sheets.Sparklines.SparklineEx.md).[typeName](GC.Spread.Sheets.Sparklines.SparklineEx.md#typename)

## Methods

### <a id="createfunction" name="createfunction"></a> createFunction

▸ **createFunction**(): [`Function`](GC.Spread.CalcEngine.Functions.Function.md)

创建一个自定义函数，用于为SparklineEx提供数据和设置。

#### Returns

[`Function`](GC.Spread.CalcEngine.Functions.Function.md)

创建的自定义函数。

#### Inherited from

[SparklineEx](GC.Spread.Sheets.Sparklines.SparklineEx.md).[createFunction](GC.Spread.Sheets.Sparklines.SparklineEx.md#createfunction)

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

#### Inherited from

[SparklineEx](GC.Spread.Sheets.Sparklines.SparklineEx.md).[fromJSON](GC.Spread.Sheets.Sparklines.SparklineEx.md#fromjson)

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

#### Inherited from

[SparklineEx](GC.Spread.Sheets.Sparklines.SparklineEx.md).[name](GC.Spread.Sheets.Sparklines.SparklineEx.md#name)

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

#### Inherited from

[SparklineEx](GC.Spread.Sheets.Sparklines.SparklineEx.md).[paint](GC.Spread.Sheets.Sparklines.SparklineEx.md#paint)

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

#### Inherited from

[SparklineEx](GC.Spread.Sheets.Sparklines.SparklineEx.md).[toJSON](GC.Spread.Sheets.Sparklines.SparklineEx.md#tojson)
