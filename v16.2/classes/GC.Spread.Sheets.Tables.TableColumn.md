# Class: TableColumn

[Sheets](../modules/GC.Spread.Sheets.md).[Tables](../modules/GC.Spread.Sheets.Tables.md).TableColumn

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Tables.TableColumn.md#constructor)

### Methods

- [cellType](GC.Spread.Sheets.Tables.TableColumn.md#celltype)
- [dataField](GC.Spread.Sheets.Tables.TableColumn.md#datafield)
- [formatter](GC.Spread.Sheets.Tables.TableColumn.md#formatter)
- [id](GC.Spread.Sheets.Tables.TableColumn.md#id)
- [name](GC.Spread.Sheets.Tables.TableColumn.md#name)
- [value](GC.Spread.Sheets.Tables.TableColumn.md#value)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new TableColumn**(`id`, `dataField?`, `name?`, `formatter?`, `cellType?`, `value?`)

表格列信息

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `number` | 表列ID |
| `dataField?` | `string` | 表列数据字段 |
| `name?` | `string` | 表格列名称 |
| `formatter?` | `string` | 表列格式 |
| `cellType?` | [`Base`](GC.Spread.Sheets.CellTypes.Base.md) | 表列的cellType |
| `value?` | `Function` | 表列值转换函数 |

## Methods

### <a id="celltype" name="celltype"></a> cellType

▸ **cellType**(`value?`): `any`

获取或设置用于自定义单元格类型的表列cellType

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`Base`](GC.Spread.Sheets.CellTypes.Base.md) | 表列的cellType |

#### Returns

`any`

如果未设置任何值,则返回表列cellType;否则,返回表列

___

### <a id="datafield" name="datafield"></a> dataField

▸ **dataField**(`value?`): `any`

获取或设置用于访问表数据源的表列数据字段

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 表列数据字段 |

#### Returns

`any`

如果未设置任何值,则返回表列数据字段;否则,返回表列

___

### <a id="formatter" name="formatter"></a> formatter

▸ **formatter**(`value?`): `any`

获取或设置表列格式的格式显示值

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 表列格式 |

#### Returns

`any`

如果未设置任何值,则返回表列格式;否则,返回表列

___

### <a id="id" name="id"></a> id

▸ **id**(`value?`): `any`

获取或设置表列ID

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 表列ID |

#### Returns

`any`

如果未设置任何值,则返回表的列ID;否则,返回表列

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置要显示的表列名称

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 表格列名称 |

#### Returns

`any`

如果未设置任何值,则返回表的列名;否则,返回表列

___

### <a id="value" name="value"></a> value

▸ **value**(`value?`): `Function`

获取或设置显示值的表列值转换功能

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `Function` | 表列值转换函数 |

#### Returns

`Function`

如果未设置任何值,则返回表列的值转换函数;否则,返回表列
