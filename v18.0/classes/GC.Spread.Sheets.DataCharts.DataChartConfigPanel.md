# Class: DataChartConfigPanel

[Sheets](../modules/GC.Spread.Sheets.md).[DataCharts](../modules/GC.Spread.Sheets.DataCharts.md).DataChartConfigPanel

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.DataCharts.DataChartConfigPanel.md#constructor)

### Methods

- [attach](GC.Spread.Sheets.DataCharts.DataChartConfigPanel.md#attach)
- [destroy](GC.Spread.Sheets.DataCharts.DataChartConfigPanel.md#destroy)
- [detach](GC.Spread.Sheets.DataCharts.DataChartConfigPanel.md#detach)
- [findControl](GC.Spread.Sheets.DataCharts.DataChartConfigPanel.md#findcontrol)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new DataChartConfigPanel**(`host`, `spread`)

表示一个数据图表配置面板。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `host` | `string` \| `HTMLElement` | 宿主元素、宿主元素的 ID 或宿主元素选择器。 |
| `spread` | [`Workbook`](GC.Spread.Sheets.Workbook.md) | 面板要附加到的工作簿。 |

## Methods

### <a id="attach" name="attach"></a> attach

▸ **attach**(`spread`): `void`

将工作簿附加到配置面板。

**`example`**
```
configPanel.attach(spread);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `spread` | [`Workbook`](GC.Spread.Sheets.Workbook.md) |

#### Returns

`void`

___

### <a id="destroy" name="destroy"></a> destroy

▸ **destroy**(): `void`

销毁配置面板。

**`example`**
```
configPanel.destroy();
```

#### Returns

`void`

___

### <a id="detach" name="detach"></a> detach

▸ **detach**(): `void`

将工作簿从配置面板分离。

**`example`**
```
configPanel.detach();
```

#### Returns

`void`

___

### <a id="findcontrol" name="findcontrol"></a> findControl

▸ `Static` **findControl**(`host`): [`DataChartConfigPanel`](GC.Spread.Sheets.DataCharts.DataChartConfigPanel.md)

通过宿主元素获取 DataChartConfigPanel 实例。

**`example`**
```
const configPanel = GC.Spread.Sheets.DataCharts.DataChartConfigPanel.findControl('host');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `host` | `string` \| `HTMLElement` | 宿主元素、宿主元素的 ID 或宿主元素选择器。 |

#### Returns

[`DataChartConfigPanel`](GC.Spread.Sheets.DataCharts.DataChartConfigPanel.md)

`DataChartConfigPanel` 实例。
