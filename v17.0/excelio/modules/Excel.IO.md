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

**`property`** {string} password the excel file's password.

**`property`** {boolean} importPictureAsFloatingObject import picture as floatingObject instead of shape.

#### Type declaration

| Name | Type |
| :------ | :------ |
| `importPictureAsFloatingObject?` | `boolean` |
| `password?` | `string` |

___

### <a id="saveoptions" name="saveoptions"></a> SaveOptions

Ƭ **SaveOptions**: `Object`

**`property`** {string} password the excel file's password.

**`property`** {boolean} xlsxStrictMode the mode of exporting process, the non-strict mode may reduce the export size. Default is true.

#### Type declaration

| Name | Type |
| :------ | :------ |
| `password?` | `string` |
| `xlsxStrictMode?` | `boolean` |
