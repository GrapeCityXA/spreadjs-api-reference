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

表单的区域分组

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `count` | `number` | 行数或列数 |

## Methods

### <a id="direction" name="direction"></a> direction

▸ **direction**(`direction?`): `any`

获取或设置区域分组的方向

**`代码示例`**
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

如果未设置任何值,则返回区域分组的方向;否则,返回区域分组

___

### <a id="expand" name="expand"></a> expand

▸ **expand**(`level`, `expand`): `void`

展开指定的级别所有区域分组

**`代码示例`**
```
//本示例使用expand方法
activeSheet.suspendPaint();
activeSheet.rowOutlines.group(0,5);
activeSheet.rowOutlines.expand(0,false);
activeSheet.resumePaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `level` | `number` | 区域分组的扩大或折叠的级别 |
| `expand` | `boolean` | 是否扩展组 |

#### Returns

`void`

___

### <a id="expandgroup" name="expandgroup"></a> expandGroup

▸ **expandGroup**(`groupInfo`, `expand`): `void`

展开或折叠行或列的指定区域分组

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `groupInfo` | [`OutlineInfo`](GC.Spread.Sheets.Outlines.OutlineInfo.md) | 区域分组的组信息 |
| `expand` | `boolean` | 是否扩展组 |

#### Returns

`void`

___

### <a id="find" name="find"></a> find

▸ **find**(`index`, `level`): [`OutlineInfo`](GC.Spread.Sheets.Outlines.OutlineInfo.md)

获取具有指定组级别和行或列索引的区域分组

**`代码示例`**
```
//本示例使用find方法
activeSheet.rowOutlines.group(0,5);
var rgi = activeSheet.rowOutlines.find(1, 0);
rgi.state(GC.Spread.Sheets.Outlines.OutlineState.collapsed);
spread.invalidateLayout();
spread.repaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 行或列的索引 |
| `level` | `number` | 区域分组的级别 |

#### Returns

[`OutlineInfo`](GC.Spread.Sheets.Outlines.OutlineInfo.md)

区域分组

___

### <a id="getcollapsed" name="getcollapsed"></a> getCollapsed

▸ **getCollapsed**(`index`): `boolean`

获取折叠的内部

**`代码示例`**
```
//本示例使用getCollapsed方法
activeSheet.suspendPaint();
activeSheet.rowOutlines.group(0,5);
activeSheet.rowOutlines.expand(0,true);
activeSheet.resumePaint();
alert(activeSheet.rowOutlines.isCollapsed(0));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 索引 |

#### Returns

`boolean`

如果折叠,返回true;否则返回false

___

### <a id="getlevel" name="getlevel"></a> getLevel

▸ **getLevel**(`index`): `number`

获取指定行或列的级别
级别的索引从零开始

**`代码示例`**
```
//本示例使用getLevel方法
activeSheet.suspendPaint();
activeSheet.rowOutlines.group(0,5);
activeSheet.rowOutlines.expand(0,true);
activeSheet.resumePaint();
alert(activeSheet.rowOutlines.getLevel(0));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 行或列的索引 |

#### Returns

`number`

行或列的级别

___

### <a id="getmaxlevel" name="getmaxlevel"></a> getMaxLevel

▸ **getMaxLevel**(): `number`

获取最深级别的编号

**`remarks`** 级别的索引从零开始

**`代码示例`**
```
//本示例使用getMaxLevel方法
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

深级别的编号

___

### <a id="getstate" name="getstate"></a> getState

▸ **getState**(`groupInfo`): [`OutlineState`](../enums/GC.Spread.Sheets.Outlines.OutlineState.md)

获取指定组的状态

**`代码示例`**
```
//本示例使用getState方法
activeSheet.suspendPaint();
activeSheet.rowOutlines.group(0,5);
var rgi = activeSheet.rowOutlines.find(1, 0);
rgi.state(GC.Spread.Sheets.Outlines.OutlineInfo.collapsed);
alert(activeSheet.rowOutlines.getState(rgi));
activeSheet.resumePaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `groupInfo` | [`OutlineInfo`](GC.Spread.Sheets.Outlines.OutlineInfo.md) | 组信息 |

#### Returns

[`OutlineState`](../enums/GC.Spread.Sheets.Outlines.OutlineState.md)

组状态

___

### <a id="group" name="group"></a> group

▸ **group**(`index`, `count`): `void`

从指定的起始索引将行或列的区域分组为区域分组

**`代码示例`**
```
//本示例使用group方法
activeSheet.suspendPaint();
activeSheet.rowOutlines.group(0,5);
activeSheet.rowOutlines.expand(0,false);
activeSheet.resumePaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 组起始索引 |
| `count` | `number` | 要分组的行数或列数 |

#### Returns

`void`

___

### <a id="iscollapsed" name="iscollapsed"></a> isCollapsed

▸ **isCollapsed**(`index`): `boolean`

确定指定索引处的区域分组是否折叠

**`代码示例`**
```
//本示例使用isCollapsed方法
activeSheet.suspendPaint();
activeSheet.rowOutlines.group(0,5);
activeSheet.rowOutlines.expand(0,true);
activeSheet.resumePaint();
alert(activeSheet.rowOutlines.isCollapsed(0));
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 区域分组中行或列的索引 |

#### Returns

`boolean`

如果指定的行或列折叠,返回true;否则返回false

___

### <a id="isgroupend" name="isgroupend"></a> isGroupEnd

▸ **isGroupEnd**(`index`, `processLevel`): `boolean`

确定指定的索引是否在组的末尾

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 索引 |
| `processLevel` | `number` | 流程级别 |

#### Returns

`boolean`

如果指定的索引在组的末尾,返回true;否则返回false

___

### <a id="refresh" name="refresh"></a> refresh

▸ **refresh**(): `void`

刷新此区域分组

#### Returns

`void`

___

### <a id="resumeadding" name="resumeadding"></a> resumeAdding

▸ **resumeAdding**(): `void`

恢复添加

#### Returns

`void`

___

### <a id="setcollapsed" name="setcollapsed"></a> setCollapsed

▸ **setCollapsed**(`index`, `collapsed`): `void`

设置折叠级别

**`代码示例`**
```
//本示例使用setCollapsed方法
activeSheet.suspendPaint();
activeSheet.rowOutlines.group(0,5);
activeSheet.rowOutlines.setCollapsed(0,false);
activeSheet.resumePaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 索引 |
| `collapsed` | `boolean` | 设置为true来折叠级别 |

#### Returns

`void`

___

### <a id="suspendadding" name="suspendadding"></a> suspendAdding

▸ **suspendAdding**(): `void`

暂停添加

#### Returns

`void`

___

### <a id="ungroup" name="ungroup"></a> ungroup

▸ **ungroup**(): `void`

删除所有区域分组

**`代码示例`**
```
//本示例使用ungroup方法
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

从指定的起始索引处的区域分组中删除一定区域的行或列

**`代码示例`**
```
//本示例使用ungroupRange方法
activeSheet.suspendPaint();
activeSheet.rowOutlines.group(0,5);
activeSheet.rowOutlines.ungroupRange(0,1);
activeSheet.resumePaint();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `index` | `number` | 组起始索引 |
| `count` | `number` | 要删除的行数或列数 |

#### Returns

`void`
