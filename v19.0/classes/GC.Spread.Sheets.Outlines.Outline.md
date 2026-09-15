# Class: Outline

[Sheets](../modules/GC.Spread.Sheets.md).[Outlines](../modules/GC.Spread.Sheets.Outlines.md).Outline

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Outlines.Outline.md#constructor)

### Methods

- [direction](GC.Spread.Sheets.Outlines.Outline.md#direction)
- [expand](GC.Spread.Sheets.Outlines.Outline.md#expand)
- [expandGroup](GC.Spread.Sheets.Outlines.Outline.md#expandgroup)
- [find](GC.Spread.Sheets.Outlines.Outline.md#find)
- [getCollapsed](GC.Spread.Sheets.Outlines.Outline.md#getcollapsed)
- [getLevel](GC.Spread.Sheets.Outlines.Outline.md#getlevel)
- [getMaxLevel](GC.Spread.Sheets.Outlines.Outline.md#getmaxlevel)
- [getState](GC.Spread.Sheets.Outlines.Outline.md#getstate)
- [group](GC.Spread.Sheets.Outlines.Outline.md#group)
- [isCollapsed](GC.Spread.Sheets.Outlines.Outline.md#iscollapsed)
- [isGroupEnd](GC.Spread.Sheets.Outlines.Outline.md#isgroupend)
- [refresh](GC.Spread.Sheets.Outlines.Outline.md#refresh)
- [resumeAdding](GC.Spread.Sheets.Outlines.Outline.md#resumeadding)
- [setCollapsed](GC.Spread.Sheets.Outlines.Outline.md#setcollapsed)
- [suspendAdding](GC.Spread.Sheets.Outlines.Outline.md#suspendadding)
- [ungroup](GC.Spread.Sheets.Outlines.Outline.md#ungroup)
- [ungroupRange](GC.Spread.Sheets.Outlines.Outline.md#ungrouprange)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Outline**(`count`)

表示工作表的大纲（范围组）。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `count` | `number` | 行数或列数。 |

## Methods

### <a id="direction" name="direction"></a> direction

▸ **direction**(`direction?`): `any`

获取或设置大纲（范围组）的方向。

**`example`**
```
activeSheet.suspendPaint();
activeSheet.rowOutlines.group(3,2);
activeSheet.columnOutlines.group(4,1);
activeSheet.rowOutlines.direction(GC.Spread.Sheets.Outlines.OutlineDirection.forward);
activeSheet.resumePaint();
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `direction?` | [`OutlineDirection`](../enums/GC.Spread.Sheets.Outlines.OutlineDirection.md) |

#### Returns

`any`

如果未设置值，则返回大纲（范围组）的方向；否则返回大纲。

___

### <a id="expand" name="expand"></a> expand

▸ **expand**(`level`, `expand`): `void`

使用指定的级别展开所有大纲（范围组）。

**`example`**
```
//此示例使用expand方法。
activeSheet.suspendPaint();
activeSheet.rowOutlines.group(0,5);
activeSheet.rowOutlines.expand(0,false);
activeSheet.resumePaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `level` | `number` | 要展开或折叠的大纲级别。 |
| `expand` | `boolean` | 是否展开组。 |

#### Returns

`void`

___

### <a id="expandgroup" name="expandgroup"></a> expandGroup

▸ **expandGroup**(`groupInfo`, `expand`): `void`

展开或折叠指定的行或列大纲（范围组）。

**`example`**
```javascript
var activeSheet = spread.getActiveSheet();
activeSheet.suspendPaint();
activeSheet.rowOutlines.group(2, 5);
var groupInfo = activeSheet.rowOutlines.find(2, 0);
activeSheet.rowOutlines.expandGroup(groupInfo, false);
activeSheet.resumePaint(); // 现在组已创建并折叠。
activeSheet.rowOutlines.expandGroup(groupInfo, true); // 现在组已展开。
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `groupInfo` | [`OutlineInfo`](GC.Spread.Sheets.Outlines.OutlineInfo.md) | 范围组的组信息。 |
| `expand` | `boolean` | 是否展开组。 |

#### Returns

`void`

___

### <a id="find" name="find"></a> find

▸ **find**(`index`, `level`): [`OutlineInfo`](GC.Spread.Sheets.Outlines.OutlineInfo.md)

获取具有指定组级别和行或列索引的大纲（范围组）。

**`example`**
```
//此示例使用find方法。
activeSheet.rowOutlines.group(0,5);
var rgi = activeSheet.rowOutlines.find(1, 0);
rgi.state(GC.Spread.Sheets.Outlines.OutlineState.collapsed);
spread.invalidateLayout();
spread.repaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 行或列的索引。 |
| `level` | `number` | 大纲（范围组）的级别。 |

#### Returns

[`OutlineInfo`](GC.Spread.Sheets.Outlines.OutlineInfo.md)

指定的范围组。

___

### <a id="getcollapsed" name="getcollapsed"></a> getCollapsed

▸ **getCollapsed**(`index`): `boolean`

获取指定索引的折叠状态。

**`example`**
```
//此示例使用 getCollapsed 方法。
activeSheet.suspendPaint();
activeSheet.rowOutlines.group(0,5);
activeSheet.rowOutlines.expand(0,true);
activeSheet.resumePaint();
alert(activeSheet.rowOutlines.isCollapsed(0));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 索引。 |

#### Returns

`boolean`

如果已折叠则返回 `true`；否则返回 `false`。

___

### <a id="getlevel" name="getlevel"></a> getLevel

▸ **getLevel**(`index`): `number`

获取指定行或列的级别。
级别索引从零开始。

**`example`**
```
//此示例使用 getLevel 方法。
activeSheet.suspendPaint();
activeSheet.rowOutlines.group(0,5);
activeSheet.rowOutlines.expand(0,true);
activeSheet.resumePaint();
alert(activeSheet.rowOutlines.getLevel(0));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 行或列的索引。 |

#### Returns

`number`

行或列的级别。

___

### <a id="getmaxlevel" name="getmaxlevel"></a> getMaxLevel

▸ **getMaxLevel**(): `number`

获取最深级别的数量。

**`remarks`** 级别索引从零开始。

**`example`**
```
//此示例使用 getMaxLevel 方法。
activeSheet.suspendPaint();
activeSheet.rowOutlines.group(0,5);
activeSheet.rowOutlines.group(1,4);
activeSheet.rowOutlines.expand(0,true);
activeSheet.columnOutlines.group(0,1);
activeSheet.resumePaint();
alert(activeSheet.rowOutlines.getMaxLevel());
```

#### Returns

`number`

最深级别的数量。

___

### <a id="getstate" name="getstate"></a> getState

▸ **getState**(`groupInfo`): [`OutlineState`](../enums/GC.Spread.Sheets.Outlines.OutlineState.md)

获取指定组的状态。

**`example`**
```
//此示例使用 getState 方法。
activeSheet.suspendPaint();
activeSheet.rowOutlines.group(0,5);
var rgi = activeSheet.rowOutlines.find(1, 0);
rgi.state(GC.Spread.Sheets.Outlines.OutlineState.collapsed);
alert(activeSheet.rowOutlines.getState(rgi));
activeSheet.resumePaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `groupInfo` | [`OutlineInfo`](GC.Spread.Sheets.Outlines.OutlineInfo.md) | 组信息。 |

#### Returns

[`OutlineState`](../enums/GC.Spread.Sheets.Outlines.OutlineState.md)

组状态。

___

### <a id="group" name="group"></a> group

▸ **group**(`index`, `count`): `void`

从指定的起始索引开始将一系列行或列分组为大纲（范围组）。

**`example`**
```
//此示例使用 group 方法。
activeSheet.suspendPaint();
activeSheet.rowOutlines.group(0,5);
activeSheet.rowOutlines.expand(0,false);
activeSheet.resumePaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 组的起始索引。 |
| `count` | `number` | 要分组的行或列的数量。 |

#### Returns

`void`

___

### <a id="iscollapsed" name="iscollapsed"></a> isCollapsed

▸ **isCollapsed**(`index`): `boolean`

确定指定索引处的范围组是否已折叠。

**`example`**
```
//此示例使用 isCollapsed 方法。
activeSheet.suspendPaint();
activeSheet.rowOutlines.group(0,5);
activeSheet.rowOutlines.expand(0,true);
activeSheet.resumePaint();
alert(activeSheet.rowOutlines.isCollapsed(0));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 范围组中行或列的索引。 |

#### Returns

`boolean`

如果指定的行或列已折叠，则为 `true`；否则为 `false`。

___

### <a id="isgroupend" name="isgroupend"></a> isGroupEnd

▸ **isGroupEnd**(`index`, `processLevel`): `boolean`

确定指定索引是否为组的末尾。

**`example`**
```
activeSheet.suspendPaint();
activeSheet.rowOutlines.group(2, 5);
activeSheet.rowOutlines.group(3, 2);
activeSheet.resumePaint();

console.log(activeSheet.rowOutlines.isGroupEnd(2, 0)); // false
console.log(activeSheet.rowOutlines.isGroupEnd(4, 0)); // false
console.log(activeSheet.rowOutlines.isGroupEnd(4, 1)); // true
console.log(activeSheet.rowOutlines.isGroupEnd(6, 0)); // true
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 索引。 |
| `processLevel` | `number` | 处理级别。 |

#### Returns

`boolean`

如果指定索引是组的末尾，则为 `true`；否则为 `false`。

___

### <a id="refresh" name="refresh"></a> refresh

▸ **refresh**(): `void`

刷新此范围组。

#### Returns

`void`

___

### <a id="resumeadding" name="resumeadding"></a> resumeAdding

▸ **resumeAdding**(): `void`

当行/列插入组范围时恢复添加组。

**`example`**
```javascript
var activeSheet = spread.getActiveSheet();
activeSheet.suspendPaint();
activeSheet.rowOutlines.group(2, 5);
activeSheet.resumePaint();

console.log(activeSheet.rowOutlines.find(3, 0).end); // 6
console.log(activeSheet.rowOutlines.find(5, 0).end); // 6
activeSheet.addRows(4, 1);
console.log(activeSheet.rowOutlines.find(3, 0).end); // 7
console.log(activeSheet.rowOutlines.find(5, 0).end); // 7

activeSheet.rowOutlines.suspendAdding();
activeSheet.addRows(4, 1);
console.log(activeSheet.rowOutlines.find(3, 0).end); // 3 // 由于添加被暂停，组被分成两部分。
console.log(activeSheet.rowOutlines.find(5, 0).end); // 8
activeSheet.rowOutlines.resumeAdding();
```

#### Returns

`void`

___

### <a id="setcollapsed" name="setcollapsed"></a> setCollapsed

▸ **setCollapsed**(`index`, `collapsed`): `void`

设置折叠级别。

**`example`**
```
//此示例使用 setCollapsed 方法。
activeSheet.suspendPaint();
activeSheet.rowOutlines.group(0,5);
activeSheet.rowOutlines.setCollapsed(0,false);
activeSheet.resumePaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 索引。 |
| `collapsed` | `boolean` | 设置为 `true` 以折叠级别。 |

#### Returns

`void`

___

### <a id="suspendadding" name="suspendadding"></a> suspendAdding

▸ **suspendAdding**(): `void`

当行/列插入组范围时暂停添加组。

**`example`**
```javascript
var activeSheet = spread.getActiveSheet();
activeSheet.suspendPaint();
activeSheet.rowOutlines.group(2, 5);
activeSheet.resumePaint();

console.log(activeSheet.rowOutlines.find(3, 0).end); // 6
console.log(activeSheet.rowOutlines.find(5, 0).end); // 6
activeSheet.addRows(4, 1);
console.log(activeSheet.rowOutlines.find(3, 0).end); // 7
console.log(activeSheet.rowOutlines.find(5, 0).end); // 7

activeSheet.rowOutlines.suspendAdding();
activeSheet.addRows(4, 1);
console.log(activeSheet.rowOutlines.find(3, 0).end); // 3 // 由于添加被暂停，组被分成两部分。
console.log(activeSheet.rowOutlines.find(5, 0).end); // 8
activeSheet.rowOutlines.resumeAdding();
```

#### Returns

`void`

___

### <a id="ungroup" name="ungroup"></a> ungroup

▸ **ungroup**(): `void`

移除所有大纲（范围组）。

**`example`**
```
//此示例使用 ungroup 方法。
activeSheet.suspendPaint();
activeSheet.rowOutlines.group(0,5);
activeSheet.rowOutlines.ungroup();
activeSheet.resumePaint();
```

#### Returns

`void`

___

### <a id="ungrouprange" name="ungrouprange"></a> ungroupRange

▸ **ungroupRange**(`index`, `count`): `void`

从指定起始索引处的大纲（范围组）中移除一系列行或列。

**`example`**
```
//此示例使用 ungroupRange 方法。
activeSheet.suspendPaint();
activeSheet.rowOutlines.group(0,5);
activeSheet.rowOutlines.ungroupRange(0,1);
activeSheet.resumePaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 组的起始索引。 |
| `count` | `number` | 要移除的行或列的数量。 |

#### Returns

`void`
