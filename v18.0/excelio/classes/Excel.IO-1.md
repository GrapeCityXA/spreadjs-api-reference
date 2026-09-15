# Class: IO

[Excel](../modules/Excel.md).IO

## Table of contents

### Constructors

- [constructor](Excel.IO-1.md#constructor)

### Properties

- [pivotTableThemes](Excel.IO-1.md#pivottablethemes)
- [slicerStyles](Excel.IO-1.md#slicerstyles)
- [tableThemes](Excel.IO-1.md#tablethemes)
- [timelineStyles](Excel.IO-1.md#timelinestyles)

### Methods

- [open](Excel.IO-1.md#open)
- [registerMaxDigitWidth](Excel.IO-1.md#registermaxdigitwidth)
- [save](Excel.IO-1.md#save)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new IO**()

代表一个excel导入导出类。

## Properties

### <a id="pivottablethemes" name="pivottablethemes"></a> pivotTableThemes

▪ `Static` **pivotTableThemes**: `Object`

内置数据透视表主题。

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

内置时间线切片器主题。

#### Index signature

▪ [key: `string`]: `any`

## Methods

### <a id="open" name="open"></a> open

▸ **open**(`file`, `successCallBack`, `errorCallBack?`, `options?`): `void`

导入 Excel 文件（xlsx）

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
| `file` | `Blob` |  Excel 文件（xlsx） |
| `successCallBack` | `Function` | 成功后的回调函数 |
| `errorCallBack?` | `Function` | 失败时的回调函数，错误参考： { errorCode: GC.Spread.Excel.IO.ErrorCode, errorMessage: string}. |
| `options?` | [`OpenOptions`](../modules/Excel.IO.md#openoptions) | 导入 Excel 的参数 |

#### Returns

`void`

___

### <a id="registermaxdigitwidth" name="registermaxdigitwidth"></a> registerMaxDigitWidth

▸ **registerMaxDigitWidth**(`fontFamily`, `fontSize`, `maxDigitWidth`): `void`

向 Excel.IO 注册缺失字体宽度

**`example`**
```
GC.Spread.Excel.IO.registerMaxDigitWidth("\ub3cb\uc6c0", 11, Math.floor(80/8.11));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fontFamily` | `string` | 默认样式字体的字体系列 |
| `fontSize` | `number` | 默认样式字体的字体大小（以 point 为单位） |
| `maxDigitWidth` | `number` | 默认样式字体的最大宽度 |

#### Returns

`void`

___

### <a id="save" name="save"></a> save

▸ **save**(`json`, `successCallBack`, `errorCallBack?`, `options?`): `void`

使用 SpreadJS JSON 创建并保存 Excel(xlsx) 文件

**`example`**
```
var workbook = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var excelIO = new GC.Spread.Excel.IO();
var json = JSON.stringify(workbook.toJSON());
excelIO.save(json, function (blob) {
   saveAs(blob, fileName); //saveAs is from FileSaver.
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
| `json` | `string` \| `object` | SpreadJS JSON 对象（或字符串） |
| `successCallBack` | `Function` | 成功后的回调函数 |
| `errorCallBack?` | `Function` | - |
| `options?` | [`SaveOptions`](../modules/Excel.IO.md#saveoptions) | 导出 Excel 的参数 |

#### Returns

`void`
