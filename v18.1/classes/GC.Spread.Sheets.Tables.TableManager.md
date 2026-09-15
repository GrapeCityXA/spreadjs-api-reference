# Class: TableManager

[Sheets](../modules/GC.Spread.Sheets.md).[Tables](../modules/GC.Spread.Sheets.Tables.md).TableManager

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Tables.TableManager.md#constructor)

### Methods

- [add](GC.Spread.Sheets.Tables.TableManager.md#add)
- [addFromDataSource](GC.Spread.Sheets.Tables.TableManager.md#addfromdatasource)
- [all](GC.Spread.Sheets.Tables.TableManager.md#all)
- [find](GC.Spread.Sheets.Tables.TableManager.md#find)
- [findByName](GC.Spread.Sheets.Tables.TableManager.md#findbyname)
- [move](GC.Spread.Sheets.Tables.TableManager.md#move)
- [remove](GC.Spread.Sheets.Tables.TableManager.md#remove)
- [resize](GC.Spread.Sheets.Tables.TableManager.md#resize)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new TableManager**(`sheet`)

表示一个可以管理工作表中所有表格的表格管理器。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheet` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 工作表。 |

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`name?`, `row?`, `column?`, `rowCount?`, `columnCount?`, `style?`): [`Table`](GC.Spread.Sheets.Tables.Table.md)

向工作表添加一个指定大小的范围表格。

**`example`**
```
//此示例添加一个表格。
activeSheet.tables.add("Table1", 0, 0, 3, 3, 'dark1');
activeSheet.getCell(0,0).text("Name");
activeSheet.getCell(0,1).text("Value");
activeSheet.getCell(0,2).text("T/F");
activeSheet.getCell(1,0).text("AW");
activeSheet.getCell(1,1).text("5");
activeSheet.getCell(1,2).text("T");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name?` | `string` | 表格名称。 |
| `row?` | `number` | 行索引。 |
| `column?` | `number` | 列索引。 |
| `rowCount?` | `number` | 表格的行数。 |
| `columnCount?` | `number` | 表格的列数。 |
| `style?` | `string` \| [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md) | 表格的样式。 |

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md)

新的表格实例。

___

### <a id="addfromdatasource" name="addfromdatasource"></a> addFromDataSource

▸ **addFromDataSource**(`name`, `row`, `column`, `dataSource`, `style`, `options?`): [`Table`](GC.Spread.Sheets.Tables.Table.md) \| `Promise`<[`Table`](GC.Spread.Sheets.Tables.Table.md)\>

向工作表添加一个指定数据源的范围表格。

**`example`**
```
var source = [
                { LastName: "Freehafer", FirstName: "Nancy", Title: "Sales Representative", Phone: "(123)555-0100"},
                { LastName: "Cencini", FirstName: "Andrew", Title: "Vice President, Sales", Phone: "(123)555-0101"},
                { LastName: "Kotas", FirstName: "Jan", Title: "Sales Representative", Phone: "(123)555-0102"},
                { LastName: "Sergienko", FirstName: "Mariya", Title: "Sales Representative", Phone: "(123)555-0103"},
            ];
 activeSheet.tables.addFromDataSource("Table1", 5, 2, source, GC.Spread.Sheets.Tables.TableThemes.dark1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 表格名称。 |
| `row` | `number` | 行索引。 |
| `column` | `number` | 列索引。 |
| `dataSource` | `string` \| `Object` \| [`Table`](GC.Data.Table.md) | 表格的数据源。 |
| `style` | [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md) | 表格的样式。 |
| `options?` | [`ITableOptions`](../interfaces/GC.Spread.Sheets.Tables.ITableOptions.md) | - |

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md) \| `Promise`<[`Table`](GC.Spread.Sheets.Tables.Table.md)\>

新的表格实例。

___

### <a id="all" name="all"></a> all

▸ **all**(): [`Table`](GC.Spread.Sheets.Tables.Table.md)[]

获取工作表中的所有表格。

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md)[]

表格实例的GC.Spread.Sheets.Tables.Table数组。该数组永远不会为null。

___

### <a id="find" name="find"></a> find

▸ **find**(`row`, `column`): [`Table`](GC.Spread.Sheets.Tables.Table.md)

获取指定单元格所在的表格。

**`example`**
```
//此示例使用 find 方法。
activeSheet.tables.add("Table1", 0, 0, 3, 3, GC.Spread.Sheets.Tables.TableThemes.dark1);
activeSheet.getCell(0,0).text("Name");
activeSheet.getCell(0,1).text("Value");
activeSheet.getCell(0,2).text("T/F");
activeSheet.getCell(1,0).text("AW");
activeSheet.getCell(1,1).text("5");
activeSheet.getCell(1,2).text("T");
//按钮点击
$("#button1").click(function () {
     var table  = activeSheet.tables.find(0,0);
     console.log(table.name());
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `column` | `number` | 列索引。 |

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md)

如果单元格属于某个表格，则返回该表格实例；否则返回 null。

___

### <a id="findbyname" name="findbyname"></a> findByName

▸ **findByName**(`name`): [`Table`](GC.Spread.Sheets.Tables.Table.md)

获取指定名称的表格。

**`example`**
```
//此示例通过名称查找表格。
var activeSheet = spread.getActiveSheet();
activeSheet.tables.add("Table1", 0, 0, 3, 3, GC.Spread.Sheets.Tables.TableThemes.dark1);
activeSheet.getCell(0,0).text("Name");
activeSheet.getCell(0,1).text("Value");
activeSheet.getCell(0,2).text("T/F");
activeSheet.getCell(1,0).text("AW");
activeSheet.getCell(1,1).text("5");
activeSheet.getCell(1,2).text("T");
//按钮点击
$("#button1").click(function () {
     var table  = activeSheet.tables.findByName("Table1");
     console.log(table.name());
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 表格名称。 |

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md)

如果找到指定名称的表格，则返回该表格实例；否则返回 null。

___

### <a id="move" name="move"></a> move

▸ **move**(`table`, `row`, `column`): `void`

更改表格位置。

**`example`**
```
var activeSheet = spread.getActiveSheet();
activeSheet.tables.add("Table1", 0, 0, 3, 3, GC.Spread.Sheets.Tables.TableThemes.dark1);
activeSheet.getCell(0,0).text("Name");
activeSheet.getCell(0,1).text("Value");
activeSheet.getCell(0,2).text("T/F");
activeSheet.getCell(1,0).text("AW");
activeSheet.getCell(1,1).text("5");
activeSheet.getCell(1,2).text("T");
//按钮点击
$("#button1").click(function () {
     var table  = activeSheet.tables.findByName("Table1");
     alert(table);
     activeSheet.tables.move(table, 3, 3);
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `table` | `string` \| [`Table`](GC.Spread.Sheets.Tables.Table.md) | 表格实例或表格名称。 |
| `row` | `number` | 新的行索引。 |
| `column` | `number` | 新的列索引。 |

#### Returns

`void`

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`table`, `options`): [`Table`](GC.Spread.Sheets.Tables.Table.md)

移除指定的表格。

**`example`**
```
var table  = activeSheet.tables.find(0,0);
activeSheet.tables.remove(table, GC.Spread.Sheets.Tables.TableRemoveOptions.keepData);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `table` | `string` \| [`Table`](GC.Spread.Sheets.Tables.Table.md) | 表格实例或表格名称。 |
| `options` | [`TableRemoveOptions`](../enums/GC.Spread.Sheets.Tables.TableRemoveOptions.md) | 指定移除表格时要保留的数据。 |

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md)

___

### <a id="resize" name="resize"></a> resize

▸ **resize**(`table`, `range`): `void`

更改表格大小。

**`example`**
```
//此示例调整表格大小。
activeSheet.tables.add("Table1", 0, 0, 3, 3, GC.Spread.Sheets.Tables.TableThemes.dark1);
activeSheet.getCell(0,0).text("Name");
activeSheet.getCell(0,1).text("Value");
activeSheet.getCell(0,2).text("T/F");
activeSheet.getCell(1,0).text("AW");
activeSheet.getCell(1,1).text("5");
activeSheet.getCell(1,2).text("T");
//按钮点击
$("#button1").click(function () {
     var table  = activeSheet.tables.find(0,0);
     activeSheet.tables.resize(table, new GC.Spread.Sheets.Range(0,0,4,4));
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `table` | `string` \| [`Table`](GC.Spread.Sheets.Tables.Table.md) | 表格或表格名称。 |
| `range` | [`Range`](GC.Spread.Sheets.Range.md) | 新的表格范围。表头必须保持在相同的行，且结果表格范围必须与原始表格范围重叠。 |

#### Returns

`void`
