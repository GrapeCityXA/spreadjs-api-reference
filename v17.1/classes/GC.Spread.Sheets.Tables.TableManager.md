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

可以管理表单中所有表格的表管理器

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheet` | [`Worksheet`](GC.Spread.Sheets.Worksheet.md) | 表单 |

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`name?`, `row?`, `column?`, `rowCount?`, `columnCount?`, `style?`): [`Table`](GC.Spread.Sheets.Tables.Table.md)

将具有指定大小的区域表添加到表单

**`代码示例`**
```
//本示例添加一个表格
activeSheet.tables.add("Table1", 0, 0, 3, 3, GC.Spread.Sheets.Tables.TableThemes.dark1);
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
| `name?` | `string` | 表格名称 |
| `row?` | `number` | 行索引 |
| `column?` | `number` | 列索引 |
| `rowCount?` | `number` | 表格行数 |
| `columnCount?` | `number` | 表格列数 |
| `style?` | [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md) | 表格样式 |

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md)

新表实例

___

### <a id="addfromdatasource" name="addfromdatasource"></a> addFromDataSource

▸ **addFromDataSource**(`name`, `row`, `column`, `dataSource`, `style`): [`Table`](GC.Spread.Sheets.Tables.Table.md)

将具有指定数据源的区域表添加到表单

**`代码示例`**
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
| `name` | `string` | 表格名称 |
| `row` | `number` | 行索引 |
| `column` | `number` | 列索引 |
| `dataSource` | `Object` | 表格的数据源 |
| `style` | [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md) | 表格样式 |
| `options?` | [`ITableOptions`](../interfaces/GC.Spread.Sheets.Tables.ITableOptions.md) | - |

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md)

新表实例

___

### <a id="all" name="all"></a> all

▸ **all**(): [`Table`](GC.Spread.Sheets.Tables.Table.md)[]

获取表单的所有表格

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md)[]

GC.Spread.Sheets.Tables.Table 表格数组实例.数组不为null

___

### <a id="find" name="find"></a> find

▸ **find**(`row`, `column`): [`Table`](GC.Spread.Sheets.Tables.Table.md)

获取指定单元格的表

**`代码示例`**
```
//本示例使用find方法
activeSheet.tables.add("Table1", 0, 0, 3, 3, GC.Spread.Sheets.Tables.TableThemes.dark1);
activeSheet.getCell(0,0).text("Name");
activeSheet.getCell(0,1).text("Value");
activeSheet.getCell(0,2).text("T/F");
activeSheet.getCell(1,0).text("AW");
activeSheet.getCell(1,1).text("5");
activeSheet.getCell(1,2).text("T");
//点击按钮
$("#button1").click(function () {
     var table  = activeSheet.tables.find(0,0);
     console.log(table.name());
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |
| `column` | `number` | 列索引 |

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md)

如果单元格属于一个表，返回表实例；否则返回null

___

### <a id="findbyname" name="findbyname"></a> findByName

▸ **findByName**(`name`): [`Table`](GC.Spread.Sheets.Tables.Table.md)

获取具有指定名称的表格

**`代码示例`**
```
//本示例按名称查找表
var activeSheet = spread.getActiveSheet();
activeSheet.tables.add("Table1", 0, 0, 3, 3, GC.Spread.Sheets.Tables.TableThemes.dark1);
activeSheet.getCell(0,0).text("Name");
activeSheet.getCell(0,1).text("Value");
activeSheet.getCell(0,2).text("T/F");
activeSheet.getCell(1,0).text("AW");
activeSheet.getCell(1,1).text("5");
activeSheet.getCell(1,2).text("T");
// button click
$("#button1").click(function () {
     var table  = activeSheet.tables.findByName("Table1");
     console.log(table.name());
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | The table name. |

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md)

The table instance if the cell belongs to a table; otherwise, null.

___

### <a id="move" name="move"></a> move

▸ **move**(`table`, `row`, `column`): `void`

Changes the table location.

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
// button click
$("#button1").click(function () {
     var table  = activeSheet.tables.findByName("Table1");
     alert(table);
     activeSheet.tables.move(table, 3, 3);
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `table` | `string` \| [`Table`](GC.Spread.Sheets.Tables.Table.md) | The table instance or the table name. |
| `row` | `number` | The new row index. |
| `column` | `number` | The new column index. |

#### Returns

`void`

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`table`, `options`): [`Table`](GC.Spread.Sheets.Tables.Table.md)

删除指定的表

**`代码示例`**
```
var table  = activeSheet.tables.find(0,0);
activeSheet.tables.remove(table, GC.Spread.Sheets.Tables.TableRemoveOptions.keepData);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `table` | `string` \| 表实例或表名称 |
| `options` | [`TableRemoveOptions`](../enums/GC.Spread.Sheets.Tables.TableRemoveOptions.md) | 删除表时保留哪些数据 |

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md)

___

### <a id="resize" name="resize"></a> resize

▸ **resize**(`table`, `range`): `void`

更改表格大小

**`代码示例`**
```
//本示例调整表的大小
activeSheet.tables.add("Table1", 0, 0, 3, 3, GC.Spread.Sheets.Tables.TableThemes.dark1);
activeSheet.getCell(0,0).text("Name");
activeSheet.getCell(0,1).text("Value");
activeSheet.getCell(0,2).text("T/F");
activeSheet.getCell(1,0).text("AW");
activeSheet.getCell(1,1).text("5");
activeSheet.getCell(1,2).text("T");
//点击按钮
$("#button1").click(function () {
     var table  = activeSheet.tables.find(0,0);
     activeSheet.tables.resize(table, new GC.Spread.Sheets.Range(0,0,4,4));
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `table` | `string` \| [`Table`](GC.Spread.Sheets.Tables.Table.md) | 表格或表格名 |
| `range` | [`Range`](GC.Spread.Sheets.Range.md) | 新表区域 页眉必须保留在同一行中，并且新表区域必须与原始表区域重叠 |

#### Returns

`void`
