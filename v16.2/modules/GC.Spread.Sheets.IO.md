# Namespace: IO

[Spread](GC.Spread.md).[Sheets](GC.Spread.Sheets.md).IO

## Table of contents

### Enumerations

- [ErrorCode](../enums/GC.Spread.Sheets.IO.ErrorCode.md)

### Type aliases

- [GetFileFunctionType](GC.Spread.Sheets.IO.md#getfilefunctiontype)
- [GetPartialValuesErrorCallbackType](GC.Spread.Sheets.IO.md#getpartialvalueserrorcallbacktype)
- [GetPartialValuesSuccessCallbackType](GC.Spread.Sheets.IO.md#getpartialvaluessuccesscallbacktype)

### Functions

- [getPartialValues](GC.Spread.Sheets.IO.md#getpartialvalues)
- [registerMaxDigitWidth](GC.Spread.Sheets.IO.md#registermaxdigitwidth)

## Type aliases

### <a id="getfilefunctiontype" name="getfilefunctiontype"></a> GetFileFunctionType

Ƭ **GetFileFunctionType**: (`filePath`: `string`) => `File` \| `Blob`

#### Type declaration

▸ (`filePath`): `File` \| `Blob`

**`description`** 获取文件流

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `filePath` | `string` | 文件路径 |

##### Returns

`File` \| `Blob`

- 返回文件或文件流

___

### <a id="getpartialvalueserrorcallbacktype" name="getpartialvalueserrorcallbacktype"></a> GetPartialValuesErrorCallbackType

Ƭ **GetPartialValuesErrorCallbackType**: (`errorMsg`: `string`) => `void`

#### Type declaration

▸ (`errorMsg`): `void`

**`description`** 获取值时错误回调

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `errorMsg` | `string` | 错误信息 |

##### Returns

`void`

___

### <a id="getpartialvaluessuccesscallbacktype" name="getpartialvaluessuccesscallbacktype"></a> GetPartialValuesSuccessCallbackType

Ƭ **GetPartialValuesSuccessCallbackType**: (`externalValues`: [`ExternalPartialValues`](GC.Spread.Sheets.md#externalpartialvalues)) => `void`

#### Type declaration

▸ (`externalValues`): `void`

**`description`** 获取值时成功回调

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `externalValues` | [`ExternalPartialValues`](GC.Spread.Sheets.md#externalpartialvalues) | 外部值列表 |

##### Returns

`void`

## Functions

### <a id="getpartialvalues" name="getpartialvalues"></a> getPartialValues

▸ **getPartialValues**(`refList`, `getFile`, `getPartialValuesSuccessCallback`, `getPartialValuesErrorCallback`): `void`

直接从文件中获取特定引用路径列表的值。

**`static`**

**`代码示例`**
```
function getFile (path) {
  // return file by path
}
let refList = spread.getExternalReferences(true);
GC.Spread.Sheets.IO.getPartialValues(refList, getFile, (externalValues) => {
  // successCallback
  spread.updateExternalReference(externalValues);
}, (errorMsg) => {
  // errorCallback
  console.log(errorMsg);
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `refList` | [`IExternalReference`](../interfaces/GC.Spread.Sheets.IExternalReference.md)[] | 外部引用的数组。 |
| `getFile` | [`GetFileFunctionType`](GC.Spread.Sheets.IO.md#getfilefunctiontype) | 根据指定的文件路径返回文件或 Blob 的函数。 |
| `getPartialValuesSuccessCallback` | [`GetPartialValuesSuccessCallbackType`](GC.Spread.Sheets.IO.md#getpartialvaluessuccesscallbacktype) | 在成功获取部分值时调用的回调函数。 |
| `getPartialValuesErrorCallback` | [`GetPartialValuesErrorCallbackType`](GC.Spread.Sheets.IO.md#getpartialvalueserrorcallbacktype) | 在获取部分值失败时调用的错误回调函数。 |

#### Returns

`void`

___

### <a id="registermaxdigitwidth" name="registermaxdigitwidth"></a> registerMaxDigitWidth

▸ **registerMaxDigitWidth**(`fontFamily`, `fontSize`, `maxDigitWidth`): `void`

将未知的最大数字宽度信息注册到 IO。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fontFamily` | `string` | 默认样式字体的字体系列 |
| `fontSize` | `number` | 默认样式字体的字号（以点为单位） |
| `maxDigitWidth` | `number` | 默认样式字体的最大数字宽度 |

#### Returns

`void`
