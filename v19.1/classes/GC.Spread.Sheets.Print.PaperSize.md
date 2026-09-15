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

指定纸张大小。<br/>
构造函数有三种模式。<br/>
如果有2个参数，参数为宽度和高度，类型为number；<br/>
如果有1个参数，参数为kind，类型为GC.Spread.Sheets.Print.PaperKind；<br/>
如果没有参数，kind选项为GC.Spread.Sheets.Print.PaperKind.letter。

**`example`**
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

获取纸张大小，单位为百分之一英寸。

**`example`**
```javascript
var paperSize = new GC.Spread.Sheets.Print.PaperSize();
console.log(paperSize.getPageSize(GC.Spread.Sheets.Print.PaperKind.a4)); // 获取a4纸张的尺寸。
console.log(paperSize.getPageSize(GC.Spread.Sheets.Print.PaperKind.a5)); // 获取a5纸张的尺寸。
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `kind` | [`PaperKind`](../enums/GC.Spread.Sheets.Print.PaperKind.md) | 纸张类型。 |

#### Returns

[`PrintSize`](../interfaces/GC.Spread.Sheets.Print.PrintSize.md)

包含纸张宽度和高度的尺寸。

___

### <a id="height" name="height"></a> height

▸ **height**(`value?`): `any`

获取或设置纸张高度，单位为百分之一英寸。

**`example`**
```javascript
var paperSize = new GC.Spread.Sheets.Print.PaperSize(GC.Spread.Sheets.Print.PaperKind.a4);
var height = paperSize.height(); // 获取纸张高度。
paperSize.height(height / 2); // 设置纸张高度。
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 纸张高度。 |

#### Returns

`any`

如果未设置值，返回纸张高度；否则返回纸张大小。

___

### <a id="kind" name="kind"></a> kind

▸ **kind**(`value?`): `any`

获取或设置纸张类型。

**`example`**
```javascript
var paperSize = new GC.Spread.Sheets.Print.PaperSize(GC.Spread.Sheets.Print.PaperKind.a4);
console.log(paperSize.kind()); // 获取纸张类型。
paperSize.kind(GC.Spread.Sheets.Print.PaperKind.a5); // 设置纸张类型。
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`PaperKind`](../enums/GC.Spread.Sheets.Print.PaperKind.md) | 纸张类型。 |

#### Returns

`any`

如果未设置值，返回纸张类型；否则返回纸张大小。

___

### <a id="width" name="width"></a> width

▸ **width**(`value?`): `any`

获取或设置纸张宽度，单位为百分之一英寸。

**`example`**
```javascript
var paperSize = new GC.Spread.Sheets.Print.PaperSize(GC.Spread.Sheets.Print.PaperKind.a4);
var width = paperSize.width(); // 获取纸张宽度。
paperSize.width(width / 2); // 设置纸张宽度。
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 纸张宽度。 |

#### Returns

`any`

如果未设置值，返回纸张宽度；否则返回纸张大小。
