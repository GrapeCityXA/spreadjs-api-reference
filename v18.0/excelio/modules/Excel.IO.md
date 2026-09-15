# Namespace: IO

[Excel](Excel.md).IO

## Table of contents

### Enumerations

- [ErrorCode](../enums/Excel.IO.ErrorCode.md)

### Type aliases

- [OpenOptions](Excel.IO.md#openoptions)
- [SaveOptions](Excel.IO.md#saveoptions)

## Type aliases

### <a id="openoptions" name="openoptions"></a> OpenOptions

Ƭ **OpenOptions**: `Object`

**`property`** {string} password Excel 文件的密码。

**`property`** {boolean} importPictureAsFloatingObject 将图片导入为浮动对象而不是形状。

#### Type declaration

| Name | Type |
| :------ | :------ |
| `importPictureAsFloatingObject?` | `boolean` |
| `password?` | `string` |

___

### <a id="saveoptions" name="saveoptions"></a> SaveOptions

Ƭ **SaveOptions**: `Object`

**`property`** {string} password Excel 文件的密码。

**`property`** {boolean} xlsxStrictMode 导出过程的模式，非严格模式可能会减少导出大小。默认为 true。

#### Type declaration

| Name | Type |
| :------ | :------ |
| `password?` | `string` |
| `xlsxStrictMode?` | `boolean` |
