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

表示数据透视表的面板。

**`example`**
```javascript
// 此示例创建一个数据透视面板。
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"),{sheetCount:3});
var sourceSheet = spread.getSheet(0);
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                  ["01-一月","妈妈","燃油",74],
                  ["15-一月","妈妈","食品",235],
                  ["17-一月","爸爸","运动",20],
                  ["21-一月","凯莉","书籍",125]];
sourceSheet.setArray(0, 0, sourceData );
sourceSheet.tables.add('sourceData', 0, 0, 5, 4);
var layout = GC.Spread.Pivot.PivotTableLayoutType.compact;
var theme = GC.Spread.Pivot.PivotTableThemes.medium2;
var options = {showRowHeader: true, showColumnHeader: true};
var pivotTable = sheet.pivotTables.add("pivotTable_1", 'sourceData', 1, 1, layout, theme, options);
pivotTable.suspendLayout();
pivotTable.options.showRowHeader = true;
pivotTable.options.showColumnHeader = true;
pivotTable.add("购买者", "购买者", GC.Spread.Pivot.PivotTableFieldType.columnField);
pivotTable.add("类型", "类型", GC.Spread.Pivot.PivotTableFieldType.rowField);
pivotTable.add("金额", "金额汇总", GC.Spread.Pivot.PivotTableFieldType.valueField, GC.Pivot.SubtotalType.sum);
var panel = new GC.Spread.Pivot.PivotPanel("myPivotPanel", pivotTable, document.getElementById("panel"));
pivotTable.resumeLayout();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 数据透视面板的名称。 |
| `pivotTable` | [`PivotTable`](GC.Spread.Pivot.PivotTable-1.md) | 与数据透视面板关联的数据透视表。 |
| `host` | `HTMLDivElement` | 数据透视面板的容器HTML元素。 |

## Methods

### <a id="attach" name="attach"></a> attach

▸ **attach**(`pivotTable`): `void`

**`description`** 将数据透视面板附加到数据透视表，使面板可控制绑定的数据透视表。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `pivotTable` | [`PivotTable`](GC.Spread.Pivot.PivotTable-1.md) | 要附加的数据透视表。 |

#### Returns

`void`

void

___

### <a id="destroy" name="destroy"></a> destroy

▸ **destroy**(): `void`

**`description`** 销毁数据透视面板。

#### Returns

`void`

___

### <a id="detach" name="detach"></a> detach

▸ **detach**(): `void`

**`description`** 分离数据透视面板与数据透视表，停止面板对绑定数据透视表的控制。

#### Returns

`void`

void

___

### <a id="panellayout" name="panellayout"></a> panelLayout

▸ **panelLayout**(`value?`): `void` \| [`PivotPanelLayoutType`](../enums/GC.Spread.Pivot.PivotPanelLayoutType.md)

**`description`** 设置或获取面板布局类型。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | [`PivotPanelLayoutType`](../enums/GC.Spread.Pivot.PivotPanelLayoutType.md) | 将面板布局选项更改为堆叠或流式。 |

#### Returns

`void` \| [`PivotPanelLayoutType`](../enums/GC.Spread.Pivot.PivotPanelLayoutType.md)

GC.Spread.Pivot.PivotPanelLayoutType | void

___

### <a id="sectionvisibility" name="sectionvisibility"></a> sectionVisibility

▸ **sectionVisibility**(`value?`): `number` \| `void`

**`description`** 获取或设置可见的分区。

**`example`**
```javascript
 var visibility = pivotPanel.sectionVisibility() // 7;
 visibility = visibility & ~GC.Spread.Pivot.PivotPanelSection.viewList; // 3
 pivotPanel.sectionVisibility(visibility);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `value?` | `number` | 通过GC.Spread.Pivot.PivotPanelSection枚举值的和来设置可见分区。 |

#### Returns

`number` \| `void`

可见性值。

___

### <a id="findcontrol" name="findcontrol"></a> findControl

▸ `Static` **findControl**(`host`): [`PivotPanel`](GC.Spread.Pivot.PivotPanel.md)

通过宿主元素获取数据透视面板实例。

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var sourceSheet = spread.getSheet(0)
var sheet = spread.getSheet(1);
var sourceData = [["日期","购买者","类型","金额"],
                 ["01-一月","妈妈","燃油",74],
                 ["15-一月","妈妈","食品",235],
                 ["17-一月","爸爸","运动",20],
                 ["21-一月","凯莉","书籍",125]];
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
| `host` | `string` \| `HTMLElement` | 宿主元素或宿主元素的ID。 |

#### Returns

[`PivotPanel`](GC.Spread.Pivot.PivotPanel.md)

数据透视面板实例。
