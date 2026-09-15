# Class: ContextMenu

[Sheets](../modules/GC.Spread.Sheets.md).[ContextMenu](../modules/GC.Spread.Sheets.ContextMenu.md).ContextMenu

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.ContextMenu.ContextMenu.md#constructor)

### Properties

- [menuData](GC.Spread.Sheets.ContextMenu.ContextMenu.md#menudata)
- [menuView](GC.Spread.Sheets.ContextMenu.ContextMenu.md#menuview)

### Methods

- [onOpenMenu](GC.Spread.Sheets.ContextMenu.ContextMenu.md#onopenmenu)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new ContextMenu**()

上下文菜单

## Properties

### <a id="menudata" name="menudata"></a> menuData

• **menuData**: [`IMenuItemData`](../interfaces/GC.Spread.Sheets.ContextMenu.IMenuItemData.md)[]

内置的menuData

**`property`** {string} [name] - 上下文菜单项的标识

**`property`** {string} [text] - 要显示的文本,如果此上下文菜单项是一个组,则文本将显示为DOM元素的标题

**`property`** {string|Function} [command] - 命令名,commandManager将使用此作为索引来查找此命令,如果此命令存在,则执行它

**`property`** {boolean} [disable] - 此上下文菜单项在当前条件下被禁用,默认值为false

**`property`** {string} [iconClass] - 此上下文菜单项的图标,它是一个类名

**`property`** {string} [group] - 此上下文菜单项是组菜单项,此属性的值应为其组标题的名称

**`property`** {Object[]} [subMenu] - 此上下文菜单项具有子菜单

**`property`** {string} [type] - 上下文菜单的类型

**`property`** {string} [workArea] - 该上下文菜单项应该显示在以下区域：概述（outline）、行标题（rowHeader）、列标题（colHeader）、角落（corner）、切片器（slicer）、图表（chart）、形状（shape）、表格（table）、无工具栏的视图（vpWithoutTb）、透视页筛选器（pivotPageFilter）、透视页左上角（pivotTopLeft）、透视页空标签（pivotEmptyLabel）、透视页标题（pivotHeader）、透视页总计（pivotGrandTotal）、透视页内容（pivotContent）、透视表（pivotTable）。

___

### <a id="menuview" name="menuview"></a> menuView

• **menuView**: [`MenuView`](GC.Spread.Sheets.ContextMenu.MenuView.md)

内置的menuView

## Methods

### <a id="onopenmenu" name="onopenmenu"></a> onOpenMenu

▸ **onOpenMenu**(`menuData`, `itemsDataForShown`, `hitInfo`, `spread`): `boolean`

open context menu

**`代码示例`**
```
   var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
   spread.contextMenu.onOpenMenu = function (menuData, itemsDataForShown, hitInfo, spread) {
          console.log(menuData);
          console.log(itemsDataForShown);
          console.log(hitInfo);
          console.log(spread);
          //您可以更改itemsDataForShown以更改筛选结果
          //如果只想更改筛选结果,则返回false或不返回任何内容
          //您还可以打开自己的上下文菜单,如果要执行此操作,请返回true
          //返回true
   };
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `menuData` | [`IMenuItemData`](../interfaces/GC.Spread.Sheets.ContextMenu.IMenuItemData.md)[] |
| `itemsDataForShown` | [`IMenuItemData`](../interfaces/GC.Spread.Sheets.ContextMenu.IMenuItemData.md)[] |
| `hitInfo` | `Object` |
| `spread` | `Object` |

#### Returns

`boolean`

是否已处理contextmenu事件
