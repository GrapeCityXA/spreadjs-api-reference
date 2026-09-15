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

内置的 menuData

**`property`** {string} [name] - 上下文菜单项的标识

**`property`** {string} [text] - 要显示的文本，如果此上下文菜单项是一个组，则文本将显示为DOM元素的标题

**`property`** {string|Function} [command] - 命令名,commandManager将使用此作为索引来查找此命令，如果此命令存在，则执行它

**`property`** {boolean} [disable] - 此上下文菜单项在当前条件下被禁用，默认值为false

**`property`** {string} [iconClass] - 此上下文菜单项的图标，它是一个类名

**`property`** {string} [group] - 此上下文菜单项是组菜单项，此属性的值应为其组标题的名称

**`property`** {Object[]} [subMenu] - 此上下文菜单项具有子菜单

**`property`** {string} [type] - 上下文菜单的类型

**`property`** {string} [workArea] - 该上下文菜单项应该显示在以下区域：概述（outline）、行标题（rowHeader）、列标题（colHeader）、角落（corner）、切片器（slicer）、图表（chart）、形状（shape）、表格（table）、无工具栏的视图（vpWithoutTb）、透视页筛选器（pivotPageFilter）、透视页左上角（pivotTopLeft）、透视页空标签（pivotEmptyLabel）、透视页标题（pivotHeader）、透视页总计（pivotGrandTotal）、透视页内容（pivotContent）、透视表（pivotTable）

___

### <a id="menuview" name="menuview"></a> menuView

• **menuView**: [`MenuView`](GC.Spread.Sheets.ContextMenu.MenuView.md)

代表内置 menuView，可以替换为自定义

**`example`**
```
var spread = new GC.Spread.Sheets.Workbook(document.getElementById('ss'));
var colors = ['rgb(255,255,255)', 'rgb(0,255,255)', 'rgb(255,0,255)', 'rgb(255,255,0)', 'rgb(255,0,0)', 'rgb(0,255,0)', 'rgb(0,0,255)', 'rgb(0,0,0)'];
function createColorpicker() {
    var colorPicker = document.createElement('div');
    colorPicker.style.width = '100%';
    colorPicker.style.backgroundColor = 'white';
    for (var j = 0; j < 8; j++) {
        var colorDom = document.createElement("div");
        colorDom.style.width = "14px";
        colorDom.style.height = "14px";
        colorDom.style.margin = "0 0 0 6px";
        colorDom.style.display = "inline-block";
        colorDom.style.border = "solid 1px #333333";
        colorDom.style.verticalAlign = "top";
        colorDom.style.backgroundColor = colors[j];
        colorPicker.appendChild(colorDom);
    }
    return colorPicker;
}
// let spread = new GC.Spread.Sheets.Workbook(document.getElementById('ss'));
let selectWithABackgroundColor = {
    text: "Select Color",
    name: "selectColorWithBg",
    workArea: "viewport",
    subMenu: [{
        name: "selectColorPicker",
        command: "selectWithBg"
    }]
};
spread.contextMenu.menuData.push(selectWithABackgroundColor);
let selectWithABackgroundColorCommand = {
    canUndo: false,
    execute: function(spread, options) {
        if (options.commandOptions) {
            var style = new GC.Spread.Sheets.Style();
            style.name = 'style1';
            style.backColor = options.commandOptions;
            var sheet = spread.getActiveSheet();
            sheet.suspendPaint();
            var selections = sheet.getSelections();
            var selectionIndex = 0
              , selectionCount = selections.length;
            for (; selectionIndex < selectionCount; selectionIndex++) {
                var selection = selections[selectionIndex];
                for (var i = selection.row; i < (selection.row + selection.rowCount); i++) {
                    for (var j = selection.col; j < (selection.col + selection.colCount); j++) {
                        sheet.setStyle(i, j, style, GC.Spread.Sheets.SheetArea.viewport);
                    }
                }
            }
            sheet.resumePaint();
        }
    }
};
spread.commandManager().register("selectWithBg", selectWithABackgroundColorCommand, null, false, false, false, false);
class CustomMenuView extends GC.Spread.Sheets.ContextMenu.MenuView {
    createMenuItemElement(menuItemData) {
        // create menu item view by your self
        // should return menu item view back
        // you can call super's createMenuItemElement here and only customize a few of menu item
        if (menuItemData.name === "selectColorPicker") {
            var containers = super.createMenuItemElement(menuItemData);
            var supMenuItemContainer = containers[0];
            while (supMenuItemContainer.firstChild) {
                supMenuItemContainer.removeChild(supMenuItemContainer.firstChild);
            }
            var colorPicker = createColorpicker();
            supMenuItemContainer.appendChild(colorPicker);

            return supMenuItemContainer;
        }
        return super.createMenuItemElement(menuItemData);
    }
    getCommandOptions(menuItemData, host, event) {
        if (menuItemData && menuItemData.name === "selectColorPicker") {
            var ele = event.target || event.srcElement;
            return ele.style.backgroundColor;
        }
        return super.getCommandOptions(menuItemData, host, event);
    }
}
spread.contextMenu.menuView = new CustomMenuView();
```

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
          alert("menu is opening");
          //you can change itemsDataForShown to change filter result
          //if you only want to change filter result,return false or don't return anything
          //you also can open your own context menu,if you want to do this,return true
          //return true;
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

是否已处理 contextmenu 事件
