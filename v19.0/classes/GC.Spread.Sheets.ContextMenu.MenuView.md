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

表示菜单视图

## Methods

### <a id="createmenuitemelement" name="createmenuitemelement"></a> createMenuItemElement

▸ **createMenuItemElement**(`menuItemData`): `HTMLElement`

创建菜单项视图

**`example`**
```
window.addEventListener('load', function() {
    var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
    var activeSheet = spread.getActiveSheet();
    activeSheet.setValue(0,0,'请右键点击');
    activeSheet.setValue(1,0,'你会发现有一个新的上下文菜单项"更改背景色"');
    activeSheet.setValue(2,0,'点击它');
    var selectWithABackgroundColor = {
        text: "更改背景色",
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
| `menuItemData` | [`IMenuItemData`](../interfaces/GC.Spread.Sheets.ContextMenu.IMenuItemData.md) | 需要显示的菜单项数据 |

#### Returns

`HTMLElement`

菜单项视图

___

### <a id="getcommandoptions" name="getcommandoptions"></a> getCommandOptions

▸ **getCommandOptions**(`menuItemData`, `host`, `event`): `any`

获取指定菜单项的命令选项。

**`example`**
```javascript
// 示例：使用 getCommandOptions 向命令传递自定义数据的基本用法
// 向上下文菜单添加一个自定义菜单项
var customMenuItem = {
    text: "Custom Action",
    name: "customAction",
    command: "customCommand",
    workArea: "viewport"
};
spread.contextMenu.menuData.push(customMenuItem);
// 注册一个将接收自定义选项的命令
var customCommand = {
    canUndo: true,
    execute: function(context, options, isUndo) {
        if (isUndo) {
            // 处理撤销逻辑
            console.log("Undo custom action");
        } else {
            // 处理正常执行逻辑
            console.log("Custom action executed with options:", options);
            if (options && options.customData) {
                alert("Custom data passed: " + options.customData);
            }
        }
    }
};
spread.commandManager().register("customCommand", customCommand);
// 创建一个自定义菜单视图，重写 getCommandOptions 方法
class CustomMenuView extends GC.Spread.Sheets.ContextMenu.MenuView {
    getCommandOptions(menuItemData, host, event) {
        // 针对自定义菜单项，返回自定义数据
        if (menuItemData.name === "customAction") {
            return {
                customData: "This is custom data from getCommandOptions",
                timestamp: new Date().toISOString(),
                clickedElement: event.target.tagName
            };
        }
        // 针对其他所有菜单项，使用默认行为
        return super.getCommandOptions(menuItemData, host, event);
    }
}
// 应用自定义菜单视图
spread.contextMenu.menuView = new CustomMenuView();
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `menuItemData` | [`IMenuItemData`](../interfaces/GC.Spread.Sheets.ContextMenu.IMenuItemData.md) | 被点击的菜单项数据。 |
| `host` | `Object` | 被点击的菜单项的容器。 |
| `event` | `Object` | 鼠标点击事件。 |

#### Returns

`any`

指定菜单项的命令选项。

___

### <a id="maxheight" name="maxheight"></a> maxHeight

▸ **maxHeight**(`value?`): `number` \| `void`

**`description`** 获取或设置上下文菜单的最大高度

**`example`**
```
spread.contextMenu.menuView.maxHeight(120);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `number` |

#### Returns

`number` \| `void`

表示上下文菜单的最大高度数值

___

### <a id="scrollable" name="scrollable"></a> scrollable

▸ **scrollable**(`value?`): `boolean` \| `void`

**`description`** 获取或设置上下文菜单是否可滚动

**`example`**
```
spread.contextMenu.menuView.maxHeight(120);
spread.contextMenu.menuView.scrollable(true);
```

#### Parameters

| Name | Type |
| :------ | :------ |
| `value?` | `boolean` |

#### Returns

`boolean` \| `void`

表示上下文菜单是否可以滚动
