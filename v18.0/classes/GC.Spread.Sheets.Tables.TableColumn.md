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
| `dataStyle?` | `string` \| [`Style`](GC.Spread.Sheets.Style.md) | the data style of the table column |
| `headerStyle?` | `string` \| [`Style`](GC.Spread.Sheets.Style.md) | the header style of the table column |
| `footerStyle?` | `string` \| [`Style`](GC.Spread.Sheets.Style.md) | the footer style of the table column |

## Methods

### <a id="celltype" name="celltype"></a> cellType

▸ **cellType**(`value?`): `any`

获取或设置用于自定义单元格类型的表列cellType

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

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`Base`](GC.Spread.Sheets.CellTypes.Base.md) | 表列的cellType |

#### Returns

`any`

如果未设置任何值，则返回表列cellType;否则，返回表列

___

### <a id="datafield" name="datafield"></a> dataField

▸ **dataField**(`value?`): `any`

获取或设置用于访问表数据源的表列数据字段

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
| `value?` | `string` | 表列数据字段 |

#### Returns

`any`

如果未设置任何值，则返回表列数据字段；否则，返回表列

___

### <a id="datastyle" name="datastyle"></a> dataStyle

▸ **dataStyle**(`value?`): `any`

Gets or sets the table column dataStyle.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` \| [`Style`](GC.Spread.Sheets.Style.md) |

#### Returns

`any`

If no value is set, returns the table column dataStyle; otherwise, returns the table column.

___

### <a id="footerstyle" name="footerstyle"></a> footerStyle

▸ **footerStyle**(`value?`): `any`

Gets or sets the table column footerStyle.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` \| [`Style`](GC.Spread.Sheets.Style.md) |

#### Returns

`any`

If no value is set, returns the table column footerStyle; otherwise, returns the table column.

___

### <a id="formatter" name="formatter"></a> formatter

▸ **formatter**(`value?`): `any`

获取或设置表列格式的格式显示值

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
| `value?` | `string` | 表列格式 |

#### Returns

`any`

如果未设置任何值，则返回表列格式；否则，返回表列

___

### <a id="headerstyle" name="headerstyle"></a> headerStyle

▸ **headerStyle**(`value?`): `any`

Gets or sets the table column headerStyle.

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` \| [`Style`](GC.Spread.Sheets.Style.md) |

#### Returns

`any`

If no value is set, returns the table column headerStyle; otherwise, returns the table column.

___

### <a id="id" name="id"></a> id

▸ **id**(`value?`): `any`

获取或设置表列ID

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
| `value?` | `number` | 表列ID |

#### Returns

`any`

如果未设置任何值，则返回表的列ID;否则，返回表列

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置要显示的表列名称

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
| `value?` | `string` | 表格列名称 |

#### Returns

`any`

如果未设置任何值，则返回表的列名；否则，返回表列

___

### <a id="value" name="value"></a> value

▸ **value**(`value?`): `Function`

获取或设置显示值的表列值转换功能

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

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `Function` | 表列值转换函数 |

#### Returns

`Function`

如果未设置任何值，则返回表列的值转换函数；否则，返回表列
