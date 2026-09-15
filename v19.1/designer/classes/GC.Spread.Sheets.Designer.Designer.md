# Class: Designer

[Sheets](../modules/GC.Spread.Sheets.md).[Designer](../modules/GC.Spread.Sheets.Designer.md).Designer

## Table of contents

### Constructors

- [constructor](GC.Spread.Sheets.Designer.Designer.md#constructor)

### Methods

- [activeRibbonTab](GC.Spread.Sheets.Designer.Designer.md#activeribbontab)
- [bind](GC.Spread.Sheets.Designer.Designer.md#bind)
- [destroy](GC.Spread.Sheets.Designer.Designer.md#destroy)
- [getData](GC.Spread.Sheets.Designer.Designer.md#getdata)
- [getWorkbook](GC.Spread.Sheets.Designer.Designer.md#getworkbook)
- [refresh](GC.Spread.Sheets.Designer.Designer.md#refresh)
- [setConfig](GC.Spread.Sheets.Designer.Designer.md#setconfig)
- [setData](GC.Spread.Sheets.Designer.Designer.md#setdata)
- [setWorkbook](GC.Spread.Sheets.Designer.Designer.md#setworkbook)
- [showDialog](GC.Spread.Sheets.Designer.Designer.md#showdialog)
- [showMessageBox](GC.Spread.Sheets.Designer.Designer.md#showmessagebox)
- [unbind](GC.Spread.Sheets.Designer.Designer.md#unbind)
- [unbindAll](GC.Spread.Sheets.Designer.Designer.md#unbindall)
- [waitForDefaultTemplateLoaded](GC.Spread.Sheets.Designer.Designer.md#waitfordefaulttemplateloaded)
- [RegisterComponent](GC.Spread.Sheets.Designer.Designer.md#registercomponent)

## Constructors

### <a id="constructor" name="constructor"></a> constructor

• **new Designer**(`host`, `config?`, `spread?`, `spreadOptions?`)

使用指定的托管DOM元素、自定义配置和现有工作簿来创建一个Designer实例。

**`example`**
```javascript
var designer = new GC.Spread.Sheets.Designer.Designer(document.getElementById("hostDiv"));
var customConfig = {
      ribbon: [
          {
              id: "home",
              text: "主页",
              buttonGroups: [
                {
                  label: "撤销",
                  thumbnailClass: "ribbon-thumbnail-undoRedo",
                  commandGroup: {
                    children: [
                      {
                        direction: "vertical",
                        commands: [
                          "undo",
                          "redo"
                        ]
                      }
                    ]
                  }
                }
              ]
          }
      ],
      contextMenu: [
          "contextMenuCut",
          "contextMenuCopy",
      ],
      fileMenu: "fileMenuButton",
      sidePanels: [
          {
              position: "top",
              allowResize: true,
              command: "formulaBarPanel",
              uiTemplate: "formulaBarTemplate"
          },
      ]
 };
var customDesigner = new GC.Spread.Sheets.Designer.Designer(document.getElementById("hostDiv2"), customConfig);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `host` | `string` \| `HTMLDivElement` | Designer组件将挂载到的HTML区域。 |
| `config?` | [`IDesignerConfig`](../interfaces/GC.Spread.Sheets.Designer.IDesignerConfig.md) | 设计器的配置对象。 |
| `spread?` | `Object` | 工作簿实例。 |
| `spreadOptions?` | `Object` | 工作簿的初始化选项。 |

## Methods

### <a id="activeribbontab" name="activeribbontab"></a> activeRibbonTab

▸ **activeRibbonTab**(`ribbonTabId?`): `string`

获取或设置设计器当前活动的功能区选项卡ID，选项卡ID定义在DefaultConfig中。

**`example`**
```javascript
// 此示例在设计器初始化后设置活动的功能区选项卡。
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var designer = new GC.Spread.Sheets.Designer.Designer(document.getElementById("gc-designer-container"), undefined, spread);
let currentActiveRibbonTab = designer.activeRibbonTab(); // 获取当前活动选项卡ID。
if (currentActiveRibbonTab !== "insert") {
    designer.activeRibbonTab("insert"); // 将"插入"选项卡设为活动状态。
}
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ribbonTabId?` | `string` | 要激活的功能区选项卡ID。 |

#### Returns

`string`

- 当前活动的功能区选项卡ID。

___

### <a id="bind" name="bind"></a> bind

▸ **bind**(`type`, `fn?`): `void`

为设计器绑定事件处理函数。

**`example`**
```javascript
// 此示例演示如何绑定事件。
designer.bind(GC.Spread.Sheets.Designer.Events.FileLoading, function(type, message){
    if (message.fileType = GC.Spread.Sheets.Designer.FileType.Excel){
        let spreadJsonData = message.data;
        if(spreadJsonData.sheetCount >= 3) {
             message.cancel = true;
        }
    };
});
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `string` | 事件类型。 |
| `fn?` | `any` | 事件触发时执行的函数。 |

#### Returns

`void`

___

### <a id="destroy" name="destroy"></a> destroy

▸ **destroy**(): `void`

销毁设计器实例并解绑所有事件。

**`example`**
```javascript
// 此示例在创建设计器后销毁它。
var designer = new GC.Spread.Sheets.Designer.Designer(document.getElementById("hostDiv"));
designer.destroy();
```

#### Returns

`void`

___

### <a id="getdata" name="getdata"></a> getData

▸ **getData**(`key`): `any`

获取状态或值。数据分为两种类型：一种是仅在单个组件中使用的本地数据，
另一种是在整个设计器环境中使用的全局数据。designer.getData(key)可以通过
键获取存储在设计器实例中的全局数据。

**`example`**
```javascript
// 此示例在一个位置（如功能区->主页）设置全局数据，并在另一个位置（如功能区->设置）
// 获取该数据，前提是这两个位置都有设计器实例。
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var config = GC.Spread.Sheets.Designer.DefaultConfig;
var logInCommand = {
   title: "登录",
   text: "登录",
   iconClass: "ribbon-button-login",
   bigButton: true,
   commandName: "login",
   execute: (context, propertyName) => {
       alert('登录新设计器。');
       context.setData("isLogIn", true); // 设置数据
    }
};
var getGiftCommand = {
    title: "领取礼品",
    text: "领取礼品",
    iconClass: "ribbon-button-get-gift",
    bigButton: 'true',
    commandName: "getGift",
    execute: (context, propertyName) => {
        let isLogIn = context.getData("isLogIn"); // 获取数据
        if (isLogIn) {
            alert("领取礼品");
        }
        else {
            alert("请先登录");
        }
    }
};
config.commandMap = {
    login: logInCommand,
    getGift: getGiftCommand,
};
var logInCommandGroup = {
    label: "登录",
    thumbnailClass: "Login",
    commandGroup: {
        children: [
            {
                direction: "vertical",
                commands: [
                    "Login"
                ]
            }
        ]
    }
};
var getGiftCommandGroup = {
    label: "礼品",
    thumbnailClass: "Gift",
    commandGroup: {
        children: [
            {
                direction: "vertical",
                commands: [
                    "getGift"
                ]
            }
        ]
     }
 };
 if (config && config.ribbon) {
 config.ribbon[0].buttonGroups.unshift(logInCommandGroup);
 config.ribbon[5].buttonGroups.unshift(getGiftCommandGroup);
 }
 var d = new GC.Spread.Sheets.Designer.Designer(document.getElementById("gc-designer-container"), config, spread);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | 数据名称，唯一标识一个状态数据。 |

#### Returns

`any`

- 该数据名称对应的值或状态，可以是对象、字符串或其他类型。

___

### <a id="getworkbook" name="getworkbook"></a> getWorkbook

▸ **getWorkbook**(): `Object`

获取现有设计器的工作簿实例。

**`example`**
```javascript
// 此示例将获取现有设计器的工作簿。
var designer = new GC.Spread.Sheets.Designer.Designer(document.getElementById("hostDiv"));
var workbook = designer.getWorkbook();
var sheet = workbook.getActiveSheet();
```

#### Returns

`Object`

现有设计器的工作簿实例。

___

### <a id="refresh" name="refresh"></a> refresh

▸ **refresh**(): `void`

刷新设计器布局和功能区区域。

**`example`**
```javascript
// 此示例在更改设计器内容HTML元素大小时刷新设计器和功能区。
var designerContent = document.getElementById("gc-designer-container");
designerContent.style.width = width + "px";
designerContent.style.height = height + "px";
designer.refresh();
```

#### Returns

`void`

___

### <a id="setconfig" name="setconfig"></a> setConfig

▸ **setConfig**(`config`): `void`

使用自定义配置初始化设计器。

**`example`**
```javascript
// 此示例将自定义配置应用于现有设计器
var designer = new GC.Spread.Sheets.Designer.Designer(document.getElementById("hostDiv"));
var config = {
      ribbon: [
          {
              id: "home",
              text: "主页",
              buttonGroups: [
                {
                  label: "撤销",
                  thumbnailClass: "ribbon-thumbnail-undoRedo",
                  commandGroup: {
                    children: [
                      {
                        direction: "vertical",
                        commands: [
                          "undo",
                          "redo"
                        ]
                      }
                    ]
                  }
                }
              ]
          }
      ],
      contextMenu: [
          "contextMenuCut",
          "contextMenuCopy",
      ],
      fileMenu: "fileMenuButton",
      sidePanels: [
          {
              position: "top",
              allowResize: true,
              command: "formulaBarPanel",
              uiTemplate: "formulaBarTemplate"
          },
      ]
 };
designer.setConfig(config);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `config` | [`IDesignerConfig`](../interfaces/GC.Spread.Sheets.Designer.IDesignerConfig.md) | 设计器配置对象。 |

#### Returns

`void`

___

### <a id="setdata" name="setdata"></a> setData

▸ **setData**(`key`, `value`): `void`

设置状态或值。数据分为两种类型：一种是仅在单个组件中使用的本地数据，
另一种是在整个设计器环境中使用的全局数据。designer.setData(key, value) 可通过
键值对在拥有设计器实例的上下文中设置全局数据。

**`example`**
```javascript
// 此示例在功能区->主页设置全局数据，并在功能区->设置获取该数据（需共享设计器实例）。
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var config = GC.Spread.Sheets.Designer.DefaultConfig;
var logInCommand = {
   title: "登录",
   text: "登录",
   iconClass: "ribbon-button-login",
   bigButton: true,
   commandName: "login",
   execute: (context, propertyName) => {
       alert('登录新设计器。');
       context.setData("isLogIn", true); // 设置数据
    }
};
var getGiftCommand = {
    title: "领取礼品",
    text: "领取礼品",
    iconClass: "ribbon-button-get-gift",
    bigButton: 'true',
    commandName: "getGift",
    execute: (context, propertyName) => {
        let isLogIn = context.getData("isLogIn"); // 获取数据
        if (isLogIn) {
            alert("领取礼品");
        }
        else {
            alert("请先登录");
        }
    }
};
config.commandMap = {
    login: logInCommand,
    getGift: getGiftCommand,
};
var logInCommandGroup = {
    label: "登录",
    thumbnailClass: "Login",
    commandGroup: {
        children: [
            {
                direction: "vertical",
                commands: [
                    "Login"
                ]
            }
        ]
    }
};
var getGiftCommandGroup = {
    label: "礼品",
    thumbnailClass: "Gift",
    commandGroup: {
        children: [
            {
                direction: "vertical",
                commands: [
                    "getGift"
                ]
            }
        ]
     }
 };
 if (config && config.ribbon) {
 config.ribbon[0].buttonGroups.unshift(logInCommandGroup);
 config.ribbon[5].buttonGroups.unshift(getGiftCommandGroup);
 }
 var d = new GC.Spread.Sheets.Designer.Designer(document.getElementById("gc-designer-container"), config, spread);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `key` | `string` | 数据名称，唯一标识状态数据，多次设置相同键将仅保留最新值。 |
| `value` | `any` | 数据对应的值或状态，可为对象、字符串或其他类型。 |

#### Returns

`void`

___

### <a id="setworkbook" name="setworkbook"></a> setWorkbook

▸ **setWorkbook**(`spread`): `void`

使用现有工作簿实例替换设计器的工作簿。

**`example`**
```javascript
// 此示例将现有工作簿设置到设计器中。
var spread = new GC.Spread.Sheets.Workbook(document.getElementById("ss"));
var designer = new GC.Spread.Sheets.Designer.Designer(document.getElementById("hostDiv"));
designer.setWorkbook(spread);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `spread` | `Object` | 用于替换设计器原有工作簿的现有实例。 |

#### Returns

`void`

___

### <a id="showdialog" name="showdialog"></a> showDialog

▸ **showDialog**(`templateName`, `bindingData`, `successCallback`, `errCallback?`, `validCallback?`, `popupElement?`): `void`

显示带选项的对话框，选项将应用于通过模板名称获取的对话框模板。

**`example`**
```javascript
// 示例：以下代码将打开"setText"模板对话框，选项应用于模板，点击确定后设置文本和水平对齐。
var inputCommand = {
    title: "输入",
    text: "输入",
    iconClass: "ribbon-button-input-text",
    bigButton: true,
    commandName: "inputText",
    execute: (context, propertyName) => {
        var dialogOption = {
            text: "",
            isCenter: false,
        };
        context.showDialog("setText", dialogOption, (result) => {
            if (!result) {
                 return;
             }
            var text = result.text;
            var isCenter = result.isCenter;
            var spread = context.getWorkbook();
            var sheet = spread.getActiveSheet();
            var column = sheet.getActiveColumnIndex();
            var row = sheet.getActiveRowIndex();
            sheet.setValue(row, column, text);
            if (isCenter) {
                var style = new GC.Spread.Sheets.Style();
                style.hAlign = GC.Spread.Sheets.HorizontalAlign.center;
                sheet.setStyle(row, column, style);
            }
        }, (error) => {
            console.error(error);
        }, (value) => { checkResult(context, value); });
    }
};
var config = GC.Spread.Sheets.Designer.DefaultConfig;
config.commandMap = {
    input: inputCommand,
};
var inputCommandGroup = {
    label: "输入",
    thumbnailClass: "input",
    commandGroup: {
        children: [
            {
                direction: "vertical",
                commands: [
                    "input"
                ]
            }
        ]
    }
};
if (config && config.ribbon) {
    config.ribbon[0].buttonGroups.push(inputCommandGroup);
}
var setTextTemplate = {
    title: "示例",
    content: [
        {
            type: "ColumnSet",
            children: [
                {
                    type: "Column",
                    children: [
                        {
                            type: "TextBlock",
                            text: "文本:",
                        }
                    ]
                },
                {
                    type: "Column",
                    children: [
                        {
                            type: "TextEditor",
                            margin: "0 0 0 10px",
                            bindingPath: "text"
                        }
                     ]
                }
            ]
        },
        {
            type: "CheckBox",
            bindingPath: "isCenter",
            text: "居中",
         },
    ]
};
GC.Spread.Sheets.Designer.registerTemplate("setText", setTextTemplate);
function checkResult(context, value) {
    if (value.text === "") {
        context.showMessageBox("请不要输入空值。", "警告", GC.Spread.Sheets.Designer.MessageBoxIcon.warning);
        return false;
    } else {
        return true;
    }
}
var designer = new GC.Spread.Sheets.Designer.Designer(document.getElementById("gc-designer-container"), config);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `templateName` | `string` | 模板名称。 |
| `bindingData` | `Object` | 对话框绑定数据。 |
| `successCallback` | `Function` | 对话框关闭后执行的回调。若点击确定，返回对话框数据；若取消或关闭，返回null。 |
| `errCallback?` | `Function` | 对话框发生异常时执行的回调。 |
| `validCallback?` | `Function` | 对话框验证回调，点击确定并关闭对话框后、返回结果前执行，可修改结果或执行其他操作，需返回处理后的结果。 |
| `popupElement?` | `HTMLElement` | 对话框依赖的目标HTML元素。 |

#### Returns

`void`

___

### <a id="showmessagebox" name="showmessagebox"></a> showMessageBox

▸ **showMessageBox**(`text`, `title`, `icon`, `successCallback?`, `errCallback?`, `buttons?`): `void`

该函数将显示带输入选项的消息框。

**`example`**
```javascript
// 示例：以下代码将显示标题为"这是标题"、文本为"这是错误文本"、图标为黄色三角形感叹号的消息框。
var showCommand = {
    title: "显示",
    text: "显示",
    iconClass: "ribbon-button-show",
    bigButton: true,
    commandName: "show",
    execute: (context, propertyName) => {
        context.showMessageBox("这是标题", "这是错误文本", GC.Spread.Sheets.Designer.MessageBoxIcon.warning);  // 显示消息框
    }
};
var config = GC.Spread.Sheets.Designer.DefaultConfig;
config.commandMap = {
    showMessage: showCommand
};
var showCommandGroup = {
    label: "显示",
    thumbnailClass: "Show",
    commandGroup: {
        children: [
            {
                direction: "vertical",
                commands: [
                    "showMessage"
                ]
            }
        ]
    }
};
if (config && config.ribbon) {
    config.ribbon[0].buttonGroups.push(showCommandGroup);
}
var designer = new GC.Spread.Sheets.Designer.Designer(document.getElementById("gc-designer-container"), config);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `text` | `string` | 消息框的错误文本 |
| `title` | `string` | 消息框的标题 |
| `icon` | [`MessageBoxIcon`](../enums/GC.Spread.Sheets.Designer.MessageBoxIcon.md) | 消息框的图标 |
| `successCallback?` | `Function` | 对话框关闭后执行的回调函数。参数"data"表示点击的按钮类型，类型为GC.Spread.Sheets.Designer.MessageBoxResult，1代表"确定"，2代表"是"，3代表"否"，4代表"取消"。 |
| `errCallback?` | `Function` | 对话框发生异常时执行的回调函数。 |
| `buttons?` | [`MessageBoxButtons`](../enums/GC.Spread.Sheets.Designer.MessageBoxButtons.md) | 消息框的按钮配置 |

#### Returns

`void`

___

### <a id="unbind" name="unbind"></a> unbind

▸ **unbind**(`type`, `fn?`): `void`

移除设计器中事件的绑定。

**`example`**
```javascript
designer.bind(GC.Spread.Sheets.Designer.Events.FileLoaded, function(event,data){
    console.log("文件已加载")
});
designer.unbind(GC.Spread.Sheets.Designer.Events.FileLoaded);
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `type` | `string` | 事件类型。 |
| `fn?` | `any` | 要移除绑定的函数（可选）。 |

#### Returns

`void`

___

### <a id="unbindall" name="unbindall"></a> unbindAll

▸ **unbindAll**(): `void`

移除设计器中所有事件的绑定。

**`example`**
```javascript
designer.bind(GC.Spread.Sheets.Designer.Events.FileLoaded, function(event,data){
    console.log("文件已加载")
});
designer.unbindAll();
```

#### Returns

`void`

___

### <a id="waitfordefaulttemplateloaded" name="waitfordefaulttemplateloaded"></a> waitForDefaultTemplateLoaded

▸ **waitForDefaultTemplateLoaded**(): `Promise`<`void`\>

返回一个 Promise，该 Promise 会在默认模板完成加载后 resolve。
如果未提供 templatesConfig，则该 Promise 会立即 resolve。
在创建或重新配置设计器后，可使用此方法确保模板
在操作工作簿之前已完成加载。

**`example`**
```javascript
var config = GC.Spread.Sheets.Designer.DefaultConfig;
config.templatesConfig = "templates/config.json";
var designer = new GC.Spread.Sheets.Designer.Designer(document.getElementById("gc-designer-container"), config);
await designer.waitForDefaultTemplateLoaded();
// 现在可以安全地操作工作簿
var workbook = designer.getWorkbook();
workbook.getActiveSheet().setValue(0, 0, "Hello");
```

#### Returns

`Promise`<`void`\>

当默认模板加载完成时 resolve 的 Promise。

___

### <a id="registercomponent" name="registercomponent"></a> RegisterComponent

▸ `Static` **RegisterComponent**(`name`, `constructor`): `boolean`

注册自定义组件

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | `string` | 组件名称，后续可通过此名称引用 |
| `constructor` | `any` | 组件类 |

#### Returns

`boolean`

是否注册成功
