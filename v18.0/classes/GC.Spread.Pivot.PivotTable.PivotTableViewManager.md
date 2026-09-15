# Class: PivotTableViewManager

[Pivot](../modules/GC.Spread.Pivot.md).[PivotTable](../modules/GC.Spread.Pivot.PivotTable.md).PivotTableViewManager

## Table of contents

### Constructors

- [constructor](GC.Spread.Pivot.PivotTable.PivotTableViewManager.md#constructor)

### Methods

- [add](GC.Spread.Pivot.PivotTable.PivotTableViewManager.md#add)
- [all](GC.Spread.Pivot.PivotTable.PivotTableViewManager.md#all)
- [apply](GC.Spread.Pivot.PivotTable.PivotTableViewManager.md#apply)
- [get](GC.Spread.Pivot.PivotTable.PivotTableViewManager.md#get)
- [remove](GC.Spread.Pivot.PivotTable.PivotTableViewManager.md#remove)
- [save](GC.Spread.Pivot.PivotTable.PivotTableViewManager.md#save)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new PivotTableViewManager**(`applyCallback`, `saveCallback`)

透视表视图管理器

#### Parameters

| Name | Type |
| :------ | :------ |
| `applyCallback` | `Function` |
| `saveCallback` | `Function` |

## Methods

### <a id="add" name="add"></a> add

▸ **add**(`view`): `boolean`

添加视图到透视表视图管理器

**`代码示例`**
``` javascript
var viewsManager = pivotTable.views;
viewsManager.add({
    name: 'config1',
    config: pivotTable.serialize()
});
viewsManager.get('config1');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `view` | [`IPivotTableView`](../modules/GC.Spread.Pivot.md#ipivottableview) | 添加的视图 |

#### Returns

`boolean`

___

### <a id="all" name="all"></a> all

▸ **all**(): [`IPivotTableView`](../modules/GC.Spread.Pivot.md#ipivottableview)[]

从透视表视图管理器获取所有视图

**`代码示例`**
``` javascript
var viewsManager = pivotTable.views;
viewsManager.save('config1');
console.log(viewsManager.all());
```

#### Returns

[`IPivotTableView`](../modules/GC.Spread.Pivot.md#ipivottableview)[]

___

### <a id="apply" name="apply"></a> apply

▸ **apply**(`name`): `void`

将视图应用到当前透视表视图管理器

**`代码示例`**
``` javascript
var viewsManager = pivotTable.views;
viewsManager.save('config1');
viewsManager.apply('config1');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要应用的视图名称 |

#### Returns

`void`

___

### <a id="get" name="get"></a> get

▸ **get**(`name`): [`IPivotTableView`](../modules/GC.Spread.Pivot.md#ipivottableview)

从透视表视图管理器获取视图

**`代码示例`**
``` javascript
var viewsManager = pivotTable.views;
viewsManager.save('config1');
viewsManager.get('config1');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要查询的视图名称 |

#### Returns

[`IPivotTableView`](../modules/GC.Spread.Pivot.md#ipivottableview)

___

### <a id="remove" name="remove"></a> remove

▸ **remove**(`name`): `void`

从透视表视图管理器中删除视图

**`代码示例`**
``` javascript
var viewsManager = pivotTable.views;
viewsManager.remove('config1');
viewsManager.get('config1');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要删除的视图的名称 |

#### Returns

`void`

___

### <a id="save" name="save"></a> save

▸ **save**(`name`): `boolean`

保存视图到透视表视图管理器

**`代码示例`**
``` javascript
var viewsManager = pivotTable.views;
viewsManager.save('config1');
viewsManager.get('config1');
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 要保存的视图的名称 |

#### Returns

`boolean`
