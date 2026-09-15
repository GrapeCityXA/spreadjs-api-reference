# Namespace: InputMask

[Spread](GC.Spread.md).[Sheets](GC.Spread.Sheets.md).InputMask

## Table of contents

### Interfaces

- [INamedPattern](../interfaces/GC.Spread.Sheets.InputMask.INamedPattern.md)
- [IValidatePatternResult](../interfaces/GC.Spread.Sheets.InputMask.IValidatePatternResult.md)

### Functions

- [getNamedPatterns](GC.Spread.Sheets.InputMask.md#getnamedpatterns)
- [namedPattern](GC.Spread.Sheets.InputMask.md#namedpattern)
- [validatePattern](GC.Spread.Sheets.InputMask.md#validatepattern)

## Functions

### <a id="getnamedpatterns" name="getnamedpatterns"></a> getNamedPatterns

▸ **getNamedPatterns**(): [`INamedPattern`](../interfaces/GC.Spread.Sheets.InputMask.INamedPattern.md)[]

获取所有命名的模式。

**`static`**

#### Returns

[`INamedPattern`](../interfaces/GC.Spread.Sheets.InputMask.INamedPattern.md)[]

返回所有命名的模式。

___

### <a id="namedpattern" name="namedpattern"></a> namedPattern

▸ **namedPattern**(`name`, `pattern?`): `string` \| `void`

设置或获取命名的模式。

**`static`**

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 模式名称。 |
| `pattern?` | ``null`` \| `string` | 模式字符串。 |

#### Returns

`string` \| `void`

如果未设置模式，则返回命名的模式字符串，否则返回 void。

___

### <a id="validatepattern" name="validatepattern"></a> validatePattern

▸ **validatePattern**(`pattern`): [`IValidatePatternResult`](../interfaces/GC.Spread.Sheets.InputMask.IValidatePatternResult.md)

验证模式是否有效。

**`static`**

**`example`**
```javascript
let verifyResult = GC.Spread.Sheets.InputMask.validatePattern('[a0_]{8}');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pattern` | `string` | 模式字符串。 |

#### Returns

[`IValidatePatternResult`](../interfaces/GC.Spread.Sheets.InputMask.IValidatePatternResult.md)

返回验证结果。
