# Class: TableSheet

[Sheets](../modules/GC.Spread.Sheets.md).[TableSheet](../modules/GC.Spread.Sheets.TableSheet.md).TableSheet

## Hierarchy

- **`TableSheet`**

  ↳ [`GanttSheet`](GC.Spread.Sheets.GanttSheet.GanttSheet.md)

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.TableSheet.TableSheet.md#constructor)

### Properties

- [options](GC.Spread.Sheets.TableSheet.TableSheet.md#options)

### Methods

- [addHierarchyItemAbove](GC.Spread.Sheets.TableSheet.TableSheet.md#addhierarchyitemabove)
- [addHierarchyItemAfter](GC.Spread.Sheets.TableSheet.TableSheet.md#addhierarchyitemafter)
- [addHierarchyItemBefore](GC.Spread.Sheets.TableSheet.TableSheet.md#addhierarchyitembefore)
- [addHierarchyItemBelow](GC.Spread.Sheets.TableSheet.TableSheet.md#addhierarchyitembelow)
- [addRow](GC.Spread.Sheets.TableSheet.TableSheet.md#addrow)
- [applyFreeHeaderArea](GC.Spread.Sheets.TableSheet.TableSheet.md#applyfreeheaderarea)
- [applyTableTheme](GC.Spread.Sheets.TableSheet.TableSheet.md#applytabletheme)
- [cancelChanges](GC.Spread.Sheets.TableSheet.TableSheet.md#cancelchanges)
- [collapseAllHierarchyLevels](GC.Spread.Sheets.TableSheet.TableSheet.md#collapseallhierarchylevels)
- [demoteHierarchyLevel](GC.Spread.Sheets.TableSheet.TableSheet.md#demotehierarchylevel)
- [detailColumnsVisible](GC.Spread.Sheets.TableSheet.TableSheet.md#detailcolumnsvisible)
- [expandAllHierarchyLevels](GC.Spread.Sheets.TableSheet.TableSheet.md#expandallhierarchylevels)
- [expandGroup](GC.Spread.Sheets.TableSheet.TableSheet.md#expandgroup)
- [expandGroupItem](GC.Spread.Sheets.TableSheet.TableSheet.md#expandgroupitem)
- [expandHierarchyLevel](GC.Spread.Sheets.TableSheet.TableSheet.md#expandhierarchylevel)
- [getChanges](GC.Spread.Sheets.TableSheet.TableSheet.md#getchanges)
- [getDataView](GC.Spread.Sheets.TableSheet.TableSheet.md#getdataview)
- [groupBy](GC.Spread.Sheets.TableSheet.TableSheet.md#groupby)
- [groupOutlinePosition](GC.Spread.Sheets.TableSheet.TableSheet.md#groupoutlineposition)
- [hasRowState](GC.Spread.Sheets.TableSheet.TableSheet.md#hasrowstate)
- [moveDown](GC.Spread.Sheets.TableSheet.TableSheet.md#movedown)
- [moveUp](GC.Spread.Sheets.TableSheet.TableSheet.md#moveup)
- [printInfo](GC.Spread.Sheets.TableSheet.TableSheet.md#printinfo)
- [promoteHierarchyLevel](GC.Spread.Sheets.TableSheet.TableSheet.md#promotehierarchylevel)
- [removeGroupBy](GC.Spread.Sheets.TableSheet.TableSheet.md#removegroupby)
- [removeRow](GC.Spread.Sheets.TableSheet.TableSheet.md#removerow)
- [resetRow](GC.Spread.Sheets.TableSheet.TableSheet.md#resetrow)
- [rowActionOptions](GC.Spread.Sheets.TableSheet.TableSheet.md#rowactionoptions)
- [saveRow](GC.Spread.Sheets.TableSheet.TableSheet.md#saverow)
- [setDataView](GC.Spread.Sheets.TableSheet.TableSheet.md#setdataview)
- [setDefaultRowHeight](GC.Spread.Sheets.TableSheet.TableSheet.md#setdefaultrowheight)
- [submitChanges](GC.Spread.Sheets.TableSheet.TableSheet.md#submitchanges)
- [togglePinnedColumns](GC.Spread.Sheets.TableSheet.TableSheet.md#togglepinnedcolumns)
- [togglePinnedRows](GC.Spread.Sheets.TableSheet.TableSheet.md#togglepinnedrows)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new TableSheet**(`name?`, `dataView?`, `options?`)

具有指定名称、数据视图和选项设置的集算表

**`代码示例`**
``` javascript
//本示例创建了一个空的集算表
var tableSheet = spread.addSheetTab(0, "", GC.Spread.Sheets.SheetType.tableSheet);

//本示例创建了一个带名称的集算表
var tableSheet = spread.addSheetTab(0, "tableSheet1", GC.Spread.Sheets.SheetType.tableSheet);

//本示例创建了一个带有名称和数据源的集算表
var dataManager = spread.dataManager();
var myTable = dataManager.addTable("myTable", {
    remote: {
        read: {
            url: 'https://demodata.grapecity.com/northwind/api/v1/Orders'
        }
    }
});
myTable.fetch().then(function() {
    var myView = myTable.addView("myView");
    var tableSheet = spread.addSheetTab(0, "tableSheet1", GC.Spread.Sheets.SheetType.tableSheet);
    tableSheet.setDataView(myView);
});

//本示例创建了一个带有名称和选项的集算表
var style = new GC.Spread.Sheets.Style();
var tableSheet = spread.addSheetTab(0, "tableSheet1", GC.Spread.Sheets.SheetType.tableSheet);
tableSheet.options = {allowAddNew: false, alternatingRowOptions: { step: [1, 1], style: style}};
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `name?` | `string` |
| `dataView?` | [`View`](GC.Data.View.md) |
| `options?` | [`ITableSheetOptions`](../interfaces/GC.Spread.Sheets.TableSheet.ITableSheetOptions.md) |

## Properties

### <a id="options" name="options"></a> options

• **options**: [`ITableSheetOptions`](../interfaces/GC.Spread.Sheets.TableSheet.ITableSheetOptions.md)

Represents the options of the table sheet.

**`property`** {boolean} [allowAddNew] - 是否允许添加新的空行。

**`property`** {string} [sheetTabColor] - 用于表示工作表选项卡颜色的颜色字符串，例如“red”、“#FFFF00”、“rgb(255,0,0)”、“Accent 5”等。

**`property`** {GC.Spread.Sheets.TableSheet.IAlternatingRowOptions} [alternatingRowOptions] - 定义交替行样式选项。

**`property`** {number} [defaultStackRowHeight] - Tablesheet默认堆叠行高，默认会计算平均高度。

**`property`** {GC.Spread.Sheets.TableSheet.IMenuItemVisibility} [menuItemVisibility] - Tablesheet默认堆叠行高，默认会计算平均高度。

**`property`** {boolean} [showRowNumber] - 是否显示行号标题。

**`property`** {boolean} [enableDefineColumn] -是否启用定义列。

**`property`** {string} [defineColumnCommand] - 指定用于定义列选项的命令。

**`property`** {string} [submitDefineColumnCommand] - 指定用于提交定义的列选项的命令。

**`property`** {GC.Spread.Sheets.TableSheet.IColumnTypeItem[]} [columnTypeItems] - 指定列类型。

**`property`** {GC.Spread.Sheets.TableSheet.IGroupLayoutOptions} [groupLayout] - 指定组布局的选项。

**`example`**
```
//本示例更改集算表的选项
tableSheet.options.allowAddNew = false;
tableSheet.options.alternatingRowOptions = { step: [1, 1], style: new GC.Spread.Sheets.Style("lightyellow")};
```

## Methods

### <a id="addhierarchyitemabove" name="addhierarchyitemabove"></a> addHierarchyItemAbove

▸ **addHierarchyItemAbove**(`row`, `rowData`): `void`

将新的行数据添加为指定行的父

**`代码示例`**
``` javascript
// 此示例添加新行数据作为指定行的父行
tableSheet.addHierarchyItemAbove(8, {id: 8, name: "grapecity"});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |
| `rowData` | `any` | 行数据 |

#### Returns

`void`

___

### <a id="addhierarchyitemafter" name="addhierarchyitemafter"></a> addHierarchyItemAfter

▸ **addHierarchyItemAfter**(`row`, `rowData`): `void`

在指定的行之后添加新的行数据

**`代码示例`**
``` javascript
// 此示例在指定的行之后添加新的行数据
tableSheet.addHierarchyItemAfter(8, {id: 8, name: "grapecity"});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |
| `rowData` | `any` | 行数据 |

#### Returns

`void`

___

### <a id="addhierarchyitembefore" name="addhierarchyitembefore"></a> addHierarchyItemBefore

▸ **addHierarchyItemBefore**(`row`, `rowData`): `void`

在指定行之前添加新行数据

**`代码示例`**
``` javascript
// 此示例在指定行之前添加新行数据
tableSheet.addHierarchyItemBefore(8, {id: 8, name: "grapecity"});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |
| `rowData` | `any` | 行数据 |

#### Returns

`void`

___

### <a id="addhierarchyitembelow" name="addhierarchyitembelow"></a> addHierarchyItemBelow

▸ **addHierarchyItemBelow**(`row`, `rowData`): `void`

添加新行数据作为指定行的子项

**`代码示例`**
``` javascript
// 此示例添加新行数据作为指定行的子项
tableSheet.addHierarchyItemBelow(8, {id: 8, name: "grapecity"});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |
| `rowData` | `any` | 行数据 |

#### Returns

`void`

___

### <a id="addrow" name="addrow"></a> addRow

▸ **addRow**(`rowData`): `void`

将新行添加到集算表中

**`代码示例`**
``` javascript
//本例添加了一个包含数据的新行
tableSheet.addRow({id: 8, name: "grapecity"});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rowData` | `any` | 行数据 |

#### Returns

`void`

___

### <a id="applyfreeheaderarea" name="applyfreeheaderarea"></a> applyFreeHeaderArea

▸ **applyFreeHeaderArea**(`sheetJson?`): `any`

将工作表JSON应用于集算表列标题自由布局区域

#### Parameters

| Name | Type | Description          |
| :----------- | :---- | :------------------- |
| `sheetJson?` | `any` | 通过toJSON方法获取的工作表JSON |

#### Returns

`any`

___

### <a id="applytabletheme" name="applytabletheme"></a> applyTableTheme

▸ **applyTableTheme**(`tableTheme`): `void`

将表格主题应用于集算表

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tableTheme` | [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md) | 表格主题实例 |

#### Returns

`void`

___

### <a id="cancelchanges" name="cancelchanges"></a> cancelChanges

▸ **cancelChanges**(): `void`

取消批处理模式下的数据管理器的更改

**`代码示例`**
``` javascript
//本例在批处理模式下手动取消更改
tableSheet.cancelChanges();
```

#### Returns

`void`

___

### <a id="collapseallhierarchylevels" name="collapseallhierarchylevels"></a> collapseAllHierarchyLevels

▸ **collapseAllHierarchyLevels**(): `void`

折迭所有层次结构级别

**`代码示例`**
``` javascript
// 此示例折迭所有层次结构级别
tableSheet.collapseAllHierarchyLevels();
```

#### Returns

`void`

___

### <a id="demotehierarchylevel" name="demotehierarchylevel"></a> demoteHierarchyLevel

▸ **demoteHierarchyLevel**(`row`, `withChildren?`): `void`

降级指定行的层次结构数据级别

**`代码示例`**
``` javascript
// 此示例通过指定的索引降级层次结构数据级别
tableSheet.demoteHierarchyLevel(8);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |
| `withChildren?` | `boolean` | 可选，默认情况下，子项将随记录一起降级 |

#### Returns

`void`

___

### <a id="detailcolumnsvisible" name="detailcolumnsvisible"></a> detailColumnsVisible

▸ **detailColumnsVisible**(`value?`): `boolean`

集算表分组后是否显示或隐藏详情列

**`代码示例`**
``` javascript
//本示例显示了如何隐藏详情栏
tableSheet.detailColumnsVisible(false);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 布尔值，表示详情列的可见性 |

#### Returns

`boolean`

返回详情列的可见性

___

### <a id="expandallhierarchylevels" name="expandallhierarchylevels"></a> expandAllHierarchyLevels

▸ **expandAllHierarchyLevels**(): `void`

展开所有层次结构级别

**`代码示例`**
``` javascript
// 此示例扩展所有层次结构级别
tableSheet.expandAllHierarchyLevels();
```

#### Returns

`void`

___

### <a id="expandgroup" name="expandgroup"></a> expandGroup

▸ **expandGroup**(`field`, `expand`): `void`

通过指定的字段扩展或折叠一个级别的分组

**`代码示例`**
``` javascript
//本示例显示了如何折叠一个级别的分组，它是由 "LastName"分组
tableSheet.expandGroup("LastName", false);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `field` | `string` | 字段名称 |
| `expand` | `boolean` | 布尔值,true 意味着扩大分组，false 意味着折叠分组 |

#### Returns

`void`

___

### <a id="expandgroupitem" name="expandgroupitem"></a> expandGroupItem

▸ **expandGroupItem**(`level`, `index`, `expand`): `void`

按指定的级别和索引扩展或折叠一个分组

**`代码示例`**
``` javascript
//本示例显示了如何折叠一个分组，该分组的级别为1,起始索引为10
tableSheet.expandGroupItem(1, 10, false);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `level` | `number` | 分组级别 |
| `index` | `number` | 分组起始索引 |
| `expand` | `boolean` | 布尔值,true 意味着扩大分组,false 意味着折叠分组 |

#### Returns

`void`

___

### <a id="expandhierarchylevel" name="expandhierarchylevel"></a> expandHierarchyLevel

▸ **expandHierarchyLevel**(`level`): `void`

按指定级别展开层次结构数据

**`代码示例`**
``` javascript
// 此示例按指定级别扩展层次结构数据
tableSheet.expandHierarchyLevel(8);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `level` | `number` | 要扩展的级别 |

#### Returns

`void`

___

### <a id="getchanges" name="getchanges"></a> getChanges

▸ **getChanges**(): [`IDataViewChanges`](../interfaces/GC.Spread.Sheets.TableSheet.IDataViewChanges.md)[]

在 autoSync 或批处理模式下获取数据管理器的更改

**`代码示例`**
``` javascript
// 此示例在autoSync或批处理模式下手动进行更改，包括更新的行、插入的行和删除的行
tableSheet.getChanges();
```

#### Returns

[`IDataViewChanges`](../interfaces/GC.Spread.Sheets.TableSheet.IDataViewChanges.md)[]

Returns a object array, each object could contain "type", "dataItem", "oldDataItem", "column", "originalColumn", and "index".
The "type" is the change type, could be one of "insert", "update", "delete", "addColumn", "updateColumn", "removeColumn".
the "dataItem" is the current row data.
The "oldDataItem" is the original row data, only used for "update".
The "column" is the current column.
The "data" is the default value of the current added column.
The "originalColumn" is the original column, only used for "update column".
The "index" is the view index of table sheet.

___

### <a id="getdataview" name="getdataview"></a> getDataView

▸ **getDataView**(): [`View`](GC.Data.View.md)

获取集算表的数据视图

**`代码示例`**
``` javascript
//本示例获取数据源
tableSheet.getDataView();
```

#### Returns

[`View`](GC.Data.View.md)

返回数据视图

___

### <a id="groupby" name="groupby"></a> groupBy

▸ **groupBy**(`options?`): [`IGroupByOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IGroupByOptions.md)[]

按选项对集算表进行分组

**`代码示例`**
``` javascript
//本示例设置了分组选项和分组集算表
tablesheet.groupBy([
     {
         caption: 'Category',
         field: 'category',
         summaryFields:[
             {
                 caption: 'SUM(Quantity)', width: 120, style: { formatter: "$ #,##0.00" }
                 formula: '=SUM([Quantity])',
                 slice: 'Office'
             }
         ]
     }
 ])
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options?` | [`IGroupByOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IGroupByOptions.md)[] | groupBy 的选项 |

#### Returns

[`IGroupByOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IGroupByOptions.md)[]

___

### <a id="groupoutlineposition" name="groupoutlineposition"></a> groupOutlinePosition

▸ **groupOutlinePosition**(`value?`): `boolean`

对集算表进行分组后，是否在视图区和列头区或行头区显示或隐藏分组列

**`代码示例`**
``` javascript
//本示例显示了如何隐藏分组列
tableSheet.groupOutlinePosition(GC.Spread.Sheets.TableSheet.GroupOutlinePosition.none);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`GroupOutlinePosition`](../enums/GC.Spread.Sheets.TableSheet.GroupOutlinePosition.md) | 分组列位置的值 |

#### Returns

`boolean`

返回分组列的位置

___

### <a id="hasrowstate" name="hasrowstate"></a> hasRowState

▸ **hasRowState**(`type`, `row`): `boolean`

判断具有指定状态的行

**`代码示例`**
``` javascript
// 此示例判断具有指定状态的行
tableSheet.hasRowState(GC.Data.RowColumnStates.selected, 0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | [`RowColumnStates`](../enums/GC.Data.RowColumnStates.md) | 行状态的类型 |
| `row` | `number` | 行索引 |

#### Returns

`boolean`

___

### <a id="movedown" name="movedown"></a> moveDown

▸ **moveDown**(`row`): `void`

向下移动指定行的层次结构数据

**`代码示例`**
``` javascript
// 此示例按指定的索引向下移动层次结构数据
tableSheet.moveDown(8);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |

#### Returns

`void`

___

### <a id="moveup" name="moveup"></a> moveUp

▸ **moveUp**(`row`): `void`

向上移动指定行的层次结构数据

**`代码示例`**
``` javascript
// 此示例通过向上移动指定的索引来移动层次结构数据
tableSheet.moveUp(8);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |

#### Returns

`void`

___

### <a id="printinfo" name="printinfo"></a> printInfo

▸ **printInfo**(`value?`): `any`

获取或设置表集算表的打印信息

**`代码示例`**
``` javascript
//设置打印
var printInfo = tableSheet.printInfo();
printInfo.bestFitRows(true);
printInfo.bestFitColumns(true);
tableSheet.printInfo(printInfo);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`PrintInfo`](GC.Spread.Sheets.Print.PrintInfo.md) |

#### Returns

`any`

如果没有设置值，则返回表集算表的打印信息；否则，返回集算表

___

### <a id="promotehierarchylevel" name="promotehierarchylevel"></a> promoteHierarchyLevel

▸ **promoteHierarchyLevel**(`row`): `void`

提升指定行的层次结构数据级别

**`代码示例`**
``` javascript
// 此示例通过指定的索引提升层次结构数据级别
tableSheet.promoteHierarchyLevel(8);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |

#### Returns

`void`

___

### <a id="removegroupby" name="removegroupby"></a> removeGroupBy

▸ **removeGroupBy**(): `void`

删除集算表的分组状态

**`代码示例`**
``` javascript
//本示例展示了删除集算表的分组状态
tablesheet.removeGroupBy()
```

#### Returns

`void`

___

### <a id="removerow" name="removerow"></a> removeRow

▸ **removeRow**(`row`): `void`

从集算表中删除指定的行

**`代码示例`**
``` javascript
//本示例按指定的索引删除行
//当autoSync为true时，变化将被同步
tableSheet.removeRow(8);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |

#### Returns

`void`

___

### <a id="resetrow" name="resetrow"></a> resetRow

▸ **resetRow**(`row`): `void`

重置集算表中指定行的更改

**`代码示例`**
``` javascript
//本示例按指定的索引重置行
tableSheet.resetRow(8);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |

#### Returns

`void`

___

### <a id="rowactionoptions" name="rowactionoptions"></a> rowActionOptions

▸ **rowActionOptions**(`options?`): [`IRowActionOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IRowActionOptions.md)[]

获取或设置行操作的选项

**`代码示例`**
``` javascript
//本示例设置了行操作的选项
let options = tableSheet.rowActionOptions();
options.push({
     icons: ["./comment.png"],
     iconSelector: (item) => {
         return item.comment && item.comment.length > 0;
     }
 });
tableSheet.rowActionOptions(options);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options?` | [`IRowActionOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IRowActionOptions.md)[] | 行操作的选项 |

#### Returns

[`IRowActionOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IRowActionOptions.md)[]

___

### <a id="saverow" name="saverow"></a> saveRow

▸ **saveRow**(`row`): `void`

将集算表中指定行的更改保存到数据管理器，包括更新的行或插入的行

**`代码示例`**
``` javascript
//本例按指定的索引保存行
//当autoSync为true时，变化将被同步
tableSheet.saveRow(8);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |

#### Returns

`void`

___

### <a id="setdataview" name="setdataview"></a> setDataView

▸ **setDataView**(`dataView`): `void`

设置集算表的数据视图

**`代码示例`**
``` javascript
//本示例设置数据源
var dataManager = new GC.Data.DataManager();
var myTable = dataManager.addTable("myTable", {
    remote: {
        read: {
            url: 'https://demodata.grapecity.com/northwind/api/v1/Orders'
        }
    }
});
myTable.fetch().then(function() {
    var myView = myTable.addView("myView");
    tableSheet.setDataView(myView);
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `dataView` | [`View`](GC.Data.View.md) | 要绑定的数据视图 |

#### Returns

`void`

___

### <a id="setdefaultrowheight" name="setdefaultrowheight"></a> setDefaultRowHeight

▸ **setDefaultRowHeight**(`value`, `sheetArea?`): `void`

设置视图区域中所有行的默认高度(以像素为单位)

**`代码示例`**
``` javascript
//本示例以像素为单位设置默认行高
tableSheet.setDefaultRowHeight(50);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `number` | 以像素为单位的高度 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`void`

___

### <a id="submitchanges" name="submitchanges"></a> submitChanges

▸ **submitChanges**(): `void`

以批处理方式向服务器提交数据管理器的更改，包括更新的行、插入的行和删除的行

**`代码示例`**
``` javascript
//本示例以批处理模式手动提交更改
tableSheet.submitChanges();
```

#### Returns

`void`

___

### <a id="togglepinnedcolumns" name="togglepinnedcolumns"></a> togglePinnedColumns

▸ **togglePinnedColumns**(`index`): `void`

用指定的列索引数组固定或取消固定列

**`代码示例`**
``` javascript
//本示例将几个列排在一起
tableSheet.togglePinnedColumns([1,2,4]);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number`[] | 要固定或取消固定的列索引数组 |

#### Returns

`void`

返回固定列数

___

### <a id="togglepinnedrows" name="togglepinnedrows"></a> togglePinnedRows

▸ **togglePinnedRows**(`indexes`): `void`

用指定的行索引数组固定或取消固定行

**`代码示例`**
``` javascript
//本示例将固定几行
tableSheet.togglePinnedRows([1,2,4]);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `indexes` | `number`[] |

#### Returns

`void`

返回固定行数
