# Interface: IMenuItemData

[Sheets](../modules/GC.Spread.Sheets.md).[ContextMenu](../modules/GC.Spread.Sheets.ContextMenu.md).IMenuItemData

## Table of contents

### Properties

- [command](GC.Spread.Sheets.ContextMenu.IMenuItemData.md#command)
- [commandOptions](GC.Spread.Sheets.ContextMenu.IMenuItemData.md#commandoptions)
- [disable](GC.Spread.Sheets.ContextMenu.IMenuItemData.md#disable)
- [group](GC.Spread.Sheets.ContextMenu.IMenuItemData.md#group)
- [iconClass](GC.Spread.Sheets.ContextMenu.IMenuItemData.md#iconclass)
- [itemClass](GC.Spread.Sheets.ContextMenu.IMenuItemData.md#itemclass)
- [menuContent](GC.Spread.Sheets.ContextMenu.IMenuItemData.md#menucontent)
- [metaData](GC.Spread.Sheets.ContextMenu.IMenuItemData.md#metadata)
- [name](GC.Spread.Sheets.ContextMenu.IMenuItemData.md#name)
- [needKeepFocus](GC.Spread.Sheets.ContextMenu.IMenuItemData.md#needkeepfocus)
- [placeholder](GC.Spread.Sheets.ContextMenu.IMenuItemData.md#placeholder)
- [status](GC.Spread.Sheets.ContextMenu.IMenuItemData.md#status)
- [subMenu](GC.Spread.Sheets.ContextMenu.IMenuItemData.md#submenu)
- [text](GC.Spread.Sheets.ContextMenu.IMenuItemData.md#text)
- [title](GC.Spread.Sheets.ContextMenu.IMenuItemData.md#title)
- [type](GC.Spread.Sheets.ContextMenu.IMenuItemData.md#type)
- [visible](GC.Spread.Sheets.ContextMenu.IMenuItemData.md#visible)
- [workArea](GC.Spread.Sheets.ContextMenu.IMenuItemData.md#workarea)

## Properties

### <a id="command" name="command"></a> command

• `Optional` **command**: `string` \| `Function`

表示命令名称（也可直接传入命令执行函数）。

___

### <a id="commandoptions" name="commandoptions"></a> commandOptions

• `Optional` **commandOptions**: `any`

表示命令执行时传递给命令的附加选项。

___

### <a id="disable" name="disable"></a> disable

• `Optional` **disable**: `boolean`

表示该上下文菜单项是否处于禁用状态。

___

### <a id="group" name="group"></a> group

• `Optional` **group**: `string`

表示该上下文菜单项为分组菜单项，此属性值应为其分组标题的名称。

___

### <a id="iconclass" name="iconclass"></a> iconClass

• `Optional` **iconClass**: `string`

表示该上下文菜单项的图标样式类名。

___

### <a id="itemclass" name="itemclass"></a> itemClass

• `Optional` **itemClass**: `string`

表示要应用到该菜单项上的附加CSS类名。

___

### <a id="menucontent" name="menucontent"></a> menuContent

• `Optional` **menuContent**: `string`

表示该菜单项的自定义HTML内容。

___

### <a id="metadata" name="metadata"></a> metaData

• `Optional` **metaData**: [`ICommandMetaData`](GC.Spread.Sheets.ICommandMetaData.md)

表示与命令关联的元数据（例如权限要求等）。

___

### <a id="name" name="name"></a> name

• `Optional` **name**: `string`

表示上下文菜单项的唯一标识。

___

### <a id="needkeepfocus" name="needkeepfocus"></a> needKeepFocus

• `Optional` **needKeepFocus**: `boolean`

表示执行该菜单项后，电子表格是否应保持焦点状态。

___

### <a id="placeholder" name="placeholder"></a> placeholder

• `Optional` **placeholder**: `string`

表示用于动态替换菜单项文本的占位符值。

___

### <a id="status" name="status"></a> status

• `Optional` **status**: `any`

表示该菜单项的状态信息。

___

### <a id="submenu" name="submenu"></a> subMenu

• `Optional` **subMenu**: [`IMenuItemData`](GC.Spread.Sheets.ContextMenu.IMenuItemData.md)[]

表示该上下文菜单项包含子菜单。

___

### <a id="text" name="text"></a> text

• `Optional` **text**: `string`

表示要显示的菜单项文本。

___

### <a id="title" name="title"></a> title

• `Optional` **title**: `string`

表示该菜单项的工具提示标题。

___

### <a id="type" name="type"></a> type

• `Optional` **type**: `string`

表示上下文菜单项的类型。常用值包括 "separator"（分隔符）、"groupHeader"（分组标题）和 "splitSubMenu"（拆分子菜单）。

___

### <a id="visible" name="visible"></a> visible

• `Optional` **visible**: `boolean`

表示该菜单项是否可见。

___

### <a id="workarea" name="workarea"></a> workArea

• `Optional` **workArea**: `string`

表示该上下文菜单项应在工作表的哪个区域显示。属性值可为多个条件用空格分隔的集合，支持的区域包括："outline"（大纲区域）、"rowHeader"（行标题栏）、"colHeader"（列标题栏）、"corner"（边角区域）、"slicer"（切片器）、"chart"（图表）、"shape"（形状）、"table"（表格）、"vpWithoutTb"（无表格视图区域）、"pivotPageFilter"（数据透视表页筛选器）、"pivotTopLeft"（数据透视表左上角区域）、"pivotEmptyLabel"（数据透视表空标签区域）、"pivotHeader"（数据透视表标题栏）、"pivotGrandTotal"（数据透视表总计区域）、"pivotContent"（数据透视表内容区域）、"pivotTable"（数据透视表）、"sheetTab"（工作表标签）、"timeline"（时间线）。
