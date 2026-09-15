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
- [columnLayoutStyle](GC.Spread.Sheets.Tables.Table.md#columnlayoutstyle)
- [dataRange](GC.Spread.Sheets.Tables.Table.md#datarange)
- [deleteColumns](GC.Spread.Sheets.Tables.Table.md#deletecolumns)
- [deleteRows](GC.Spread.Sheets.Tables.Table.md#deleterows)
- [expandBoundRows](GC.Spread.Sheets.Tables.Table.md#expandboundrows)
- [filterButtonVisible](GC.Spread.Sheets.Tables.Table.md#filterbuttonvisible)
- [footerIndex](GC.Spread.Sheets.Tables.Table.md#footerindex)
- [getColumnDataField](GC.Spread.Sheets.Tables.Table.md#getcolumndatafield)
- [getColumnFormula](GC.Spread.Sheets.Tables.Table.md#getcolumnformula)
- [getColumnName](GC.Spread.Sheets.Tables.Table.md#getcolumnname)
- [getColumnValue](GC.Spread.Sheets.Tables.Table.md#getcolumnvalue)
- [getDirtyRows](GC.Spread.Sheets.Tables.Table.md#getdirtyrows)
- [getSlicerData](GC.Spread.Sheets.Tables.Table.md#getslicerdata)
- [getStyleName](GC.Spread.Sheets.Tables.Table.md#getstylename)
- [headerIndex](GC.Spread.Sheets.Tables.Table.md#headerindex)
- [highlightFirstColumn](GC.Spread.Sheets.Tables.Table.md#highlightfirstcolumn)
- [highlightLastColumn](GC.Spread.Sheets.Tables.Table.md#highlightlastcolumn)
- [insertColumns](GC.Spread.Sheets.Tables.Table.md#insertcolumns)
- [insertRows](GC.Spread.Sheets.Tables.Table.md#insertrows)
- [layoutStyle](GC.Spread.Sheets.Tables.Table.md#layoutstyle)
- [name](GC.Spread.Sheets.Tables.Table.md#name)
- [range](GC.Spread.Sheets.Tables.Table.md#range)
- [rowFilter](GC.Spread.Sheets.Tables.Table.md#rowfilter)
- [setColumnDataField](GC.Spread.Sheets.Tables.Table.md#setcolumndatafield)
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

表示可以在工作表中添加的表格。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name?` | `string` | 表格名称。 |
| `row?` | `number` | 表格行索引。 |
| `col?` | `number` | 表格列索引。 |
| `rowCount?` | `number` | 表格行数。 |
| `colCount?` | `number` | 表格列数。 |
| `style?` | `string` \| [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md) | 表格样式或样式名称。 |

## Methods

### <a id="allowautoexpand" name="allowautoexpand"></a> allowAutoExpand

▸ **allowAutoExpand**(`allowAutoExpandState?`): `boolean` \| [`Table`](GC.Spread.Sheets.Tables.Table.md)

获取或设置表格的自动扩展状态。

**`example`**
```
console.log(table.allowAutoExpand());
table.allowAutoExpand(true);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `allowAutoExpandState?` | `boolean` |

#### Returns

`boolean` \| [`Table`](GC.Spread.Sheets.Tables.Table.md)

如果未设置自动扩展状态，则返回表格的自动扩展状态；否则返回表格。

___

### <a id="autogeneratecolumns" name="autogeneratecolumns"></a> autoGenerateColumns

▸ **autoGenerateColumns**(`value?`): `any`

获取或设置绑定数据源时是否自动生成列。

**`example`**
```
var data = {
    sales: [
        {orderDate: '1/6/2013', item: 'Pencil', units: 95},
        {orderDate: '4/1/2013', item: 'Binder', units: 60},
        {orderDate: '6/8/2013', item: 'Pen Set', units: 16}
    ]
};
var table = sheet.tables.add('tableSales', 0, 0, 5, 1); // 只有1列
var tableColumn1 = new GC.Spread.Sheets.Tables.TableColumn(1, "orderDate", "Order Date", "d/M/yy");
var tableColumn2 = new GC.Spread.Sheets.Tables.TableColumn(2, "item", "Item");
var tableColumn3 = new GC.Spread.Sheets.Tables.TableColumn(3, "units", "Units");

table.autoGenerateColumns(false);
table.bind([tableColumn1, tableColumn2, tableColumn3], 'sales', data);
console.log(table.dataRange().colCount);    // 1

table.autoGenerateColumns(true);
table.bind([tableColumn1, tableColumn2, tableColumn3], 'sales', data);
console.log(table.dataRange().colCount);    // 3
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置值，则返回绑定数据源时是否自动生成列；否则返回表格。

___

### <a id="bandcolumns" name="bandcolumns"></a> bandColumns

▸ **bandColumns**(`value?`): `any`

获取或设置是否显示交替列样式。

**`example`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
sTable.bandColumns(true);
sTable.bandRows(true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否显示交替列样式。 |

#### Returns

`any`

如果未设置值，则返回是否显示交替列样式；否则返回表格。

___

### <a id="bandrows" name="bandrows"></a> bandRows

▸ **bandRows**(`value?`): `any`

获取或设置是否显示交替行样式。

**`example`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
sTable.bandColumns(true);
sTable.bandRows(true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否显示交替行样式。 |

#### Returns

`any`

如果未设置值，则返回是否显示交替行样式；否则返回表格。

___

### <a id="bind" name="bind"></a> bind

▸ **bind**(`columns`, `path?`, `dataSource?`): [`Table`](GC.Spread.Sheets.Tables.Table.md) \| `Promise`<[`Table`](GC.Spread.Sheets.Tables.Table.md)\>

获取或设置表格的数据源、绑定列和路径。

**`example`**
```
var data = {
  name: 'Jones', region: 'East',
  sales: [
    {orderDate: '1/6/2013', item: 'Pencil', units: 95, cost: 1.99, isMakeMoney: true},
    {orderDate: '4/1/2013', item: 'Binder', units: 60, cost: 4.99, isMakeMoney: false},
    {orderDate: '6/8/2013', item: 'Pen Set', units: 16, cost: 15.99, isMakeMoney: false}
  ]
};
var convert = function (item) {
  return item['cost'] + '$';
}
var table = sheet.tables.add('tableSales', 0, 0, 5, 5);
var tableColumn1 = new GC.Spread.Sheets.Tables.TableColumn(1, "orderDate", "Order Date", "d/M/yy");
var tableColumn2 = new GC.Spread.Sheets.Tables.TableColumn(2, "item", "Item");
var tableColumn3 = new GC.Spread.Sheets.Tables.TableColumn(3, "units", "Units");
var tableColumn4 = new GC.Spread.Sheets.Tables.TableColumn(4, "cost", "Cost", null, null, convert);
var tableColumn5 = new GC.Spread.Sheets.Tables.TableColumn(5, "isMakeMoney", "IsMakeMoney", null, new GC.Spread.Sheets.CellTypes.CheckBox());
table.autoGenerateColumns(false);

table.bind([tableColumn1, tableColumn2, tableColumn3, tableColumn4, tableColumn5], 'sales', data);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columns` | [`TableColumn`](GC.Spread.Sheets.Tables.TableColumn.md)[] | 包含数据字段和名称的表格列信息数组。每个项目都是 GC.Spread.Sheets.Tables.TableColumn。 |
| `path?` | `string` | - |
| `dataSource?` | `string` \| `object` \| [`Table`](GC.Data.Table.md) | - |

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md) \| `Promise`<[`Table`](GC.Spread.Sheets.Tables.Table.md)\>

返回表格。

___

### <a id="bindcolumns" name="bindcolumns"></a> bindColumns

▸ **bindColumns**(`columns`): `void`

使用指定的数据字段绑定列。

**`example`**
```
var table = sheet.tables.add('tableSales', 0, 0, 5, 2);
var tableColumn1 = new GC.Spread.Sheets.Tables.TableColumn(1, "orderDate", "Order Date", "d/M/yy");
var tableColumn2 = new GC.Spread.Sheets.Tables.TableColumn(2, "item", "Item");
table.bindColumns([tableColumn1, tableColumn2]);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columns` | [`TableColumn`](GC.Spread.Sheets.Tables.TableColumn.md)[] | 包含数据字段和名称的表格列信息数组。每个项目都是 GC.Spread.Sheets.Tables.TableColumn。 |

#### Returns

`void`

___

### <a id="bindingpath" name="bindingpath"></a> bindingPath

▸ **bindingPath**(`value?`): `any`

获取或设置表格中单元格级绑定的绑定路径。

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `string` |

#### Returns

`any`

如果未设置值，则返回表格中单元格级绑定的绑定路径；否则返回表格。

___

### <a id="clearpendingchanges" name="clearpendingchanges"></a> clearPendingChanges

▸ **clearPendingChanges**(): `void`

清除当前表格的脏数据状态。

**`example`**
```
// 表格绑定数据
var data = {
    sales: [
        {orderDate: '1/6/2013', item: 'Pencil'},
        {orderDate: '4/1/2013', item: 'Binder'},
        {orderDate: '6/8/2013', item: 'Pen Set'}
    ]
};
var table = sheet.tables.add('tableSales', 0, 0, 5, 5);
var tableColumn1 = new GC.Spread.Sheets.Tables.TableColumn(1, "orderDate", "Order Date", "d/M/yy");
var tableColumn2 = new GC.Spread.Sheets.Tables.TableColumn(2, "item", "Item");
table.bind([tableColumn1, tableColumn2], 'sales', data);
sheet.setValue(1, 1, 'dirty data');
console.log(table.getDirtyRows()); // [{row:0, item: ..., originalItem: ...}]

table.clearPendingChanges();
console.log(table.getDirtyRows()); // [ ]
```

#### Returns

`void`

___

### <a id="columnlayoutstyle" name="columnlayoutstyle"></a> columnLayoutStyle

▸ **columnLayoutStyle**(`tableColumnIndex`, `value?`): [`Table`](GC.Spread.Sheets.Tables.Table.md) \| [`ITableLayoutStyle`](../interfaces/GC.Spread.Sheets.Tables.ITableLayoutStyle.md)

获取或设置表格列的布局样式。

**`example`**
```
var table = activeSheet.tables.find(0,0);
var dataStyle = new GC.Spread.Sheets.Style();
dataStyle.backColor = "red";
var footerStyle = new GC.Spread.Sheets.Style();
footerStyle.backColor = "green";
var layoutStyle = {};
layoutStyle.data = dataStyle;
layoutStyle.footer = footerStyle;
table.columnLayoutStyle(1, layoutStyle);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tableColumnIndex` | `number` | 表格列的列索引。索引从零开始。 |
| `value?` | [`ITableLayoutStyle`](../interfaces/GC.Spread.Sheets.Tables.ITableLayoutStyle.md) | - |

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md) \| [`ITableLayoutStyle`](../interfaces/GC.Spread.Sheets.Tables.ITableLayoutStyle.md)

如果未设置值，则返回表格列的布局样式；否则返回表格。

___

### <a id="datarange" name="datarange"></a> dataRange

▸ **dataRange**(): [`Range`](GC.Spread.Sheets.Range.md)

获取表格数据区域的单元格范围。

**`example`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
var drange = sTable.dataRange();
alert(drange.row);
```

#### Returns

[`Range`](GC.Spread.Sheets.Range.md)

表格数据范围。

___

### <a id="deletecolumns" name="deletecolumns"></a> deleteColumns

▸ **deleteColumns**(`col`, `count`): `void`

在指定的表格列索引处删除指定数量的列。

**`example`**
```
var table = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
table.deleteColumns(3, 1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `col` | `number` | 要删除的第一列的索引，基于表格索引。 |
| `count` | `number` | 要删除的列数。 |

#### Returns

`void`

___

### <a id="deleterows" name="deleterows"></a> deleteRows

▸ **deleteRows**(`row`, `count`): `void`

删除指定表格行索引处的行。

**`example`**
```
var table = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
table.deleteRows(3, 1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 要删除的第一行的索引，基于表格索引。 |
| `count` | `number` | 要删除的行数。 |

#### Returns

`void`

___

### <a id="expandboundrows" name="expandboundrows"></a> expandBoundRows

▸ **expandBoundRows**(`value?`): `any`

获取或设置表格绑定模式下的行扩展模式。

**`example`**
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

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置值，则返回是否通过工作表或表格插入/删除行来扩展；否则返回表格。

___

### <a id="filterbuttonvisible" name="filterbuttonvisible"></a> filterButtonVisible

▸ **filterButtonVisible**(`tableColumnIndex?`, `value?`): `any`

获取或设置表格列的过滤器按钮是否显示。

**`example`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
sTable.bandColumns(true);
sTable.bandRows(true);
sTable.filterButtonVisible(2, false);
alert(sTable.filterButtonVisible(2));
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `tableColumnIndex?` | `number` \| `boolean` |
| `value?` | `boolean` |

#### Returns

`any`

表格列的过滤器按钮显示状态。
如果未设置参数，则返回`false`，如果所有过滤器按钮都不可见，则返回`true`。
如果只设置一个数字，则返回指定表格列的过滤器按钮是否显示。
如果只设置一个布尔值，则应用于所有过滤器按钮并返回表格。
如果提供两个参数，则应用于指定表格列的过滤器按钮并返回表格。

___

### <a id="footerindex" name="footerindex"></a> footerIndex

▸ **footerIndex**(): `number`

获取表格页脚的索引。

**`example`**
```
var sTable = sheet.tables.add("table1", 0, 0, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
sTable.showFooter(true);

var footerIndex = sTable.footerIndex();
console.log(footerIndex) // 10
// Cause the table's footer is on row 11.
```

#### Returns

`number`

页脚索引。

___

### <a id="getcolumndatafield" name="getcolumndatafield"></a> getColumnDataField

▸ **getColumnDataField**(`tableColumnIndex`): `string`

获取指定表格列索引的表格列数据字段。

**`example`**
```
table.setColumnDataField(3, "name");
const dataField = table.getColumnDataField(3); // "name"
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tableColumnIndex` | `number` | 表格列的列索引。索引从零开始。 |

#### Returns

`string`

指定表格列的数据字段。

___

### <a id="getcolumnformula" name="getcolumnformula"></a> getColumnFormula

▸ **getColumnFormula**(`tableColumnIndex`): `string`

获取指定索引的表格页脚公式。

**`example`**
```
var sTable = sheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
//set footer formula
sTable.setColumnFormula(4, "SUM(F3:F11)");

//get footer formula
var columnFormula = sTable.getColumnFormula(4);
console.log(columnFormula); // "SUM(F3:F11)"
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tableColumnIndex` | `number` | 表格页脚的列索引。索引从零开始。 |

#### Returns

`string`

表格页脚公式。

___

### <a id="getcolumnname" name="getcolumnname"></a> getColumnName

▸ **getColumnName**(`tableColumnIndex`): `string`

获取指定表格索引的表格标题文本。

**`example`**
```
var sTable = sheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
sTable.setColumnName(4, "SUM");

var value = sTable.getColumnName(4);
console.log(value); // "SUM"
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tableColumnIndex` | `number` | 表格标题的列索引。索引从零开始。 |

#### Returns

`string`

指定列索引的表格标题文本。

___

### <a id="getcolumnvalue" name="getcolumnvalue"></a> getColumnValue

▸ **getColumnValue**(`tableColumnIndex`): `string`

获取指定索引的表格页脚值。

**`example`**
```
var sTable = sheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
// 设置页脚值
sTable.setColumnValue(0, "Total");

// 获取页脚值
var value = sTable.getColumnValue(0);
console.log(value) // "Total"
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tableColumnIndex` | `number` | 表格页脚的列索引。索引从零开始。 |

#### Returns

`string`

表格页脚值。

___

### <a id="getdirtyrows" name="getdirtyrows"></a> getDirtyRows

▸ **getDirtyRows**(): [`IRowState`](../interfaces/GC.Spread.Sheets.Tables.IRowState.md)[]

获取脏数据行数组。

**`example`**
```
// 表格绑定数据
var data = {
    sales: [
        {orderDate: '1/6/2013', item: 'Pencil'},
        {orderDate: '4/1/2013', item: 'Binder'},
        {orderDate: '6/8/2013', item: 'Pen Set'}
    ]
};
var table = sheet.tables.add('tableSales', 0, 0, 5, 5);
var tableColumn1 = new GC.Spread.Sheets.Tables.TableColumn(1, "orderDate", "Order Date", "d/M/yy");
var tableColumn2 = new GC.Spread.Sheets.Tables.TableColumn(2, "item", "Item");
table.bind([tableColumn1, tableColumn2], 'sales', data);

console.log(table.getDirtyRows()); // [ ]

sheet.setValue(1, 1, 'dirty data');
console.log(table.getDirtyRows()); // [{row:0, item: ..., originalItem: ...}]
```

#### Returns

[`IRowState`](../interfaces/GC.Spread.Sheets.Tables.IRowState.md)[]

脏数据行集合。数组中的项包含三个属性：row：指定表格行索引，item：指定当前行的数据项，originalItem：指定该行的原始数据项。

___

### <a id="getslicerdata" name="getslicerdata"></a> getSlicerData

▸ **getSlicerData**(): [`TableSlicerData`](GC.Spread.Sheets.Slicers.TableSlicerData.md)

获取表格的切片器数据。

**`example`**
```
var activeSheet = spread.getActiveSheet();
var dataSource = [
    { Name: "Bob", City: "NewYork", Birthday: "1968/6/8" },
    { Name: "Betty", City: "NewYork", Birthday: "1972/7/3" },
    { Name: "Alice", City: "Washington", Birthday: "2012/2/15" },
];
var table = activeSheet.tables.addFromDataSource("table1", 1, 1, dataSource);
var slicerData = table.getSlicerData();
console.log(slicerData instanceof GC.Spread.Sheets.Slicers.TableSlicerData); // true
console.log(table.getSlicerData() === slicerData); // true
```

#### Returns

[`TableSlicerData`](GC.Spread.Sheets.Slicers.TableSlicerData.md)

表格的切片器数据。

___

### <a id="getstylename" name="getstylename"></a> getStyleName

▸ **getStyleName**(): `undefined` \| `string`

获取或设置表格的样式名称。

#### Returns

`undefined` \| `string`

表格样式名称。

___

### <a id="headerindex" name="headerindex"></a> headerIndex

▸ **headerIndex**(): `number`

获取表格标题的索引。

**`example`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
var hindex = sTable.headerIndex();
alert(hindex);
```

#### Returns

`number`

标题索引。

___

### <a id="highlightfirstcolumn" name="highlightfirstcolumn"></a> highlightFirstColumn

▸ **highlightFirstColumn**(`value?`): `any`

获取或设置是否突出显示第一列。

**`example`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
sTable.highlightFirstColumn(true);
sTable.highlightLastColumn(true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否突出显示第一列。 |

#### Returns

`any`

如果未设置值，则返回是否突出显示第一列；否则返回表格。

___

### <a id="highlightlastcolumn" name="highlightlastcolumn"></a> highlightLastColumn

▸ **highlightLastColumn**(`value?`): `any`

获取或设置是否突出显示最后一列。

**`example`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
sTable.highlightFirstColumn(true);
sTable.highlightLastColumn(true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 是否突出显示最后一列。 |

#### Returns

`any`

如果未设置值，则返回是否突出显示最后一列；否则返回表格。

___

### <a id="insertcolumns" name="insertcolumns"></a> insertColumns

▸ **insertColumns**(`col`, `count`, `isInsertAfter?`): `void`

在指定的表格列索引之前插入指定数量的列。

**`example`**
```
var table = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
table.insertColumns(3, 1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `col` | `number` | 要添加新列的表格列索引，基于表格索引。 |
| `count` | `number` | 要添加的列数。 |
| `isInsertAfter?` | `boolean` | - |

#### Returns

`void`

___

### <a id="insertrows" name="insertrows"></a> insertRows

▸ **insertRows**(`row`, `count`, `isInsertAfter?`): `void`

在指定的表格行索引之前插入指定数量的行。

**`example`**
```
var table = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
table.insertRows(3, 1);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 要插入的第一行的索引，基于表格索引。 |
| `count` | `number` | 要添加的行数。 |
| `isInsertAfter?` | `boolean` | - |

#### Returns

`void`

___

### <a id="layoutstyle" name="layoutstyle"></a> layoutStyle

▸ **layoutStyle**(`value?`): [`Table`](GC.Spread.Sheets.Tables.Table.md) \| [`ITableLayoutStyle`](../interfaces/GC.Spread.Sheets.Tables.ITableLayoutStyle.md)

获取或设置表格数据区域的样式。

**`example`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
var dataStyle = new GC.Spread.Sheets.Style();
dataStyle.backColor = "red";
var footerStyle = new GC.Spread.Sheets.Style();
footerStyle.backColor = "green";
var layoutStyle = {};
layoutStyle.data = dataStyle;
layoutStyle.footer = footerStyle;
table.layoutStyle(layoutStyle);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`ITableLayoutStyle`](../interfaces/GC.Spread.Sheets.Tables.ITableLayoutStyle.md) |

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md) \| [`ITableLayoutStyle`](../interfaces/GC.Spread.Sheets.Tables.ITableLayoutStyle.md)

如果未设置值，则返回表格数据区域的样式；否则返回表格。

___

### <a id="name" name="name"></a> name

▸ **name**(`value?`): `any`

获取或设置表格名称。

**`example`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
var tname = sTable.name();
alert(tname);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` | 表格名称。 |

#### Returns

`any`

如果未设置值，则返回表格名称；否则返回表格。

___

### <a id="range" name="range"></a> range

▸ **range**(): [`Range`](GC.Spread.Sheets.Range.md)

获取表格的整个范围。

**`example`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
var drange = sTable.range();
alert(drange.row);
```

#### Returns

[`Range`](GC.Spread.Sheets.Range.md)

表格的整个范围。

___

### <a id="rowfilter" name="rowfilter"></a> rowFilter

▸ **rowFilter**(): [`HideRowFilter`](GC.Spread.Sheets.Filter.HideRowFilter.md)

获取表格的行过滤器。

**`example`**
```
var table = sheet.tables.add('table1', 0, 0, 5, 5);

let rowFilter = table.rowFilter();
console.log(rowFilter.range);
```

#### Returns

[`HideRowFilter`](GC.Spread.Sheets.Filter.HideRowFilter.md)

行过滤器。

___

### <a id="setcolumndatafield" name="setcolumndatafield"></a> setColumnDataField

▸ **setColumnDataField**(`tableColumnIndex`, `dataField`): [`Table`](GC.Spread.Sheets.Tables.Table.md)

设置指定表格列索引的表格列数据字段。

**`example`**
```
let data = {
    name: 'Jones', region: 'East',
    sales: [
        {orderDate: '1/6/2013', item: 'Pencil', units: 95, cost: 1.99, isMakeMoney: true},
        {orderDate: '4/1/2013', item: 'Binder', units: 60, cost: 4.99, isMakeMoney: false},
        {orderDate: '6/8/2013', item: 'Pen Set', units: 16, cost: 15.99, isMakeMoney: false}
    ]
};
let spreadNS = GC.Spread.Sheets;
let table = sheet.tables.add('tableSales', 0, 0, 4, 2);
let tableColumn1 = new spreadNS.Tables.TableColumn(1);
tableColumn1.name("OrderDate");
tableColumn1.dataField("orderDate");
tableColumn1.formatter("d/M/yy");
let tableColumn2 = new spreadNS.Tables.TableColumn(2);
tableColumn2.name("Item");
tableColumn2.dataField("item");
table.bind([tableColumn1, tableColumn2], 'sales', data);

// to update the name and dataField of tableColumn2
table.setColumnName(1, 'Cost');
table.setColumnDataField(1, 'cost');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tableColumnIndex` | `number` | 表格列的列索引。索引从零开始。 |
| `dataField` | `string` | 表格列数据字段。 |

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md)

表格。

___

### <a id="setcolumndataformula" name="setcolumndataformula"></a> setColumnDataFormula

▸ **setColumnDataFormula**(`tableColumnIndex`, `formula`): [`Table`](GC.Spread.Sheets.Tables.Table.md)

设置指定索引的表格数据范围公式。

**`example`**
```
// 此示例使用表格中的结构化引用公式。
activeSheet.tables.add("Table1", 0, 0, 4, 3, GC.Spread.Sheets.Tables.TableThemes.dark1);
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
activeSheet.tables.findByName("Table1").setColumnDataFormula(2, null); // to clear the column data formula
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tableColumnIndex` | `number` | 表格列的列索引。索引从零开始。 |
| `formula` | ``null`` \| `string` | 数据范围公式。 |

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md)

表格。

___

### <a id="setcolumnformula" name="setcolumnformula"></a> setColumnFormula

▸ **setColumnFormula**(`tableColumnIndex`, `formula`): [`Table`](GC.Spread.Sheets.Tables.Table.md)

设置指定索引的表格页脚公式。

**`example`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
sTable.showFooter(true);
// 设置页脚值
sTable.setColumnValue(0, "Total");
// 设置页脚公式
sTable.setColumnFormula(4, "SUM(F3:F11)");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tableColumnIndex` | `number` | 表格页脚的列索引。索引从零开始。 |
| `formula` | `string` | 表格页脚公式。 |

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md)

表格。

___

### <a id="setcolumnname" name="setcolumnname"></a> setColumnName

▸ **setColumnName**(`tableColumnIndex`, `name`): [`Table`](GC.Spread.Sheets.Tables.Table.md)

设置指定表格索引的表格标题文本。

**`example`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
sTable.showFooter(true);
sTable.setColumnName(4, "SUM");
// 设置页脚值
sTable.setColumnValue(0, "Total");
// 设置页脚公式
sTable.setColumnFormula(4, "SUM(F3:F11)");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tableColumnIndex` | `number` | 表格标题的列索引。索引从零开始。 |
| `name` | `string` | 表格标题文本。 |

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md)

表格。

___

### <a id="setcolumnvalue" name="setcolumnvalue"></a> setColumnValue

▸ **setColumnValue**(`tableColumnIndex`, `value`): [`Table`](GC.Spread.Sheets.Tables.Table.md)

设置指定索引的表格页脚值。

**`example`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
sTable.showFooter(true);
// 设置页脚值
sTable.setColumnValue(0, "Total");
// 设置页脚公式
sTable.setColumnFormula(4, "SUM(F3:F11)");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tableColumnIndex` | `number` | 表格页脚的列索引。索引从零开始。 |
| `value` | `Object` | 表格页脚值。 |

#### Returns

[`Table`](GC.Spread.Sheets.Tables.Table.md)

表格。

___

### <a id="showfooter" name="showfooter"></a> showFooter

▸ **showFooter**(`value?`, `isFooterInserted?`): `any`

获取或设置表格页脚是否显示。

**`example`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
sTable.showFooter(true);
//设置页脚值
sTable.setColumnValue(0, "Total");
//设置页脚公式
sTable.setColumnFormula(4, "SUM(F3:F11)");
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |
| `isFooterInserted?` | `boolean` |

#### Returns

`any`

如果未设置值，则返回是否显示页脚；否则返回表格。

___

### <a id="showheader" name="showheader"></a> showHeader

▸ **showHeader**(`value?`): `any`

获取或设置是否显示表格标题。

**`example`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
sTable.showHeader(true);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置值，则返回是否显示标题；否则返回表格。

___

### <a id="showresizehandle" name="showresizehandle"></a> showResizeHandle

▸ **showResizeHandle**(`value?`): `any`

获取或设置是否显示表格的调整大小手柄。

**`example`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
sTable.showResizeHandle(true);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置值，则返回是否显示表格的调整大小手柄，默认为false；否则返回表格。

___

### <a id="style" name="style"></a> style

▸ **style**(`value?`): `any`

获取或设置表格的样式。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `string` \| [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md) | 表格的样式或样式名称。 |

#### Returns

`any`

如果未设置值，则返回表格样式；否则返回表格。

___

### <a id="usefooterdropdownlist" name="usefooterdropdownlist"></a> useFooterDropDownList

▸ **useFooterDropDownList**(`value?`): `any`

获取或设置是否在总计行使用页脚下拉列表。

**`example`**
```
var sTable = activeSheet.tables.add("table1", 1, 1, 10, 5, GC.Spread.Sheets.Tables.TableThemes.medium2);
sTable.useFooterDropDownList(true);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`any`

如果未设置值，则返回是否在总计行使用页脚下拉列表，默认为false；否则返回表格。
