# Class: GanttSheet

[Sheets](../modules/GC.Spread.Sheets.md).[GanttSheet](../modules/GC.Spread.Sheets.GanttSheet.md).GanttSheet

## Hierarchy

- [`TableSheet`](GC.Spread.Sheets.TableSheet.TableSheet.md)

  ↳ **`GanttSheet`**

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.GanttSheet.GanttSheet.md#constructor)

### Properties

- [gridlines](GC.Spread.Sheets.GanttSheet.GanttSheet.md#gridlines)
- [mapping](GC.Spread.Sheets.GanttSheet.GanttSheet.md#mapping)
- [options](GC.Spread.Sheets.GanttSheet.GanttSheet.md#options)
- [project](GC.Spread.Sheets.GanttSheet.GanttSheet.md#project)

### Methods

- [addHierarchyItemAbove](GC.Spread.Sheets.GanttSheet.GanttSheet.md#addhierarchyitemabove)
- [addHierarchyItemAfter](GC.Spread.Sheets.GanttSheet.GanttSheet.md#addhierarchyitemafter)
- [addHierarchyItemBefore](GC.Spread.Sheets.GanttSheet.GanttSheet.md#addhierarchyitembefore)
- [addHierarchyItemBelow](GC.Spread.Sheets.GanttSheet.GanttSheet.md#addhierarchyitembelow)
- [addRow](GC.Spread.Sheets.GanttSheet.GanttSheet.md#addrow)
- [applyFreeHeaderArea](GC.Spread.Sheets.GanttSheet.GanttSheet.md#applyfreeheaderarea)
- [applyTableTheme](GC.Spread.Sheets.GanttSheet.GanttSheet.md#applytabletheme)
- [bindGanttView](GC.Spread.Sheets.GanttSheet.GanttSheet.md#bindganttview)
- [cancelChanges](GC.Spread.Sheets.GanttSheet.GanttSheet.md#cancelchanges)
- [collapseAllHierarchyLevels](GC.Spread.Sheets.GanttSheet.GanttSheet.md#collapseallhierarchylevels)
- [demoteHierarchyLevel](GC.Spread.Sheets.GanttSheet.GanttSheet.md#demotehierarchylevel)
- [detailColumnsVisible](GC.Spread.Sheets.GanttSheet.GanttSheet.md#detailcolumnsvisible)
- [expandAllHierarchyLevels](GC.Spread.Sheets.GanttSheet.GanttSheet.md#expandallhierarchylevels)
- [expandGroup](GC.Spread.Sheets.GanttSheet.GanttSheet.md#expandgroup)
- [expandGroupItem](GC.Spread.Sheets.GanttSheet.GanttSheet.md#expandgroupitem)
- [expandHierarchyLevel](GC.Spread.Sheets.GanttSheet.GanttSheet.md#expandhierarchylevel)
- [getActiveTask](GC.Spread.Sheets.GanttSheet.GanttSheet.md#getactivetask)
- [getChanges](GC.Spread.Sheets.GanttSheet.GanttSheet.md#getchanges)
- [getDataView](GC.Spread.Sheets.GanttSheet.GanttSheet.md#getdataview)
- [getSelections](GC.Spread.Sheets.GanttSheet.GanttSheet.md#getselections)
- [getTaskByRow](GC.Spread.Sheets.GanttSheet.GanttSheet.md#gettaskbyrow)
- [groupBy](GC.Spread.Sheets.GanttSheet.GanttSheet.md#groupby)
- [groupOutlinePosition](GC.Spread.Sheets.GanttSheet.GanttSheet.md#groupoutlineposition)
- [hasRowState](GC.Spread.Sheets.GanttSheet.GanttSheet.md#hasrowstate)
- [moveDown](GC.Spread.Sheets.GanttSheet.GanttSheet.md#movedown)
- [moveUp](GC.Spread.Sheets.GanttSheet.GanttSheet.md#moveup)
- [printInfo](GC.Spread.Sheets.GanttSheet.GanttSheet.md#printinfo)
- [promoteHierarchyLevel](GC.Spread.Sheets.GanttSheet.GanttSheet.md#promotehierarchylevel)
- [removeGroupBy](GC.Spread.Sheets.GanttSheet.GanttSheet.md#removegroupby)
- [removeRow](GC.Spread.Sheets.GanttSheet.GanttSheet.md#removerow)
- [resetRow](GC.Spread.Sheets.GanttSheet.GanttSheet.md#resetrow)
- [resumePaint](GC.Spread.Sheets.GanttSheet.GanttSheet.md#resumepaint)
- [rowActionOptions](GC.Spread.Sheets.GanttSheet.GanttSheet.md#rowactionoptions)
- [saveRow](GC.Spread.Sheets.GanttSheet.GanttSheet.md#saverow)
- [setDataView](GC.Spread.Sheets.GanttSheet.GanttSheet.md#setdataview)
- [setDefaultRowHeight](GC.Spread.Sheets.GanttSheet.GanttSheet.md#setdefaultrowheight)
- [submitChanges](GC.Spread.Sheets.GanttSheet.GanttSheet.md#submitchanges)
- [suspendPaint](GC.Spread.Sheets.GanttSheet.GanttSheet.md#suspendpaint)
- [togglePinnedColumns](GC.Spread.Sheets.GanttSheet.GanttSheet.md#togglepinnedcolumns)
- [togglePinnedRows](GC.Spread.Sheets.GanttSheet.GanttSheet.md#togglepinnedrows)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new GanttSheet**(`name?`, `dataView?`)

使用指定的数据视图和选项创建一个甘特表

#### Parameters

| Name | Type |
| :------ | :------ |
| `name?` | `string` |
| `dataView?` | [`View`](GC.Data.View.md) |

#### Overrides

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[constructor](GC.Spread.Sheets.TableSheet.TableSheet.md#constructor)

## Properties

### <a id="gridlines" name="gridlines"></a> gridlines

• **gridlines**: [`GanttGridlines`](GC.Spread.Sheets.GanttSheet.GanttGridlines.md)

获取甘特图的网格线，并配置行类型和颜色

**`readonly`**

___

### <a id="mapping" name="mapping"></a> mapping

• **mapping**: [`GanttMapping`](GC.Spread.Sheets.GanttSheet.GanttMapping.md)

获取此甘特表的映射，用于转换或转换查看的数据

**`readonly`**

___

### <a id="options" name="options"></a> options

• **options**: [`ITableSheetOptions`](../interfaces/GC.Spread.Sheets.TableSheet.ITableSheetOptions.md)

表示集算表的选项

**`property`** {boolean} [allowAddNew] - 是否允许添加新的空行

**`property`** {string} [sheetTabColor] - 用来表示表格颜色的颜色字符串，例如“红色”，“＃ffff00”，“ RGB（255,0,0）”，“ Accent 5”，等等

**`property`** {GC.Spread.Sheets.TableSheet.IAlternatingRowOptions} [alternatingRowOptions] - 定义交替的行样式选项

**`property`** {number} [defaultStackRowHeight] - 集算表默认堆栈行高将默认计算平均高度

**`property`** {GC.Spread.Sheets.TableSheet.IMenuItemVisibility} [menuItemVisibility] - 集算表默认堆栈行高将默认计算平均高度

**`example`**
```
// 此示例更改了集算表的选项
tableSheet.options.allowAddNew = false;
tableSheet.options.alternatingRowOptions = { step: [1, 1], style: new GC.Spread.Sheets.Style("lightyellow")};
```

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[options](GC.Spread.Sheets.TableSheet.TableSheet.md#options)

___

### <a id="project" name="project"></a> project

• **project**: [`Project`](GC.Spread.Sheets.GanttSheet.Project.md)

获取该项目以显示和编辑此甘特表

**`readonly`**

## Methods

### <a id="addhierarchyitemabove" name="addhierarchyitemabove"></a> addHierarchyItemAbove

▸ **addHierarchyItemAbove**(`row`, `rowData`): `void`

将新的行数据添加为指定行的父

**`example`**
```
//此示例将一个新的行数据添加为指定行的父
tableSheet.addHierarchyItemAbove(8, {id: 8, name: "grapecity"});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |
| `rowData` | `any` | 行数据 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[addHierarchyItemAbove](GC.Spread.Sheets.TableSheet.TableSheet.md#addhierarchyitemabove)

___

### <a id="addhierarchyitemafter" name="addhierarchyitemafter"></a> addHierarchyItemAfter

▸ **addHierarchyItemAfter**(`row`, `rowData`): `void`

在指定的行之后添加新的行数据

**`example`**
```
//此示例在指定的行之后添加了一个新的行数据
tableSheet.addHierarchyItemAfter(8, {id: 8, name: "grapecity"});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |
| `rowData` | `any` | 行数据 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[addHierarchyItemAfter](GC.Spread.Sheets.TableSheet.TableSheet.md#addhierarchyitemafter)

___

### <a id="addhierarchyitembefore" name="addhierarchyitembefore"></a> addHierarchyItemBefore

▸ **addHierarchyItemBefore**(`row`, `rowData`): `void`

在指定的行之前添加新的行数据

**`example`**
```
//此示例在指定的行之前添加了一个新的行数据
tableSheet.addHierarchyItemBefore(8, {id: 8, name: "grapecity"});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |
| `rowData` | `any` | 行数据 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[addHierarchyItemBefore](GC.Spread.Sheets.TableSheet.TableSheet.md#addhierarchyitembefore)

___

### <a id="addhierarchyitembelow" name="addhierarchyitembelow"></a> addHierarchyItemBelow

▸ **addHierarchyItemBelow**(`row`, `rowData`): `void`

将新的行数据添加为指定行的子

**`example`**
```
//此示例将一个新的行数据添加为指定行的孩子
tableSheet.addHierarchyItemBelow(8, {id: 8, name: "grapecity"});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |
| `rowData` | `any` | 行数据 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[addHierarchyItemBelow](GC.Spread.Sheets.TableSheet.TableSheet.md#addhierarchyitembelow)

___

### <a id="addrow" name="addrow"></a> addRow

▸ **addRow**(`rowData`): `void`

在表格表中添加了新行

**`example`**
```
//此示例添加了一个带有数据的新行
tableSheet.addRow({id: 8, name: "grapecity"});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rowData` | `any` | 行数据 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[addRow](GC.Spread.Sheets.TableSheet.TableSheet.md#addrow)

___

### <a id="applyfreeheaderarea" name="applyfreeheaderarea"></a> applyFreeHeaderArea

▸ **applyFreeHeaderArea**(`sheetJson?`): `any`

将工作表JSON应用于集算表列标题布局区域

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheetJson?` | `any` | 工作表JSON，可以通过工作表的toJson方法获得 |

#### Returns

`any`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[applyFreeHeaderArea](GC.Spread.Sheets.TableSheet.TableSheet.md#applyfreeheaderarea)

___

### <a id="applytabletheme" name="applytabletheme"></a> applyTableTheme

▸ **applyTableTheme**(`tableTheme`): `void`

将表主题应用于当前的表格

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tableTheme` | [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md) | 表主题实例 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[applyTableTheme](GC.Spread.Sheets.TableSheet.TableSheet.md#applytabletheme)

___

### <a id="bindganttview" name="bindganttview"></a> bindGanttView

▸ **bindGanttView**(`dataView`, `options?`): `void`

设置表格的数据视图

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `dataView` | [`View`](GC.Data.View.md) | 要绑定的数据视图 |
| `options?` | [`IGanttSheetOptions`](../modules/GC.Spread.Sheets.GanttSheet.md#iganttsheetoptions) | - |

#### Returns

`void`

___

### <a id="cancelchanges" name="cancelchanges"></a> cancelChanges

▸ **cancelChanges**(): `void`

在批处理模式下取消数据管理器的更改

**`example`**
```
//此示例在批处理模式下手动取消更改
tableSheet.cancelChanges();
```

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[cancelChanges](GC.Spread.Sheets.TableSheet.TableSheet.md#cancelchanges)

___

### <a id="collapseallhierarchylevels" name="collapseallhierarchylevels"></a> collapseAllHierarchyLevels

▸ **collapseAllHierarchyLevels**(): `void`

折叠所有层次结构

**`example`**
```
//此示例折叠了所有层次结构级别
tableSheet.collapseAllHierarchyLevels();
```

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[collapseAllHierarchyLevels](GC.Spread.Sheets.TableSheet.TableSheet.md#collapseallhierarchylevels)

___

### <a id="demotehierarchylevel" name="demotehierarchylevel"></a> demoteHierarchyLevel

▸ **demoteHierarchyLevel**(`row`, `withChildren?`): `void`

降低指定行的层次结构数据级

**`example`**
```
//此示例通过指定的索引降低了层次结构数据级别
tableSheet.demoteHierarchyLevel(8);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |
| `withChildren?` | `boolean` | 可选，默认情况下，子记录将被降级 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[demoteHierarchyLevel](GC.Spread.Sheets.TableSheet.TableSheet.md#demotehierarchylevel)

___

### <a id="detailcolumnsvisible" name="detailcolumnsvisible"></a> detailColumnsVisible

▸ **detailColumnsVisible**(`value?`): `boolean`

是否显示或隐藏表格之后的详细列

**`example`**
```
//该示例显示了如何隐藏详细列
tableSheet.detailColumnsVisible(false);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 布尔值，指示细节列的可见性 |

#### Returns

`boolean`

返回细节列的可见性

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[detailColumnsVisible](GC.Spread.Sheets.TableSheet.TableSheet.md#detailcolumnsvisible)

___

### <a id="expandallhierarchylevels" name="expandallhierarchylevels"></a> expandAllHierarchyLevels

▸ **expandAllHierarchyLevels**(): `void`

展开所有层次结构级别

**`example`**
```
//此示例展开了所有层次结构级别
tableSheet.expandAllHierarchyLevels();
```

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[expandAllHierarchyLevels](GC.Spread.Sheets.TableSheet.TableSheet.md#expandallhierarchylevels)

___

### <a id="expandgroup" name="expandgroup"></a> expandGroup

▸ **expandGroup**(`field`, `expand`): `void`

通过指定字段展开或折叠一个级别的分组

**`example`**
```
//该示例显示了如何折叠一个级别的分组，该分组由 “LastName” 分组
tableSheet.expandGroup("LastName", false);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `field` | `string` | 字段名称 |
| `expand` | `boolean` | 布尔值，True 代表展开分组，False 代表分组折叠 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[expandGroup](GC.Spread.Sheets.TableSheet.TableSheet.md#expandgroup)

___

### <a id="expandgroupitem" name="expandgroupitem"></a> expandGroupItem

▸ **expandGroupItem**(`level`, `index`, `expand`): `void`

通过指定的级别和索引展开或折叠一个分组

**`example`**
```
//该样本显示了如何折叠一个分组，哪个级别为1，启动索引为10
tableSheet.expandGroupItem(1, 10, false);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `level` | `number` | 分组级别 |
| `index` | `number` | 分组开始索引 |
| `expand` | `boolean` | 布尔值，True 代表展开分组，False 代表分组折叠 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[expandGroupItem](GC.Spread.Sheets.TableSheet.TableSheet.md#expandgroupitem)

___

### <a id="expandhierarchylevel" name="expandhierarchylevel"></a> expandHierarchyLevel

▸ **expandHierarchyLevel**(`level`): `void`

按指定级别展开层次结构数据

**`example`**
```
//此示例按指定级别展开层次结构数据
tableSheet.expandHierarchyLevel(8);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `level` | `number` | 展开的级别 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[expandHierarchyLevel](GC.Spread.Sheets.TableSheet.TableSheet.md#expandhierarchylevel)

___

### <a id="getactivetask" name="getactivetask"></a> getActiveTask

▸ **getActiveTask**(): [`Task`](GC.Spread.Sheets.GanttSheet.Task.md)

在活动行中获取任务

#### Returns

[`Task`](GC.Spread.Sheets.GanttSheet.Task.md)

在活动行中的任务

___

### <a id="getchanges" name="getchanges"></a> getChanges

▸ **getChanges**(): [`IDataViewChanges`](../interfaces/GC.Spread.Sheets.TableSheet.IDataViewChanges.md)[]

在AutoSync或批处理模式下获取数据管理器的更改

**`example`**
```
//此示例以AutoSync或批处理模式手动更改，包括更新的行，插入的行和删除行
tableSheet.getChanges();
```

#### Returns

[`IDataViewChanges`](../interfaces/GC.Spread.Sheets.TableSheet.IDataViewChanges.md)[]

- 返回对象数组，每个对象都可以包含 “type”，“dataitem”，“olddataitem” 和 “index”
    - “type” 是更改类型，可以是 “insert”，“update” 或 “delete” 之一
    - “dataitem” 是当前行数据
    - “oldDataitem” 是原始行数据，仅用于“update”
    - “index” 是表格的视图索引

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[getChanges](GC.Spread.Sheets.TableSheet.TableSheet.md#getchanges)

___

### <a id="getdataview" name="getdataview"></a> getDataView

▸ **getDataView**(): [`View`](GC.Data.View.md)

获取表格的数据视图

**`example`**
```
//此示例获取数据源
tableSheet.getDataView();
```

#### Returns

[`View`](GC.Data.View.md)

返回数据视图

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[getDataView](GC.Spread.Sheets.TableSheet.TableSheet.md#getdataview)

___

### <a id="getselections" name="getselections"></a> getSelections

▸ **getSelections**(): [`Range`](GC.Spread.Sheets.Range.md)[]

获取选择区域

#### Returns

[`Range`](GC.Spread.Sheets.Range.md)[]

选择的区域

___

### <a id="gettaskbyrow" name="gettaskbyrow"></a> getTaskByRow

▸ **getTaskByRow**(`rowIndex`): [`Task`](GC.Spread.Sheets.GanttSheet.Task.md)

在指定的行中获取任务

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rowIndex` | `number` | 一个数字指示行索引 |

#### Returns

[`Task`](GC.Spread.Sheets.GanttSheet.Task.md)

指定行的任务

___

### <a id="groupby" name="groupby"></a> groupBy

▸ **groupBy**(`options?`): [`IGroupByOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IGroupByOptions.md)[]

按选项对表格进行分组

**`example`**
```
//此示例设置组选项并将表格分组
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

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[groupBy](GC.Spread.Sheets.TableSheet.TableSheet.md#groupby)

___

### <a id="groupoutlineposition" name="groupoutlineposition"></a> groupOutlinePosition

▸ **groupOutlinePosition**(`value?`): `boolean`

是在视窗区域和列标题区域中显示或隐藏分组大纲，还是将表格之后的行标头区域分组

**`example`**
```
//该示例显示了如何隐藏分组大纲
tableSheet.groupOutlinePosition(GC.Spread.Sheets.TableSheet.GroupOutlinePosition.none);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`GroupOutlinePosition`](../enums/GC.Spread.Sheets.TableSheet.GroupOutlinePosition.md) | 表示分组大纲位置的值 |

#### Returns

`boolean`

返回分组大纲的位置

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[groupOutlinePosition](GC.Spread.Sheets.TableSheet.TableSheet.md#groupoutlineposition)

___

### <a id="hasrowstate" name="hasrowstate"></a> hasRowState

▸ **hasRowState**(`type`, `row`): `boolean`

用指定的状态对行进行判断

**`example`**
```
//此示例用指定的状态来判断行
tableSheet.hasRowState(GC.Data.RowColumnStates.selected, 0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | [`RowColumnStates`](../enums/GC.Data.RowColumnStates.md) | 行状态的类型 |
| `row` | `number` | 行索引 |

#### Returns

`boolean`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[hasRowState](GC.Spread.Sheets.TableSheet.TableSheet.md#hasrowstate)

___

### <a id="movedown" name="movedown"></a> moveDown

▸ **moveDown**(`row`): `void`

通过指定的行向下移动层次结构数据

**`example`**
```
//此示例通过指定的索引向下移动层次结构数据
tableSheet.moveDown(8);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[moveDown](GC.Spread.Sheets.TableSheet.TableSheet.md#movedown)

___

### <a id="moveup" name="moveup"></a> moveUp

▸ **moveUp**(`row`): `void`

通过指定的行移动层次结构数据

**`example`**
```
//此示例通过指定的索引移动层次结构数据
tableSheet.moveUp(8);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[moveUp](GC.Spread.Sheets.TableSheet.TableSheet.md#moveup)

___

### <a id="printinfo" name="printinfo"></a> printInfo

▸ **printInfo**(`value?`): `any`

获取或设置表格的打印信息

**`example`**
```
//此示例设置打印信息
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

如果未设置值，请返回表格的打印信息；否则，返回表格

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[printInfo](GC.Spread.Sheets.TableSheet.TableSheet.md#printinfo)

___

### <a id="promotehierarchylevel" name="promotehierarchylevel"></a> promoteHierarchyLevel

▸ **promoteHierarchyLevel**(`row`): `void`

提升指定行的层次结构数据级别

**`example`**
```
//此示例通过指定的索引来促进层次结构数据级别
tableSheet.promoteHierarchyLevel(8);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[promoteHierarchyLevel](GC.Spread.Sheets.TableSheet.TableSheet.md#promotehierarchylevel)

___

### <a id="removegroupby" name="removegroupby"></a> removeGroupBy

▸ **removeGroupBy**(): `void`

删除表格的组状态

**`example`**
```
//此示例显示了删除表格的组状态
tablesheet.removeGroupBy()
```

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[removeGroupBy](GC.Spread.Sheets.TableSheet.TableSheet.md#removegroupby)

___

### <a id="removerow" name="removerow"></a> removeRow

▸ **removeRow**(`row`): `void`

从表格上删除指定的行

**`example`**
```
//此示例按指定索引删除行
//当autoSync为true时，更改将同步
tableSheet.removeRow(8);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[removeRow](GC.Spread.Sheets.TableSheet.TableSheet.md#removerow)

___

### <a id="resetrow" name="resetrow"></a> resetRow

▸ **resetRow**(`row`): `void`

重置表格表的指定行的更改

**`example`**
```
//此示例通过指定的索引重置一行
tableSheet.resetRow(8);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[resetRow](GC.Spread.Sheets.TableSheet.TableSheet.md#resetrow)

___

### <a id="resumepaint" name="resumepaint"></a> resumePaint

▸ **resumePaint**(): `void`

恢复甘特表的绘制

#### Returns

`void`

___

### <a id="rowactionoptions" name="rowactionoptions"></a> rowActionOptions

▸ **rowActionOptions**(`options?`): [`IRowActionOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IRowActionOptions.md)[]

获取或设置行动作的选项

**`example`**
```
//此示例设置了行操作的选项
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
| `options?` | [`IRowActionOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IRowActionOptions.md)[] | 行动作的选项 |

#### Returns

[`IRowActionOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IRowActionOptions.md)[]

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[rowActionOptions](GC.Spread.Sheets.TableSheet.TableSheet.md#rowactionoptions)

___

### <a id="saverow" name="saverow"></a> saveRow

▸ **saveRow**(`row`): `void`

将表格表的指定行的更改保存到数据管理器，包括更新的行或插入的行

**`example`**
```
//此示例通过指定的索引保存一行
//当autoSync为true时，更改将同步
tableSheet.saveRow(8);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[saveRow](GC.Spread.Sheets.TableSheet.TableSheet.md#saverow)

___

### <a id="setdataview" name="setdataview"></a> setDataView

▸ **setDataView**(`dataView`): `void`

Sets the data view of table sheet.

**`example`**
```
//此示例设置数据源
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
    tableSheet.setDataView(myView);
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `dataView` | [`View`](GC.Data.View.md) | 要绑定的数据视图 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[setDataView](GC.Spread.Sheets.TableSheet.TableSheet.md#setdataview)

___

### <a id="setdefaultrowheight" name="setdefaultrowheight"></a> setDefaultRowHeight

▸ **setDefaultRowHeight**(`value`, `sheetArea?`): `void`

为视图区域的所有行设置像素的默认高度

**`example`**
```
//此示例设置像素中的默认行高度
tableSheet.setDefaultRowHeight(50);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `number` | 高度的像素 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[setDefaultRowHeight](GC.Spread.Sheets.TableSheet.TableSheet.md#setdefaultrowheight)

___

### <a id="submitchanges" name="submitchanges"></a> submitChanges

▸ **submitChanges**(): `void`

在批处理模式下将数据管理器的更改提交到服务器，包括更新的行，插入的行和删除行

**`example`**
```
//此示例以批处理模式手动提交更改
tableSheet.submitChanges();
```

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[submitChanges](GC.Spread.Sheets.TableSheet.TableSheet.md#submitchanges)

___

### <a id="suspendpaint" name="suspendpaint"></a> suspendPaint

▸ **suspendPaint**(): `void`

暂停甘特表的绘制

#### Returns

`void`

___

### <a id="togglepinnedcolumns" name="togglepinnedcolumns"></a> togglePinnedColumns

▸ **togglePinnedColumns**(`index`): `void`

带有指定列索引数组的 pin 或 unpin 列

**`example`**
```
//此示例 pin 某些列
tableSheet.togglePinnedColumns([1,2,4]);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number`[] | 列索引的阵列要执行 pin 或 unpin |

#### Returns

`void`

返回固定列的计数

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[togglePinnedColumns](GC.Spread.Sheets.TableSheet.TableSheet.md#togglepinnedcolumns)

___

### <a id="togglepinnedrows" name="togglepinnedrows"></a> togglePinnedRows

▸ **togglePinnedRows**(`indexes`): `void`

带有指定的行索引数组的 pin 或 unpin 行

**`example`**
```
//此示例固定某几行
tableSheet.togglePinnedRows([1,2,4]);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `indexes` | `number`[] |

#### Returns

`void`

返回固定行的计数

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[togglePinnedRows](GC.Spread.Sheets.TableSheet.TableSheet.md#togglepinnedrows)
