# Class: IO

[GC.Spread.Excel](../modules/GC.Spread.Excel.md).IO

## Table of contents

### Constructors

- [constructor](GC.Spread.Excel.IO-1.md#constructor)

### Properties

- [pivotTableThemes](GC.Spread.Excel.IO-1.md#pivottablethemes)
- [slicerStyles](GC.Spread.Excel.IO-1.md#slicerstyles)
- [tableThemes](GC.Spread.Excel.IO-1.md#tablethemes)
- [timelineStyles](GC.Spread.Excel.IO-1.md#timelinestyles)

### Methods

- [open](GC.Spread.Excel.IO-1.md#open)
- [registerMaxDigitWidth](GC.Spread.Excel.IO-1.md#registermaxdigitwidth)
- [save](GC.Spread.Excel.IO-1.md#save)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new IO**()

表示一个 excel 导入和导出类。

## Properties

### <a id="pivottablethemes" name="pivottablethemes"></a> pivotTableThemes

▪ `Static` **pivotTableThemes**: `Object`

内置透视表主题。

#### Index signature

▪ [key: `string`]: `any`

___

### <a id="slicerstyles" name="slicerstyles"></a> slicerStyles

▪ `Static` **slicerStyles**: `Object`

内置项目切片器主题。

#### Index signature

▪ [key: `string`]: `any`

___

### <a id="tablethemes" name="tablethemes"></a> tableThemes

▪ `Static` **tableThemes**: `Object`

内置表格主题。

#### Index signature

▪ [key: `string`]: `any`

___

### <a id="timelinestyles" name="timelinestyles"></a> timelineStyles

▪ `Static` **timelineStyles**: `Object`

内置时间轴切片器主题。

#### Index signature

▪ [key: `string`]: `any`

## Methods

### <a id="open" name="open"></a> open

▸ **open**(`file`, `successCallBack`, `errorCallBack?`, `options?`): `void`

导入一个 excel 文件。

**`example`**
```
var workbook = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var excelIO = new GC.Spread.Excel.IO();
var excelFile = document.getElementById("fileDemo").files[0];
excelIO.open(excelFile, function (json) {
   workbook.fromJSON(json);
}, function (e) {
   console.log(e);
}, {
   password: "password",
   importPictureAsFloatingObject: false
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `file` | `Blob` | 要导入的 excel 文件。 |
| `successCallBack` | `Function` | 成功加载文件后调用的函数。 `function (json) { }`. |
| `errorCallBack?` | `Function` | 如果发生错误，调用的函数。异常参数对象结构 `{ errorCode: GC.Spread.Excel.IO.ErrorCode, errorMessage: string}`. |
| `options?` | [`OpenOptions`](../modules/GC.Spread.Excel.IO.md#openoptions) | 导入 excel 的选项。 |

#### Returns

`void`

___

### <a id="registermaxdigitwidth" name="registermaxdigitwidth"></a> registerMaxDigitWidth

▸ **registerMaxDigitWidth**(`fontFamily`, `fontSize`, `maxDigitWidth`): `void`

注册一个未知最大数字宽度信息到 ExcelIO。

**`example`**
```
GC.Spread.Excel.IO.registerMaxDigitWidth("\ub3cb\uc6c0", 11, Math.floor(80/8.11));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fontFamily` | `string` | 默认样式的字体。 |
| `fontSize` | `number` | 默认样式的字体大小（以点为单位）。 |
| `maxDigitWidth` | `number` | 默认样式的字体最大数字宽度。 |

#### Returns

`void`

___

### <a id="save" name="save"></a> save

▸ **save**(`json`, `successCallBack`, `errorCallBack?`, `options?`): `void`

使用 SpreadJS json 创建并保存一个 excel 文件。

**`example`**
```
var workbook = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var excelIO = new GC.Spread.Excel.IO();
var json = JSON.stringify(workbook.toJSON());
excelIO.save(json, function (blob) {
   saveAs(blob, fileName); // saveAs 是来自 FileSaver.
}, function (e) {
   console.log(e);
}, {
   password: "password",
   xlsxStrictMode: false
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `json` | `string` \| `object` | 电子表格 json 对象，或字符串。 |
| `successCallBack` | `Function` | 成功导出文件后调用的函数。 `function (blob) { }`. |
| `errorCallBack?` | `Function` | 如果发生错误，调用的函数。异常参数对象结构 `{ errorCode: GC.Spread.Excel.IO.ErrorCode, errorMessage: string}`. |
| `options?` | [`SaveOptions`](../modules/GC.Spread.Excel.IO.md#saveoptions) | 导出 excel 的选项。 |

#### Returns

`void`
