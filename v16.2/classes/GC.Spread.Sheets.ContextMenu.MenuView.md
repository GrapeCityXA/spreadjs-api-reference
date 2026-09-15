# Class: MenuView

[Sheets](../modules/GC.Spread.Sheets.md).[ContextMenu](../modules/GC.Spread.Sheets.ContextMenu.md).MenuView

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.ContextMenu.MenuView.md#constructor)

### Methods

- [createMenuItemElement](GC.Spread.Sheets.ContextMenu.MenuView.md#createmenuitemelement)
- [getCommandOptions](GC.Spread.Sheets.ContextMenu.MenuView.md#getcommandoptions)
- [maxHeight](GC.Spread.Sheets.ContextMenu.MenuView.md#maxheight)
- [scrollable](GC.Spread.Sheets.ContextMenu.MenuView.md#scrollable)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new MenuView**()

菜单视图

## Methods

### <a id="createmenuitemelement" name="createmenuitemelement"></a> createMenuItemElement

▸ **createMenuItemElement**(`menuItemData`): `HTMLElement`

创建菜单项视图

**`代码示例`**
```
$(document).ready(function () {
   var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
   function CustomMenuView() {
  }
  CustomMenuView.prototype = new GC.Spread.Sheets.ContextMenu.MenuView();
  CustomMenuView.prototype.createMenuItemElement = function (menuItemData) {
     var self = this;
     var menuItemView = GC.Spread.Sheets.ContextMenu.MenuView.prototype.createMenuItemElement.call(self, menuItemData);
     if (menuItemData.name === "markWithABg") {
         var subMenuView = menuItemView.find(".gc-ui-contextmenu-container");
         $(subMenuView[0]).colorpicker();
     }
     return menuItemView;
 };
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `menuItemData` | [`IMenuItemData`](../interfaces/GC.Spread.Sheets.ContextMenu.IMenuItemData.md) | 需要显示的菜单项的数据 |

#### Returns

`HTMLElement`

菜单项视图

___

### <a id="getcommandoptions" name="getcommandoptions"></a> getCommandOptions

▸ **getCommandOptions**(`menuItemData`, `host`, `event`): `any`

获取指定菜单项的命令选项

**`代码示例`**
```
  var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
  function CustomMenuView() {
  }
  CustomMenuView.prototype = new GC.Spread.Sheets.ContextMenu.MenuView();
  CustomMenuView.prototype.getCommandOptions = function (menuItemData, host, event) {
     if (menuItemData &amp;&amp; menuItemData.name === "markWithABg") {
         var ele = event.target || event.srcElement;
         if (ele.className.indexOf("colorpicker-div-inner-colorcell") !== -1) {
             ele = ele.parentElement;
         }
         return ele.style.background;
     }
  };
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `menuItemData` | [`IMenuItemData`](../interfaces/GC.Spread.Sheets.ContextMenu.IMenuItemData.md) | 单击的菜单项的数据 |
| `host` | `Object` | 单击的菜单项的容器 |
| `event` | `Object` | 鼠标单击事件 |

#### Returns

`any`

command 指定菜单项的选项

___

### <a id="maxheight" name="maxheight"></a> maxHeight

▸ **maxHeight**(`value?`): `number` \| `void`

**`description`** 获取或设置上下文菜单的最大高度

**`代码示例`**
```
  var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
  spread.contextMenu.menuView.maxHeight(400);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`number` \| `void`

number | void

___

### <a id="scrollable" name="scrollable"></a> scrollable

▸ **scrollable**(`value?`): `boolean` \| `void`

**`description`** 获取或设置可滚动的上下文菜单

**`代码示例`**
```
  var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
  spread.contextMenu.menuView.scrollable(false);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`boolean` \| `void`

boolean | void
