# Class: RowFilterBase

[Sheets](../modules/GC.Spread.Sheets.md).[Filter](../modules/GC.Spread.Sheets.Filter.md).RowFilterBase

## Hierarchy

- **`RowFilterBase`**

  ↳ [`HideRowFilter`](GC.Spread.Sheets.Filter.HideRowFilter.md)

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Filter.RowFilterBase.md#constructor)

### Properties

- [extendedRange](GC.Spread.Sheets.Filter.RowFilterBase.md#extendedrange)
- [range](GC.Spread.Sheets.Filter.RowFilterBase.md#range)
- [typeName](GC.Spread.Sheets.Filter.RowFilterBase.md#typename)

### Methods

- [addFilterItem](GC.Spread.Sheets.Filter.RowFilterBase.md#addfilteritem)
- [filter](GC.Spread.Sheets.Filter.RowFilterBase.md#filter)
- [filterButtonVisible](GC.Spread.Sheets.Filter.RowFilterBase.md#filterbuttonvisible)
- [fromJSON](GC.Spread.Sheets.Filter.RowFilterBase.md#fromjson)
- [getFilterItems](GC.Spread.Sheets.Filter.RowFilterBase.md#getfilteritems)
- [getFilteredItems](GC.Spread.Sheets.Filter.RowFilterBase.md#getfiltereditems)
- [getSortState](GC.Spread.Sheets.Filter.RowFilterBase.md#getsortstate)
- [isFiltered](GC.Spread.Sheets.Filter.RowFilterBase.md#isfiltered)
- [isRowFilteredOut](GC.Spread.Sheets.Filter.RowFilterBase.md#isrowfilteredout)
- [onFilter](GC.Spread.Sheets.Filter.RowFilterBase.md#onfilter)
- [openFilterDialog](GC.Spread.Sheets.Filter.RowFilterBase.md#openfilterdialog)
- [removeFilterItems](GC.Spread.Sheets.Filter.RowFilterBase.md#removefilteritems)
- [reset](GC.Spread.Sheets.Filter.RowFilterBase.md#reset)
- [sortColumn](GC.Spread.Sheets.Filter.RowFilterBase.md#sortcolumn)
- [toJSON](GC.Spread.Sheets.Filter.RowFilterBase.md#tojson)
- [unfilter](GC.Spread.Sheets.Filter.RowFilterBase.md#unfilter)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new RowFilterBase**(`range?`)

一个行筛选基础，它支持用于筛选表单中行的行筛选

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](GC.Spread.Sheets.Range.md) | 筛选区域 |

## Properties

### <a id="extendedrange" name="extendedrange"></a> extendedRange

• **extendedRange**: [`Range`](GC.Spread.Sheets.Range.md)

行筛选的extendedRange

___

### <a id="range" name="range"></a> range

• **range**: [`Range`](GC.Spread.Sheets.Range.md)

行筛选的区域

___

### <a id="typename" name="typename"></a> typeName

• **typeName**: `string`

支持序列化的类型名称字符串

## Methods

### <a id="addfilteritem" name="addfilteritem"></a> addFilterItem

▸ **addFilterItem**(`col`, `condition`): `void`

将指定的筛选添加到行筛选

**`example`**
```
sheet.setRowCount(3);
sheet.setColumnCount(1);
sheet.setArray(0, 0,
    [
        [ 1 ],
        [ 2 ],
        [ 3 ]
    ]);
sheet.rowFilter(new GC.Spread.Sheets.Filter.HideRowFilter(new GC.Spread.Sheets.Range(-1, -1, -1, -1)));
var condition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.textCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.TextCompareType.equalsTo,expected: '3'});
sheet.rowFilter().addFilterItem(0, condition);
sheet.rowFilter().filter(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `col` | `number` | 列索引 |
| `condition` | [`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md) | 要筛选的条件 |

#### Returns

`void`

___

### <a id="filter" name="filter"></a> filter

▸ **filter**(`col?`): `void`

筛选指定的列

**`example`**
```
sheet.setRowCount(2);
sheet.setColumnCount(1);
sheet.setArray(0, 0,
    [
        [ "a" ],
        [ "b" ]
    ]);
sheet.rowFilter(new GC.Spread.Sheets.Filter.HideRowFilter(new GC.Spread.Sheets.Range(-1, -1, -1, -1)));
var condition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.textCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.TextCompareType.equalsTo,expected: 'a'});
var rowFilter = sheet.rowFilter();
rowFilter.addFilterItem(0, condition);
rowFilter.filter(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `col?` | `number` | 要筛选的列的索引；如果省略，则将筛选区域内的所有列 |

#### Returns

`void`

___

### <a id="filterbuttonvisible" name="filterbuttonvisible"></a> filterButtonVisible

▸ **filterButtonVisible**(`col?`, `value?`): `any`

获取或设置是否显示表单列的筛选按钮

**`example`**
```
sheet.setArray(2, 2,
    [
        [ 1, 4 ],
        [ 2, 5 ],
        [ 3, 6 ]
    ] );
sheet.rowFilter(new GC.Spread.Sheets.Filter.HideRowFilter(new GC.Spread.Sheets.Range(2, 2, 3, 2)));
console.log(sheet.rowFilter().filterButtonVisible()); // true
sheet.rowFilter().filterButtonVisible(2, false);
console.log(sheet.rowFilter().filterButtonVisible(2)); // false
console.log(sheet.rowFilter().filterButtonVisible(3)); // true
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `col?` | `number` | 筛选按钮的列索引 |
| `value?` | `boolean` | 是否显示筛选按钮 |

#### Returns

`any`

     没有参数时，如果所有筛选按钮都不可见，返回false,否则返回true
     有一个参数 col 时，如果指定的列筛选按钮不可见，返回false,否则返回true
     一个参数值` GC.Spread.Sheets.Filter.RowFilterBase `将所有筛选按钮设置为可见(true)/ 不可见(false)
     两个参数col,value ` GC.Spread.Sheets.Filter.RowFilterBase `将指定的列筛选按钮设置为可见(true)/ 不可见(false)

___

### <a id="fromjson" name="fromjson"></a> fromJSON

▸ **fromJSON**(`settings`): `void`

从指定的JSON字符串加载对象状态

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `settings` | `Object` | 设置反序列化的行筛选数据 |

#### Returns

`void`

___

### <a id="getfilteritems" name="getfilteritems"></a> getFilterItems

▸ **getFilterItems**(`col`): [`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)[]

获取指定列的筛选

**`example`**
```
sheet.getCell(0, 0).value("a");
sheet.getCell(0, 1).value("b");
sheet.getCell(1, 0).value("ac");
sheet.getCell(1, 1).value("bd");
sheet.rowFilter( new GC.Spread.Sheets.Filter.HideRowFilter(new GC.Spread.Sheets.Range( -1, -1, -1, -1)));
var condition1 =  new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.textCondition, { compareType: GC.Spread.Sheets.ConditionalFormatting.TextCompareType.equalsTo,expected: 'a' });
var condition2 = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.textCondition, { compareType: GC.Spread.Sheets.ConditionalFormatting.TextCompareType.equalsTo,beginsWith: '' });
sheet.rowFilter().addFilterItem(0, condition1);
sheet.rowFilter().addFilterItem(1, condition2);
console.log(sheet.rowFilter().getFilterItems(0)); // result is array, length is 1, and the item equals to condition1.
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `col` | `number` | 列索引 |

#### Returns

[`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)[]

返回包含属于指定列的条件的集合

___

### <a id="getfiltereditems" name="getfiltereditems"></a> getFilteredItems

▸ **getFilteredItems**(): [`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)[]

获取所有筛选条件

**`example`**
```
sheet.setRowCount(3);
sheet.setColumnCount(2);
sheet.setArray(0, 0,
    [
        [ 1, 2 ],
        [ 3, 4 ],
        [ 5, 6 ]
    ]);
sheet.rowFilter(new GC.Spread.Sheets.Filter.HideRowFilter(new GC.Spread.Sheets.Range(-1, -1, -1, -1)));
var condition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.numberCondition, { compareType: GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.greaterThan, expected: 1 });
var condition1 = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.numberCondition, { compareType: GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.greaterThan, expected: 4 });
sheet.rowFilter().addFilterItem(0, condition);
sheet.rowFilter().addFilterItem(1, condition1);
console.log(sheet.rowFilter().getFilteredItems().length); // 0
sheet.rowFilter().filter();
console.log(sheet.rowFilter().getFilteredItems().length); // 2
sheet.rowFilter().removeFilterItems(0);
console.log(sheet.rowFilter().getFilteredItems().length); // 1
sheet.rowFilter().removeFilterItems(1);
console.log(sheet.rowFilter().getFilteredItems().length); // 0
```

#### Returns

[`Condition`](GC.Spread.Sheets.ConditionalFormatting.Condition.md)[]

返回包含所有筛选条件的集合

___

### <a id="getsortstate" name="getsortstate"></a> getSortState

▸ **getSortState**(`col`): [`SortState`](../enums/GC.Spread.Sheets.SortState.md)

获取当前的排序状态

**`example`**
```
sheet.setArray(0, 0, [
    [ 4 ],
    [ 3 ],
    [ 2 ],
    [ 1 ],
    [ 0 ]
]);
sheet.rowFilter( new GC.Spread.Sheets.Filter.HideRowFilter( new GC.Spread.Sheets.Range( 0, 0, 5, 1 ) ) );
sheet.rowFilter().addFilterItem( 0, new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.numberCondition, { compareType: GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.greaterThan, expected: 2 }));
sheet.rowFilter().filter(0);
sheet.rowFilter().sortColumn(0, false);
console.log(sheet.rowFilter().getSortState(0)); // 2
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `col` | `number` | 列索引 |

#### Returns

[`SortState`](../enums/GC.Spread.Sheets.SortState.md)

当前筛选的排序状态

___

### <a id="isfiltered" name="isfiltered"></a> isFiltered

▸ **isFiltered**(`col?`): `boolean`

获取一个值，该值是否筛选任何行或指定的列

**`代码示例`**
```
//本示例使用isFiltered方法
activeSheet.setValue(0, 0, "North");
activeSheet.setValue(1, 0, "South");
activeSheet.setValue(2, 0, "East");
activeSheet.setValue(3, 0, "South");
activeSheet.setValue(4, 0, "North");
activeSheet.setValue(5, 0, "North");
activeSheet.setValue(6, 0, "West");
activeSheet.setColumnWidth(0, 80);
//设置一个行筛选
activeSheet.rowFilter(new GC.Spread.Sheets.Filter.HideRowFilter(new GC.Spread.Sheets.Range(0, 0, 7, 1)));
//button
$("#button1").click(function () {
    var rowFilter = spread.getActiveSheet().rowFilter();
    if (rowFilter.isFiltered(0)) {
        alert("Row-filtering executed for Column1");
    } else {
        alert("Row-filtering not executed for Column1");
    }
});
//Add button control to page
<input type="button" id="button1" value="button1"/>
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `col?` | `number` | 列索引 |

#### Returns

`boolean`

不传参时，如果某些行被筛选，返回true;否则返回false.
                    传一个col参数时，如果指定的列已筛选，返回true;否则为false

___

### <a id="isrowfilteredout" name="isrowfilteredout"></a> isRowFilteredOut

▸ **isRowFilteredOut**(`row`): `boolean`

确定是否将指定的行筛选掉

**`example`**
```
sheet.setRowCount(2);
sheet.setColumnCount(1);
sheet.setArray(0, 0,
    [
        [ 1 ],
        [ 2 ]
    ] );
sheet.rowFilter(new GC.Spread.Sheets.Filter.HideRowFilter(new GC.Spread.Sheets.Range(-1, -1, -1, -1)));
var condition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.textCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.TextCompareType.equalsTo,expected: '2'});
sheet.rowFilter().addFilterItem(0, condition);
sheet.rowFilter().filter(0);
sheet.addRows(1, 1);
console.log(sheet.rowFilter().isFiltered()); // true
console.log(sheet.rowFilter().isRowFilteredOut(0)); // true
console.log(sheet.rowFilter().isRowFilteredOut(1)); // false
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | `number` | 行索引 |

#### Returns

`boolean`

如果该行被筛选，返回true;否则返回false

___

### <a id="onfilter" name="onfilter"></a> onFilter

▸ **onFilter**(`args`): `void`

当某些列被筛选或未筛选时执行操作

**`example`**
```
sheet.setRowCount(3);
sheet.setColumnCount(2);
sheet.setArray(0, 0,
    [
        [ 1, 2 ],
        [ 3, 4 ],
        [ 5, 6 ]
    ]);
function HighLightFilter(range) {
    GC.Spread.Sheets.Filter.RowFilterBase.call(this, range);
}
HighLightFilter.prototype = new  GC.Spread.Sheets.Filter.RowFilterBase(new GC.Spread.Sheets.Range(-1, -1, -1, -1));
var doFilterCalled = false;
HighLightFilter.prototype.onFilter = function(args) {
    if ( args.action ===  GC.Spread.Sheets.Filter.FilterActionType.filter ) {
        doFilterCalled = true;
    }
};
sheet.rowFilter(new HighLightFilter(new GC.Spread.Sheets.Range(-1, -1, -1, -1)));
var condition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.numberCondition, { compareType: GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.greaterThan, expected: 1 });
sheet.rowFilter().addFilterItem(0, condition);
sheet.rowFilter().filter();
console.log(doFilterCalled); // true
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `args` | [`IFilteredArgs`](../interfaces/GC.Spread.Sheets.Filter.IFilteredArgs.md) | 包含action、sheet、range、filteredRows和filteredOutRows的对象 |

#### Returns

`void`

___

### <a id="openfilterdialog" name="openfilterdialog"></a> openFilterDialog

▸ **openFilterDialog**(`filterButtonHitInfo`): `void`

当用户单击筛选按钮时，打开筛选对话框

**`example`**
```
sheet.setRowCount(3);
sheet.setColumnCount(2);
sheet.setArray(0, 0,
    [
        [ 1, 2 ],
        [ 3, 4 ],
        [ 5, 6 ]
    ]);
function HighLightFilter(range) {
    GC.Spread.Sheets.Filter.RowFilterBase.call(this, range);
}
HighLightFilter.prototype = new  GC.Spread.Sheets.Filter.RowFilterBase(new GC.Spread.Sheets.Range(-1, -1, -1, -1));
HighLightFilter.prototype.openFilterDialog = function(args) {
    console.log(args.row, args.col);
};
sheet.rowFilter(new HighLightFilter(new GC.Spread.Sheets.Range(-1, -1, -1, -1)));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `filterButtonHitInfo` | [`IFilterButtonHitInfo`](../interfaces/GC.Spread.Sheets.IFilterButtonHitInfo.md) | 有关筛选按钮的点击测试信息 |

#### Returns

`void`

___

### <a id="removefilteritems" name="removefilteritems"></a> removeFilterItems

▸ **removeFilterItems**(`col`): `void`

删除指定的筛选

**`example`**
```
sheet.setRowCount(3);
sheet.setColumnCount(1);
sheet.setArray(0, 0,
    [
        [ 1 ],
        [ 2 ],
        [ 3 ]
    ]);
sheet.rowFilter(new GC.Spread.Sheets.Filter.HideRowFilter(new GC.Spread.Sheets.Range( -1, -1, -1, -1)));
var condition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.textCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.TextCompareType.equalsTo, expected: '3'});
var rowFilter = sheet.rowFilter();
rowFilter.addFilterItem(0, condition);
rowFilter.removeFilterItems(0);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `col` | `number` | 列索引 |

#### Returns

`void`

___

### <a id="reset" name="reset"></a> reset

▸ **reset**(): `void`

清除所有筛选

**`example`**
```
sheet.rowFilter(new GC.Spread.Sheets.Filter.HideRowFilter(new GC.Spread.Sheets.Range(-1, -1, -1, -1)));
sheet.rowFilter().reset();
console.log(sheet.rowFilter().isFiltered()); // false
```

#### Returns

`void`

___

### <a id="sortcolumn" name="sortcolumn"></a> sortColumn

▸ **sortColumn**(`col`, `ascending`): `void`

按指定顺序对指定列进行排序

**`example`**
```
sheet.setArray(0, 0, [
    [ 4 ],
    [ 3 ],
    [ 2 ],
    [ 1 ],
    [ 0 ]
]);
sheet.rowFilter(new GC.Spread.Sheets.Filter.HideRowFilter(new GC.Spread.Sheets.Range(0, 0, 5, 1)));
sheet.rowFilter().addFilterItem(0, new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.numberCondition, { compareType: GC.Spread.Sheets.ConditionalFormatting.GeneralComparisonOperators.greaterThan, expected: 2 }));
sheet.rowFilter().filter(0);
sheet.rowFilter().sortColumn(0, true);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `col` | `number` | 列索引 |
| `ascending` | `boolean` | 排序时设置为true为升序 |

#### Returns

`void`

___

### <a id="tojson" name="tojson"></a> toJSON

▸ **toJSON**(): `Object`

将对象状态保存为JSON字符串

#### Returns

`Object`

行筛选数据

___

### <a id="unfilter" name="unfilter"></a> unfilter

▸ **unfilter**(`col?`): `void`

从指定的列中删除筛选

**`example`**
```
sheet.setRowCount(2);
sheet.setColumnCount(1);
sheet.setArray(0, 0,
    [
        [ "a" ],
        [ "b" ]
    ]);
sheet.rowFilter(new GC.Spread.Sheets.Filter.HideRowFilter(new GC.Spread.Sheets.Range(-1, -1, -1, -1)));
var condition = new GC.Spread.Sheets.ConditionalFormatting.Condition(GC.Spread.Sheets.ConditionalFormatting.ConditionType.textCondition, {compareType: GC.Spread.Sheets.ConditionalFormatting.TextCompareType.equalsTo,expected: 'a'});
var rowFilter = sheet.rowFilter();
rowFilter.addFilterItem(0, condition);
rowFilter.unfilter();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `col?` | `number` | 要删除筛选的列的索引；如果省略，则删除该区域内所有列筛选 |

#### Returns

`void`
