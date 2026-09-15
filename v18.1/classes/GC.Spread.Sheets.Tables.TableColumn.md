# Class: TableColumn

[Sheets](../modules/GC.Spread.Sheets.md).[Tables](../modules/GC.Spread.Sheets.Tables.md).TableColumn

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Tables.TableColumn.md#constructor)

### Methods

- [cellType](GC.Spread.Sheets.Tables.TableColumn.md#celltype)
- [dataField](GC.Spread.Sheets.Tables.TableColumn.md#datafield)
- [dataStyle](GC.Spread.Sheets.Tables.TableColumn.md#datastyle)
- [footerStyle](GC.Spread.Sheets.Tables.TableColumn.md#footerstyle)
- [formatter](GC.Spread.Sheets.Tables.TableColumn.md#formatter)
- [headerStyle](GC.Spread.Sheets.Tables.TableColumn.md#headerstyle)
- [id](GC.Spread.Sheets.Tables.TableColumn.md#id)
- [name](GC.Spread.Sheets.Tables.TableColumn.md#name)
- [value](GC.Spread.Sheets.Tables.TableColumn.md#value)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new TableColumn**(`id`, `dataField?`, `name?`, `formatter?`, `cellType?`, `value?`, `dataStyle?`, `headerStyle?`, `footerStyle?`)

表示表格列信息。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `number` | 表格列ID。 |
| `dataField?` | `string` | 表格列数据字段。 |
| `name?` | `string` | 表格列名称。 |
| `formatter?` | `string` | 表格列格式化器。 |
| `cellType?` | [`Base`](GC.Spread.Sheets.CellTypes.Base.md) | 表格列单元格类型。 |
| `value?` | `Function` | 表格列值转换函数。 |
| `dataStyle?` | `string` \| [`Style`](GC.Spread.Sheets.Style.md) | 表格列数据样式 |
| `headerStyle?` | `string` \| [`Style`](GC.Spread.Sheets.Style.md) | 表格列标题样式 |
| `footerStyle?` | `string` \| [`Style`](GC.Spread.Sheets.Style.md) | 表格列页脚样式 |

## Methods

### <a id="celltype" name="celltype"></a> cellType

▸ **cellType**(`value?`): `any`

获取或设置表格列的自定义单元格类型。

**`example`**
```
var data = {
     sales: [
         { name: 'Pencil', isMakeMoney: true },
         { name: 'Binder', isMakeMoney: true },
         { name: 'Pen Set', isMakeMoney: false }
     ]
 };
 var table = sheet.tables.add('tableSales', 0, 0, 5, 2);
 var tableColumn1 = new GC.Spread.Sheets.Tables.TableColumn();
 tableColumn1.name("name");
 tableColumn1.dataField("name");
 var tableColumn2 = new GC.Spread.Sheets.Tables.TableColumn();
 tableColumn2.name("IsMakeMoney");
 tableColumn2.dataField("isMakeMoney");
 tableColumn2.cellType(new GC.Spread.Sheets.CellTypes.CheckBox());
 table.autoGenerateColumns(false);
 table.bind([tableColumn1, tableColumn2], 'sales', data);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`Base`](GC.Spread.Sheets.CellTypes.Base.md) |

#### Returns

`any`

如果未设置值，则返回表格列单元格类型；否则返回表格列。

___

### <a id="datafield" name="datafield"></a> dataField

▸ **dataField**(`value?`): `any`

获取或设置表格列的数据字段，用于访问表格的数据源。

**`example`**
```
var data = {
     sales: [
         { name: 'Pencil' },
         { name: 'Binder' },
         { name: 'Pen Set' }
     ]
 };
 var table = sheet.tables.add('tableSales', 0, 0, 5, 2);
 var tableColumn1 = new GC.Spread.Sheets.Tables.TableColumn();
 tableColumn1.name("name");
 tableColumn1.dataField("name");
 table.bind([tableColumn1], 'sales', data);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置值，则返回表格列数据字段；否则返回表格列。

___

### <a id="datastyle" name="datastyle"></a> dataStyle

▸ **dataStyle**(`value?`): `any`

获取或设置表格列的数据样式。

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` \| [`Style`](GC.Spread.Sheets.Style.md) |

#### Returns

`any`

如果未设置值，则返回表格列数据样式；否则返回表格列。

___

### <a id="footerstyle" name="footerstyle"></a> footerStyle

▸ **footerStyle**(`value?`): `any`

获取或设置表格列的页脚样式。

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` \| [`Style`](GC.Spread.Sheets.Style.md) |

#### Returns

`any`

如果未设置值，则返回表格列页脚样式；否则返回表格列。

___

### <a id="formatter" name="formatter"></a> formatter

▸ **formatter**(`value?`): `any`

获取或设置表格列的格式化器，用于格式化显示值。

**`example`**
```
var data = {
     sales: [
         { name: 'Pencil', orderDate: new Date(2013, 3, 1) },
         { name: 'Binder', orderDate: new Date(2013, 4, 1) },
         { name: 'Pen Set', orderDate: new Date(2013, 6, 8) }
     ]
 };
 var table = sheet.tables.add('tableSales', 0, 0, 5, 2);
 var tableColumn1 = new GC.Spread.Sheets.Tables.TableColumn();
 tableColumn1.name("name");
 tableColumn1.dataField("name");
 var tableColumn2 = new GC.Spread.Sheets.Tables.TableColumn();
 tableColumn2.name("Order Date");
 tableColumn2.dataField("orderDate");
 tableColumn2.formatter("d/M/yy");
 table.autoGenerateColumns(false);
 table.bind([tableColumn1, tableColumn2], 'sales', data);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 表格列格式化器。 |

#### Returns

`any`

如果未设置值，则返回表格列格式化器；否则返回表格列。

___

### <a id="headerstyle" name="headerstyle"></a> headerStyle

▸ **headerStyle**(`value?`): `any`

获取或设置表格列的表头样式。

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` \| [`Style`](GC.Spread.Sheets.Style.md) |

#### Returns

`any`

如果未设置值，则返回表格列的表头样式；否则返回表格列。

___

### <a id="id" name="id"></a> id

▸ **id**(`value?`): `any`

获取或设置表格列的ID。

**`example`**
```
var data = {
     sales: [
         { name: 'Pencil' },
         { name: 'Binder' },
         { name: 'Pen Set' }
     ]
 };
 var table = sheet.tables.add('tableSales', 0, 0, 5, 2);
 var tableColumn1 = new GC.Spread.Sheets.Tables.TableColumn();
 tableColumn1.id("name");
 tableColumn1.dataField("name");
 table.bind([tableColumn1], 'sales', data);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 表格列的ID。 |

#### Returns

`any`

如果未设置值，则返回表格列的ID；否则返回表格列。

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置表格列的显示名称。

**`example`**
```
var data = {
     sales: [
         { name: 'Pencil' },
         { name: 'Binder' },
         { name: 'Pen Set' }
     ]
 };
 var table = sheet.tables.add('tableSales', 0, 0, 5, 2);
 var tableColumn1 = new GC.Spread.Sheets.Tables.TableColumn();
 tableColumn1.name("name");
 tableColumn1.dataField("name");
 table.bind([tableColumn1], 'sales', data);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 表格列的名称。 |

#### Returns

`any`

如果未设置值，则返回表格列的名称；否则返回表格列。

___

### <a id="value" name="value"></a> value

▸ **value**(`value?`): `Function`

获取或设置表格列的值转换函数，用于显示值。

**`example`**
```
var data = {
     sales: [
         { name: 'Pencil', orderDate: new Date(2013, 3, 1), cost: 1.99 },
         { name: 'Binder', orderDate: new Date(2013, 4, 1), cost: 4.99 },
         { name: 'Pen Set', orderDate: new Date(2013, 6, 8), cost: 15.99 }
     ]
 };
 var table = sheet.tables.add('tableSales', 0, 0, 5, 3);
 var tableColumn1 = new GC.Spread.Sheets.Tables.TableColumn();
 tableColumn1.name("name");
 tableColumn1.dataField("name");
 var tableColumn2 = new GC.Spread.Sheets.Tables.TableColumn();
 tableColumn2.name("Order Date");
 tableColumn2.dataField("orderDate");
 tableColumn2.formatter("d/M/yy");
 var tableColumn3 = new GC.Spread.Sheets.Tables.TableColumn();
 tableColumn3.name("Cost");
 tableColumn3.dataField("cost");
 tableColumn3.value(function (item) {
     return item['cost'] + '$';
 });
 table.autoGenerateColumns(false);
 table.bind([tableColumn1, tableColumn2, tableColumn3], 'sales', data);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `Function` |

#### Returns

`Function`

如果未设置值，则返回表格列的值转换函数；否则返回表格列。
