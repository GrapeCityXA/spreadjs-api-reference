# Namespace: IO

[Spread](GC.Spread.md).[Excel](GC.Spread.Excel.md).IO

## Table of contents

### Enumerations

- [ErrorCode](../enums/GC.Spread.Excel.IO.ErrorCode.md)

### Type aliases

- [OpenOptions](GC.Spread.Excel.IO.md#openoptions)
- [SaveOptions](GC.Spread.Excel.IO.md#saveoptions)

## Type aliases

### <a id="openoptions" name="openoptions"></a> OpenOptions

Ƭ **OpenOptions**: `Object`

**`property`** {string} password 要导入的 excel 文件的密码。

**`property`** {boolean} importPictureAsFloatingObject 导入图片作为浮动对象而不是形状。

#### Type declaration

| Name | Type |
| :------ | :------ |
| `importPictureAsFloatingObject?` | `boolean` |
| `password?` | `string` |

___

### <a id="saveoptions" name="saveoptions"></a> SaveOptions

Ƭ **SaveOptions**: `Object`

**`property`** {string} password 要导出的 excel 文件的密码。

**`property`** {boolean} xlsxStrictMode 导出过程的模式，非严格模式可能会减少导出大小。默认是 true.

#### Type declaration

| Name | Type |
| :------ | :------ |
| `password?` | `string` |
| `xlsxStrictMode?` | `boolean` |
