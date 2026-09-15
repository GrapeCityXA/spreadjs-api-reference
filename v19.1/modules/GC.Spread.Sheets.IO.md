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

**`description`** 通过文件路径获取文件。

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `filePath` | `string` | 文件路径。 |

##### Returns

`File` \| `Blob`

- 返回文件或文件blob。

___

### <a id="getpartialvalueserrorcallbacktype" name="getpartialvalueserrorcallbacktype"></a> GetPartialValuesErrorCallbackType

Ƭ **GetPartialValuesErrorCallbackType**: (`errorMsg`: `string`) => `void`

#### Type declaration

▸ (`errorMsg`): `void`

**`description`** 获取部分值的错误回调。

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `errorMsg` | `string` | 错误消息。 |

##### Returns

`void`

___

### <a id="getpartialvaluessuccesscallbacktype" name="getpartialvaluessuccesscallbacktype"></a> GetPartialValuesSuccessCallbackType

Ƭ **GetPartialValuesSuccessCallbackType**: (`externalValues`: [`ExternalPartialValues`](GC.Spread.Sheets.md#externalpartialvalues)) => `void`

#### Type declaration

▸ (`externalValues`): `void`

**`description`** 获取部分值的成功回调。

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `externalValues` | [`ExternalPartialValues`](GC.Spread.Sheets.md#externalpartialvalues) | 外部值列表。 |

##### Returns

`void`

## Functions

### <a id="getpartialvalues" name="getpartialvalues"></a> getPartialValues

▸ **getPartialValues**(`refList`, `getFile`, `getPartialValuesSuccessCallback`, `getPartialValuesErrorCallback`): `void`

直接从文件中获取特定引用路径列表的值。

**`static`**

**`example`**
```javascript
function getFile (path) {
  // 返回指定文件路径的文件或blob
}
let refList = spread.getExternalReferences(true);
GC.Spread.Sheets.IO.getPartialValues(refList, getFile, (externalValues) => {
  // 成功回调函数
  spread.updateExternalReference(externalValues);
}, (errorMsg) => {
  // 错误回调函数
  console.log(errorMsg);
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `refList` | [`IExternalReference`](../interfaces/GC.Spread.Sheets.IExternalReference.md)[] | 外部引用的数组。 |
| `getFile` | [`GetFileFunctionType`](GC.Spread.Sheets.IO.md#getfilefunctiontype) | 返回指定文件路径的文件或blob的函数。 |
| `getPartialValuesSuccessCallback` | [`GetPartialValuesSuccessCallbackType`](GC.Spread.Sheets.IO.md#getpartialvaluessuccesscallbacktype) | 成功回调函数，当获取值成功时调用。 |
| `getPartialValuesErrorCallback` | [`GetPartialValuesErrorCallbackType`](GC.Spread.Sheets.IO.md#getpartialvalueserrorcallbacktype) | 错误回调函数，当获取值失败时调用。 |

#### Returns

`void`

___

### <a id="registermaxdigitwidth" name="registermaxdigitwidth"></a> registerMaxDigitWidth

▸ **registerMaxDigitWidth**(`fontFamily`, `fontSize`, `maxDigitWidth`): `void`

向 IO 模块注册指定字体的最大数字宽度信息。

**`example`**
```javascript
// 为自定义字体注册最大数字宽度
GC.Spread.Sheets.IO.registerMaxDigitWidth("Arial", 12, 7.2);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `fontFamily` | `string` | 默认样式对应的字体家族。 |
| `fontSize` | `number` | 默认样式对应的字体大小（以点为单位）。 |
| `maxDigitWidth` | `number` | 默认样式对应的字体最大数字宽度。 |

#### Returns

`void`
