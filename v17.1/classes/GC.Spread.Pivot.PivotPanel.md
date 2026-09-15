# Class: PivotPanel

[Spread](../modules/GC.Spread.md).[Pivot](../modules/GC.Spread.Pivot.md).PivotPanel

## Table of contents

### Constructors

- [constructor](GC.Spread.Pivot.PivotPanel.md#constructor)

### Methods

- [attach](GC.Spread.Pivot.PivotPanel.md#attach)
- [destroy](GC.Spread.Pivot.PivotPanel.md#destroy)
- [detach](GC.Spread.Pivot.PivotPanel.md#detach)
- [panelLayout](GC.Spread.Pivot.PivotPanel.md#panellayout)
- [sectionVisibility](GC.Spread.Pivot.PivotPanel.md#sectionvisibility)
- [findControl](GC.Spread.Pivot.PivotPanel.md#findcontrol)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new PivotPanel**(`name`, `pivotTable`, `host`)

数据透视表的透视面板

**`代码示例`**
```
//本示例创建了一个透视面板
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                  ["01-Jan","Mom","Fuel",74],
                  ["15-Jan","Mom","Food",235],
                  ["17-Jan","Dad","Sports",20],
                  ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.suspendLayout();
pivotTable.options.showRowHeader =true;
pivotTable.options.showColumnHeader =true;
pivotTable.add("Buyer", "Buyer", GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("Type", "Type", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("Amount", "Sum of Amount",   GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
var panel = new GC.Spread.Pivot.PivotPanel("myPivotPanel", pivotTable, document.getElementById("panel"));
pivotTable.resumeLayout();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 透视面板名称 |
| `pivotTable` | [`PivotTable`](GC.Spread.Pivot.PivotTable-1.md) | 与透视面板相关的透视表 |
| `host` | `HTMLDivElement` | 透视面板的容器html元素 |

## Methods

### <a id="attach" name="attach"></a> attach

▸ **attach**(`pivotTable`): `any`

**`description`** 添加到透视面板的透视表，则透视面板可以控制绑定的透视表

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pivotTable` | [`PivotTable`](GC.Spread.Pivot.PivotTable-1.md) | 添加的数据透视表 |

#### Returns

`any`

void

___

### <a id="destroy" name="destroy"></a> destroy

▸ **destroy**(): `any`

**`description`** 销毁数据透视面板

#### Returns

`any`

___

### <a id="detach" name="detach"></a> detach

▸ **detach**(): `void`

**`description`** 分离透视面板的透视表，停止透视面板控件绑定的透视表

#### Returns

`void`

void

___

### <a id="panellayout" name="panellayout"></a> panelLayout

▸ **panelLayout**(`value?`): `void` \| [`PivotPanelLayoutType`](../enums/GC.Spread.Pivot.PivotPanelLayoutType.md)

**`description`** 设置或获取panelLayout类型

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | [`PivotPanelLayoutType`](../enums/GC.Spread.Pivot.PivotPanelLayoutType.md) |

#### Returns

`void` \| [`PivotPanelLayoutType`](../enums/GC.Spread.Pivot.PivotPanelLayoutType.md)

GC.Spread.Pivot.PivotPanelLayoutType | void

___

### <a id="sectionvisibility" name="sectionvisibility"></a> sectionVisibility

▸ **sectionVisibility**(`value?`): `number` \| `void`

**`description`** 获取或设置哪些部分可见

**`代码示例`**
```
 var visibility = pivotPanel.sectionVisibility() // 7;
 visibility = visibility & ~GC.Spread.Pivot.PivotPanelSection.viewList; // 3
 pivotPanel.sectionVisibility(visibility);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`number` \| `void`

可见值

___

### <a id="findcontrol" name="findcontrol"></a> findControl

▸ `Static` **findControl**(`host`): [`PivotPanel`](GC.Spread.Pivot.PivotPanel.md)

通过宿主元素获取数据透视面板实例

**`代码示例`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["Date","Buyer","Type","Amount"],
                 ["01-Jan","Mom","Fuel",74],
                 ["15-Jan","Mom","Food",235],
                 ["17-Jan","Dad","Sports",20],
                 ["21-Jan","Kelly","Books",125]];
sourceSheet.setArray(0, 0, sourceData);
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
var pivotTable = sheet.pivotTables.get("pivotTable_1");
var panel = new GC.Spread.Pivot.PivotPanel("sourceData", pivotTable, document.getElementById("pivotPanel"));
var pivotPanel = GC.Spread.Pivot.PivotPanel.findControl("pivotPanel");
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `host` | `string` \| `HTMLElement` | 宿主元素或宿主元素id |

#### Returns

[`PivotPanel`](GC.Spread.Pivot.PivotPanel.md)

PivotPanel实例
