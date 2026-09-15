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

表示上下文菜单

## Properties

### <a id="menudata" name="menudata"></a> menuData

• **menuData**: [`IMenuItemData`](../interfaces/GC.Spread.Sheets.ContextMenu.IMenuItemData.md)[]

表示内置的菜单数据

**`property`** {string} [name] - 表示上下文菜单项的标识。

**`property`** {string} [text] - 表示要显示的文本，如果此上下文菜单项是一个组，文本将作为DOM元素的标题显示。

**`property`** {string|Function} [command] - 表示命令名称，commandManager将使用它作为索引来查找此命令，如果此命令存在，则执行它。

**`property`** {boolean} [disable] - 表示此上下文菜单项在当前条件下是否禁用，默认值为false.

**`property`** {string} [iconClass] - 表示此上下文菜单项的图标，它是一个类名。

**`property`** {string} [group] - 表示此上下文菜单项是一个组菜单项，此属性的值应该是其组头的名称。

**`property`** {Object[]} [subMenu] - 表示此上下文菜单项有子菜单。

**`property`** {string} [type] - 表示上下文菜单的类型。

**`property`** {string} [workArea] - 表示此上下文菜单项应该显示在哪个区域，值可以是一组条件，用空格分隔。包括："outline"、"rowHeader"、"colHeader"、"corner"、"slicer"、"chart"、"shape"、"table"、"vpWithoutTb"、"pivotPageFilter"、"pivotTopLeft"、"pivotEmptyLabel"、"pivotHeader"、"pivotGrandTotal"、"pivotContent"、"pivotTable"。

___

### <a id="menuview" name="menuview"></a> menuView

• **menuView**: [`MenuView`](GC.Spread.Sheets.ContextMenu.MenuView.md)

表示内置的菜单视图，可以替换为自定义视图

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
        // 自行创建菜单项视图
        // 应该返回菜单项视图
        // 你可以在这里调用super的createMenuItemElement，只自定义少数菜单项
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

打开上下文菜单

**`example`**
```
   var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
   spread.contextMenu.onOpenMenu = function (menuData, itemsDataForShown, hitInfo, spread) {
          console.log(menuData);
          console.log(itemsDataForShown);
          console.log(hitInfo);
          console.log(spread);
          alert("菜单正在打开");
          //你可以修改itemsDataForShown来改变过滤结果
          //如果你只想改变过滤结果，返回false或不返回任何内容
          //你也可以打开自己的上下文菜单，如果你想这样做，返回true
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

表示上下文菜单事件是否已处理完成
