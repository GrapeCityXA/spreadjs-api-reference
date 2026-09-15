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
``` javascript
window.addEventListener('load', function() {
    var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
    var activeSheet = spread.getActiveSheet();
    activeSheet.setValue(0,0,'please right click');
    activeSheet.setValue(1,0,'you will find there is a new context menu item "Change BackColor"');
    activeSheet.setValue(2,0,'click it');
    var selectWithABackgroundColor = {
        text: "Change BackColor",
        name: "changeColorWithBg",
        workArea: "viewport",
        subMenu: [
             {
                 name: "selectColorPicker",
                 command: "changeBackColor"
             }
         ]
    };
    spread.contextMenu.menuData.push(selectWithABackgroundColor);
    var changeBackgroundColorCommand = {
        canUndo: false,
        execute: function(spread, options) {
            spread.suspendPaint();
            spread.options.backColor = options.commandOptions;
            spread.resumePaint();
        }
    };
    var commandManager = spread.commandManager();
    commandManager.register("changeBackColor", changeBackgroundColorCommand, null, false, false, false, false);
    function CustomMenuView() {
    }
    CustomMenuView.prototype = new GC.Spread.Sheets.ContextMenu.MenuView();
    CustomMenuView.prototype.createMenuItemElement = function(menuItemData) {
        var self = this;
        if (menuItemData.name === "selectColorPicker") {
            var containers = GC.Spread.Sheets.ContextMenu.MenuView.prototype.createMenuItemElement.call(self, menuItemData);
            var supMenuItemContainer = containers[0];
            while (supMenuItemContainer.firstChild) {
                supMenuItemContainer.removeChild(supMenuItemContainer.firstChild);
            }
            var colorPicker = createColorpicker();
            supMenuItemContainer.appendChild(colorPicker);
            return supMenuItemContainer;
        } else {
            var menuItemView = GC.Spread.Sheets.ContextMenu.MenuView.prototype.createMenuItemElement.call(self, menuItemData);
            return menuItemView;
        }
    };
    CustomMenuView.prototype.getCommandOptions = function(menuItemData, host, event) {
       if (menuItemData && menuItemData.name === "selectColorPicker") {
           var ele = event.target || event.srcElement;
           return ele.style.backgroundColor;
       }
    };
    CustomMenuView.prototype.getCommandOptions = function(menuItemData, host, event) {
        if (menuItemData && menuItemData.name === "selectColorPicker") {
            var ele = event.target || event.srcElement;
            return ele.style.backgroundColor;
        }
    };
    var colors = ['rgb(255,255,255)', 'rgb(0,255,255)', 'rgb(255,0,255)', 'rgb(255,255,0)', 'rgb(255,0,0)',
        'rgb(0,255,0)', 'rgb(0,0,255)', 'rgb(0,0,0)'];
    function createColorpicker() {
        var colorPicker = document.createElement('div');
        colorPicker.className = 'colorPickerContent';
        for (var j = 0; j < 8; j++) {
            var colorDom = document.createElement("div");
            colorDom.className = 'colorDom';
            colorDom.style.width = 14 + 'px';
            colorDom.style.height = 14 + 'px';
            colorDom.style.margin = "0 0 0 6px";
            colorDom.style.display = 'inline-block';
            colorDom.style['backgroundColor'] = colors[j];
            colorPicker.appendChild(colorDom);
        }
        return colorPicker;
    }
    spread.contextMenu.menuView = new CustomMenuView();
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
``` javascript
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

指定菜单项的命令选项

___

### <a id="maxheight" name="maxheight"></a> maxHeight

▸ **maxHeight**(`value?`): `number` \| `void`

**`description`** 获取或设置上下文菜单的最大高度

**`代码示例`**
``` javascript
  var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
  spread.contextMenu.menuView.maxHeight(400);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`number` \| `void`

represent the number of context menu's max height

___

### <a id="scrollable" name="scrollable"></a> scrollable

▸ **scrollable**(`value?`): `boolean` \| `void`

**`description`** 获取或设置可滚动的上下文菜单

**`代码示例`**
``` javascript
  var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
  spread.contextMenu.menuView.scrollable(false);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`boolean` \| `void`

represent whether the context menu can scroll
