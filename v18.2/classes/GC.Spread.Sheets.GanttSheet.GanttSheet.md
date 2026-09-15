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

使用指定的数据视图和选项创建甘特图表。

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

获取甘特图表的网格线，并配置线条类型和颜色。

**`readonly`**

___

### <a id="mapping" name="mapping"></a> mapping

• **mapping**: [`GanttMapping`](GC.Spread.Sheets.GanttSheet.GanttMapping.md)

获取此甘特图表的映射，用于转换或转换回视图中的数据。

**`readonly`**

___

### <a id="options" name="options"></a> options

• **options**: [`ITableSheetOptions`](../interfaces/GC.Spread.Sheets.TableSheet.ITableSheetOptions.md)

表示计算表的选项。

**`property`** {boolean} [allowAddNew] - 是否允许添加新的空行。

**`property`** {string} [sheetTabColor] - 用于表示工作表标签颜色的颜色字符串，如"red"、"#FFFF00"、"rgb(255,0,0)"、"Accent 5"等。

**`property`** {GC.Spread.Sheets.TableSheet.IAlternatingRowOptions} [alternatingRowOptions] - 定义交替行样式选项。

**`property`** {number} [defaultStackRowHeight] - 计算表默认堆叠行高，默认将计算平均高度。

**`property`** {GC.Spread.Sheets.TableSheet.IMenuItemVisibility} [menuItemVisibility] - 计算表菜单项的可见性。

**`property`** {boolean} [showRowNumber] - 是否显示行号标题。

**`property`** {boolean} [enableDefineColumn] - 是否启用定义列。

**`property`** {string} [defineColumnCommand] - 指定定义列选项的命令。

**`property`** {string} [submitDefineColumnCommand] - 指定提交已定义列选项的命令。

**`property`** {GC.Spread.Sheets.TableSheet.IColumnTypeItem[]} [columnTypeItems] - 指定列类型。

**`property`** {GC.Spread.Sheets.TableSheet.IGroupLayoutOptions} [groupLayout] - 指定分组布局的选项。

