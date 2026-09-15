# Class: ShapeStyle

[Sheets](../modules/GC.Spread.Sheets.md).[Shapes](../modules/GC.Spread.Sheets.Shapes.md).ShapeStyle

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Shapes.ShapeStyle.md#constructor)

### Properties

- [fill](GC.Spread.Sheets.Shapes.ShapeStyle.md#fill)
- [line](GC.Spread.Sheets.Shapes.ShapeStyle.md#line)
- [textEffect](GC.Spread.Sheets.Shapes.ShapeStyle.md#texteffect)
- [textFrame](GC.Spread.Sheets.Shapes.ShapeStyle.md#textframe)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new ShapeStyle**(`style?`)

形状样式

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `style?` | `Object` | 样式是与ShapeStyle实例具有相同结构的对象，它是可选的 |

## Properties

### <a id="fill" name="fill"></a> fill

• **fill**: [`IShapeFill`](../interfaces/GC.Spread.Sheets.Shapes.IShapeFill.md) \| [`IShapeGradientFill`](../interfaces/GC.Spread.Sheets.Shapes.IShapeGradientFill.md) \| [`IShapePictureFill`](../interfaces/GC.Spread.Sheets.Shapes.IShapePictureFill.md) \| [`IShapeTextureFill`](../interfaces/GC.Spread.Sheets.Shapes.IShapeTextureFill.md)

填充选项

**`example`**
```
//本示例设置形状的背景色和背景色透明度
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var oldStyle = heart.style();
oldStyle.fill = {
    type: GC.Spread.Sheets.Shapes.ShapeFillType.solid,
    color: "red",
    transparency: 0.5
};
heart.style(oldStyle);

//本示例为形状设置渐变背景
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var oldStyle = heart.style();
oldStyle.fill = {
    type: GC.Spread.Sheets.Shapes.GradientFillType.linear,
    angle: 45,
    stops: [
        { color: 'blue', position: 0},
        { color: 'pink', position: 1}
    ]
};
heart.style(oldStyle);

//本示例设置形状的图片背景
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var oldStyle = heart.style();
oldStyle.fill = { src: "data:image/svg+xml;base64....." };
heart.style(oldStyle);

//本示例使用形状的公式设置背景色和背景色透明度
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
sheet.setValue(0, 1, 1);
sheet.setValue(1, 1, "red");
sheet.setValue(2, 1, 0.5);
var oldStyle = heart.style();
oldStyle.fill = {
    type: "=Sheet1!B1",
    color: "=Sheet1!B2",
    transparency: "=Sheet1!B3"
};
heart.style(oldStyle);

//本示例使用形状公式设置渐变背景
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var oldStyle = heart.style();
oldStyle.fill = {
    type: "=Sheet1!A1",
    angle: "=Sheet1!B1",
    stops: [
        { color: "=Sheet1!A2", position: "=Sheet1!B2"},
        { color: "=Sheet1!A3", position: "=Sheet1!B3"}
    ]
};
heart.style(oldStyle);
```

___

### <a id="line" name="line"></a> line

• **line**: [`IShapeLine`](../interfaces/GC.Spread.Sheets.Shapes.IShapeLine.md)

线形选项

**`example`**
```
//本示例设置形状的线条颜色、线条样式、线条宽度、端口类型、连接类型和线条颜色透明度
var shape = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var oldStyle = shape.style();
oldStyle.line.color = "red";
oldStyle.line.lineStyle = GC.Spread.Sheets.Shapes.PresetLineDashStyle.dashDot;
oldStyle.line.width = 5;
oldStyle.line.capType = GC.Spread.Sheets.Shapes.LineCapStyle.square;
oldStyle.line.joinType = GC.Spread.Sheets.Shapes.LineJoinStyle.miter;
oldStyle.line.compoundType = GC.Spread.Sheets.Shapes.CompoundType.double;
oldStyle.line.transparency = 0.5;
shape.style(oldStyle);

//本示例使用形状公式设置线条颜色，线条样式，线条宽度，盖帽类型，连接类型和线条颜色透明度
var shape = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
sheet.setValue(0, 1, "red");
sheet.setValue(1, 1, 4);
sheet.setValue(2, 1, 5);
sheet.setValue(3, 1, 1);
sheet.setValue(4, 1, 1);
sheet.setValue(5, 1, 0.5);
var oldStyle = shape.style();
oldStyle.line.color = "=Sheet1!B1";
oldStyle.line.lineStyle = "=Sheet1!B2";
oldStyle.line.width = "=Sheet1!B3";
oldStyle.line.capType = "=Sheet1!B4";
oldStyle.line.joinType = "=Sheet1!B5";
oldStyle.line.transparency = "=Sheet1!B6";
oldStyle.line.compoundType = "=Sheet1!B7";
shape.style(oldStyle);

//本示例设置形状的线的箭头始端样式，宽度，长度和箭头末端样式，宽度，高度
var shape = sheet.shapes.addConnector("Shape1", GC.Spread.Sheets.Shapes.ConnectorType.straight, 100, 60, 200, 160);
var oldStyle = shape.style();
oldStyle.line.beginArrowheadStyle = GC.Spread.Sheets.Shapes.ArrowheadStyle.triangle;
oldStyle.line.beginArrowheadWidth = GC.Spread.Sheets.Shapes.ArrowheadWidth.narrow;
oldStyle.line.beginArrowheadLength = GC.Spread.Sheets.Shapes.ArrowheadLength.short;
oldStyle.line.endArrowheadStyle = GC.Spread.Sheets.Shapes.ArrowheadStyle.diamond;
oldStyle.line.endArrowheadWidth = GC.Spread.Sheets.Shapes.ArrowheadWidth.wide;
oldStyle.line.endArrowheadLength = GC.Spread.Sheets.Shapes.ArrowheadLength.long;
shape.style(oldStyle);
```

___

### <a id="texteffect" name="texteffect"></a> textEffect

• **textEffect**: [`IShapeTextEffect`](../interfaces/GC.Spread.Sheets.Shapes.IShapeTextEffect.md)

文字效果选项

**`example`**
```
//本示例设置形状的字体颜色，字体颜色透明度和字体
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var oldStyle = heart.style();
oldStyle.textEffect.color = "red";
oldStyle.textEffect.transparency = 0.5;
oldStyle.textEffect.font = "20px Arial";
heart.style(oldStyle);
heart.text("Heart");

//本示例设置字体颜色，字体颜色透明度和带有形状公式的字体
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
sheet.setValue(0, 1, "red");
sheet.setValue(1, 1, 0.5);
sheet.setValue(2, 1, "20px Arial");
var oldStyle = heart.style();
oldStyle.textEffect.color = "=Sheet1!B1";
oldStyle.textEffect.transparency = "=Sheet1!B2";
oldStyle.textEffect.font = "=Sheet1!B3";
heart.style(oldStyle);
heart.text("Heart");
```

___

### <a id="textframe" name="textframe"></a> textFrame

• **textFrame**: [`IShapeTextFrame`](../interfaces/GC.Spread.Sheets.Shapes.IShapeTextFrame.md)

文本框架选项

**`example`**
```
//本示例为文本设置文本的水平对齐方式和垂直对齐方式
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
var oldStyle = heart.style();
oldStyle.textFrame.vAlign = GC.Spread.Sheets.VerticalAlign.center;
oldStyle.textFrame.hAlign = GC.Spread.Sheets.HorizontalAlign.center;
heart.style(oldStyle);
heart.text("Heart");

//本示例使用形状的公式设置文本的水平对齐方式和垂直对齐方式
var heart = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.heart, 100, 60, 200, 160);
sheet.setValue(0, 1, 1);
sheet.setValue(1, 1, 1);
var oldStyle = heart.style();
oldStyle.textFrame.vAlign = "=Sheet1!B1";
oldStyle.textFrame.hAlign = "=Sheet1!B2";
heart.style(oldStyle);
heart.text("Heart");

//本示例设置了形状的resizeToFitText属性
var rectangle = sheet.shapes.add("Shape1", GC.Spread.Sheets.Shapes.AutoShapeType.rectangle, 100, 60, 200, 160);
var oldStyle = rectangle.style();
oldStyle.textFrame.resizeToFitText = true;
rectangle.style(style);
```
