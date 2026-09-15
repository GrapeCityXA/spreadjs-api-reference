# Class: GeneralSlicerData

[Spread](../modules/GC.Spread.md).[Slicers](../modules/GC.Spread.Slicers.md).GeneralSlicerData

## Hierarchy

- **`GeneralSlicerData`**

  ↳ [`TableSlicerData`](GC.Spread.Sheets.Slicers.TableSlicerData.md)

## Table of contents

### Constructors

- [constructor](GC.Spread.Slicers.GeneralSlicerData.md#constructor)

### Properties

- [columnNames](GC.Spread.Slicers.GeneralSlicerData.md#columnnames)
- [data](GC.Spread.Slicers.GeneralSlicerData.md#data)

### Methods

- [aggregateData](GC.Spread.Slicers.GeneralSlicerData.md#aggregatedata)
- [attachListener](GC.Spread.Slicers.GeneralSlicerData.md#attachlistener)
- [clearPreview](GC.Spread.Slicers.GeneralSlicerData.md#clearpreview)
- [detachListener](GC.Spread.Slicers.GeneralSlicerData.md#detachlistener)
- [doFilter](GC.Spread.Slicers.GeneralSlicerData.md#dofilter)
- [doUnfilter](GC.Spread.Slicers.GeneralSlicerData.md#dounfilter)
- [getColumnIndex](GC.Spread.Slicers.GeneralSlicerData.md#getcolumnindex)
- [getData](GC.Spread.Slicers.GeneralSlicerData.md#getdata)
- [getExclusiveData](GC.Spread.Slicers.GeneralSlicerData.md#getexclusivedata)
- [getExclusiveRowIndex](GC.Spread.Slicers.GeneralSlicerData.md#getexclusiverowindex)
- [getFilteredIndexes](GC.Spread.Slicers.GeneralSlicerData.md#getfilteredindexes)
- [getFilteredOutIndexes](GC.Spread.Slicers.GeneralSlicerData.md#getfilteredoutindexes)
- [getFilteredOutRanges](GC.Spread.Slicers.GeneralSlicerData.md#getfilteredoutranges)
- [getFilteredOutRowIndexes](GC.Spread.Slicers.GeneralSlicerData.md#getfilteredoutrowindexes)
- [getFilteredRanges](GC.Spread.Slicers.GeneralSlicerData.md#getfilteredranges)
- [getFilteredRowIndexes](GC.Spread.Slicers.GeneralSlicerData.md#getfilteredrowindexes)
- [getRowIndexes](GC.Spread.Slicers.GeneralSlicerData.md#getrowindexes)
- [inPreview](GC.Spread.Slicers.GeneralSlicerData.md#inpreview)
- [onColumnNameChanged](GC.Spread.Slicers.GeneralSlicerData.md#oncolumnnamechanged)
- [onColumnsRemoved](GC.Spread.Slicers.GeneralSlicerData.md#oncolumnsremoved)
- [onDataChanged](GC.Spread.Slicers.GeneralSlicerData.md#ondatachanged)
- [onFiltered](GC.Spread.Slicers.GeneralSlicerData.md#onfiltered)
- [onRowsAdded](GC.Spread.Slicers.GeneralSlicerData.md#onrowsadded)
- [onRowsRemoved](GC.Spread.Slicers.GeneralSlicerData.md#onrowsremoved)
- [resumeFilteredEvents](GC.Spread.Slicers.GeneralSlicerData.md#resumefilteredevents)
- [suspendFilteredEvents](GC.Spread.Slicers.GeneralSlicerData.md#suspendfilteredevents)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new GeneralSlicerData**(`data`, `columnNames`)

表示通用切片器数据。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | `any`[][] | 切片器数据；它是一个矩阵数组。 |
| `columnNames` | `string`[] | 切片器数据的列名。 |

## Properties

### <a id="columnnames" name="columnnames"></a> columnNames

• **columnNames**: `string`[]

表示通用切片器数据的列名。

___

### <a id="data" name="data"></a> data

• **data**: `any`[][]

表示通用切片器的数据源。

## Methods

### <a id="aggregatedata" name="aggregatedata"></a> aggregateData

▸ **aggregateData**(`columnName`, `aggregateType`, `range?`): `number`

按指定的列名聚合数据。

**`example`**
```
var slicerData = new GC.Spread.Slicers.GeneralSlicerData(
    [
        [
            { value: 'Bob', text: 'Bob' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1968/6/8"), text: '6/8/1968' },
            { value: 10000, text: '10 000' }
        ],
        [
            { value: 'Betty', text: 'Betty' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1972/7/3"), text: '7/3/1972' },
            { value: 8000, text: '8 000' }
        ],
        [
            { value: 'Alice', text: 'Alice' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2012/2/15"), text: '2/15/2012' },
            { value: 5500, text: '5 500' }
        ],
        [
            { value: 'Chris', text: 'Chris' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2001/9/2"), text: '9/2/2001' },
            { value: 6200, text: '6 200' }
        ],
        [
            { value: 'James', text: 'James' },
            { value: 'Phoenix', text: 'Phoenix' },
            { value: new Date("1995/11/22"), text: '11/22/1995' },
            { value: 16150, text: '16 150' }
        ]
    ], ["Name", "City", "Birthday", "Salary"]
);
console.log(slicerData.aggregateData('Salary', GC.Spread.Slicers.SlicerAggregateType.average));
console.log(slicerData.aggregateData('Salary', GC.Spread.Slicers.SlicerAggregateType.count, {min: 8000, max: 20000}));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnName` | `string` | 列名。 |
| `aggregateType` | [`SlicerAggregateType`](../enums/GC.Spread.Slicers.SlicerAggregateType.md) | 聚合类型。 |
| `range?` | [`ISlicerRangeConditional`](../interfaces/GC.Spread.Slicers.ISlicerRangeConditional.md) | 特定范围。 |

#### Returns

`number`

聚合后的数据。

___

### <a id="attachlistener" name="attachlistener"></a> attachListener

▸ **attachListener**(`listener`): `void`

附加监听器。SlicerData 将在适当的时候调用相应的接口。

**`example`**
```
//定义数据源。
var slicerData = new GC.Spread.Slicers.GeneralSlicerData(
    [
        [
            { value: 'Bob', text: 'Bob' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1968/6/8"), text: '6/8/1968' },
            { value: 10000, text: '10 000' }
        ],
        [
            { value: 'Betty', text: 'Betty' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1972/7/3"), text: '7/3/1972' },
            { value: 8000, text: '8 000' }
        ],
        [
            { value: 'Alice', text: 'Alice' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2012/2/15"), text: '2/15/2012' },
            { value: 5500, text: '5 500' }
        ],
        [
            { value: 'Chris', text: 'Chris' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2001/9/2"), text: '9/2/2001' },
            { value: 6200, text: '6 200' }
        ],
        [
            { value: 'James', text: 'James' },
            { value: 'Phoenix', text: 'Phoenix' },
            { value: new Date("1995/11/22"), text: '11/22/1995' },
            { value: 16150, text: '16 150' }
        ]
    ], ["Name", "City", "Birthday", "Salary"]
);
//定义自定义切片器。
function MySlicer(container) {
    this.container = container;
    this.slicerData = null;
    this.columnName = null;
}
MySlicer.prototype.setData = function (slicerData, columnName) {
    this.slicerData = slicerData;
    this.columnName = columnName;
    // 在此附加监听器
    this.slicerData.attachListener(this);
    this.onDataLoaded();
}
MySlicer.prototype.onDataLoaded = function () {
    //创建切片器 DOM 树。
    var columnName = this.columnName,
        exclusiveData = this.slicerData.getExclusiveData(columnName);
    $(this.container).append($('<span>' + this.columnName + ':</span>' + '<br />'));
    var domString = "";
    for (var i = 0; i < exclusiveData.length; i++) {
        domString += '<input type="checkbox" name="' + columnName + '" value="' + exclusiveData[i] + '">';
        domString += '<span>' + exclusiveData[i] + '</span>';
        domString += '<br />';
    }
    $(this.container).append($(domString));
    //为 DOM 附加事件。
    var self = this;
    $("[name='" + self.columnName + "']").change(function () {
        var slicer = self,
            exclusiveData = slicer.slicerData.getExclusiveData(slicer.columnName),
            parent = $(this).parent(),
            items = parent.children(),
            indexes = [];
        for (var i = 0, length = items.length; i < length; i++) {
            if (items[i].checked) {
                var value = items[i].value;
                if (!isNaN(parseInt(value))) {
                    value = parseInt(value);
                }
                indexes.push(exclusiveData.indexOf(value))
            }
        }
        if (indexes.length === 0) {
            slicer.slicerData.doUnfilter(slicer.columnName);
        } else {
            slicer.slicerData.doFilter(slicer.columnName, { exclusiveRowIndexes: indexes });
        }
    });
};
MySlicer.prototype.onFiltered = function () {
    //如果数据已被 Spread.Sheets 表格过滤，则同步状态。
    var slicerData = this.slicerData;
    var exclusiveIndexes = slicerData.getFilteredIndexes(this.columnName);
    $.each($("#slicerContainer").children("input"), function (i, input) {
    });
}
MySlicer.prototype.onColumnsRemoved = function (columnName) {
    if (columnName === this.columnName) {
         this.slicerData.detachListener(this);
         this.slicerData = null;
         $("#slicerContainer").remove();
    }
}

// 创建一个自定义切片器，并将此切片器添加到 “slicerContainer” div 中。
var slicer = new MySlicer($("#slicerContainer")[0]);
slicer.setData(slicerData, 'Name');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | [`ISlicerListener`](../interfaces/GC.Spread.Slicers.ISlicerListener.md) | 监听器。 |

#### Returns

`void`

___

### <a id="clearpreview" name="clearpreview"></a> clearPreview

▸ **clearPreview**(): `void`

清除预览过滤状态。
您可以通过 slicerData.inPreview() API 检查切片器是否正在预览中进行过滤。
如果您将 doFilter() 与 isPreview 标志设置为 true，（例如 slicerData.doFilter('Name', {exclusiveRowIndexes: [1]}, true);）
您可以通过 clearPreview() API 清除预览状态。
这将移除预览过滤状态。

**`example`**
```
var slicerData = new GC.Spread.Slicers.GeneralSlicerData(
    [
        [
            { value: 'Bob', text: 'Bob' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1968/6/8"), text: '6/8/1968' },
            { value: 10000, text: '10 000' }
        ],
        [
            { value: 'Betty', text: 'Betty' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1972/7/3"), text: '7/3/1972' },
            { value: 8000, text: '8 000' }
        ],
        [
            { value: 'Bob', text: 'Bob' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2012/2/15"), text: '2/15/2012' },
            { value: 8000, text: '5 500' }
        ],
    ], ["Name", "City", "Birthday", "Salary"]
);
console.log(slicerData.getFilteredOutIndexes('Name', GC.Spread.Slicers.FilteredOutDataType.all)); // []
slicerData.doFilter('Name', {exclusiveRowIndexes: [1, 2]});
console.log(slicerData.getFilteredOutIndexes('Name', GC.Spread.Slicers.FilteredOutDataType.all)); // [0]
console.log(slicerData.inPreview()); // false
slicerData.clearPreview();
console.log(slicerData.getFilteredOutIndexes('Name', GC.Spread.Slicers.FilteredOutDataType.all)); // [0]
slicerData.doUnfilter('Name');
console.log(slicerData.getFilteredOutIndexes('Name', GC.Spread.Slicers.FilteredOutDataType.all)); // []

slicerData.doFilter('Name', {exclusiveRowIndexes: [1, 2]}, true);
console.log(slicerData.getFilteredOutIndexes('Name', GC.Spread.Slicers.FilteredOutDataType.all)); // [0]
console.log(slicerData.inPreview()); // true
slicerData.clearPreview();
console.log(slicerData.inPreview()); // false
console.log(slicerData.getFilteredOutIndexes('Name', GC.Spread.Slicers.FilteredOutDataType.all)); // []
```

#### Returns

`void`

___

### <a id="detachlistener" name="detachlistener"></a> detachListener

▸ **detachListener**(`listener`): `void`

分离监听器。

**`example`**
```
//定义数据源。
var slicerData = new GC.Spread.Slicers.GeneralSlicerData(
    [
        [
            { value: 'Bob', text: 'Bob' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1968/6/8"), text: '6/8/1968' },
            { value: 10000, text: '10 000' }
        ],
        [
            { value: 'Betty', text: 'Betty' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1972/7/3"), text: '7/3/1972' },
            { value: 8000, text: '8 000' }
        ],
        [
            { value: 'Alice', text: 'Alice' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2012/2/15"), text: '2/15/2012' },
            { value: 5500, text: '5 500' }
        ],
        [
            { value: 'Chris', text: 'Chris' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2001/9/2"), text: '9/2/2001' },
            { value: 6200, text: '6 200' }
        ],
        [
            { value: 'James', text: 'James' },
            { value: 'Phoenix', text: 'Phoenix' },
            { value: new Date("1995/11/22"), text: '11/22/1995' },
            { value: 16150, text: '16 150' }
        ]
    ], ["Name", "City", "Birthday", "Salary"]
);
//定义自定义切片器。
function MySlicer(container) {
    this.container = container;
    this.slicerData = null;
    this.columnName = null;
}
MySlicer.prototype.setData = function (slicerData, columnName) {
    this.slicerData = slicerData;
    this.columnName = columnName;
    // 在此附加监听器
    this.slicerData.attachListener(this);
    this.onDataLoaded();
}
MySlicer.prototype.onDataLoaded = function () {
    //创建切片器 DOM 树。
    var columnName = this.columnName,
        exclusiveData = this.slicerData.getExclusiveData(columnName);
    $(this.container).append($('<span>' + this.columnName + ':</span>' + '<br />'));
    var domString = "";
    for (var i = 0; i < exclusiveData.length; i++) {
        domString += '<input type="checkbox" name="' + columnName + '" value="' + exclusiveData[i] + '">';
        domString += '<span>' + exclusiveData[i] + '</span>';
        domString += '<br />';
    }
    $(this.container).append($(domString));
    //为 DOM 附加事件。
    var self = this;
    $("[name='" + self.columnName + "']").change(function () {
        var slicer = self,
            exclusiveData = slicer.slicerData.getExclusiveData(slicer.columnName),
            parent = $(this).parent(),
            items = parent.children(),
            indexes = [];
        for (var i = 0, length = items.length; i < length; i++) {
            if (items[i].checked) {
                var value = items[i].value;
                if (!isNaN(parseInt(value))) {
                    value = parseInt(value);
                }
                indexes.push(exclusiveData.indexOf(value))
            }
        }
        if (indexes.length === 0) {
            slicer.slicerData.doUnfilter(slicer.columnName);
        } else {
            slicer.slicerData.doFilter(slicer.columnName, { exclusiveRowIndexes: indexes });
        }
    });
};
MySlicer.prototype.onFiltered = function () {
    //Sync the status if the data has been filtered by the Spread.Sheets table.
    var slicerData = this.slicerData;
    var exclusiveIndexes = slicerData.getFilteredIndexes(this.columnName);
    $.each($("#slicerContainer").children("input"), function (i, input) {
    });
}
MySlicer.prototype.onColumnRemoved = function (columnName) {
    if (columnName === this.columnName) {
         this.slicerData.detachListener(this);
         this.slicerData = null;
         $("#slicerContainer").remove();
    }
}

// 创建一个自定义切片器，并将此切片器添加到 “slicerContainer” div 中。
var slicer = new MySlicer($("#slicerContainer")[0]);
slicer.setData(slicerData, 'Name');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | [`ISlicerListener`](../interfaces/GC.Spread.Slicers.ISlicerListener.md) | The listener. |

#### Returns

`void`

___

### <a id="dofilter" name="dofilter"></a> doFilter

▸ **doFilter**(`columnName`, `conditional`, `isPreview?`): `void`

过滤对应于指定列名和独占数据索引的数据。

**`example`**
```
var slicerData = new GC.Spread.Slicers.GeneralSlicerData(
    [
        [
            { value: 'Bob', text: 'Bob' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1968/6/8"), text: '6/8/1968' },
            { value: 10000, text: '10 000' }
        ],
        [
            { value: 'Betty', text: 'Betty' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1972/7/3"), text: '7/3/1972' },
            { value: 8000, text: '8 000' }
        ],
        [
            { value: 'Alice', text: 'Alice' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2012/2/15"), text: '2/15/2012' },
            { value: 5500, text: '5 500' }
        ],
        [
            { value: 'Chris', text: 'Chris' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2001/9/2"), text: '9/2/2001' },
            { value: 6200, text: '6 200' }
        ],
        [
            { value: 'James', text: 'James' },
            { value: 'Phoenix', text: 'Phoenix' },
            { value: new Date("1995/11/22"), text: '11/22/1995' },
            { value: 16150, text: '16 150' }
        ]
    ], ["Name", "City", "Birthday", "Salary"]
);
console.log(slicerData.getFilteredOutIndexes('Name', GC.Spread.Slicers.FilteredOutDataType.all)); // []
slicerData.doFilter('Name', {exclusiveRowIndexes: [1, 2]});
console.log(slicerData.getFilteredOutIndexes('Name', GC.Spread.Slicers.FilteredOutDataType.all)); // [0, 3, 4]
slicerData.doUnfilter('Name');
console.log(slicerData.getFilteredOutIndexes('Name', GC.Spread.Slicers.FilteredOutDataType.all)); // []
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnName` | `string` | 列名 |
| `conditional` | [`ISlicerConditional`](../interfaces/GC.Spread.Slicers.ISlicerConditional.md) | 条件过滤 |
| `isPreview?` | `boolean` | - |

#### Returns

`void`

___

### <a id="dounfilter" name="dounfilter"></a> doUnfilter

▸ **doUnfilter**(`columnName`): `void`

取消过滤对应于指定列名的数据。

**`example`**
```
var slicerData = new GC.Spread.Slicers.GeneralSlicerData(
    [
        [
            { value: 'Bob', text: 'Bob' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1968/6/8"), text: '6/8/1968' },
            { value: 10000, text: '10 000' }
        ],
        [
            { value: 'Betty', text: 'Betty' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1972/7/3"), text: '7/3/1972' },
            { value: 8000, text: '8 000' }
        ],
        [
            { value: 'Alice', text: 'Alice' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2012/2/15"), text: '2/15/2012' },
            { value: 5500, text: '5 500' }
        ],
        [
            { value: 'Chris', text: 'Chris' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2001/9/2"), text: '9/2/2001' },
            { value: 6200, text: '6 200' }
        ],
        [
            { value: 'James', text: 'James' },
            { value: 'Phoenix', text: 'Phoenix' },
            { value: new Date("1995/11/22"), text: '11/22/1995' },
            { value: 16150, text: '16 150' }
        ]
    ], ["Name", "City", "Birthday", "Salary"]
);
console.log(slicerData.getFilteredOutIndexes('Name', GC.Spread.Slicers.FilteredOutDataType.all)); // []
slicerData.doFilter('Name', {exclusiveRowIndexes: [1, 2]});
console.log(slicerData.getFilteredOutIndexes('Name', GC.Spread.Slicers.FilteredOutDataType.all)); // [0, 3, 4]
slicerData.doUnfilter('Name');
console.log(slicerData.getFilteredOutIndexes('Name', GC.Spread.Slicers.FilteredOutDataType.all)); // []
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnName` | `string` | 列名 |

#### Returns

`void`

___

### <a id="getcolumnindex" name="getcolumnindex"></a> getColumnIndex

▸ **getColumnIndex**(`columnName`): `number`

获取指定列名的列索引。

**`example`**
```
var slicerData = new GC.Spread.Slicers.GeneralSlicerData(
    [
        [
            { value: 'Bob', text: 'Bob' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1968/6/8"), text: '6/8/1968' },
            { value: 10000, text: '10 000' }
        ],
        [
            { value: 'Betty', text: 'Betty' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1972/7/3"), text: '7/3/1972' },
            { value: 8000, text: '8 000' }
        ],
        [
            { value: 'Alice', text: 'Alice' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2012/2/15"), text: '2/15/2012' },
            { value: 5500, text: '5 500' }
        ],
        [
            { value: 'Chris', text: 'Chris' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2001/9/2"), text: '9/2/2001' },
            { value: 6200, text: '6 200' }
        ],
        [
            { value: 'James', text: 'James' },
            { value: 'Phoenix', text: 'Phoenix' },
            { value: new Date("1995/11/22"), text: '11/22/1995' },
            { value: 16150, text: '16 150' }
        ]
    ], ["Name", "City", "Birthday", "Salary"]
);
console.log(slicerData.getColumnIndex('Name')); // 0
console.log(slicerData.getColumnIndex('Unknown')); // -1
console.log(slicerData.getColumnIndex('Salary')); // 3
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnName` | `string` | 列名 |

#### Returns

`number`

列索引

___

### <a id="getdata" name="getdata"></a> getData

▸ **getData**(`columnName`, `range?`): `string`[]

获取指定列名的数据。

**`example`**
```
var slicerData = new GC.Spread.Slicers.GeneralSlicerData(
    [
        [
            { value: 'Bob', text: 'Bob' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1968/6/8"), text: '6/8/1968' },
            { value: 10000, text: '10 000' }
        ],
        [
            { value: 'Betty', text: 'Betty' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1972/7/3"), text: '7/3/1972' },
            { value: 8000, text: '8 000' }
        ],
        [
            { value: 'Alice', text: 'Alice' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2012/2/15"), text: '2/15/2012' },
            { value: 5500, text: '5 500' }
        ],
        [
            { value: 'Chris', text: 'Chris' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2001/9/2"), text: '9/2/2001' },
            { value: 6200, text: '6 200' }
        ],
        [
            { value: 'James', text: 'James' },
            { value: 'Phoenix', text: 'Phoenix' },
            { value: new Date("1995/11/22"), text: '11/22/1995' },
            { value: 16150, text: '16 150' }
        ]
    ], ["Name", "City", "Birthday", "Salary"]
);

console.log(slicerData.getData('Name')); // ['Bob', 'Betty', 'Alice', 'Chris', 'James']
console.log(slicerData.getData('Salary')); // ['10 000', '8 000', '5 500', '6 200', '16 150']
console.log(slicerData.getData('Salary', {min: 5000, max: 10000})); // ['5 500', '6 200', '8 000', '10 000']
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnName` | `string` | 列名 |
| `range?` | [`ISlicerRangeConditional`](../interfaces/GC.Spread.Slicers.ISlicerRangeConditional.md) | - |

#### Returns

`string`[]

对应于指定列名的数据

___

### <a id="getexclusivedata" name="getexclusivedata"></a> getExclusiveData

▸ **getExclusiveData**(`columnName`): `any`[]

获取指定列名的独占数据。

**`example`**
```
var slicerData = new GC.Spread.Slicers.GeneralSlicerData(
    [
        [
            { value: 'Bob', text: 'Bob' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1968/6/8"), text: '6/8/1968' },
            { value: 10000, text: '10 000' }
        ],
        [
            { value: 'Betty', text: 'Betty' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1972/7/3"), text: '7/3/1972' },
            { value: 8000, text: '8 000' }
        ],
        [
            { value: 'Bob', text: 'Bob' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2012/2/15"), text: '2/15/2012' },
            { value: 8000, text: '8 000' }
        ],
    ], ["Name", "City", "Birthday", "Salary"]
);
console.log(slicerData.getData('Name')); // ['Bob', 'Betty', 'Bob']
console.log(slicerData.getExclusiveData('Name')); // ['Bob', 'Betty']
console.log(slicerData.getData('Salary')); // ['10 000', '8 000', '8 000']
console.log(slicerData.getExclusiveData('Salary')); // ['10 000', '8 000']
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnName` | `string` | 列名 |

#### Returns

`any`[]

对应于指定列名的独占数据

___

### <a id="getexclusiverowindex" name="getexclusiverowindex"></a> getExclusiveRowIndex

▸ **getExclusiveRowIndex**(`columnName`, `rowIndex`): `number`

获取指定列名和数据索引的独占数据索引。

**`example`**
```
var slicerData = new GC.Spread.Slicers.GeneralSlicerData(
    [
        [
            { value: 'Bob', text: 'Bob' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1968/6/8"), text: '6/8/1968' },
            { value: 10000, text: '10 000' }
        ],
        [
            { value: 'Betty', text: 'Betty' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1972/7/3"), text: '7/3/1972' },
            { value: 8000, text: '8 000' }
        ],
        [
            { value: 'Bob', text: 'Bob' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2012/2/15"), text: '2/15/2012' },
            { value: 8000, text: '8 000' }
        ],
    ], ["Name", "City", "Birthday", "Salary"]
);
console.log(slicerData.getRowIndexes('Name', 0)); // [0, 2]
console.log(slicerData.getExclusiveRowIndex('Name', 0)); // 0
console.log(slicerData.getExclusiveRowIndex('Name', 1)); // 1
console.log(slicerData.getExclusiveRowIndex('Name', 2)); // 0
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnName` | `string` | 列名 |
| `rowIndex` | `number` | 数据索引 |

#### Returns

`number`

对应于指定列名和数据索引的独占数据索引

___

### <a id="getfilteredindexes" name="getfilteredindexes"></a> getFilteredIndexes

▸ **getFilteredIndexes**(`columnName`): `number`[]

获取指定列名的过滤独占数据索引。

**`example`**
```
var slicerData = new GC.Spread.Slicers.GeneralSlicerData(
    [
        [
            { value: 'Bob', text: 'Bob' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1968/6/8"), text: '6/8/1968' },
            { value: 10000, text: '10 000' }
        ],
        [
            { value: 'Betty', text: 'Betty' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1972/7/3"), text: '7/3/1972' },
            { value: 8000, text: '8 000' }
        ],
        [
            { value: 'Alice', text: 'Alice' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2012/2/15"), text: '2/15/2012' },
            { value: 5500, text: '5 500' }
        ],
        [
            { value: 'Chris', text: 'Chris' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2001/9/2"), text: '9/2/2001' },
            { value: 6200, text: '6 200' }
        ],
        [
            { value: 'James', text: 'James' },
            { value: 'Phoenix', text: 'Phoenix' },
            { value: new Date("1995/11/22"), text: '11/22/1995' },
            { value: 16150, text: '16 150' }
        ]
    ], ["Name", "City", "Birthday", "Salary"]
);
console.log(slicerData.getFilteredIndexes('Name')); // [0, 1, 2, 3, 4]
slicerData.doFilter('Name', {exclusiveRowIndexes: [1, 2]});
console.log(slicerData.getFilteredIndexes('Name')); // [1, 2]
slicerData.doUnfilter('Name');
console.log(slicerData.getFilteredIndexes('Name')); // [0, 1, 2, 3, 4]
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnName` | `string` | 列名 |

#### Returns

`number`[]

对应于指定列名的过滤独占数据索引

___

### <a id="getfilteredoutindexes" name="getfilteredoutindexes"></a> getFilteredOutIndexes

▸ **getFilteredOutIndexes**(`columnName`, `filteredOutDataType`): `number`[]

获取指定列名的过滤独占数据索引。

**`example`**
```
var slicerData = new GC.Spread.Slicers.GeneralSlicerData(
    [
        [
            { value: 'Bob', text: 'Bob' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1968/6/8"), text: '6/8/1968' },
            { value: 10000, text: '10 000' }
        ],
        [
            { value: 'Betty', text: 'Betty' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1972/7/3"), text: '7/3/1972' },
            { value: 8000, text: '8 000' }
        ],
        [
            { value: 'Alice', text: 'Alice' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2012/2/15"), text: '2/15/2012' },
            { value: 5500, text: '5 500' }
        ],
        [
            { value: 'Chris', text: 'Chris' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2001/9/2"), text: '9/2/2001' },
            { value: 6200, text: '6 200' }
        ],
        [
            { value: 'James', text: 'James' },
            { value: 'Phoenix', text: 'Phoenix' },
            { value: new Date("1995/11/22"), text: '11/22/1995' },
            { value: 16150, text: '16 150' }
        ]
    ], ["Name", "City", "Birthday", "Salary"]
);
console.log(slicerData.getFilteredOutIndexes('Name', GC.Spread.Slicers.FilteredOutDataType.all)); // []
slicerData.doFilter('Name', {exclusiveRowIndexes: [1, 2]});
console.log(slicerData.getFilteredOutIndexes('Name', GC.Spread.Slicers.FilteredOutDataType.all)); // [0, 3, 4]
slicerData.doUnfilter('Name');
console.log(slicerData.getFilteredOutIndexes('Name', GC.Spread.Slicers.FilteredOutDataType.all)); // []
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnName` | `string` | 列名 |
| `filteredOutDataType` | [`FilteredOutDataType`](../enums/GC.Spread.Slicers.FilteredOutDataType.md) | 过滤独占数据索引的类型 |

#### Returns

`number`[]

对应于指定列名的过滤独占数据索引

___

### <a id="getfilteredoutranges" name="getfilteredoutranges"></a> getFilteredOutRanges

▸ **getFilteredOutRanges**(`columnName`): [`ISlicerRangeConditional`](../interfaces/GC.Spread.Slicers.ISlicerRangeConditional.md)[]

获取其他列的过滤范围。

**`example`**
```
var slicerData = new GC.Spread.Slicers.GeneralSlicerData(
    [
        [
            { value: 'Bob', text: 'Bob' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1968/6/8"), text: '6/8/1968' },
            { value: 10000, text: '10 000' }
        ],
        [
            { value: 'Betty', text: 'Betty' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1972/7/3"), text: '7/3/1972' },
            { value: 8000, text: '8 000' }
        ],
        [
            { value: 'Alice', text: 'Alice' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2012/2/15"), text: '2/15/2012' },
            { value: 5500, text: '5 500' }
        ],
        [
            { value: 'Chris', text: 'Chris' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2001/9/2"), text: '9/2/2001' },
            { value: 6200, text: '6 200' }
        ],
        [
            { value: 'James', text: 'James' },
            { value: 'Phoenix', text: 'Phoenix' },
            { value: new Date("1995/11/22"), text: '11/22/1995' },
            { value: 16150, text: '16 150' }
        ]
    ], ["Name", "City", "Birthday", "Salary"]
);
slicerData.doFilter('Salary', {
    ranges: [
        { min: 5000, max: 10000 },
        { min: 5000, max: 200000 },
        { min: 60000, max: 61000 }
    ]
});
console.log(slicerData.getFilteredOutRanges('Salary')); // [{min: 60000, max: 61000}]
console.log(slicerData.getFilteredRanges('Salary')); // [{min: 5000, max: 10000}, {min: 5000, max: 200000}]
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnName` | `string` | 列名 |

#### Returns

[`ISlicerRangeConditional`](../interfaces/GC.Spread.Slicers.ISlicerRangeConditional.md)[]

对应于指定列名的过滤范围

___

### <a id="getfilteredoutrowindexes" name="getfilteredoutrowindexes"></a> getFilteredOutRowIndexes

▸ **getFilteredOutRowIndexes**(): `number`[]

获取过滤后的行索引。

**`example`**
```
var slicerData = new GC.Spread.Slicers.GeneralSlicerData(
    [
        [
            { value: 'Bob', text: 'Bob' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1968/6/8"), text: '6/8/1968' },
            { value: 10000, text: '10 000' }
        ],
        [
            { value: 'Betty', text: 'Betty' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1972/7/3"), text: '7/3/1972' },
            { value: 8000, text: '8 000' }
        ],
        [
            { value: 'Alice', text: 'Alice' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2012/2/15"), text: '2/15/2012' },
            { value: 5500, text: '5 500' }
        ],
        [
            { value: 'Chris', text: 'Chris' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2001/9/2"), text: '9/2/2001' },
            { value: 6200, text: '6 200' }
        ],
        [
            { value: 'James', text: 'James' },
            { value: 'Phoenix', text: 'Phoenix' },
            { value: new Date("1995/11/22"), text: '11/22/1995' },
            { value: 16150, text: '16 150' }
        ]
    ], ["Name", "City", "Birthday", "Salary"]
);
slicerData.doFilter('Salary', {
     exclusiveRowIndexes: [0, 1, 2]
});
console.log(slicerData.getFilteredOutRowIndexes('Salary')); // [3, 4]
console.log(slicerData.getFilteredRowIndexes('Salary')); // [0, 1, 2]
```

#### Returns

`number`[]

过滤后的行索引。

___

### <a id="getfilteredranges" name="getfilteredranges"></a> getFilteredRanges

▸ **getFilteredRanges**(`columnName`): [`ISlicerRangeConditional`](../interfaces/GC.Spread.Slicers.ISlicerRangeConditional.md)[]

获取指定列名的过滤范围。

**`example`**
```
var slicerData = new GC.Spread.Slicers.GeneralSlicerData(
    [
        [
            { value: 'Bob', text: 'Bob' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1968/6/8"), text: '6/8/1968' },
            { value: 10000, text: '10 000' }
        ],
        [
            { value: 'Betty', text: 'Betty' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1972/7/3"), text: '7/3/1972' },
            { value: 8000, text: '8 000' }
        ],
        [
            { value: 'Alice', text: 'Alice' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2012/2/15"), text: '2/15/2012' },
            { value: 5500, text: '5 500' }
        ],
        [
            { value: 'Chris', text: 'Chris' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2001/9/2"), text: '9/2/2001' },
            { value: 6200, text: '6 200' }
        ],
        [
            { value: 'James', text: 'James' },
            { value: 'Phoenix', text: 'Phoenix' },
            { value: new Date("1995/11/22"), text: '11/22/1995' },
            { value: 16150, text: '16 150' }
        ]
    ], ["Name", "City", "Birthday", "Salary"]
);
slicerData.doFilter('Salary', {
    ranges: [
        { min: 5000, max: 10000 },
        { min: 5000, max: 200000 },
        { min: 60000, max: 61000 }
    ]
});
console.log(slicerData.getFilteredOutRanges('Salary')); // [{min: 60000, max: 61000}]
console.log(slicerData.getFilteredRanges('Salary')); // [{min: 5000, max: 10000}, {min: 5000, max: 200000}]
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnName` | `string` | 列名 |

#### Returns

[`ISlicerRangeConditional`](../interfaces/GC.Spread.Slicers.ISlicerRangeConditional.md)[]

对应于指定列名的过滤范围

___

### <a id="getfilteredrowindexes" name="getfilteredrowindexes"></a> getFilteredRowIndexes

▸ **getFilteredRowIndexes**(): `number`[]

获取过滤后的行索引。

**`example`**
```
var slicerData = new GC.Spread.Slicers.GeneralSlicerData(
    [
        [
            { value: 'Bob', text: 'Bob' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1968/6/8"), text: '6/8/1968' },
            { value: 10000, text: '10 000' }
        ],
        [
            { value: 'Betty', text: 'Betty' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1972/7/3"), text: '7/3/1972' },
            { value: 8000, text: '8 000' }
        ],
        [
            { value: 'Alice', text: 'Alice' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2012/2/15"), text: '2/15/2012' },
            { value: 5500, text: '5 500' }
        ],
        [
            { value: 'Chris', text: 'Chris' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2001/9/2"), text: '9/2/2001' },
            { value: 6200, text: '6 200' }
        ],
        [
            { value: 'James', text: 'James' },
            { value: 'Phoenix', text: 'Phoenix' },
            { value: new Date("1995/11/22"), text: '11/22/1995' },
            { value: 16150, text: '16 150' }
        ]
    ], ["Name", "City", "Birthday", "Salary"]
);
slicerData.doFilter('Salary', {
     exclusiveRowIndexes: [0, 1, 2]
});
console.log(slicerData.getFilteredOutRowIndexes('Salary')); // [3, 4]
console.log(slicerData.getFilteredRowIndexes('Salary')); // [0, 1, 2]
```

#### Returns

`number`[]

过滤后的行索引。

___

### <a id="getrowindexes" name="getrowindexes"></a> getRowIndexes

▸ **getRowIndexes**(`columnName`, `exclusiveRowIndex`): `number`[]

获取指定列名和独占数据索引的数据索引。

**`example`**
```
var slicerData = new GC.Spread.Slicers.GeneralSlicerData(
    [
        [
            { value: 'Bob', text: 'Bob' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1968/6/8"), text: '6/8/1968' },
            { value: 10000, text: '10 000' }
        ],
        [
            { value: 'Betty', text: 'Betty' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1972/7/3"), text: '7/3/1972' },
            { value: 8000, text: '8 000' }
        ],
        [
            { value: 'Bob', text: 'Bob' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2012/2/15"), text: '2/15/2012' },
            { value: 8000, text: '8 000' }
        ],
    ], ["Name", "City", "Birthday", "Salary"]
);
console.log(slicerData.getRowIndexes('Name', 0)); // [0, 2]
console.log(slicerData.getRowIndexes('Name', 1)); // [1]
console.log(slicerData.getRowIndexes('Name', 2)); // undefined
console.log(slicerData.getRowIndexes('Salary', 1)); // [1, 2]
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnName` | `string` | 列名 |
| `exclusiveRowIndex` | `number` | 独占数据索引 |

#### Returns

`number`[]

对应于指定列名和独占数据索引的数据索引

___

### <a id="inpreview" name="inpreview"></a> inPreview

▸ **inPreview**(): `boolean`

获取切片器是否处于预览状态。
如果您将 doFilter() 与 isPreview 标志设置为 true，（例如 slicerData.doFilter('Name', {exclusiveRowIndexes: [1]}, true);）
您可以通过 slicerData.inPreview() API 检查切片器是否正在预览中进行过滤。

**`example`**
```
var slicerData = new GC.Spread.Slicers.GeneralSlicerData(
    [
        [
            { value: 'Bob', text: 'Bob' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1968/6/8"), text: '6/8/1968' },
            { value: 10000, text: '10 000' }
        ],
        [
            { value: 'Betty', text: 'Betty' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1972/7/3"), text: '7/3/1972' },
            { value: 8000, text: '8 000' }
        ],
        [
            { value: 'Bob', text: 'Bob' },
            { value: 'Washington', text: 'Washington' },
            { value: new Date("2012/2/15"), text: '2/15/2012' },
            { value: 8000, text: '5 500' }
        ],
    ], ["Name", "City", "Birthday", "Salary"]
);
console.log(slicerData.getFilteredOutIndexes('Name', GC.Spread.Slicers.FilteredOutDataType.all)); // []
slicerData.doFilter('Name', {exclusiveRowIndexes: [1, 2]});
console.log(slicerData.getFilteredOutIndexes('Name', GC.Spread.Slicers.FilteredOutDataType.all)); // [0]
console.log(slicerData.inPreview()); // false
slicerData.clearPreview();
console.log(slicerData.getFilteredOutIndexes('Name', GC.Spread.Slicers.FilteredOutDataType.all)); // [0]
slicerData.doUnfilter('Name');
console.log(slicerData.getFilteredOutIndexes('Name', GC.Spread.Slicers.FilteredOutDataType.all)); // []

slicerData.doFilter('Name', {exclusiveRowIndexes: [1, 2]}, true);
console.log(slicerData.getFilteredOutIndexes('Name', GC.Spread.Slicers.FilteredOutDataType.all)); // [0]
console.log(slicerData.inPreview()); // true
slicerData.clearPreview();
console.log(slicerData.inPreview()); // false
console.log(slicerData.getFilteredOutIndexes('Name', GC.Spread.Slicers.FilteredOutDataType.all)); // []
```

#### Returns

`boolean`

___

### <a id="oncolumnnamechanged" name="oncolumnnamechanged"></a> onColumnNameChanged

▸ **onColumnNameChanged**(`oldName`, `newName`): `void`

更改切片器数据中的列名。

**`example`**
```
var slicerData = new GC.Spread.Slicers.GeneralSlicerData(
     [
          [
               { value: 'Bob', text: 'Bob' },
               { value: 'NewYork', text: 'NewYork' },
               { value: new Date("1968/6/8"), text: '6/8/1968' },
               { value: 10000, text: '10 000' }
          ],
          [
               { value: 'Betty', text: 'Betty' },
               { value: 'NewYork', text: 'NewYork' },
               { value: new Date("1972/7/3"), text: '7/3/1972' },
               { value: 8000, text: '8 000' }
          ]
     ], ["Name", "City", "Birthday", "Salary"]
);
console.log(slicerData.getExclusiveData('Name')); // ['Bob', 'Betty']
slicerData.onColumnNameChanged('Name', 'NewName');
console.log(slicerData.getExclusiveData('Name')); // []
console.log(slicerData.getExclusiveData('NewName')); // ['Bob', 'Betty']
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `oldName` | `string` | 旧列名 |
| `newName` | `string` | 新列名 |

#### Returns

`void`

___

### <a id="oncolumnsremoved" name="oncolumnsremoved"></a> onColumnsRemoved

▸ **onColumnsRemoved**(`colIndex`, `colCount`): `void`

删除切片器数据中的列。

**`example`**
```
var slicerData = new GC.Spread.Slicers.GeneralSlicerData(
     [
          [
               { value: 'Bob', text: 'Bob' },
               { value: 'NewYork', text: 'NewYork' },
               { value: new Date("1968/6/8"), text: '6/8/1968' },
               { value: 10000, text: '10 000' }
          ],
          [
               { value: 'Betty', text: 'Betty' },
               { value: 'NewYork', text: 'NewYork' },
               { value: new Date("1972/7/3"), text: '7/3/1972' },
               { value: 8000, text: '8 000' }
          ]
     ], ["Name", "City", "Birthday", "Salary"]
);
console.log(slicerData.getData('Name')); // ['Bob', 'Betty']
slicerData.onColumnsRemoved(0, 1);
console.log(slicerData.getData('Name')); // []
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `colIndex` | `number` | 起始列索引 |
| `colCount` | `number` | 要删除的列数 |

#### Returns

`void`

___

### <a id="ondatachanged" name="ondatachanged"></a> onDataChanged

▸ **onDataChanged**(`changedDataItems`): `void`

更改切片器数据源中的数据项。

**`example`**
```
var slicerData = new GC.Spread.Slicers.GeneralSlicerData(
     [
          [
               { value: 'Bob', text: 'Bob' },
               { value: 'NewYork', text: 'NewYork' },
               { value: new Date("1968/6/8"), text: '6/8/1968' },
               { value: 10000, text: '10 000' }
          ],
          [
               { value: 'Betty', text: 'Betty' },
               { value: 'NewYork', text: 'NewYork' },
               { value: new Date("1972/7/3"), text: '7/3/1972' },
               { value: 8000, text: '8 000' }
          ]
     ], ["Name", "City", "Birthday", "Salary"]
);
console.log(slicerData.getData('Name')); // ['Bob', 'Betty']
slicerData.onDataChanged([{columnName: 'Name', rowIndex: 1, row: 1, data: {value: 'Alice', text: 'Alice'}}]);
console.log(slicerData.getData('Name')); // ['Bob', 'Alice']
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `changedDataItems` | [`ISlicerDataItem`](../interfaces/GC.Spread.Slicers.ISlicerDataItem.md) | 数据源中的更改数据项 |

#### Returns

`void`

___

### <a id="onfiltered" name="onfiltered"></a> onFiltered

▸ **onFiltered**(): `void`

在切片器数据被过滤后发生。

#### Returns

`void`

___

### <a id="onrowsadded" name="onrowsadded"></a> onRowsAdded

▸ **onRowsAdded**(`rowIndex`, `rowCount`): `void`

在切片器数据源中添加行。

**`example`**
```
var slicerData = new GC.Spread.Slicers.GeneralSlicerData(
     [
          [
               { value: 'Bob', text: 'Bob' },
               { value: 'NewYork', text: 'NewYork' },
               { value: new Date("1968/6/8"), text: '6/8/1968' },
               { value: 10000, text: '10 000' }
          ],
          [
               { value: 'Betty', text: 'Betty' },
               { value: 'NewYork', text: 'NewYork' },
               { value: new Date("1972/7/3"), text: '7/3/1972' },
               { value: 8000, text: '8 000' }
          ]
     ], ["Name", "City", "Birthday", "Salary"]
);
console.log(slicerData.getData('Name')); // ['Bob', 'Betty']
slicerData.onRowsAdded(1, 2);
console.log(slicerData.getData('Name')); // ['Bob', undefined, undefined, 'Betty']
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rowIndex` | `number` | 起始行索引 |
| `rowCount` | `number` | 要添加的行数 |

#### Returns

`void`

___

### <a id="onrowsremoved" name="onrowsremoved"></a> onRowsRemoved

▸ **onRowsRemoved**(`rowIndex`, `rowCount`): `void`

从切片器数据源中删除行。

**`example`**
```
var slicerData = new GC.Spread.Slicers.GeneralSlicerData(
     [
          [
               { value: 'Bob', text: 'Bob' },
               { value: 'NewYork', text: 'NewYork' },
               { value: new Date("1968/6/8"), text: '6/8/1968' },
               { value: 10000, text: '10 000' }
          ],
          [
               { value: 'Betty', text: 'Betty' },
               { value: 'NewYork', text: 'NewYork' },
               { value: new Date("1972/7/3"), text: '7/3/1972' },
               { value: 8000, text: '8 000' }
          ]
     ], ["Name", "City", "Birthday", "Salary"]
);
console.log(slicerData.getData('Name')); // ['Bob', 'Betty']
slicerData.onRowsAdded(1, 2);
console.log(slicerData.getData('Name')); // ['Bob', undefined, undefined, 'Betty']
slicerData.onRowsRemoved(2, 1);
console.log(slicerData.getData('Name')); // ['Bob', undefined, 'Betty']
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rowIndex` | `number` | 起始行索引 |
| `rowCount` | `number` | 要删除的行数 |

#### Returns

`void`

___

### <a id="resumefilteredevents" name="resumefilteredevents"></a> resumeFilteredEvents

▸ **resumeFilteredEvents**(): `void`

恢复 onFiltered 事件。

**`example`**
```
var slicerData = new GC.Spread.Slicers.GeneralSlicerData(
    [
        [
            { value: 'Bob', text: 'Bob' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1968/6/8"), text: '6/8/1968' },
            { value: 10000, text: '10 000' }
        ],
        [
            { value: 'Betty', text: 'Betty' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1972/7/3"), text: '7/3/1972' },
            { value: 8000, text: '8 000' }
        ],
    ], ["Name", "City", "Birthday", "Salary"]
);
// 定义自定义切片器。
function MySlicer(container) {
    this.container = container;
    this.slicerData = null;
    this.columnName = null;
}
MySlicer.prototype.setData = function (slicerData, columnName) {
    this.slicerData = slicerData;
    this.columnName = columnName;
    // 在此附加监听器
    this.slicerData.attachListener(this);
}
MySlicer.prototype.onFiltered = function () {
    console.log('filter event triggered');
}
// 创建一个自定义切片器，并将此切片器添加到 “slicerContainer” div 中。
var slicer = new MySlicer($("#slicerContainer")[0]);
slicer.setData(slicerData, 'Name');
slicerData.doFilter('Name', {exclusiveRowIndexes: [1]});
// 观察控制台日志：'filter event triggered'
slicerData.suspendFilteredEvents();
slicerData.doFilter('Name', {exclusiveRowIndexes: [0]});
// 观察控制台日志：nothing
slicerData.suspendFilteredEvents();
slicerData.doFilter('Name', {exclusiveRowIndexes: [0, 1]});
// 观察控制台日志：'filter event triggered'
```

#### Returns

`void`

___

### <a id="suspendfilteredevents" name="suspendfilteredevents"></a> suspendFilteredEvents

▸ **suspendFilteredEvents**(): `void`

暂停 onFiltered 事件。

**`example`**
```
var slicerData = new GC.Spread.Slicers.GeneralSlicerData(
    [
        [
            { value: 'Bob', text: 'Bob' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1968/6/8"), text: '6/8/1968' },
            { value: 10000, text: '10 000' }
        ],
        [
            { value: 'Betty', text: 'Betty' },
            { value: 'NewYork', text: 'NewYork' },
            { value: new Date("1972/7/3"), text: '7/3/1972' },
            { value: 8000, text: '8 000' }
        ],
    ], ["Name", "City", "Birthday", "Salary"]
);
// 定义自定义切片器。
function MySlicer(container) {
    this.container = container;
    this.slicerData = null;
    this.columnName = null;
}
MySlicer.prototype.setData = function (slicerData, columnName) {
    this.slicerData = slicerData;
    this.columnName = columnName;
    // 在此附加监听器
    this.slicerData.attachListener(this);
}
MySlicer.prototype.onFiltered = function () {
    console.log('filter event triggered');
}
// 创建一个自定义切片器，并将此切片器添加到 “slicerContainer” div 中。
var slicer = new MySlicer($("#slicerContainer")[0]);
slicer.setData(slicerData, 'Name');
slicerData.doFilter('Name', {exclusiveRowIndexes: [1]});
// 观察控制台日志：'filter event triggered'
slicerData.suspendFilteredEvents();
slicerData.doFilter('Name', {exclusiveRowIndexes: [0]});
// 观察控制台日志：nothing
slicerData.suspendFilteredEvents();
slicerData.doFilter('Name', {exclusiveRowIndexes: [0, 1]});
// 观察控制台日志：'filter event triggered'
```

#### Returns

`void`
