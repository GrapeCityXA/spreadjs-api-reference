# Class: PaperSize

[Sheets](../modules/GC.Spread.Sheets.md).[Print](../modules/GC.Spread.Sheets.Print.md).PaperSize

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Print.PaperSize.md#constructor)

### Methods

- [getPageSize](GC.Spread.Sheets.Print.PaperSize.md#getpagesize)
- [height](GC.Spread.Sheets.Print.PaperSize.md#height)
- [kind](GC.Spread.Sheets.Print.PaperSize.md#kind)
- [width](GC.Spread.Sheets.Print.PaperSize.md#width)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new PaperSize**(`widthOrKind?`, `height?`)

纸张尺寸
该构造函数有3种模式
如果有2个参数，参数为宽度和高度，类型为数字
如果有1个参数，该参数为种类，是GC.Spread.Sheets.Print.PaperKind类型
如果没有参数，结果与第二种模式相同，种类选项为GC.Spread.Sheets.Print.PaperKind.letter

**`代码示例`**
```
var printInfo = new GC.Spread.Sheets.Print.PrintInfo();
printInfo.pageHeaderFooter({
    normal: {
        header: {
            left: "Header Left"
        }
    }
});
printInfo.paperSize(new GC.Spread.Sheets.Print.PaperSize(GC.Spread.Sheets.Print.PaperKind.a4));
spread.print(0);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `widthOrKind?` | `number` |
| `height?` | `number` |

## Methods

### <a id="getpagesize" name="getpagesize"></a> getPageSize

▸ **getPageSize**(`kind`): [`PrintSize`](../interfaces/GC.Spread.Sheets.Print.PrintSize.md)

获取纸张尺寸，以百分之一英寸为单位

**`example`**
```
var paperSize = new GC.Spread.Sheets.Print.PaperSize();
console.log(paperSize.getPageSize(GC.Spread.Sheets.Print.PaperKind.a4)); // Get the size of a4 paper.
console.log(paperSize.getPageSize(GC.Spread.Sheets.Print.PaperKind.a5)); // Get the size of a5 paper.
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | [`PaperKind`](../enums/GC.Spread.Sheets.Print.PaperKind.md) | 纸张种类 |

#### Returns

[`PrintSize`](../interfaces/GC.Spread.Sheets.Print.PrintSize.md)

The size which contains width and height of the paper.

___

### <a id="height" name="height"></a> height

▸ **height**(`value?`): `any`

获取或设置纸张的高度，以百分之一英寸为单位

**`example`**
```
var paperSize = new GC.Spread.Sheets.Print.PaperSize(GC.Spread.Sheets.Print.PaperKind.a4);
var height = paperSize.height(); // Get the height of the paper.
paperSize.height(height / 2); // Set the height of paper.
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`any`

如果未设置任何值，则返回纸张的高度；否则，返回纸张尺寸

___

### <a id="kind" name="kind"></a> kind

▸ **kind**(`value?`): `any`

获取或设置纸张的种类

**`example`**
```
var paperSize = new GC.Spread.Sheets.Print.PaperSize(GC.Spread.Sheets.Print.PaperKind.a4);
console.log(paperSize.kind()); // Get the kind of the paper.
paperSize.kind(GC.Spread.Sheets.Print.PaperKind.a5); // Set the kind of paper.
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`PaperKind`](../enums/GC.Spread.Sheets.Print.PaperKind.md) |

#### Returns

`any`

如果未设置任何值，则返回纸张类型；否则，返回纸张尺寸

___

### <a id="width" name="width"></a> width

▸ **width**(`value?`): `any`

获取或设置纸张的宽度，以百分之一英寸为单位

**`example`**
```
var paperSize = new GC.Spread.Sheets.Print.PaperSize(GC.Spread.Sheets.Print.PaperKind.a4);
var width = paperSize.width(); // Get the width of the paper.
paperSize.width(width / 2); // Set the width of paper.
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 纸张的宽度 |

#### Returns

`any`

如果未设置任何值，则返回纸张的宽度；否则，返回纸张尺寸
