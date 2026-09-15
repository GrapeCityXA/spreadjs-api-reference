# Class: Table

[Sheets](../modules/GC.Spread.Sheets.md).[Tables](../modules/GC.Spread.Sheets.Tables.md).Table

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Tables.Table.md#constructor)

### Methods

- [allowAutoExpand](GC.Spread.Sheets.Tables.Table.md#allowautoexpand)
- [autoGenerateColumns](GC.Spread.Sheets.Tables.Table.md#autogeneratecolumns)
- [bandColumns](GC.Spread.Sheets.Tables.Table.md#bandcolumns)
- [bandRows](GC.Spread.Sheets.Tables.Table.md#bandrows)
- [bind](GC.Spread.Sheets.Tables.Table.md#bind)
- [bindColumns](GC.Spread.Sheets.Tables.Table.md#bindcolumns)
- [bindingPath](GC.Spread.Sheets.Tables.Table.md#bindingpath)
- [clearPendingChanges](GC.Spread.Sheets.Tables.Table.md#clearpendingchanges)
- [dataRange](GC.Spread.Sheets.Tables.Table.md#datarange)
- [deleteColumns](GC.Spread.Sheets.Tables.Table.md#deletecolumns)
- [deleteRows](GC.Spread.Sheets.Tables.Table.md#deleterows)
- [expandBoundRows](GC.Spread.Sheets.Tables.Table.md#expandboundrows)
- [filterButtonVisible](GC.Spread.Sheets.Tables.Table.md#filterbuttonvisible)
- [footerIndex](GC.Spread.Sheets.Tables.Table.md#footerindex)
- [getColumnFormula](GC.Spread.Sheets.Tables.Table.md#getcolumnformula)
- [getColumnName](GC.Spread.Sheets.Tables.Table.md#getcolumnname)
- [getColumnValue](GC.Spread.Sheets.Tables.Table.md#getcolumnvalue)
- [getDirtyRows](GC.Spread.Sheets.Tables.Table.md#getdirtyrows)
- [headerIndex](GC.Spread.Sheets.Tables.Table.md#headerindex)
- [highlightFirstColumn](GC.Spread.Sheets.Tables.Table.md#highlightfirstcolumn)
- [highlightLastColumn](GC.Spread.Sheets.Tables.Table.md#highlightlastcolumn)
- [insertColumns](GC.Spread.Sheets.Tables.Table.md#insertcolumns)
- [insertRows](GC.Spread.Sheets.Tables.Table.md#insertrows)
- [name](GC.Spread.Sheets.Tables.Table.md#name)
- [range](GC.Spread.Sheets.Tables.Table.md#range)
- [rowFilter](GC.Spread.Sheets.Tables.Table.md#rowfilter)
- [setColumnDataFormula](GC.Spread.Sheets.Tables.Table.md#setcolumndataformula)
- [setColumnFormula](GC.Spread.Sheets.Tables.Table.md#setcolumnformula)
- [setColumnName](GC.Spread.Sheets.Tables.Table.md#setcolumnname)
- [setColumnValue](GC.Spread.Sheets.Tables.Table.md#setcolumnvalue)
- [showFooter](GC.Spread.Sheets.Tables.Table.md#showfooter)
- [showHeader](GC.Spread.Sheets.Tables.Table.md#showheader)
- [showResizeHandle](GC.Spread.Sheets.Tables.Table.md#showresizehandle)
- [style](GC.Spread.Sheets.Tables.Table.md#style)
- [useFooterDropDownList](GC.Spread.Sheets.Tables.Table.md#usefooterdropdownlist)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Table**(`name?`, `row?`, `col?`, `rowCount?`, `colCount?`, `style?`)

可被添加到表单的表格

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name?` | `string` | 表格名称 |
| `row?` | `number` | 表格行索引 |
| `col?` | `number` | 表格列索引 |
| `rowCount?` | `number` | 表格行数 |
| `colCount?` | `number` | 表格列数 |
| `style?` | [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md) | 表格样式 |

## Methods

### <a id="allowautoexpand" name="allowautoexpand"></a> allowAutoExpand

▸ **allowAutoExpand**(`allowAutoExpandState?`): `boolean` \| [`Table`](GC.Spread.Sheets.Tables.Table.md)

获取或设置表格的allowAutoExpandState

**`代码示例`**
```
table.allowAutoExpand();
table.allowAutoExpand(true);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `allowAutoExpandState?` | `boolean` |

#### Returns

`boolean` \| [`Table`](GC.Spread.Sheets.Tables.Table.md)

如果未设置allowAutoExpandState,则返回表格allowAutoExpandState; 否则,返回表格

___

### <a id="autogeneratecolumns" name="autogeneratecolumns"></a> autoGenerateColumns

▸ **autoGenerateColumns**(`value?`): `any`

获取或设置绑定到数据源时是否自动生成列

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 绑定到数据源时是否自动生成列 |

#### Returns

`any`

如果未设置任何值,则返回绑定到数据源时是否自动生成列;否则,返回表格

___

### <a id="bandcolumns" name="bandcolumns"></a> bandColumns

▸ **bandColumns**(`value?`): `any`

获取或设置一个值,该值指示是否显示交替的列样式

**`代码示例`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
sTable.bandColumns(true);
sTable.bandRows(true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否显示交替的列样式 |

#### Returns

`any`

如果未设置任何值,则返回是否显示交替的列样式;否则,返回表格

___

### <a id="bandrows" name="bandrows"></a> bandRows

▸ **bandRows**(`value?`): `any`

获取或设置一个值,该值指示是否显示交替的行样式

**`代码示例`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
sTable.bandColumns(true);
sTable.bandRows(true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否显示交替的行样式 |

#### Returns

`any`

如果未设置任何值,则返回是否显示交替的行样式;否则,返回表格

___

### <a id="bind" name="bind"></a> bind

▸ **bind**(`columns`, `path?`, `dataSource?`): [`Table`](GC.Spread.Sheets.Tables.Table.md)

获取或设置表的数据源以及绑定列和路径

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columns` | [`TableColumn`](GC.Spread.Sheets.Tables.TableColumn.md)[] | 具有数据字段和名称的表列信息的数组.每个项都是GC.Spread.Sheets.Tables.TableColumn |
| `path?` | `string` | - |
| `dataSource?` | `object` | 表格的数据源 |

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md)

返回表格

___

### <a id="bindcolumns" name="bindcolumns"></a> bindColumns

▸ **bindColumns**(`columns`): `void`

使用指定的数据字段绑定列

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columns` | [`TableColumn`](GC.Spread.Sheets.Tables.TableColumn.md)[] | 具有数据字段和名称的表列信息的数组.每个项都是GC.Spread.Sheets.Tables.TableColumn |

#### Returns

`void`

___

### <a id="bindingpath" name="bindingpath"></a> bindingPath

▸ **bindingPath**(`value?`): `any`

获取或设置表格中单元格级别绑定的绑定路径

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 表格中单元格级别绑定的绑定路径 |

#### Returns

`any`

如果未设置任何值,则返回表格中单元格级别绑定的绑定路径;否则,返回表格

___

### <a id="clearpendingchanges" name="clearpendingchanges"></a> clearPendingChanges

▸ **clearPendingChanges**(): `void`

从当前表中清除脏数据状态

**`代码示例`**
```
table.clearPendingChanges();
```

#### Returns

`void`

___

### <a id="datarange" name="datarange"></a> dataRange

▸ **dataRange**(): [`Range`](GC.Spread.Sheets.Range.md)

获取表格数据区域的单元格区域

**`代码示例`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableTheme.medium2);
var drange = sTable.dataRange();
alert(drange.row);
```

#### Returns

[`Range`](GC.Spread.Sheets.Range.md)

表格数据区域

___

### <a id="deletecolumns" name="deletecolumns"></a> deleteColumns

▸ **deleteColumns**(`col`, `count`): `void`

删除表格中指定表格列索引处的列

**`代码示例`**
```
var table = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableTheme.medium2);
table.deleteColumns(3, 1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `col` | `number` | 基于表格索引,要删除的第一列的索引 |
| `count` | `number` | 要删除的列数 |

#### Returns

`void`

___

### <a id="deleterows" name="deleterows"></a> deleteRows

▸ **deleteRows**(`row`, `count`): `void`

删除此表格中指定表格行索引处的行

**`代码示例`**
```
var table = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableTheme.medium2);
table.deleteRows(3, 1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 基于表格索引,要删除的第一行的索引 |
| `count` | `number` | 要删除的行数 |

#### Returns

`void`

___

### <a id="expandboundrows" name="expandboundrows"></a> expandBoundRows

▸ **expandBoundRows**(`value?`): `any`

获取或设置表格绑定扩展行时的值

**`代码示例`**
```
var spread = GC.Spread.Sheets.findControl("ss") || GC.Spread.Sheets.findControl("sampleDiv");
var sheet = spread.getActiveSheet();
var data = {
    name: 'Jones', region: 'East',
    sales: [
        { orderDate: '1/6/2013', item: 'Pencil', units: 95, cost: 1.99 },
        { orderDate: '4/1/2013', item: 'Binder', units: 60, cost: 4.99 },
        { orderDate: '6/8/2013', item: 'Pen Set', units: 16, cost: 15.99 },
        { orderDate: '8/1/2013', item: 'Pencil', units: 20, cost: 24.99 },
        { orderDate: '10/8/2013', item: 'Binder', units: 31, cost: 16.99 }
    ]
};
var table1 = sheet.tables.add('tableRecords', 0, 0, 4, 4);
var table2 = sheet.tables.add('tableBelow', 4, 0, 4, 7);
table1.bindingPath('sales');
var dataSource = new GC.Spread.Sheets.Bindings.CellBindingSource(data);
table1.expandBoundRows(true);
sheet.setDataSource(dataSource);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 按工作表展开还是按表插入/删除行 |

#### Returns

`any`

如果未设置值,返回按表展开还是按表插入/删除行;否则,返回表格

___

### <a id="filterbuttonvisible" name="filterbuttonvisible"></a> filterButtonVisible

▸ **filterButtonVisible**(`tableColumnIndex?`, `value?`): `any`

获取或设置是否显示表格列的筛选按钮

**`代码示例`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableTheme.medium2);
sTable.bandColumns(true);
sTable.bandRows(true);
sTable.filterButtonVisible(2, false);
alert(sTable.filterButtonVisible(2));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tableColumnIndex?` | `number` | 筛选按钮的表格列索引 |
| `value?` | `boolean` | 是否显示表格列的筛选按钮 |

#### Returns

`any`

表格列的筛选按钮显示状态
 如果没有设置参数,如果所有筛选按钮都不可见返回false,否则返回true
 如果仅设置一个参数,则返回是否显示指定的表格列的筛选按钮
 如果仅设置了指示是否显示筛选按钮的布尔值,则将其应用于所有筛选按钮并返回表格
 如果提供了两个参数,则将其应用于指定的表格列的筛选按钮并返回表

___

### <a id="footerindex" name="footerindex"></a> footerIndex

▸ **footerIndex**(): `number`

获取表单中的页脚索引

**`代码示例`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableTheme.medium2);
sTable.showFooter(true);
sTable.setColumnName(4, "SUM");
//设置页脚值
sTable.setColumnValue(0, "Total");
//设置页脚公式
sTable.setColumnFormula(4, "SUM(F3:F11)");
var value = sTable.footerIndex();
alert(value);
```

#### Returns

`number`

页脚索引

___

### <a id="getcolumnformula" name="getcolumnformula"></a> getColumnFormula

▸ **getColumnFormula**(`tableColumnIndex`): `string`

获取具有指定索引的页脚公式

**`代码示例`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableTheme.medium2);
sTable.showFooter(true);
//设置页脚值
sTable.setColumnValue(0, "Total");
//设置页脚公式
sTable.setColumnFormula(4, "SUM(F3:F11)");
var value = sTable.getColumnFormula(4);
alert(value);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tableColumnIndex` | `number` | 页脚的列索引.索引从零开始 |

#### Returns

`string`

页脚公式

___

### <a id="getcolumnname" name="getcolumnname"></a> getColumnName

▸ **getColumnName**(`tableColumnIndex`): `string`

获取具有指定索引的表头文本

**`代码示例`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableTheme.medium2);
sTable.showFooter(true);
sTable.setColumnName(4, "SUM");
//设置页脚值
sTable.setColumnValue(0, "Total");
//设置页脚公式
sTable.setColumnFormula(4, "SUM(F3:F11)");
var value = sTable.getColumnName(4);
alert(value);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tableColumnIndex` | `number` | 表头的列索引。该索引从零开始。 |

#### Returns

`string`

按索引指定的列的标题文本

___

### <a id="getcolumnvalue" name="getcolumnvalue"></a> getColumnValue

▸ **getColumnValue**(`tableColumnIndex`): `string`

获取具有指定索引的表格页脚值

**`代码示例`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableTheme.medium2);
sTable.showFooter(true);
//设置页脚值
sTable.setColumnValue(0, "Total");
//设置页脚公式
sTable.setColumnFormula(4, "SUM(F3:F11)");
var value = sTable.getColumnValue(0);
alert(value);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tableColumnIndex` | `number` | 页脚的列索引.索引从零开始 |

#### Returns

`string`

表格页脚值

___

### <a id="getdirtyrows" name="getdirtyrows"></a> getDirtyRows

▸ **getDirtyRows**(): [`IRowState`](../interfaces/GC.Spread.Sheets.Tables.IRowState.md)[]

获取脏行的数组

#### Returns

[`IRowState`](../interfaces/GC.Spread.Sheets.Tables.IRowState.md)[]

脏行集合 数组中的项包含三个属性,row：指定表行索引,item：指定当前行的数据项,originalItem：指定该行的原始数据项

___

### <a id="headerindex" name="headerindex"></a> headerIndex

▸ **headerIndex**(): `number`

获取表单表头索引

**`代码示例`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableTheme.medium2);
var hindex = sTable.headerIndex();
alert(hindex);
```

#### Returns

`number`

表头索引

___

### <a id="highlightfirstcolumn" name="highlightfirstcolumn"></a> highlightFirstColumn

▸ **highlightFirstColumn**(`value?`): `any`

获取或设置一个值,该值指示是否高亮显示第一列

**`代码示例`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
sTable.highlightFirstColumn(true);
sTable.highlightLastColumn(true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否高亮显示第一列 |

#### Returns

`any`

如果未设置任何值,则返回是否高亮显示第一列;否则,返回表

___

### <a id="highlightlastcolumn" name="highlightlastcolumn"></a> highlightLastColumn

▸ **highlightLastColumn**(`value?`): `any`

获取或设置一个值,该值指示是否高亮显示最后一列

**`代码示例`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
sTable.highlightFirstColumn(true);
sTable.highlightLastColumn(true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否高亮显示最后一列 |

#### Returns

`any`

如果未设置任何值,则返回是否高亮显示最后一列;否则,返回表格

___

### <a id="insertcolumns" name="insertcolumns"></a> insertColumns

▸ **insertColumns**(`col`, `count`, `isInsertAfter?`): `void`

在该表中的指定表格列索引之前插入计数编号列

**`代码示例`**
```
var table = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableTheme.medium2);
table.insertColumns(3, 1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `col` | `number` | 基于表格索引在其上添加新列的列索引 |
| `count` | `number` | 要添加的列数 |
| `isInsertAfter?` | `boolean` | 是否在指定的列索引之前或之后插入列 默认情况下,在之前插入 |

#### Returns

`void`

___

### <a id="insertrows" name="insertrows"></a> insertRows

▸ **insertRows**(`row`, `count`, `isInsertAfter?`): `void`

在此表中的指定表格行索引之前插入行

**`代码示例`**
```
var table = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableTheme.medium2);
table.insertRows(3, 1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 基于表格索引,要插入的起始行的索引 |
| `count` | `number` | 要添加的行数 |
| `isInsertAfter?` | `boolean` | 是否在指定的行索引之前或之后插入行 默认情况下,在之前插入 |

#### Returns

`void`

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置表格名

**`代码示例`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableTheme.medium2);
var tname = sTable.name();
alert(tname);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 表格名称 |

#### Returns

`any`

如果未设置任何值,则返回表格名;否则,返回表格

___

### <a id="range" name="range"></a> range

▸ **range**(): [`Range`](GC.Spread.Sheets.Range.md)

获取整个表格的区域

**`代码示例`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableTheme.medium2);
var drange = sTable.range();
alert(drange.row);
```

#### Returns

[`Range`](GC.Spread.Sheets.Range.md)

整个表格的区域

___

### <a id="rowfilter" name="rowfilter"></a> rowFilter

▸ **rowFilter**(): [`HideRowFilter`](GC.Spread.Sheets.Filter.HideRowFilter.md)

获取表格的行筛选

#### Returns

[`HideRowFilter`](GC.Spread.Sheets.Filter.HideRowFilter.md)

行筛选

___

### <a id="setcolumndataformula" name="setcolumndataformula"></a> setColumnDataFormula

▸ **setColumnDataFormula**(`tableColumnIndex`, `formula`): [`Table`](GC.Spread.Sheets.Tables.Table.md)

使用指定的索引为表格的数据区域设置公式

**`代码示例`**
```
//本示例在表格中使用结构化引用公式
activeSheet.tables.add("Table1", 0, 0, 4, 3, GC.Spread.Sheets.Tables.TableTheme.dark1);
activeSheet.getCell(0,0).text("Value1");
activeSheet.getCell(0,1).text("Value2");
activeSheet.getCell(0,2).text("Total");
activeSheet.getCell(1,0).text("1");
activeSheet.getCell(2,0).text("2");
activeSheet.getCell(3,0).text("3");
activeSheet.getCell(1,1).text("5");
activeSheet.getCell(2,1).text("5");
activeSheet.getCell(3,1).text("5");
activeSheet.tables.findByName("Table1").setColumnDataFormula(2, "=[Value1]*[Value2]");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tableColumnIndex` | `number` | 表格的列索引 索引从零开始 |
| `formula` | `string` | 数据区域公式 |

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md)

表格

___

### <a id="setcolumnformula" name="setcolumnformula"></a> setColumnFormula

▸ **setColumnFormula**(`tableColumnIndex`, `formula`): [`Table`](GC.Spread.Sheets.Tables.Table.md)

使用指定的索引设置表尾公式

**`代码示例`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
sTable.showFooter(true);
//设置页脚值
sTable.setColumnValue(0, "Total");
//设置页脚公式
sTable.setColumnFormula(4, "SUM(F3:F11)");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tableColumnIndex` | `number` | 页脚的列索引.索引从零开始 |
| `formula` | `string` | 页脚公式 |

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md)

表格

___

### <a id="setcolumnname" name="setcolumnname"></a> setColumnName

▸ **setColumnName**(`tableColumnIndex`, `name`): [`Table`](GC.Spread.Sheets.Tables.Table.md)

用指定的表格索引设置表头文本

**`代码示例`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
sTable.showFooter(true);
sTable.setColumnName(4, "SUM");
//设置页脚值
sTable.setColumnValue(0, "Total");
//设置页脚公式
sTable.setColumnFormula(4, "SUM(F3:F11)");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tableColumnIndex` | `number` | 表头的列索引。该索引从零开始。 |
| `name` | `string` | 表头文字 |

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md)

表格

___

### <a id="setcolumnvalue" name="setcolumnvalue"></a> setColumnValue

▸ **setColumnValue**(`tableColumnIndex`, `value`): [`Table`](GC.Spread.Sheets.Tables.Table.md)

用指定的索引设置表尾值

**`代码示例`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
sTable.showFooter(true);
//设置页脚值
sTable.setColumnValue(0, "Total");
//设置页脚公式
sTable.setColumnFormula(4, "SUM(F3:F11)");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tableColumnIndex` | `number` | 页脚的列索引.索引从零开始 |
| `value` | `Object` | 表格页脚值 |

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md)

表格

___

### <a id="showfooter" name="showfooter"></a> showFooter

▸ **showFooter**(`value?`, `isFooterInserted?`): `any`

获取或设置一个值,该值指示是否显示表脚

**`代码示例`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
sTable.showFooter(true);
//设置页脚值
sTable.setColumnValue(0, "Total");
//设置页脚公式
sTable.setColumnFormula(4, "SUM(F3:F11)");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否显示表脚 |
| `isFooterInserted?` | `boolean` | 决定添加表脚的方式,是插入总计行还是仅覆盖下一行.删除表脚是相同的 |

#### Returns

`any`

如果未设置任何值,则返回是否显示表脚;否则,返回表格

___

### <a id="showheader" name="showheader"></a> showHeader

▸ **showHeader**(`value?`): `any`

获取或设置一个值,该值指示是否显示表头

**`代码示例`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
sTable.showHeader(true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否显示表头 |

#### Returns

`any`

如果未设置任何值,则返回是否显示表头.否则,返回表格

___

### <a id="showresizehandle" name="showresizehandle"></a> showResizeHandle

▸ **showResizeHandle**(`value?`): `any`

获取或设置一个值,该值指示是否显示表格的调整大小句柄

**`代码示例`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
sTable.showResizeHandle(true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否显示表格的调整大小句柄 |

#### Returns

`any`

如果未设置任何值,则返回是否显示表格的调整大小句柄,默认为false;否则,返回表格

___

### <a id="style" name="style"></a> style

▸ **style**(`value?`): `any`

获取或设置表格的样式

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md) | 表格的样式 |

#### Returns

`any`

如果未设置任何值,则返回表格样式 否则,返回表格

___

### <a id="usefooterdropdownlist" name="usefooterdropdownlist"></a> useFooterDropDownList

▸ **useFooterDropDownList**(`value?`): `any`

获取或设置一个值,该值指示是否对总行使用页脚下拉列表

**`代码示例`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
sTable.useFooterDropDownList(true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否使用页脚下拉列表 |

#### Returns

`any`

如果未设置任何值,则返回是否对总行使用页脚下拉列表,默认为false;否则,返回表格
