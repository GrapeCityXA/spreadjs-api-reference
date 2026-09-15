# Class: AtomicComponentBase<ValueType, OptionsType\>

[Sheets](../modules/GC.Spread.Sheets.md).[Designer](../modules/GC.Spread.Sheets.Designer.md).AtomicComponentBase

## Type parameters

| Name |
| :------ |
| `ValueType` |
| `OptionsType` |

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Designer.AtomicComponentBase.md#constructor)

### Methods

- [getTemplate](GC.Spread.Sheets.Designer.AtomicComponentBase.md#gettemplate)
- [onDestroy](GC.Spread.Sheets.Designer.AtomicComponentBase.md#ondestroy)
- [onEnableChanged](GC.Spread.Sheets.Designer.AtomicComponentBase.md#onenablechanged)
- [onInit](GC.Spread.Sheets.Designer.AtomicComponentBase.md#oninit)
- [onMounted](GC.Spread.Sheets.Designer.AtomicComponentBase.md#onmounted)
- [onValueChanged](GC.Spread.Sheets.Designer.AtomicComponentBase.md#onvaluechanged)
- [raiseValueChanged](GC.Spread.Sheets.Designer.AtomicComponentBase.md#raisevaluechanged)
- [updateValue](GC.Spread.Sheets.Designer.AtomicComponentBase.md#updatevalue)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new AtomicComponentBase**<`ValueType`, `OptionsType`\>(`host`, `options`)

表示定义原子组件的抽象类。

#### Type parameters

| Name |
| :------ |
| `ValueType` |
| `OptionsType` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `host` | `HTMLElement` | 组件挂载的HTML区域 |
| `options` | `OptionsType` | 组件选项 |

## Methods

### <a id="gettemplate" name="gettemplate"></a> getTemplate

▸ **getTemplate**(`options`): `string`

在此设置内部HTML。当主机挂载到DOM时调用。

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | `OptionsType` |

#### Returns

`string`

___

### <a id="ondestroy" name="ondestroy"></a> onDestroy

▸ **onDestroy**(`host`): `void`

组件即将销毁时调用。

#### Parameters

| Name | Type |
| :------ | :------ |
| `host` | `HTMLElement` |

#### Returns

`void`

___

### <a id="onenablechanged" name="onenablechanged"></a> onEnableChanged

▸ **onEnableChanged**(`prevEnable`, `nextEnable`, `host`, `options`): `void`

值状态改变时调用此函数。

#### Parameters

| Name | Type |
| :------ | :------ |
| `prevEnable` | `boolean` |
| `nextEnable` | `boolean` |
| `host` | `HTMLElement` |
| `options` | `OptionsType` |

#### Returns

`void`

___

### <a id="oninit" name="oninit"></a> onInit

▸ **onInit**(`options`): `void`

组件初始化自身时调用。

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | `OptionsType` |

#### Returns

`void`

___

### <a id="onmounted" name="onmounted"></a> onMounted

▸ **onMounted**(`host`, `options`): `void`

组件的主机附加到DOM树时调用。

#### Parameters

| Name | Type |
| :------ | :------ |
| `host` | `HTMLElement` |
| `options` | `OptionsType` |

#### Returns

`void`

___

### <a id="onvaluechanged" name="onvaluechanged"></a> onValueChanged

▸ **onValueChanged**(`prevValue`, `nextValue`, `host`, `options`): `void`

启用状态改变时调用此函数。

#### Parameters

| Name | Type |
| :------ | :------ |
| `prevValue` | `ValueType` |
| `nextValue` | `ValueType` |
| `host` | `HTMLElement` |
| `options` | `OptionsType` |

#### Returns

`void`

___

### <a id="raisevaluechanged" name="raisevaluechanged"></a> raiseValueChanged

▸ **raiseValueChanged**(): `void`

向设计器触发值改变事件，这将调用命令的execute函数。

#### Returns

`void`

___

### <a id="updatevalue" name="updatevalue"></a> updateValue

▸ **updateValue**(`host`, `options`): `ValueType`

获取组件最新值。框架需要组件值时调用。

#### Parameters

| Name | Type |
| :------ | :------ |
| `host` | `HTMLElement` |
| `options` | `OptionsType` |

#### Returns

`ValueType`