**`example`**
```
//此示例更改计算表的选项。
tableSheet.options.allowAddNew = false;
tableSheet.options.alternatingRowOptions = { step: [1, 1], style: new GC.Spread.Sheets.Style("lightyellow")};
```

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[options](GC.Spread.Sheets.TableSheet.TableSheet.md#options)

___

### <a id="project" name="project"></a> project

• **project**: [`Project`](GC.Spread.Sheets.GanttSheet.Project.md)

获取此甘特图表的项目，用于显示和编辑。

**`readonly`**

## Methods

### <a id="addhierarchyitemabove" name="addhierarchyitemabove"></a> addHierarchyItemAbove

▸ **addHierarchyItemAbove**(`row`, `rowData`): `void`

在指定行的上方添加新的行数据作为其父级。

**`example`**
```
//此示例在指定行的上方添加新的行数据作为其父级。
tableSheet.addHierarchyItemAbove(8, {id: 8, name: "spreadjs"});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `rowData` | `any` | 行数据。 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[addHierarchyItemAbove](GC.Spread.Sheets.TableSheet.TableSheet.md#addhierarchyitemabove)

___

### <a id="addhierarchyitemafter" name="addhierarchyitemafter"></a> addHierarchyItemAfter

▸ **addHierarchyItemAfter**(`row`, `rowData`): `void`

在指定行之后添加新的行数据。

**`example`**
```
//此示例在指定行之后添加新的行数据。
tableSheet.addHierarchyItemAfter(8, {id: 8, name: "spreadjs"});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `rowData` | `any` | 行数据。 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[addHierarchyItemAfter](GC.Spread.Sheets.TableSheet.TableSheet.md#addhierarchyitemafter)

___

### <a id="addhierarchyitembefore" name="addhierarchyitembefore"></a> addHierarchyItemBefore

▸ **addHierarchyItemBefore**(`row`, `rowData`): `void`

在指定行之前添加新的行数据。

**`example`**
```
//此示例在指定行之前添加新的行数据。
tableSheet.addHierarchyItemBefore(8, {id: 8, name: "spreadjs"});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `rowData` | `any` | 行数据。 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[addHierarchyItemBefore](GC.Spread.Sheets.TableSheet.TableSheet.md#addhierarchyitembefore)

___

### <a id="addhierarchyitembelow" name="addhierarchyitembelow"></a> addHierarchyItemBelow

▸ **addHierarchyItemBelow**(`row`, `rowData`): `void`

在指定行下方添加新的行数据作为其子级。

**`example`**
```
//此示例在指定行下方添加新的行数据作为其子级。
tableSheet.addHierarchyItemBelow(8, {id: 8, name: "spreadjs"});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `rowData` | `any` | 行数据。 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[addHierarchyItemBelow](GC.Spread.Sheets.TableSheet.TableSheet.md#addhierarchyitembelow)

___

### <a id="addrow" name="addrow"></a> addRow

▸ **addRow**(`rowData`): `Promise`<`void`\>

向计算表添加新行。

**`example`**
```
//此示例添加一个带数据的行。
tableSheet.addRow({id: 8, name: "spreadjs"});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rowData` | `any` | 行数据。 |

#### Returns

`Promise`<`void`\>

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[addRow](GC.Spread.Sheets.TableSheet.TableSheet.md#addrow)

___

### <a id="applyfreeheaderarea" name="applyfreeheaderarea"></a> applyFreeHeaderArea

▸ **applyFreeHeaderArea**(`sheetJson?`): `any`

将工作表JSON应用到TableSheet列标题自由布局区域。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheetJson?` | `any` | 工作表JSON，可以通过工作表的toJSON方法轻松获取。 |

#### Returns

`any`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[applyFreeHeaderArea](GC.Spread.Sheets.TableSheet.TableSheet.md#applyfreeheaderarea)

___

### <a id="applytabletheme" name="applytabletheme"></a> applyTableTheme

▸ **applyTableTheme**(`tableTheme`): `void`

将表格主题应用到当前TableSheet。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `tableTheme` | [`TableTheme`](GC.Spread.Sheets.Tables.TableTheme.md) | 表格主题实例。 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[applyTableTheme](GC.Spread.Sheets.TableSheet.TableSheet.md#applytabletheme)

___

### <a id="bindganttview" name="bindganttview"></a> bindGanttView

▸ **bindGanttView**(`dataView`, `options?`): `void`

设置表格的数据视图。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `dataView` | [`View`](GC.Data.View.md) | 要绑定的数据视图。 |
| `options?` | [`IGanttSheetOptions`](../modules/GC.Spread.Sheets.GanttSheet.md#iganttsheetoptions) | - |

#### Returns

`void`

___

### <a id="cancelchanges" name="cancelchanges"></a> cancelChanges

▸ **cancelChanges**(): `void`

取消批处理模式下数据管理器的更改。

**`example`**
```
//此示例在批处理模式下手动取消更改。
tableSheet.cancelChanges();
```

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[cancelChanges](GC.Spread.Sheets.TableSheet.TableSheet.md#cancelchanges)

___

### <a id="collapseallhierarchylevels" name="collapseallhierarchylevels"></a> collapseAllHierarchyLevels

▸ **collapseAllHierarchyLevels**(): `void`

折叠所有层级。

**`example`**
```
//此示例折叠所有层级。
tableSheet.collapseAllHierarchyLevels();
```

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[collapseAllHierarchyLevels](GC.Spread.Sheets.TableSheet.TableSheet.md#collapseallhierarchylevels)

___

### <a id="demotehierarchylevel" name="demotehierarchylevel"></a> demoteHierarchyLevel

▸ **demoteHierarchyLevel**(`row`, `withChildren?`): `void`

降低指定行的层级数据级别。

**`example`**
```
//此示例通过指定索引降低层级数据级别。
tableSheet.demoteHierarchyLevel(8);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |
| `withChildren?` | `boolean` | 可选，默认情况下子项将随记录一起降级。 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[demoteHierarchyLevel](GC.Spread.Sheets.TableSheet.TableSheet.md#demotehierarchylevel)

___

### <a id="detailcolumnsvisible" name="detailcolumnsvisible"></a> detailColumnsVisible

▸ **detailColumnsVisible**(`value?`): `boolean`

在表格分组后是否显示或隐藏明细列。

**`example`**
```
//此示例展示如何隐藏明细列。
tableSheet.detailColumnsVisible(false);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `boolean` | 一个布尔值，表示明细列的可见性。 |

#### Returns

`boolean`

返回明细列的可见性。

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[detailColumnsVisible](GC.Spread.Sheets.TableSheet.TableSheet.md#detailcolumnsvisible)

___

### <a id="expandallhierarchylevels" name="expandallhierarchylevels"></a> expandAllHierarchyLevels

▸ **expandAllHierarchyLevels**(): `void`

展开所有层级。

**`example`**
```
//此示例展开所有层级。
tableSheet.expandAllHierarchyLevels();
```

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[expandAllHierarchyLevels](GC.Spread.Sheets.TableSheet.TableSheet.md#expandallhierarchylevels)

___

### <a id="expandgroup" name="expandgroup"></a> expandGroup

▸ **expandGroup**(`field`, `expand`): `void`

通过指定字段展开或折叠一级分组。

**`example`**
```
//此示例展示如何折叠按"LastName"分组的一级分组。
tableSheet.expandGroup("LastName", false);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `field` | `string` | 字段名称。 |
| `expand` | `boolean` | 一个布尔值，true表示展开分组，false表示折叠分组。 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[expandGroup](GC.Spread.Sheets.TableSheet.TableSheet.md#expandgroup)

___

### <a id="expandgroupitem" name="expandgroupitem"></a> expandGroupItem

▸ **expandGroupItem**(`level`, `index`, `expand`): `void`

通过指定级别和索引展开或折叠一个分组。

**`example`**
```
//此示例展示如何折叠一个分组，其级别为1且起始索引为10。
tableSheet.expandGroupItem(1, 10, false);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `level` | `number` | 分组级别。 |
| `index` | `number` | 分组起始索引。 |
| `expand` | `boolean` | 一个布尔值，true表示展开分组，false表示折叠分组。 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[expandGroupItem](GC.Spread.Sheets.TableSheet.TableSheet.md#expandgroupitem)

___

### <a id="expandhierarchylevel" name="expandhierarchylevel"></a> expandHierarchyLevel

▸ **expandHierarchyLevel**(`level`): `void`

展开指定级别的层级数据。

**`example`**
```
//此示例展开指定级别的层级数据。
tableSheet.expandHierarchyLevel(8);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `level` | `number` | 要展开的级别。 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[expandHierarchyLevel](GC.Spread.Sheets.TableSheet.TableSheet.md#expandhierarchylevel)

___

### <a id="getactivetask" name="getactivetask"></a> getActiveTask

▸ **getActiveTask**(): [`Task`](GC.Spread.Sheets.GanttSheet.Task.md)

获取活动行中的任务。

#### Returns

[`Task`](GC.Spread.Sheets.GanttSheet.Task.md)

活动行中的任务。

___

### <a id="getchanges" name="getchanges"></a> getChanges

▸ **getChanges**(): [`IDataViewChanges`](../interfaces/GC.Spread.Sheets.TableSheet.IDataViewChanges.md)[]

获取自动同步或批处理模式下数据管理器的更改。

**`example`**
```
//此示例在自动同步或批处理模式下手动获取更改，包括更新的行、插入的行、删除的行、添加列、更新列、删除列。
tableSheet.getChanges();
```

#### Returns

[`IDataViewChanges`](../interfaces/GC.Spread.Sheets.TableSheet.IDataViewChanges.md)[]

返回一个对象数组，每个对象可能包含"type"、"dataItem"、"oldDataItem"、"column"、"originalColumn"和"index"。
"type"是更改类型，可以是"insert"、"update"、"delete"、"addColumn"、"updateColumn"、"removeColumn"之一。
"dataItem"是当前行数据。
"oldDataItem"是原始行数据，仅用于"update"。
"column"是当前列。
"data"是当前添加列的默认值。
"originalColumn"是原始列，仅用于"update column"。
"index"是表格的视图索引。

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[getChanges](GC.Spread.Sheets.TableSheet.TableSheet.md#getchanges)

___

### <a id="getdataview" name="getdataview"></a> getDataView

▸ **getDataView**(): [`View`](GC.Data.View.md)

获取表格的数据视图。

**`example`**
```
//此示例获取数据源。
tableSheet.getDataView();
```

#### Returns

[`View`](GC.Data.View.md)

返回数据视图。

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[getDataView](GC.Spread.Sheets.TableSheet.TableSheet.md#getdataview)

___

### <a id="getselections" name="getselections"></a> getSelections

▸ **getSelections**(): [`Range`](GC.Spread.Sheets.Range.md)[]

获取选中的范围。

#### Returns

[`Range`](GC.Spread.Sheets.Range.md)[]

选中的范围。

___

### <a id="gettaskbyrow" name="gettaskbyrow"></a> getTaskByRow

▸ **getTaskByRow**(`rowIndex`): [`Task`](GC.Spread.Sheets.GanttSheet.Task.md)

获取指定行中的任务。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rowIndex` | `number` | 表示行索引的数字。 |

#### Returns

[`Task`](GC.Spread.Sheets.GanttSheet.Task.md)

指定行中的任务。

___

### <a id="groupby" name="groupby"></a> groupBy

▸ **groupBy**(`options?`): [`IGroupByOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IGroupByOptions.md)[]

根据选项对表格进行分组。

**`example`**
```
//此示例设置分组选项并对表格进行分组。
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
| `options?` | [`IGroupByOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IGroupByOptions.md)[] | 分组选项。 |

#### Returns

[`IGroupByOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IGroupByOptions.md)[]

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[groupBy](GC.Spread.Sheets.TableSheet.TableSheet.md#groupby)

___

### <a id="groupoutlineposition" name="groupoutlineposition"></a> groupOutlinePosition

▸ **groupOutlinePosition**(`value?`): `boolean`

在表格分组后，是否在视口区域、列标题区域或行标题区域显示或隐藏分组轮廓。

**`example`**
```
//此示例展示如何隐藏分组轮廓。
tableSheet.groupOutlinePosition(GC.Spread.Sheets.TableSheet.GroupOutlinePosition.none);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`GroupOutlinePosition`](../enums/GC.Spread.Sheets.TableSheet.GroupOutlinePosition.md) | 表示分组轮廓位置的值。 |

#### Returns

`boolean`

返回分组轮廓的位置。

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[groupOutlinePosition](GC.Spread.Sheets.TableSheet.TableSheet.md#groupoutlineposition)

___

### <a id="hasrowstate" name="hasrowstate"></a> hasRowState

▸ **hasRowState**(`type`, `row`): `boolean`

判断指定行是否具有指定状态。

**`example`**
```
//此示例判断指定行是否具有指定状态。
tableSheet.hasRowState(GC.Data.RowColumnStates.selected, 0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | [`RowColumnStates`](../enums/GC.Data.RowColumnStates.md) | 行状态类型。 |
| `row` | `number` | 行索引。 |

#### Returns

`boolean`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[hasRowState](GC.Spread.Sheets.TableSheet.TableSheet.md#hasrowstate)

___

### <a id="movedown" name="movedown"></a> moveDown

▸ **moveDown**(`row`): `void`

将指定行的层级数据向下移动。

**`example`**
```
//此示例将指定索引的层级数据向下移动。
tableSheet.moveDown(8);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[moveDown](GC.Spread.Sheets.TableSheet.TableSheet.md#movedown)

___

### <a id="moveup" name="moveup"></a> moveUp

▸ **moveUp**(`row`): `void`

将指定行的层级数据向上移动。

**`example`**
```
//此示例将指定索引的层级数据向上移动。
tableSheet.moveUp(8);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[moveUp](GC.Spread.Sheets.TableSheet.TableSheet.md#moveup)

___

### <a id="printinfo" name="printinfo"></a> printInfo

▸ **printInfo**(`value?`): `any`

获取或设置表格的打印信息。

**`example`**
```
//此示例设置打印信息。
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

如果未设置值，则返回表格的打印信息；否则返回表格。

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[printInfo](GC.Spread.Sheets.TableSheet.TableSheet.md#printinfo)

___

### <a id="promotehierarchylevel" name="promotehierarchylevel"></a> promoteHierarchyLevel

▸ **promoteHierarchyLevel**(`row`): `void`

提升指定行的层级数据级别。

**`example`**
```
//此示例通过指定索引提升层级数据级别。
tableSheet.promoteHierarchyLevel(8);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[promoteHierarchyLevel](GC.Spread.Sheets.TableSheet.TableSheet.md#promotehierarchylevel)

___

### <a id="removegroupby" name="removegroupby"></a> removeGroupBy

▸ **removeGroupBy**(): `void`

移除表格的分组状态。

**`example`**
```
//此示例展示如何移除表格的分组状态。
tablesheet.removeGroupBy()
```

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[removeGroupBy](GC.Spread.Sheets.TableSheet.TableSheet.md#removegroupby)

___

### <a id="removerow" name="removerow"></a> removeRow

▸ **removeRow**(`row`): `Promise`<`void`\>

从表格中移除指定行。

**`example`**
```
//此示例通过指定索引移除行。
//当autoSync为true时，更改将被同步。
tableSheet.removeRow(8);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |

#### Returns

`Promise`<`void`\>

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[removeRow](GC.Spread.Sheets.TableSheet.TableSheet.md#removerow)

___

### <a id="resetrow" name="resetrow"></a> resetRow

▸ **resetRow**(`row`): `void`

重置表格中指定行的更改。

**`example`**
```
//此示例通过指定索引重置行。
tableSheet.resetRow(8);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[resetRow](GC.Spread.Sheets.TableSheet.TableSheet.md#resetrow)

___

### <a id="resumepaint" name="resumepaint"></a> resumePaint

▸ **resumePaint**(): `void`

恢复甘特图表的绘制。

#### Returns

`void`

___

### <a id="rowactionoptions" name="rowactionoptions"></a> rowActionOptions

▸ **rowActionOptions**(`options?`): [`IRowActionOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IRowActionOptions.md)[]

获取或设置行操作的选项。

**`example`**
```
//此示例设置行操作的选项。
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
| `options?` | [`IRowActionOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IRowActionOptions.md)[] | 行操作的选项。 |

#### Returns

[`IRowActionOptions`](../interfaces/GC.Spread.Sheets.TableSheet.IRowActionOptions.md)[]

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[rowActionOptions](GC.Spread.Sheets.TableSheet.TableSheet.md#rowactionoptions)

___

### <a id="saverow" name="saverow"></a> saveRow

▸ **saveRow**(`row`): `Promise`<`void`\>

将表格中指定行的更改保存到数据管理器，包括更新的行或插入的行。

**`example`**
```
//此示例通过指定索引保存行。
//当autoSync为true时，更改将被同步。
tableSheet.saveRow(8);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引。 |

#### Returns

`Promise`<`void`\>

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[saveRow](GC.Spread.Sheets.TableSheet.TableSheet.md#saverow)

___

### <a id="setdataview" name="setdataview"></a> setDataView

▸ **setDataView**(`dataView`): `void`

设置表格的数据视图。

**`example`**
```
//此示例设置数据源。
var dataManager = spread.dataManager();
var myTable = dataManager.addTable("myTable", {
    remote: {
        read: {
            url: 'https://demodata.mescius.io/northwind/api/v1/Orders'
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
| `dataView` | [`View`](GC.Data.View.md) | 要绑定的数据视图。 |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[setDataView](GC.Spread.Sheets.TableSheet.TableSheet.md#setdataview)

___

### <a id="setdefaultrowheight" name="setdefaultrowheight"></a> setDefaultRowHeight

▸ **setDefaultRowHeight**(`value`, `sheetArea?`): `void`

设置视口区域中所有行的默认高度（以像素为单位）。

**`example`**
```
//此示例设置默认行高（以像素为单位）。
tableSheet.setDefaultRowHeight(50);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value` | `number` | 高度（以像素为单位）。 |
| `sheetArea?` | [`SheetArea`](../enums/GC.Spread.Sheets.SheetArea.md) | - |

#### Returns

`void`

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[setDefaultRowHeight](GC.Spread.Sheets.TableSheet.TableSheet.md#setdefaultrowheight)

___

### <a id="submitchanges" name="submitchanges"></a> submitChanges

▸ **submitChanges**(): `Promise`<`void`\>

以批处理模式将数据管理器的更改提交到服务器，包括更新的行、插入的行和删除的行。

**`example`**
```
//此示例以批处理模式手动提交更改。
tableSheet.submitChanges();
```

#### Returns

`Promise`<`void`\>

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[submitChanges](GC.Spread.Sheets.TableSheet.TableSheet.md#submitchanges)

___

### <a id="suspendpaint" name="suspendpaint"></a> suspendPaint

▸ **suspendPaint**(): `void`

暂停甘特图表的绘制。

#### Returns

`void`

___

### <a id="togglepinnedcolumns" name="togglepinnedcolumns"></a> togglePinnedColumns

▸ **togglePinnedColumns**(`index`): `void`

固定或取消固定指定列索引数组的列。

**`example`**
```
//此示例固定多个列。
tableSheet.togglePinnedColumns([1,2,4]);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number`[] | 要固定或取消固定的列索引数组。 |

#### Returns

`void`

返回固定列的数量。

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[togglePinnedColumns](GC.Spread.Sheets.TableSheet.TableSheet.md#togglepinnedcolumns)

___

### <a id="togglepinnedrows" name="togglepinnedrows"></a> togglePinnedRows

▸ **togglePinnedRows**(`indexes`): `void`

固定或取消固定指定行索引数组的行。

**`example`**
```
//此示例固定多个行。
tableSheet.togglePinnedRows([1,2,4]);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `indexes` | `number`[] |

#### Returns

`void`

返回固定行的数量。

#### Inherited from

[TableSheet](GC.Spread.Sheets.TableSheet.TableSheet.md).[togglePinnedRows](GC.Spread.Sheets.TableSheet.TableSheet.md#togglepinnedrows)
