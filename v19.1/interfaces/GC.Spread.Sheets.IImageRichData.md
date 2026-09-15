# Interface: IImageRichData

[Spread](../modules/GC.Spread.md).[Sheets](../modules/GC.Spread.Sheets.md).IImageRichData

## Hierarchy

- [`IRichData`](GC.Spread.Sheets.IRichData.md)

  ↳ **`IImageRichData`**

## Table of contents

### Properties

- [richDataType](GC.Spread.Sheets.IImageRichData.md#richdatatype)
- [value](GC.Spread.Sheets.IImageRichData.md#value)

## Properties

### <a id="richdatatype" name="richdatatype"></a> richDataType

• **richDataType**: ``"Image"``

用于标识这是图像富数据对象的判别标签。

#### Overrides

[IRichData](GC.Spread.Sheets.IRichData.md).[richDataType](GC.Spread.Sheets.IRichData.md#richdatatype)

___

### <a id="value" name="value"></a> value

• **value**: `Object`

富数据值，其结构取决于 richDataType。

#### Type declaration

| Name | Type | Description |
| :------ | :------ | :------ |
| `altText?` | `string` | 可选。用于无障碍访问的图像替代文本。 |
| `clipHeight?` | `number` | 可选。源图像中要绘制到目标上下文的子矩形高度。默认值为图像高度。 |
| `clipWidth?` | `number` | 可选。源图像中要绘制到目标上下文的子矩形宽度。默认值为图像宽度。 |
| `clipX?` | `number` | 可选。源图像中要绘制到目标上下文的子矩形左上角 x 坐标。默认值为 0。 |
| `clipY?` | `number` | 可选。源图像中要绘制到目标上下文的子矩形左上角 y 坐标。默认值为 0。 |
| `drawType?` | `number` | 可选。指定图像尺寸调整方式。0 - 保持纵横比以适应单元格。1 - 让图像填满整个单元格。2 - 保持原始尺寸，即使会被裁剪。3 - 自定义。默认值为 1。 |
| `hAlign?` | `number` | 可选。图像的水平对齐方式。0 - 左对齐，1 - 居中，2 - 右对齐。默认值为 0（左对齐）。 |
| `height?` | `number` | 可选。如果 drawType 为 3（自定义），则使用此值作为高度。 |
| `imageBase64Data?` | `string` | 可选。base64 编码的图像数据。 |
| `src` | `string` | 图标路径 |
| `vAlign?` | `number` | 可选。图像的垂直对齐方式。0 - 顶部，1 - 居中，2 - 底部。默认值为 0（顶部）。 |
| `width?` | `number` | 可选。如果 drawType 为 3（自定义），则使用此值作为宽度。 |

#### Overrides

[IRichData](GC.Spread.Sheets.IRichData.md).[value](GC.Spread.Sheets.IRichData.md#value)
